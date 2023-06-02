# Comparing `tmp/nnusf-0.2.6.tar.gz` & `tmp/nnusf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnusf-0.2.6.tar", max compression
+gzip compressed data, was "nnusf-0.3.0.tar", max compression
```

## Comparing `nnusf-0.2.6.tar` & `nnusf-0.3.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0    35149 2023-05-14 09:19:38.702520 nnusf-0.2.6/LICENSE
--rw-r--r--   0        0        0     2606 2023-05-14 09:19:38.702520 nnusf-0.2.6/README.md
--rw-r--r--   0        0        0     2281 2023-05-14 09:21:33.418794 nnusf-0.2.6/pyproject.toml
--rw-r--r--   0        0        0       46 2023-05-14 09:21:33.422794 nnusf-0.2.6/src/nnusf/__init__.py
--rw-r--r--   0        0        0      133 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/__init__.py
--rw-r--r--   0        0        0      172 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/base.py
--rw-r--r--   0        0        0     4109 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/data.py
--rw-r--r--   0        0        0     2082 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/extra.py
--rw-r--r--   0        0        0     3407 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/fit.py
--rw-r--r--   0        0        0      201 2023-05-14 09:19:38.806521 nnusf-0.2.6/src/nnusf/cli/log.py
--rw-r--r--   0        0        0     5735 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/cli/plot.py
--rw-r--r--   0        0        0      879 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/cli/report.py
--rw-r--r--   0        0        0     6815 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/cli/theory.py
--rw-r--r--   0        0        0      277 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/__init__.py
--rw-r--r--   0        0        0     2989 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/coefficients.py
--rw-r--r--   0        0        0     1002 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/combine_tables.py
--rw-r--r--   0        0        0     1439 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/filters.py
--rw-r--r--   0        0        0     6470 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/loader.py
--rw-r--r--   0        0        0     9416 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/matching_grids.py
--rw-r--r--   0        0        0    13188 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/data/utils.py
--rwxr-xr-x   0        0        0     6128 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_bebcwa59.py
--rwxr-xr-x   0        0        0     6675 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_ccfr.py
--rwxr-xr-x   0        0        0    17661 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_cdhsw.py
--rwxr-xr-x   0        0        0    10365 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_charm.py
--rwxr-xr-x   0        0        0    11707 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_chorus.py
--rwxr-xr-x   0        0        0     9449 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/filters/filter_nutev.py
--rw-r--r--   0        0        0      104 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/get/__init__.py
--rw-r--r--   0        0        0      172 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/get/base.py
--rw-r--r--   0        0        0      698 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/get/gettheory.py
--rw-r--r--   0        0        0      201 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/get/log.py
--rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/lhapdf/__init__.py
--rw-r--r--   0        0        0     6001 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/lhapdf/dump_grids.py
--rw-r--r--   0        0        0     9503 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/lhapdf/utils.py
--rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/__init__.py
--rw-r--r--   0        0        0     7303 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/covmat.py
--rw-r--r--   0        0        0    17946 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/fit.py
--rw-r--r--   0        0        0     4344 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/kinematics.py
--rw-r--r--   0        0        0     3559 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/matching.py
--rw-r--r--   0        0        0     2952 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/sf.py
--rw-r--r--   0        0        0     5572 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/sfs_lhapdf.py
--rw-r--r--   0        0        0     6132 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/th_covmat.py
--rw-r--r--   0        0        0     7191 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plot/utils.py
--rw-r--r--   0        0        0     1384 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/plotstyle.mplstyle
--rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/__init__.py
--rw-r--r--   0        0        0     7125 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/assets/index.html
--rwxr-xr-x   0        0        0    68365 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/assets/report.css
--rw-r--r--   0        0        0     9969 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/genfiles.py
--rw-r--r--   0        0        0     5641 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/reports/genhtml.py
--rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/scripts/__init__.py
--rw-r--r--   0        0        0     2329 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/scripts/gettheory.py
--rw-r--r--   0        0        0     1369 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/scripts/integrate.py
--rw-r--r--   0        0        0     3315 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/scripts/isoscalar.py
--rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/__init__.py
--rw-r--r--   0        0        0     5283 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/callbacks.py
--rw-r--r--   0        0        0     3339 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/compute_expchi2.py
--rw-r--r--   0        0        0     2957 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/layers.py
--rw-r--r--   0        0        0     3926 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/load_data.py
--rw-r--r--   0        0        0     4238 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/load_fit_data.py
--rw-r--r--   0        0        0     5351 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/model_gen.py
--rw-r--r--   0        0        0     2603 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/postfit.py
--rw-r--r--   0        0        0     3120 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/run_sffit.py
--rw-r--r--   0        0        0     2241 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/scaling.py
--rw-r--r--   0        0        0    11423 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/sum_rules.py
--rw-r--r--   0        0        0     2728 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/train_model.py
--rw-r--r--   0        0        0     8001 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/sffit/utils.py
--rw-r--r--   0        0        0        0 2023-05-14 09:19:38.810521 nnusf-0.2.6/src/nnusf/theory/__init__.py
--rw-r--r--   0        0        0  1626320 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/assets/genie.hdf5
--rw-r--r--   0        0        0      649 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/assets/theory_nnusf.yaml
--rw-r--r--   0        0        0     1245 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/bodek_yang/__init__.py
--rw-r--r--   0        0        0      157 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/bodek_yang/cuts.py
--rw-r--r--   0        0        0     1532 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/bodek_yang/load.py
--rw-r--r--   0        0        0      800 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/bodek_yang/runcards.py
--rw-r--r--   0        0        0     4209 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/compare_to_data.py
--rw-r--r--   0        0        0       47 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/data_vs_theory/__init__.py
--rw-r--r--   0        0        0      646 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/data_vs_theory/runcards.py
--rw-r--r--   0        0        0      885 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/defs.py
--rw-r--r--   0        0        0     1991 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/grids.py
--rw-r--r--   0        0        0       47 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/highq/__init__.py
--rw-r--r--   0        0        0     1377 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/highq/load.py
--rw-r--r--   0        0        0     3960 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/highq/runcards.py
--rw-r--r--   0        0        0    12073 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/predictions.py
--rw-r--r--   0        0        0     5969 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/runcards.py
--rw-r--r--   0        0        0       47 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/yadknots/__init__.py
--rw-r--r--   0        0        0     1187 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/theory/yadknots/runcards.py
--rw-r--r--   0        0        0     6366 2023-05-14 09:19:38.822521 nnusf-0.2.6/src/nnusf/utils.py
--rw-r--r--   0        0        0     1610 2023-05-14 09:19:38.822521 nnusf-0.2.6/tests/test_loader.py
--rw-r--r--   0        0        0      156 2023-05-14 09:19:38.822521 nnusf-0.2.6/tests/theory/test_bodek_yang.py
--rw-r--r--   0        0        0     4244 1970-01-01 00:00:00.000000 nnusf-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-02 15:26:22.741579 nnusf-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2606 2023-06-02 15:26:22.741579 nnusf-0.3.0/README.md
+-rw-r--r--   0        0        0     2738 2023-06-02 15:27:50.643104 nnusf-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-02 15:27:50.643104 nnusf-0.3.0/src/nnusf/__init__.py
+-rw-r--r--   0        0        0      133 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/base.py
+-rw-r--r--   0        0        0     4109 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/data.py
+-rw-r--r--   0        0        0     2082 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/extra.py
+-rw-r--r--   0        0        0     3407 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/fit.py
+-rw-r--r--   0        0        0      201 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/log.py
+-rw-r--r--   0        0        0     5735 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/plot.py
+-rw-r--r--   0        0        0      879 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/report.py
+-rw-r--r--   0        0        0     6815 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/cli/theory.py
+-rw-r--r--   0        0        0      277 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/data/__init__.py
+-rw-r--r--   0        0        0     2989 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/data/coefficients.py
+-rw-r--r--   0        0        0     1002 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/data/combine_tables.py
+-rw-r--r--   0        0        0     1439 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/data/filters.py
+-rw-r--r--   0        0        0     6470 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/data/loader.py
+-rw-r--r--   0        0        0     9416 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/data/matching_grids.py
+-rw-r--r--   0        0        0    13188 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/data/utils.py
+-rwxr-xr-x   0        0        0     6128 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/filters/filter_bebcwa59.py
+-rwxr-xr-x   0        0        0     6675 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/filters/filter_ccfr.py
+-rwxr-xr-x   0        0        0    17661 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/filters/filter_cdhsw.py
+-rwxr-xr-x   0        0        0    10365 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/filters/filter_charm.py
+-rwxr-xr-x   0        0        0    11707 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/filters/filter_chorus.py
+-rwxr-xr-x   0        0        0     9449 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/filters/filter_nutev.py
+-rw-r--r--   0        0        0      104 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/get/__init__.py
+-rw-r--r--   0        0        0      172 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/get/base.py
+-rw-r--r--   0        0        0      698 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/get/gettheory.py
+-rw-r--r--   0        0        0      201 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/get/log.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/lhapdf/__init__.py
+-rw-r--r--   0        0        0     6001 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/lhapdf/dump_grids.py
+-rw-r--r--   0        0        0     9503 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/lhapdf/utils.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/covmat.py
+-rw-r--r--   0        0        0    17946 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/fit.py
+-rw-r--r--   0        0        0     4344 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/kinematics.py
+-rw-r--r--   0        0        0     3559 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/matching.py
+-rw-r--r--   0        0        0     2952 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/sf.py
+-rw-r--r--   0        0        0     5572 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/sfs_lhapdf.py
+-rw-r--r--   0        0        0     6132 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/th_covmat.py
+-rw-r--r--   0        0        0     7191 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plot/utils.py
+-rw-r--r--   0        0        0     1384 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/plotstyle.mplstyle
+-rw-r--r--   0        0        0        0 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/reports/__init__.py
+-rw-r--r--   0        0        0     7125 2023-06-02 15:26:22.857581 nnusf-0.3.0/src/nnusf/reports/assets/index.html
+-rwxr-xr-x   0        0        0    68365 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/reports/assets/report.css
+-rw-r--r--   0        0        0     9969 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/reports/genfiles.py
+-rw-r--r--   0        0        0     5641 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/reports/genhtml.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/scripts/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/scripts/gettheory.py
+-rw-r--r--   0        0        0     1369 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/scripts/integrate.py
+-rw-r--r--   0        0        0     3315 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/scripts/isoscalar.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/__init__.py
+-rw-r--r--   0        0        0     5283 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/callbacks.py
+-rw-r--r--   0        0        0     3339 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/compute_expchi2.py
+-rw-r--r--   0        0        0     2957 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/layers.py
+-rw-r--r--   0        0        0     3926 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/load_data.py
+-rw-r--r--   0        0        0     4238 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/load_fit_data.py
+-rw-r--r--   0        0        0     5351 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/model_gen.py
+-rw-r--r--   0        0        0     2603 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/postfit.py
+-rw-r--r--   0        0        0     3120 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/run_sffit.py
+-rw-r--r--   0        0        0     2241 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/scaling.py
+-rw-r--r--   0        0        0    11423 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/sum_rules.py
+-rw-r--r--   0        0        0     2728 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/train_model.py
+-rw-r--r--   0        0        0     8001 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/sffit/utils.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:26:22.861582 nnusf-0.3.0/src/nnusf/theory/__init__.py
+-rw-r--r--   0        0        0  1626320 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/assets/genie.hdf5
+-rw-r--r--   0        0        0      649 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/assets/theory_nnusf.yaml
+-rw-r--r--   0        0        0     1245 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/bodek_yang/__init__.py
+-rw-r--r--   0        0        0      157 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/bodek_yang/cuts.py
+-rw-r--r--   0        0        0     1532 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/bodek_yang/load.py
+-rw-r--r--   0        0        0      800 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/bodek_yang/runcards.py
+-rw-r--r--   0        0        0     4209 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/compare_to_data.py
+-rw-r--r--   0        0        0       47 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/data_vs_theory/__init__.py
+-rw-r--r--   0        0        0      646 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/data_vs_theory/runcards.py
+-rw-r--r--   0        0        0      885 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/defs.py
+-rw-r--r--   0        0        0     1991 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/grids.py
+-rw-r--r--   0        0        0       47 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/highq/__init__.py
+-rw-r--r--   0        0        0     1377 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/highq/load.py
+-rw-r--r--   0        0        0     3960 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/highq/runcards.py
+-rw-r--r--   0        0        0    12073 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/predictions.py
+-rw-r--r--   0        0        0     5969 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/runcards.py
+-rw-r--r--   0        0        0       47 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/yadknots/__init__.py
+-rw-r--r--   0        0        0     1187 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/theory/yadknots/runcards.py
+-rw-r--r--   0        0        0     6366 2023-06-02 15:26:22.873582 nnusf-0.3.0/src/nnusf/utils.py
+-rw-r--r--   0        0        0     1610 2023-06-02 15:26:22.873582 nnusf-0.3.0/tests/test_loader.py
+-rw-r--r--   0        0        0      156 2023-06-02 15:26:22.873582 nnusf-0.3.0/tests/theory/test_bodek_yang.py
+-rw-r--r--   0        0        0     4188 1970-01-01 00:00:00.000000 nnusf-0.3.0/PKG-INFO
```

### Comparing `nnusf-0.2.6/LICENSE` & `nnusf-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/README.md` & `nnusf-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/pyproject.toml` & `nnusf-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nnusf"
-version = "0.2.6"
+version = "0.3.0"
 description = "Predictions for all-energy neutrino structure functions"
 readme = "README.md"
 authors = [
   "Alessandro Candido <candido.ale@gmail.com>",
   "Alfonso Garcia <pochoarus@msn.com>",
   "Giacomo Magni <giac.magni@gmail.com>",
   "Tanjona R. Rabemananjara <tanjona.lspc@gmail.com>",
@@ -28,41 +28,63 @@
 ]
 packages = [{ include = "nnusf", from = "src" },]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 h5py = "^3.7.0"
 PyYAML = "^6.0"
-yadism = "^0.12.3"
+yadism = "0.12.3"
 pineappl = "^0.5.0"
 matplotlib = "^3.5.2"
 seaborn = "0.12.2"
 pandas = "^1.4.2"
 rich = "^12.5.1"
 scipy = "^1.8.1"
-tensorflow = "<2.9.10"
+tensorflow = "<2.11.2"
 pylint = "^2.14.4"
 appdirs = "^1.4.4"
 banana-hep = "^0.6.6"
 click = "^8.1.3"
 greenlet = "^1.1.2"
 pendulum = "^2.1.2"
 pytzdata = "^2020.1"
 SQLAlchemy = "^1.4.39"
 termcolor = "1.1.0"
 pygit2 = "^1.10.1"
 setuptools = "^65.5.1"
 particle = "^0.21.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1"
-pytest-cov = "^2.12.1"
+poethepoet = "^0.10.0"
+pylint = "^2.9.3"
 ipython = "^8.4.0"
 pdbpp = "^0.10.3"
 
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+pytest = "^6.2.4"
+pytest-cov = "^2.12.1"
+pytest-env = "^0.6.2"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = ">6.0"
+recommonmark = "^0.7.1"
+sphinxcontrib-bibtex = "^2.3.0"
+sphinxcontrib-details-directive = "^0.1.0"
+nbsphinx = "^0.8.6"
+furo = "^2023.5.20"
+m2r2 = "^0.3.3.post2"
+sphinx-design = "^0.4.1"
+sphinx-copybutton = "^0.5.2"
+
 [tool.poetry.scripts]
 nnu = "nnusf.cli:command"
 nns = "nnusf.get:command"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `nnusf-0.2.6/src/nnusf/cli/data.py` & `nnusf-0.3.0/src/nnusf/cli/data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/cli/extra.py` & `nnusf-0.3.0/src/nnusf/cli/extra.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/cli/fit.py` & `nnusf-0.3.0/src/nnusf/cli/fit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/cli/plot.py` & `nnusf-0.3.0/src/nnusf/cli/plot.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/cli/report.py` & `nnusf-0.3.0/src/nnusf/cli/report.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/cli/theory.py` & `nnusf-0.3.0/src/nnusf/cli/theory.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/data/coefficients.py` & `nnusf-0.3.0/src/nnusf/data/coefficients.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/data/combine_tables.py` & `nnusf-0.3.0/src/nnusf/data/combine_tables.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/data/filters.py` & `nnusf-0.3.0/src/nnusf/data/filters.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/data/loader.py` & `nnusf-0.3.0/src/nnusf/data/loader.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/data/matching_grids.py` & `nnusf-0.3.0/src/nnusf/data/matching_grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/data/utils.py` & `nnusf-0.3.0/src/nnusf/data/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/filters/filter_bebcwa59.py` & `nnusf-0.3.0/src/nnusf/filters/filter_bebcwa59.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/filters/filter_ccfr.py` & `nnusf-0.3.0/src/nnusf/filters/filter_ccfr.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/filters/filter_cdhsw.py` & `nnusf-0.3.0/src/nnusf/filters/filter_cdhsw.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/filters/filter_charm.py` & `nnusf-0.3.0/src/nnusf/filters/filter_charm.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/filters/filter_chorus.py` & `nnusf-0.3.0/src/nnusf/filters/filter_chorus.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/filters/filter_nutev.py` & `nnusf-0.3.0/src/nnusf/filters/filter_nutev.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/get/gettheory.py` & `nnusf-0.3.0/src/nnusf/get/gettheory.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/lhapdf/dump_grids.py` & `nnusf-0.3.0/src/nnusf/lhapdf/dump_grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/lhapdf/utils.py` & `nnusf-0.3.0/src/nnusf/lhapdf/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plot/covmat.py` & `nnusf-0.3.0/src/nnusf/plot/covmat.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plot/fit.py` & `nnusf-0.3.0/src/nnusf/plot/fit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plot/kinematics.py` & `nnusf-0.3.0/src/nnusf/plot/kinematics.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plot/matching.py` & `nnusf-0.3.0/src/nnusf/plot/matching.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plot/sf.py` & `nnusf-0.3.0/src/nnusf/plot/sf.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plot/sfs_lhapdf.py` & `nnusf-0.3.0/src/nnusf/plot/sfs_lhapdf.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plot/th_covmat.py` & `nnusf-0.3.0/src/nnusf/plot/th_covmat.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plot/utils.py` & `nnusf-0.3.0/src/nnusf/plot/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/plotstyle.mplstyle` & `nnusf-0.3.0/src/nnusf/plotstyle.mplstyle`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/reports/assets/index.html` & `nnusf-0.3.0/src/nnusf/reports/assets/index.html`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/reports/assets/report.css` & `nnusf-0.3.0/src/nnusf/reports/assets/report.css`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/reports/genfiles.py` & `nnusf-0.3.0/src/nnusf/reports/genfiles.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/reports/genhtml.py` & `nnusf-0.3.0/src/nnusf/reports/genhtml.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/scripts/gettheory.py` & `nnusf-0.3.0/src/nnusf/scripts/gettheory.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/scripts/integrate.py` & `nnusf-0.3.0/src/nnusf/scripts/integrate.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/scripts/isoscalar.py` & `nnusf-0.3.0/src/nnusf/scripts/isoscalar.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/callbacks.py` & `nnusf-0.3.0/src/nnusf/sffit/callbacks.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/compute_expchi2.py` & `nnusf-0.3.0/src/nnusf/sffit/compute_expchi2.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/layers.py` & `nnusf-0.3.0/src/nnusf/sffit/layers.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/load_data.py` & `nnusf-0.3.0/src/nnusf/sffit/load_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/load_fit_data.py` & `nnusf-0.3.0/src/nnusf/sffit/load_fit_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/model_gen.py` & `nnusf-0.3.0/src/nnusf/sffit/model_gen.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/postfit.py` & `nnusf-0.3.0/src/nnusf/sffit/postfit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/run_sffit.py` & `nnusf-0.3.0/src/nnusf/sffit/run_sffit.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/scaling.py` & `nnusf-0.3.0/src/nnusf/sffit/scaling.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/sum_rules.py` & `nnusf-0.3.0/src/nnusf/sffit/sum_rules.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/train_model.py` & `nnusf-0.3.0/src/nnusf/sffit/train_model.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/sffit/utils.py` & `nnusf-0.3.0/src/nnusf/sffit/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/assets/genie.hdf5` & `nnusf-0.3.0/src/nnusf/theory/assets/genie.hdf5`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/assets/theory_nnusf.yaml` & `nnusf-0.3.0/src/nnusf/theory/assets/theory_nnusf.yaml`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/bodek_yang/__init__.py` & `nnusf-0.3.0/src/nnusf/theory/bodek_yang/__init__.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/bodek_yang/load.py` & `nnusf-0.3.0/src/nnusf/theory/bodek_yang/load.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/bodek_yang/runcards.py` & `nnusf-0.3.0/src/nnusf/theory/bodek_yang/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/compare_to_data.py` & `nnusf-0.3.0/src/nnusf/theory/compare_to_data.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/data_vs_theory/runcards.py` & `nnusf-0.3.0/src/nnusf/theory/data_vs_theory/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/defs.py` & `nnusf-0.3.0/src/nnusf/theory/defs.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/grids.py` & `nnusf-0.3.0/src/nnusf/theory/grids.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/highq/load.py` & `nnusf-0.3.0/src/nnusf/theory/highq/load.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/highq/runcards.py` & `nnusf-0.3.0/src/nnusf/theory/highq/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/predictions.py` & `nnusf-0.3.0/src/nnusf/theory/predictions.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/runcards.py` & `nnusf-0.3.0/src/nnusf/theory/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/theory/yadknots/runcards.py` & `nnusf-0.3.0/src/nnusf/theory/yadknots/runcards.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/src/nnusf/utils.py` & `nnusf-0.3.0/src/nnusf/utils.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/tests/test_loader.py` & `nnusf-0.3.0/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `nnusf-0.2.6/PKG-INFO` & `nnusf-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: nnusf
-Version: 0.2.6
+Version: 0.3.0
 Summary: Predictions for all-energy neutrino structure functions
 Home-page: https://github.com/NNPDF/nnusf
 Author: Alessandro Candido
 Author-email: candido.ale@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: banana-hep (>=0.6.6,<0.7.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
@@ -29,17 +28,17 @@
 Requires-Dist: pygit2 (>=1.10.1,<2.0.0)
 Requires-Dist: pylint (>=2.14.4,<3.0.0)
 Requires-Dist: pytzdata (>=2020.1,<2021.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Requires-Dist: seaborn (==0.12.2)
 Requires-Dist: setuptools (>=65.5.1,<66.0.0)
-Requires-Dist: tensorflow (<2.9.10)
+Requires-Dist: tensorflow (<2.11.2)
 Requires-Dist: termcolor (==1.1.0)
-Requires-Dist: yadism (>=0.12.3,<0.13.0)
+Requires-Dist: yadism (==0.12.3)
 Project-URL: Repository, https://github.com/NNPDF/nnusf
 Description-Content-Type: text/markdown
 
 <h1 align="center">NNSFν</h1>
 <p align="center">
   <a href="https://zenodo.org/account/settings/github/repository/NNPDF/nnusf#"><img alt="Zenodo" src="https://zenodo.org/badge/DOI/10.5281/zenodo.7657132 .svg"></a>
   <a href="https://arxiv.org/abs/2302.08527"><img alt="arXiv" src="https://img.shields.io/badge/arXiv-2302.08527-b31b1b?labelColor=222222"></a>
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: nnusf Version: 0.2.6 Summary: Predictions for all-
+Metadata-Version: 2.1 Name: nnusf Version: 0.3.0 Summary: Predictions for all-
 energy neutrino structure functions Home-page: https://github.com/NNPDF/nnusf
 Author: Alessandro Candido Author-email: candido.ale@gmail.com Requires-Python:
 >=3.9,<3.11 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering Classifier:
-Topic :: Scientific/Engineering :: Physics Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0) Requires-Dist: appdirs
-(>=1.4.4,<2.0.0) Requires-Dist: banana-hep (>=0.6.6,<0.7.0) Requires-Dist:
-click (>=8.1.3,<9.0.0) Requires-Dist: greenlet (>=1.1.2,<2.0.0) Requires-Dist:
-h5py (>=3.7.0,<4.0.0) Requires-Dist: matplotlib (>=3.5.2,<4.0.0) Requires-Dist:
-pandas (>=1.4.2,<2.0.0) Requires-Dist: particle (>=0.21.2,<0.22.0) Requires-
-Dist: pendulum (>=2.1.2,<3.0.0) Requires-Dist: pineappl (>=0.5.0,<0.6.0)
-Requires-Dist: pygit2 (>=1.10.1,<2.0.0) Requires-Dist: pylint (>=2.14.4,<3.0.0)
-Requires-Dist: pytzdata (>=2020.1,<2021.0) Requires-Dist: rich
-(>=12.5.1,<13.0.0) Requires-Dist: scipy (>=1.8.1,<2.0.0) Requires-Dist: seaborn
-(==0.12.2) Requires-Dist: setuptools (>=65.5.1,<66.0.0) Requires-Dist:
-tensorflow (<2.9.10) Requires-Dist: termcolor (==1.1.0) Requires-Dist: yadism
-(>=0.12.3,<0.13.0) Project-URL: Repository, https://github.com/NNPDF/nnusf
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.10 Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: SQLAlchemy (>=1.4.39,<2.0.0)
+Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: banana-hep
+(>=0.6.6,<0.7.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: greenlet
+(>=1.1.2,<2.0.0) Requires-Dist: h5py (>=3.7.0,<4.0.0) Requires-Dist: matplotlib
+(>=3.5.2,<4.0.0) Requires-Dist: pandas (>=1.4.2,<2.0.0) Requires-Dist: particle
+(>=0.21.2,<0.22.0) Requires-Dist: pendulum (>=2.1.2,<3.0.0) Requires-Dist:
+pineappl (>=0.5.0,<0.6.0) Requires-Dist: pygit2 (>=1.10.1,<2.0.0) Requires-
+Dist: pylint (>=2.14.4,<3.0.0) Requires-Dist: pytzdata (>=2020.1,<2021.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0) Requires-Dist: scipy (>=1.8.1,<2.0.0)
+Requires-Dist: seaborn (==0.12.2) Requires-Dist: setuptools (>=65.5.1,<66.0.0)
+Requires-Dist: tensorflow (<2.11.2) Requires-Dist: termcolor (==1.1.0)
+Requires-Dist: yadism (==0.12.3) Project-URL: Repository, https://github.com/
+NNPDF/nnusf Description-Content-Type: text/markdown
                              ****** NNSFÎ½ ******
                [Zenodo] [arXiv] [Docs] [PyPI] [Status] [License]
 NNSFÎ½ is a python module that provides predictions for neutrino structure
 functions. It relies on YADISM for the large-Q region while the low-Q regime is
 modelled in terms of a Neural Network (NN). The NNSFÎ½ determination is also
 made available in terms of fast interpolation LHAPDF grids that can be accessed
 through an independent driver code and directly interfaced to the GENIE Monte
```

