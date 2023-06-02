# Comparing `tmp/linear_operator-0.4.0.tar.gz` & `tmp/linear_operator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear_operator-0.4.0.tar", last modified: Fri Apr 14 20:49:42 2023, max compression
+gzip compressed data, was "linear_operator-0.5.0.tar", last modified: Fri Jun  2 19:27:08 2023, max compression
```

## Comparing `linear_operator-0.4.0.tar` & `linear_operator-0.5.0.tar`

### file list

```diff
@@ -1,177 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.232299 linear_operator-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.216298 linear_operator-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/documentation_examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/refactor.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/workflows/run_test_suite.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-14 20:49:29.000000 linear_operator-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 20:49:29.000000 linear_operator-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-04-14 20:49:42.232299 linear_operator-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-04-14 20:49:29.000000 linear_operator-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/composition_decoration_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/converting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/custom_linear_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/data_sparse_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/linear_operator.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/namespace.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-04-14 20:49:29.000000 linear_operator-0.4.0/examples/LinearOperator_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/linear_operator/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.224299 linear_operator-0.4.0/linear_operator/functions/
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_dsmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_inv_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_inv_quad_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_root_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_sqrt_inv_matmul.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/linear_operator/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121537 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14269 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/batch_repeat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/block_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/block_interleaved_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/block_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19700 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/cat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/chol_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/constant_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/dense_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/identity_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/interpolated_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/keops_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/kronecker_product_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/linear_operator_representation_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/low_rank_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/matmul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/permutation_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/psd_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/sum_batch_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/sum_kronecker_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/toeplitz_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/triangular_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/zero_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/linear_operator/test/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/test/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    55783 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/test/linear_operator_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/linear_operator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/broadcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/contour_integral_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/lanczos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/minres.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/permutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/pinverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/stochastic_lq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/toeplitz.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.224299 linear_operator-0.4.0/linear_operator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-14 20:49:42.000000 linear_operator-0.4.0/linear_operator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-14 20:49:29.000000 linear_operator-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 20:49:42.236299 linear_operator-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-14 20:49:29.000000 linear_operator-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/test/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_dsmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_inv_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_inv_quad_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_root_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.232299 linear_operator-0.4.0/test/operators/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_batch_repeat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_block_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_block_interleaved_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_cat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_chol_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_constant_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_dense_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_identity_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_interpolated_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_kronecker_product_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_kronecker_product_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_low_rank_root_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_low_rank_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_matmul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_permutation_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_psd_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_sum_batch_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_sum_kronecker_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_toeplitz_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_triangular_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_zero_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.232299 linear_operator-0.4.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_lanczos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_minres.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_permutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_toeplitz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.208408 linear_operator-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.184408 linear_operator-0.5.0/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.180408 linear_operator-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.184408 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/documentation_examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/ISSUE_TEMPLATE/refactor.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.184408 linear_operator-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/push_to_main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/run_linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/run_test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.github/workflows/run_type_checked_test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.184408 linear_operator-0.5.0/.hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.hooks/check_type_hints.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.hooks/propagate_type_hints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.hooks/propagate_type_hints.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-02 19:26:50.000000 linear_operator-0.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-02 19:26:50.000000 linear_operator-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 19:26:50.000000 linear_operator-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-02 19:27:08.208408 linear_operator-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-06-02 19:26:50.000000 linear_operator-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/composition_decoration_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/converting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/custom_linear_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/data_sparse_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/linear_operator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/namespace.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-02 19:26:50.000000 linear_operator-0.5.0/docs/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-02 19:26:50.000000 linear_operator-0.5.0/examples/LinearOperator_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/linear_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.192408 linear_operator-0.5.0/linear_operator/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)    12107 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_dsmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_inv_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_inv_quad_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_root_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/functions/_sqrt_inv_matmul.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.196408 linear_operator-0.5.0/linear_operator/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129865 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16356 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/batch_repeat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/block_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/block_interleaved_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/block_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/cat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/chol_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/constant_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/dense_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/identity_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22567 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/interpolated_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/keops_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21149 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/kernel_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16274 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23172 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/kronecker_product_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/linear_operator_representation_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/low_rank_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/matmul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/permutation_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/psd_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/sum_batch_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/sum_kronecker_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/toeplitz_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/triangular_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/operators/zero_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.196408 linear_operator-0.5.0/linear_operator/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56208 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/linear_operator_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/type_checking_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.200408 linear_operator-0.5.0/linear_operator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/broadcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/contour_integral_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/minres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/pinverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/stochastic_lq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/toeplitz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-02 19:26:50.000000 linear_operator-0.5.0/linear_operator/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.188408 linear_operator-0.5.0/linear_operator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-06-02 19:27:08.000000 linear_operator-0.5.0/linear_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 19:27:07.000000 linear_operator-0.5.0/linear_operator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-02 19:26:50.000000 linear_operator-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-02 19:27:08.208408 linear_operator-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-02 19:26:50.000000 linear_operator-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.200408 linear_operator-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.204408 linear_operator-0.5.0/test/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_dsmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_inv_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_inv_quad_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_root_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/functions/test_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.208408 linear_operator-0.5.0/test/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_batch_repeat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_block_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_block_interleaved_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_cat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_chol_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_constant_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_dense_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_identity_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_interpolated_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_kernel_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_kronecker_product_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_kronecker_product_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_low_rank_root_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_low_rank_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_matmul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_permutation_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_psd_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_sum_batch_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_sum_kronecker_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_toeplitz_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_triangular_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/operators/test_zero_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 19:27:08.208408 linear_operator-0.5.0/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_minres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-02 19:26:50.000000 linear_operator-0.5.0/test/utils/test_toeplitz.py
```

### Comparing `linear_operator-0.4.0/.conda/meta.yaml` & `linear_operator-0.5.0/.conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md` & `linear_operator-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/.github/ISSUE_TEMPLATE/documentation_examples.md` & `linear_operator-0.5.0/.github/ISSUE_TEMPLATE/documentation_examples.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md` & `linear_operator-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/.github/workflows/deploy.yml` & `linear_operator-0.5.0/.github/workflows/deploy.yml`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 name: Upload Python Package to PyPI and Anaconda
 
 on:
   release:
     types: [created]
 
 jobs:
+  run_linter:
+    uses: ./.github/workflows/run_linter.yml
+
   run_test_suite:
-    uses: ./.github/workflows/run_test_suite.yml
+    uses: ./.github/workflows/run_type_checked_test_suite.yml
 
   deploy_pypi:
     runs-on: ubuntu-latest
     needs: run_test_suite
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
```

### Comparing `linear_operator-0.4.0/.github/workflows/run_test_suite.yml` & `linear_operator-0.5.0/.github/workflows/run_test_suite.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,16 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Run Test Suite
 
 on:
-  push:
-    branches: [ main ]
-  pull_request:
-    branches: [ main ]
   workflow_call:
 
 jobs:
-  run_linter:
-    runs-on: ubuntu-latest
-    steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python
-      uses: actions/setup-python@v2
-      with:
-        python-version: "3.8"
-    - name: Install dependencies
-      run: |
-        pip install flake8==5.0.4 flake8-print==5.0.0 pre-commit
-        pre-commit install
-        pre-commit run seed-isort-config || true
-    - name: Run linting
-      run: |
-        flake8
-    - name: Run pre-commit checks
-      # skipping flake8 here (run separatey above b/c pre-commit does not include flake8-print)
-      run: |
-        SKIP=flake8 pre-commit run --files test/**/*.py linear_operator/**/*.py
-
   run_unit_tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         pytorch-version: ["latest", "stable"]
     steps:
     - uses: actions/checkout@v2
@@ -46,11 +21,11 @@
     - name: Install dependencies
       run: |
         if [[ ${{ matrix.pytorch-version }} = "latest" ]]; then
           pip install --pre torch -f https://download.pytorch.org/whl/nightly/cpu/torch_nightly.html;
         else
           pip install torch==1.11+cpu -f https://download.pytorch.org/whl/torch_stable.html;
         fi
-        pip install -e .
+        pip install -e ".[test]"
     - name: Run unit tests
       run: |
         python -m unittest discover
```

### Comparing `linear_operator-0.4.0/.gitignore` & `linear_operator-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/.pre-commit-config.yaml` & `linear_operator-0.5.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -34,7 +34,15 @@
     -   id: forbid-binary
         exclude: ^(examples/*)|(test/examples/old_variational_strategy_model.pth)
 -   repo: https://github.com/Lucas-C/pre-commit-hooks
     rev: v1.3.1
     hooks:
     -   id: forbid-crlf
     -   id: forbid-tabs
+-   repo: local
+    hooks:
+    -   id: propagate-type-hints
+        name: Propagate Type Hints
+        entry: ./.hooks/propagate_type_hints.sh
+        language: script
+        pass_filenames: true
+        require_serial: true
```

### Comparing `linear_operator-0.4.0/.readthedocs.yml` & `linear_operator-0.5.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/CONTRIBUTING.md` & `linear_operator-0.5.0/CONTRIBUTING.md`

 * *Files 18% similar despite different names*

```diff
@@ -36,30 +36,56 @@
 
 
 ### Type Hints
 
 LinearOperator aims to be fully typed using Python 3.8+
 [type hints](https://www.python.org/dev/peps/pep-0484/).
 We expect any contributions to also use proper type annotations.
-While we currently do not enforce full consistency of these in our continuous integration
-test, you should strive to type check your code locally.
-For this we recommend using [pyre](https://pyre-check.org/).
-
+We are using [jaxtyping](https://github.com/google/jaxtyping) to help us be declarative about the dimension sizes used
+in the LinearOperator methods.
+The use of [jaxtyping](https://github.com/google/jaxtyping)  makes it clearer what the functions are doing algebraically
+and where broadcasting is happening.
+
+These type hints are checked in the unit tests by using
+[typeguard](https://github.com/agronholm/typeguard) to perform run-time
+checking of the signatures to make sure they are accurate.
+The signatures are written into the base linear operator class in `_linear_oparator.py`.
+These signatures are then copied to the derived classes by running the script
+`python ./.hooks/propagate_type_hints.py`.
+This is done for:
+1. Consistency. Make sure the derived implementations are following the promised interface.
+2. Visibility. Make it easy to see what the expected signature is, along with dimensions. Repeating the signature in the derived classes enhances readability.
+3. Necessity. The way that jaxtyping and typeguard are written, they won't run type checks unless type annotations are present in the derived method signature.
+
+In short, if you want to update the type hints, update the code in the LinearOperator class in
+`_linear_oparator.py` then run `python ./.hooks/propagate_type_hints.py` to copy the new signature to the derived
+classes.
 
 ### Unit Tests
 
+#### With type checking (slower, but more thorough)
+To run the unittests with type checking, run
+```bash
+pytest --jaxtyping-packages=linear_operator,typeguard.typechecked
+```
+
+- To run tests within a specific directory, run (e.g.) `pytest test/operators --jaxtyping-packages=linear_operator,typeguard.typechecked`.
+- To run a specific file, run (e.g.) `pytest test/operators/test_matmul_linear_operator.py --jaxtyping-packages=linear_operator,typeguard.typechecked`.
+
+#### Without type checking (faster, but less thorough)
 We use python's `unittest` to run unit tests:
 ```bash
 python -m unittest
 ```
 
 - To run tests within a specific directory, run (e.g.) `python -m unittest discover -s test/operators`.
 - To run a specific unit test, run (e.g.) `python -m unittest test.operators.test_matmul_linear_operator.TestMatmulLinearOperator.test_matmul_vec`.
 
 
+
 ### Documentation
 
 LinearOperator uses sphinx to generate documentation, and ReadTheDocs to host documentation.
 To build the documentation locally, ensure that sphinx and its plugins are properly installed (see the [development installation section](#development-installation) for instructions).
 Then run:
 
 ```baseh
```

### Comparing `linear_operator-0.4.0/LICENSE` & `linear_operator-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/PKG-INFO` & `linear_operator-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear_operator
-Version: 0.4.0
+Version: 0.5.0
 Summary: A linear operator implementation, primarily designed for finite-dimensional positive definite operators (i.e. kernel matrices).
 Home-page: UNKNOWN
 Author: Geoff Pleiss
 Author-email: gpleiss@gmail.com
 License: MIT
 Project-URL: Documentation, https://linear_operator.readthedocs.io
 Project-URL: Source, https://github.com/cornellius-gp/linear_operator/
```

### Comparing `linear_operator-0.4.0/README.md` & `linear_operator-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/docs/Makefile` & `linear_operator-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/docs/make.bat` & `linear_operator-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/docs/source/composition_decoration_operators.rst` & `linear_operator-0.5.0/docs/source/composition_decoration_operators.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/docs/source/conf.py` & `linear_operator-0.5.0/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 # sys.path.insert(0, os.path.abspath('.'))
 
 import os
 import sys
 import warnings
 from typing import ForwardRef
 
+import jaxtyping
 import sphinx_rtd_theme  # noqa
+from uncompyle6.semantics.fragments import code_deparse
 
 
 sys.path.append(os.path.abspath(os.path.join(__file__, "..", "..", "..")))
 
 # -- Project information -----------------------------------------------------
 
 project = "linear_operator"
@@ -90,64 +92,103 @@
 
 # Disable documentation inheritance so as to avoid inheriting
 # docstrings in a different format, e.g. when the parent class
 # is a PyTorch class.
 
 autodoc_inherit_docstrings = False
 
-# Function to format type hints
+
+# Helper function
+# Convert any class (i.e. torch.Tensor, LinearOperator, etc.) into appropriate strings
+# For external classes, the format will be e.g. "torch.Tensor"
+# For any internal class, the format will be e.g. "~linear_operator.operators.TriangularLinearOperator"
+def _convert_internal_and_external_class_to_strings(annotation):
+    module = annotation.__module__ + "."
+    if module.split(".")[0] == "linear_operator":
+        module = "~" + module
+    elif module == "builtins.":
+        module = ""
+    res = f"{module}{annotation.__name__}"
+    return res
 
 
+# Convert jaxtyping dimensions into strings
+def _dim_to_str(dim):
+    if isinstance(dim, jaxtyping.array_types._NamedVariadicDim):
+        return "..."
+    elif isinstance(dim, jaxtyping.array_types._FixedDim):
+        res = str(dim.size)
+        if dim.broadcastable:
+            res = "#" + res
+        return res
+    elif isinstance(dim, jaxtyping.array_types._SymbolicDim):
+        expr = code_deparse(dim.expr).text.strip().split("return ")[1]
+        return f"({expr})"
+    elif "jaxtyping" not in str(dim.__class__):  # Probably the case that we have an ellipsis
+        return "..."
+    else:
+        res = str(dim.name)
+        if dim.broadcastable:
+            res = "#" + res
+        return res
+
+
+# Function to format type hints
 def _process(annotation, config):
     """
     A function to convert a type/rtype typehint annotation into a :type:/:rtype: string.
     This function is a bit hacky, and specific to the type annotations we use most frequently.
 
     This function is recursive.
     """
     # Simple/base case: any string annotation is ready to go
     if type(annotation) == str:
         return annotation
 
+    # Jaxtyping: shaped tensors or linear operator
+    elif hasattr(annotation, "__module__") and "jaxtyping" == annotation.__module__:
+        cls_annotation = _convert_internal_and_external_class_to_strings(annotation.array_type)
+        shape = " x ".join([_dim_to_str(dim) for dim in annotation.dims])
+        return f"{cls_annotation} ({shape})"
+
     # Convert Ellipsis into "..."
     elif annotation == Ellipsis:
         return "..."
 
     # Convert any class (i.e. torch.Tensor, LinearOperator, etc.) into appropriate strings
-    # For external classes, the format will be e.g. "torch.Tensor"
-    # For any internal class, the format will be e.g. "~linear_operator.operators.TriangularLinearOperator"
     elif hasattr(annotation, "__name__"):
-        module = annotation.__module__ + "."
-        if module.split(".")[0] == "linear_operator":
-            module = "~" + module
-        elif module == "builtins.":
-            module = ""
-        res = f"{module}{annotation.__name__}"
+        res = _convert_internal_and_external_class_to_strings(annotation)
+
+    elif str(annotation).startswith("typing.Callable"):
+        if len(annotation.__args__) == 2:
+            res = f"Callable[{_process(annotation.__args__[0], config)} -> {_process(annotation.__args__[1], config)}]"
+        else:
+            res = "Callable"
 
     # Convert any Union[*A*, *B*, *C*] into "*A* or *B* or *C*"
     # Also, convert any Optional[*A*] into "*A*, optional"
-    elif "typing.Union" in str(annotation):
+    elif str(annotation).startswith("typing.Union"):
         is_optional_str = ""
         args = list(annotation.__args__)
         # Hack: Optional[*A*] are represented internally as Union[*A*, Nonetype]
         # This catches this case
         if args[-1] is type(None):  # noqa E721
             del args[-1]
             is_optional_str = ", optional"
         processed_args = [_process(arg, config) for arg in args]
         res = " or ".join(processed_args) + is_optional_str
 
     # Convert any Tuple[*A*, *B*] into "(*A*, *B*)"
-    elif "typing.Tuple" in str(annotation):
+    elif str(annotation).startswith("typing.Tuple"):
         args = list(annotation.__args__)
         res = "(" + ", ".join(_process(arg, config) for arg in args) + ")"
 
     # Callable typing annotation
-    elif "typing." in str(annotation):
-        return str(annotation)
+    elif str(annotation).startswith("typing."):
+        return str(annotation)[7:]
 
     # Special cases for forward references.
     # This is brittle, as it only contains case for a select few forward refs
     # All others that aren't caught by this are handled by the final case
     elif isinstance(annotation, ForwardRef):
         res = str(annotation.__forward_arg__)
         if res == "LinearOperator":
@@ -161,15 +202,15 @@
         res = str(annotation)
 
     return res
 
 
 # Options for typehints
 
-always_document_param_types = True
+always_document_param_types = False
 # typehints_use_rtype = False
 typehints_defaults = None  # or "comma"
 simplify_optional_unions = False
 typehints_formatter = _process
 
 # Taken from https://github.com/pyro-ppl/pyro/blob/dev/docs/source/conf.py#L213
 # @jpchen's hack to get rtd builder to install latest pytorch
```

### Comparing `linear_operator-0.4.0/docs/source/custom_linear_operators.rst` & `linear_operator-0.5.0/docs/source/custom_linear_operators.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/docs/source/data_sparse_operators.rst` & `linear_operator-0.5.0/docs/source/data_sparse_operators.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 
 :hidden:`IdentityLinearOperator`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: linear_operator.operators.IdentityLinearOperator
    :members:
 
+:hidden:`KernelLinearOperator`
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: linear_operator.operators.KernelLinearOperator
+   :members:
+
 :hidden:`RootLinearOperator`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: linear_operator.operators.RootLinearOperator
    :members:
 
 :hidden:`ToeplitzLinearOperator`
```

### Comparing `linear_operator-0.4.0/docs/source/index.rst` & `linear_operator-0.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/docs/source/namespace.rst` & `linear_operator-0.5.0/docs/source/namespace.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/examples/LinearOperator_demo.ipynb` & `linear_operator-0.5.0/examples/LinearOperator_demo.ipynb`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/__init__.py` & `linear_operator-0.5.0/linear_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/beta_features.py` & `linear_operator-0.5.0/linear_operator/beta_features.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/functions/__init__.py` & `linear_operator-0.5.0/linear_operator/functions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
-from typing import Optional, Tuple, Union
+from typing import Any, Optional, Tuple, Union
 
 import torch
 
 from ._dsmm import DSMM
 
-Anysor = Union["LinearOperator", torch.Tensor]  # noqa F811
+LinearOperatorType = Any  # Want this to be "LinearOperator" but runtime type checker can't handle
 
 
-def add_diagonal(input: Anysor, diag: torch.Tensor) -> "LinearOperator":  # noqa F811
+Anysor = Union[LinearOperatorType, torch.Tensor]
+
+
+def add_diagonal(input: Anysor, diag: torch.Tensor) -> LinearOperatorType:
     r"""
     Adds an element to the diagonal of the matrix :math:`\mathbf A`.
 
     :param input: The matrix (or batch of matrices) :math:`\mathbf A` (... x N x N).
     :param diag: Diagonal to add
     :return: :math:`\mathbf A + \text{diag}(\mathbf d)`, where :math:`\mathbf A` is the linear operator
         and :math:`\mathbf d` is the diagonal component
@@ -40,15 +43,17 @@
     if hasattr(input, "add_jitter"):
         return input.add_jitter(jitter_val)
     else:
         diag = torch.eye(input.size(-1), dtype=input.dtype, device=input.device).mul_(jitter_val)
         return input + diag
 
 
-def diagonalization(input: Anysor, method: Optional[str] = None) -> Tuple[torch.Tensor, torch.Tensor]:
+def diagonalization(
+    input: Anysor, method: Optional[str] = None
+) -> Tuple[torch.Tensor, Union[torch.Tensor, LinearOperatorType]]:
     r"""
     Returns a (usually partial) diagonalization of a symmetric positive definite matrix (or batch of matrices).
     :math:`\mathbf A`.
     Options are either "lanczos" or "symeig". "lanczos" runs Lanczos while
     "symeig" runs LinearOperator.symeig.
 
     :param input: The matrix (or batch of matrices) :math:`\mathbf A` (... x N x N).
@@ -102,19 +107,16 @@
     """
     from ..operators import to_linear_operator
 
     return to_linear_operator(input).inv_quad(inv_quad_rhs, reduce_inv_quad=reduce_inv_quad)
 
 
 def inv_quad_logdet(
-    input: Anysor,
-    inv_quad_rhs: Optional[torch.Tensor] = None,
-    logdet: bool = False,
-    reduce_inv_quad: bool = True,
-) -> Tuple[torch.Tensor, torch.Tensor]:
+    input: Anysor, inv_quad_rhs: Optional[torch.Tensor] = None, logdet: bool = False, reduce_inv_quad: bool = True
+) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor]]:
     r"""
     Calls both :func:`inv_quad_logdet` and :func:`logdet` on a positive definite matrix (or batch) :math:`\mathbf A`.
     However, calling this method is far more efficient and stable than calling each method independently.
 
     :param input: :math:`\mathbf A` - the positive definite matrix (... X N X N)
     :param inv_quad_rhs: :math:`\mathbf R` - the right hand sides of the inverse quadratic term (... x N x M)
     :param logdet: Whether or not to compute the
@@ -127,18 +129,15 @@
     """
     from ..operators import to_linear_operator
 
     return to_linear_operator(input).inv_quad_logdet(inv_quad_rhs, logdet, reduce_inv_quad=reduce_inv_quad)
 
 
 def pivoted_cholesky(
-    input: Anysor,
-    rank: int,
-    error_tol: Optional[float] = None,
-    return_pivots: bool = False,
+    input: Anysor, rank: int, error_tol: Optional[float] = None, return_pivots: bool = False
 ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
     r"""
     Performs a partial pivoted Cholesky factorization of a positive definite matrix (or batch of matrices).
     :math:`\mathbf L \mathbf L^\top = \mathbf A`.
     The partial pivoted Cholesky factor :math:`\mathbf L \in \mathbb R^{N \times \text{rank}}`
     forms a low rank approximation to the LinearOperator.
 
@@ -158,15 +157,15 @@
         https://www.sciencedirect.com/science/article/pii/S0168927411001814
     """
     from ..operators import to_linear_operator
 
     return to_linear_operator(input).pivoted_cholesky(rank=rank, error_tol=error_tol, return_pivots=return_pivots)
 
 
-def root_decomposition(input: Anysor, method: Optional[str] = None) -> "LinearOperator":  # noqa F811
+def root_decomposition(input: Anysor, method: Optional[str] = None) -> LinearOperatorType:
     r"""
     Returns a (usually low-rank) root decomposition linear operator of the
     positive definite matrix (or batch of matrices) :math:`\mathbf A`.
     This can be used for sampling from a Gaussian distribution, or for obtaining a
     low-rank version of a matrix.
 
     :param input: The matrix (or batch of matrices) :math:`\mathbf A` (... x N x N).
@@ -180,15 +179,15 @@
 
 
 def root_inv_decomposition(
     input: Anysor,
     initial_vectors: Optional[torch.Tensor] = None,
     test_vectors: Optional[torch.Tensor] = None,
     method: Optional[str] = None,
-) -> "LinearOperator":  # noqa F811
+) -> LinearOperatorType:
     r"""
     Returns a (usually low-rank) inverse root decomposition linear operator
     of the PSD LinearOperator :math:`\mathbf A`.
     This can be used for sampling from a Gaussian distribution, or for obtaining a
     low-rank version of a matrix.
 
     The root_inv_decomposition is performed using a partial Lanczos tridiagonalization.
@@ -237,15 +236,17 @@
     :return: :math:`\mathbf A^{-1} \mathbf R` or :math:`\mathbf L \mathbf A^{-1} \mathbf R`.
     """
     from ..operators import to_linear_operator
 
     return to_linear_operator(input).solve(right_tensor=rhs, left_tensor=lhs)
 
 
-def sqrt_inv_matmul(input: Anysor, rhs: torch.Tensor, lhs: Optional[torch.Tensor] = None) -> torch.Tensor:
+def sqrt_inv_matmul(
+    input: Anysor, rhs: torch.Tensor, lhs: Optional[torch.Tensor] = None
+) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
     r"""
     Given a positive definite matrix (or batch of matrices) :math:`\mathbf A`
     and a right hand size :math:`\mathbf R`,
     computes
 
     .. math::
        \begin{equation}
```

### Comparing `linear_operator-0.4.0/linear_operator/functions/_diagonalization.py` & `linear_operator-0.5.0/linear_operator/functions/_diagonalization.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/functions/_inv_quad.py` & `linear_operator-0.5.0/linear_operator/functions/_inv_quad.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/functions/_inv_quad_logdet.py` & `linear_operator-0.5.0/linear_operator/functions/_inv_quad_logdet.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/functions/_matmul.py` & `linear_operator-0.5.0/linear_operator/functions/_matmul.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/functions/_pivoted_cholesky.py` & `linear_operator-0.5.0/linear_operator/functions/_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/functions/_root_decomposition.py` & `linear_operator-0.5.0/linear_operator/functions/_root_decomposition.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/functions/_solve.py` & `linear_operator-0.5.0/linear_operator/functions/_solve.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/functions/_sqrt_inv_matmul.py` & `linear_operator-0.5.0/linear_operator/functions/_sqrt_inv_matmul.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/operators/__init__.py` & `linear_operator-0.5.0/linear_operator/operators/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .chol_linear_operator import CholLinearOperator
 from .constant_mul_linear_operator import ConstantMulLinearOperator
 from .dense_linear_operator import DenseLinearOperator, to_linear_operator
 from .diag_linear_operator import ConstantDiagLinearOperator, DiagLinearOperator
 from .identity_linear_operator import IdentityLinearOperator
 from .interpolated_linear_operator import InterpolatedLinearOperator
 from .keops_linear_operator import KeOpsLinearOperator
+from .kernel_linear_operator import KernelLinearOperator
 from .kronecker_product_added_diag_linear_operator import KroneckerProductAddedDiagLinearOperator
 from .kronecker_product_linear_operator import (
     KroneckerProductDiagLinearOperator,
     KroneckerProductLinearOperator,
     KroneckerProductTriangularLinearOperator,
 )
 from .low_rank_root_added_diag_linear_operator import LowRankRootAddedDiagLinearOperator
@@ -49,14 +50,15 @@
     "ConstantDiagLinearOperator",
     "ConstantMulLinearOperator",
     "DenseLinearOperator",
     "DiagLinearOperator",
     "IdentityLinearOperator",
     "InterpolatedLinearOperator",
     "KeOpsLinearOperator",
+    "KernelLinearOperator",
     "KroneckerProductLinearOperator",
     "KroneckerProductAddedDiagLinearOperator",
     "KroneckerProductDiagLinearOperator",
     "KroneckerProductTriangularLinearOperator",
     "SumKroneckerLinearOperator",
     "LowRankRootAddedDiagLinearOperator",
     "LowRankRootLinearOperator",
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/_linear_operator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
 import functools
+import itertools
 import math
 import numbers
 import warnings
-from abc import ABC, abstractmethod
+from abc import abstractmethod
+from collections import OrderedDict
 from copy import deepcopy
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+import numpy as np
 import torch
+
+try:
+    # optional library for advanced type signatures
+    from jaxtyping import Float, Int
+except ImportError:
+    pass
 from torch import Tensor
 
 import linear_operator
 
 from .. import settings, utils
 from ..functions._diagonalization import Diagonalization
 from ..functions._inv_quad import InvQuad
@@ -31,14 +40,15 @@
 from ..utils.generic import _to_helper
 from ..utils.getitem import (
     _compute_getitem_size,
     _convert_indices_to_tensors,
     _is_noop_index,
     _is_tensor_index_moved_to_start,
     _noop_index,
+    IndexType,
 )
 from ..utils.lanczos import _postprocess_lanczos_root_inv_decomp
 from ..utils.memoize import _is_in_cache_ignore_all_args, _is_in_cache_ignore_args, add_to_cache, cached, pop_from_cache
 from ..utils.pinverse import stable_pinverse
 from ..utils.warnings import NumericalWarning, PerformanceWarning
 from .linear_operator_representation_tree import LinearOperatorRepresentationTree
 
@@ -96,17 +106,19 @@
         _HANDLED_FUNCTIONS[torch_function] = func.__name__
         _HANDLED_SECOND_ARG_FUNCTIONS[torch_function] = func.__name__
         return func
 
     return decorator
 
 
-class LinearOperator(ABC):
+class LinearOperator(object):
     r"""
     Base class for LinearOperators.
+    Unless otherwise stated, we assume that the LinearOperator represents a matrix
+    (or batch of matrices) of size (... x M x N).
 
     :ivar int batch_dim: The number of batch dimensions defined by the
         :obj:`~linear_operator.LinearOperator`.
         (This should be equal to `linear_operator.dim() - 2`.
     :ivar torch.Size batch_shape: The shape over which the
         :obj:`~linear_operator.LinearOperator` is batched.
     :ivar torch.device device: The device that the :obj:`~linear_operator.LinearOperator`
@@ -136,21 +148,32 @@
     def __init__(self, *args, **kwargs):
         if settings.debug.on():
             err = self._check_args(*args, **kwargs)
             if err is not None:
                 raise ValueError(err)
 
         self._args = args
-        self._kwargs = kwargs
+        self._differentiable_kwargs = OrderedDict()
+        self._nondifferentiable_kwargs = dict()
+        for name, val in sorted(kwargs.items()):
+            # Sorting is necessary so that the flattening in the representation tree is deterministic
+            if torch.is_tensor(val) or isinstance(val, LinearOperator):
+                self._differentiable_kwargs[name] = val
+            else:
+                self._nondifferentiable_kwargs[name] = val
 
     ####
     # The following methods need to be defined by the LinearOperator
     ####
+
     @abstractmethod
-    def _matmul(self, rhs: torch.Tensor) -> torch.Tensor:
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         r"""
         Performs a matrix multiplication :math:`\mathbf KM` with the (... x M x N) matrix :math:`\mathbf K`
         that this LinearOperator represents. Should behave as
         :func:`torch.matmul`. If the LinearOperator represents a batch of
         matrices, this method should therefore operate in batch mode as well.
 
         ..note::
@@ -176,15 +199,15 @@
             which does some additional work. Calling this method directly is discouraged.
 
         :return: The size of the (batched) matrix :math:`\mathbf K` represented by this LinearOperator
         """
         raise NotImplementedError("The class {} requires a _size function!".format(self.__class__.__name__))
 
     @abstractmethod
-    def _transpose_nonbatch(self) -> LinearOperator:
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         """
         Transposes non-batch dimensions (e.g. last two)
         Implement this method, rather than transpose() or t().
 
         ..note::
             This method is used internally by the related function
             :func:`~linear_operator.LinearOperator.transpose`, which
@@ -194,15 +217,15 @@
             "The class {} requires a _transpose_nonbatch function!".format(self.__class__.__name__)
         )
 
     ####
     # The following methods MIGHT have be over-written by LinearOperator subclasses
     # if the LinearOperator does weird things with the batch dimensions
     ####
-    def _permute_batch(self, *dims: Tuple[int, ...]) -> LinearOperator:
+    def _permute_batch(self, *dims: int) -> LinearOperator:
         """
         Permute the batch dimensions.
         This probably won't have to be overwritten by LinearOperators, unless they use batch dimensions
         in a special way (e.g. BlockDiagLinearOperator, SumBatchLinearOperator)
 
         ..note::
             This method is used internally by the related function
@@ -221,20 +244,15 @@
                 components.append(component._permute_batch(*dims))
             else:
                 components.append(component)
 
         res = self.__class__(*components, **self._kwargs)
         return res
 
-    def _getitem(
-        self,
-        row_index: Union[slice, torch.LongTensor],
-        col_index: Union[slice, torch.LongTensor],
-        *batch_indices: Tuple[Union[int, slice, torch.LongTensor], ...],
-    ) -> LinearOperator:
+    def _getitem(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> LinearOperator:
         """
         Supports subindexing of the matrix this LinearOperator represents.
 
         The indices passed into this method will either be:
         - Tensor indices
         - Slices
         - int (batch indices only)
@@ -308,15 +326,15 @@
         components = [component.unsqueeze(dim) for component in self._args]
         res = self.__class__(*components, **self._kwargs)
         return res
 
     ####
     # The following methods PROBABLY should be over-written by LinearOperator subclasses for efficiency
     ####
-    def _bilinear_derivative(self, left_vecs: torch.Tensor, right_vecs: torch.Tensor) -> Tuple[torch.Tensor, ...]:
+    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Optional[Tensor], ...]:
         r"""
         Given :math:`\mathbf U` (left_vecs) and :math:`\mathbf V` (right_vecs),
         Computes the derivatives of (:math:`\mathbf u^\top \mathbf K \mathbf v`) w.r.t. :math:`\mathbf K`.
 
         Assume a :math:`\ldots x M X N` linear operator :math:`\mathbf K(\boldsymbol \theta)`,
         represented by tensors/sub-operators :math:`\boldsymbol \theta`.
         If :math:`\mathbf U \in \mathcal R^{\ldots \times M \times D}` and
@@ -337,58 +355,62 @@
         :param left_vecs: The vectors :math:`\mathbf U = [\mathbf u_1, \ldots, \mathbf u_D]`
         :param right_vecs: The vectors :math:`\mathbf V = [\mathbf v_1, \ldots, \mathbf v_D]`
         :return: Derivative with respect to the arguments (:math:`\boldsymbol \theta`) that
             represent this this LinearOperator.
         """
         from collections import deque
 
-        args = tuple(self.representation())
-        args_with_grads = tuple(arg for arg in args if arg.requires_grad)
+        # Construct a detached version of each argument in the linear operator
+        args = []
+        for arg in self.representation():
+            # All arguments here are guaranteed to be tensors
+            if arg.dtype.is_floating_point and arg.requires_grad:
+                args.append(arg.detach().requires_grad_(True))
+            else:
+                args.append(arg.detach())
 
-        # Easy case: if we don't require any gradients, then just return!
-        if not len(args_with_grads):
-            return tuple(None for _ in args)
+        # If no arguments require gradients, then we're done!
+        if not any(arg.requires_grad for arg in args):
+            return (None,) * len(args)
 
-        # Normal case: we'll use the autograd to get us a derivative
+        # We'll use the autograd to get us a derivative
         with torch.autograd.enable_grad():
-            loss = (left_vecs * self._matmul(right_vecs)).sum()
-            loss.requires_grad_(True)
+            lin_op = self.representation_tree()(*args)
+            loss = (left_vecs * lin_op._matmul(right_vecs)).sum()
+            args_with_grads = [arg for arg in args if arg.requires_grad]
             actual_grads = deque(torch.autograd.grad(loss, args_with_grads, allow_unused=True))
 
         # Now make sure that the object we return has one entry for every item in args
         grads = []
         for arg in args:
             if arg.requires_grad:
                 grads.append(actual_grads.popleft())
             else:
                 grads.append(None)
 
         return tuple(grads)
 
-    def _expand_batch(self, batch_shape: torch.Size) -> LinearOperator:
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         """
         Expands along batch dimensions. Return size will be *batch_shape x *matrix_shape.
 
         ..note::
             This method is used internally by the related function
             :func:`~linear_operator.LinearOperator.expand`,
             which does some additional work. Calling this method directly is discouraged.
         """
         current_shape = torch.Size([1 for _ in range(len(batch_shape) - self.dim() + 2)] + list(self.batch_shape))
         batch_repeat = torch.Size(
             [expand_size // current_size for expand_size, current_size in zip(batch_shape, current_shape)]
         )
         return self.repeat(*batch_repeat, 1, 1)
 
-    def _get_indices(
-        self,
-        row_index: torch.LongTensor,
-        col_index: torch.LongTensor,
-        *batch_indices: Tuple[torch.LongTensor, ...],
-    ) -> torch.Tensor:
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         """
         This method selects elements from the LinearOperator based on tensor indices for each dimension.
         All indices are tensor indices that are broadcastable.
         There will be exactly one index per dimension of the LinearOperator
 
         ..note::
             This method is used internally by the related function
@@ -440,37 +462,43 @@
     ####
     _check_size = True
 
     ####
     # Standard LinearOperator methods
     ####
     @property
-    def _args(self) -> Tuple[Union[torch.Tensor, "LinearOperator"], ...]:
+    def _args(self) -> Tuple[Union[torch.Tensor, "LinearOperator", int], ...]:
         return self._args_memo
 
     @_args.setter
-    def _args(self, args: Tuple[Union[torch.Tensor, "LinearOperator"], ...]) -> None:
+    def _args(self, args: Tuple[Union[torch.Tensor, "LinearOperator", int], ...]) -> None:
         self._args_memo = args
 
-    def _approx_diagonal(self) -> torch.Tensor:
+    @property
+    def _kwargs(self) -> Dict[str, Any]:
+        return {**self._differentiable_kwargs, **self._nondifferentiable_kwargs}
+
+    def _approx_diagonal(self: Float[LinearOperator, "*batch N N"]) -> Float[torch.Tensor, "*batch N"]:
         """
         (Optional) returns an (approximate) diagonal of the matrix
 
         Sometimes computing an exact diagonal is a bit computationally slow
         When we don't need an exact diagonal (e.g. for the pivoted cholesky
         decomposition, this function is called
 
         Defaults to calling the exact diagonal function
 
         :return: the (batch of) diagonals (... x N)
         """
         return self._diagonal()
 
     @cached(name="cholesky")
-    def _cholesky(self, upper: bool = False) -> "TriangularLinearOperator":  # noqa F811
+    def _cholesky(
+        self: Float[LinearOperator, "*batch N N"], upper: Optional[bool] = False
+    ) -> Float[LinearOperator, "*batch N N"]:
         """
         (Optional) Cholesky-factorizes the LinearOperator
 
         ..note::
             This method is used as an internal helper. Calling this method directly is discouraged.
 
         :param upper: Upper triangular or lower triangular factor (default: False).
@@ -490,15 +518,19 @@
         if evaluated_mat.size(-1) == 1:
             return TriangularLinearOperator(evaluated_mat.clamp_min(0.0).sqrt())
 
         # contiguous call is necessary here
         cholesky = psd_safe_cholesky(evaluated_mat, upper=upper).contiguous()
         return TriangularLinearOperator(cholesky, upper=upper)
 
-    def _cholesky_solve(self, rhs, upper: bool = False) -> LinearOperator:
+    def _cholesky_solve(
+        self: Float[LinearOperator, "*batch N N"],
+        rhs: Union[Float[LinearOperator, "*batch2 N M"], Float[Tensor, "*batch2 N M"]],
+        upper: Optional[bool] = False,
+    ) -> Union[Float[LinearOperator, "... N M"], Float[Tensor, "... N M"]]:
         """
         (Optional) Assuming that `self` is a Cholesky factor, computes the cholesky solve.
 
         ..note::
             This method is used as an internal helper. Calling this method directly is discouraged.
         """
         raise NotImplementedError("_cholesky_solve not implemented for the base LinearOperator")
@@ -519,43 +551,48 @@
         if (
             self.size(-1) <= settings.max_cholesky_size.value()
             or settings.fast_computations.covar_root_decomposition.off()
         ):
             return "cholesky"
         return "lanczos"
 
-    def _diagonal(self) -> torch.Tensor:
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
         r"""
         As :func:`torch._diagonal`, returns the diagonal of the matrix
         :math:`\mathbf A` this LinearOperator represents as a vector.
 
         .. note::
             This method is used as an internal helper. Calling this method directly is discouraged.
 
         :return: The diagonal (or batch of diagonals) of :math:`\mathbf A`.
         """
         row_col_iter = torch.arange(0, self.matrix_shape[-1], dtype=torch.long, device=self.device)
         return self[..., row_col_iter, row_col_iter]
 
-    def _mul_constant(self, other: Union[float, torch.Tensor]) -> LinearOperator:
+    def _mul_constant(
+        self: Float[LinearOperator, "*batch M N"], other: Union[float, torch.Tensor]
+    ) -> Float[LinearOperator, "*batch M N"]:
         """
-        Multiplies the LinearOperator by a costant.
+        Multiplies the LinearOperator by a constant.
 
         ..note::
             This method is used internally by the related function
             :func:`~linear_operator.LinearOperator.mul`,
             which does some additional work. Calling this method directly is discouraged.
 
         :param other: The constant (or batch of constants)
         """
         from .constant_mul_linear_operator import ConstantMulLinearOperator
 
         return ConstantMulLinearOperator(self, other)
 
-    def _mul_matrix(self, other: Union[torch.Tensor, "LinearOperator"]) -> LinearOperator:
+    def _mul_matrix(
+        self: Float[LinearOperator, "... #M #N"],
+        other: Union[Float[torch.Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"]],
+    ) -> Float[LinearOperator, "... M N"]:
         r"""
         Multiplies the LinearOperator by a (batch of) matrices.
 
         ..note::
             This method is used internally by the related function :func:`~linear_operator.LinearOperator.mul`,
             which does some additional work. Calling this method directly is discouraged.
 
@@ -567,15 +604,15 @@
         self = self.evaluate_kernel()
         other = other.evaluate_kernel()
         if isinstance(self, DenseLinearOperator) or isinstance(other, DenseLinearOperator):
             return DenseLinearOperator(self.to_dense() * other.to_dense())
         else:
             return MulLinearOperator(self, other)
 
-    def _preconditioner(self) -> Tuple[Callable, "LinearOperator", torch.Tensor]:
+    def _preconditioner(self) -> Tuple[Optional[Callable], Optional[LinearOperator], Optional[torch.Tensor]]:
         r"""
         (Optional) define a preconditioner (:math:`\mathbf P`) for linear conjugate gradients
 
         :return:
             - a function which performs :math:`\mathbf P^{-1}(\cdot)`,
             - a LinearOperator representation of :math:`\mathbf P`, and
             - a Tensor containing :math:`\log \Vert \mathbf P \Vert`.
@@ -638,15 +675,17 @@
             else:
                 res = MulLinearOperator(RootLinearOperator(part1), RootLinearOperator(part2))
                 roots = res.root_decomposition().root.to_dense()
                 num_batch = num_batch // 2
 
         return res
 
-    def _root_decomposition(self) -> Union[torch.Tensor, "LinearOperator"]:
+    def _root_decomposition(
+        self: Float[LinearOperator, "... N N"]
+    ) -> Union[Float[torch.Tensor, "... N N"], Float[LinearOperator, "... N N"]]:
         """
         Returns the (usually low-rank) root of a LinearOperator of a PSD matrix.
 
         ..note::
             This method is used internally by the related function
             :func:`~linear_operator.LinearOperator.root_decomposition`, which does some additional work.
             Calling this method directly is discouraged.
@@ -671,18 +710,18 @@
         This is the inner size of the root decomposition.
         This is primarily used to determine if it will be cheaper to compute a
         different root or not
         """
         return settings.max_root_decomposition_size.value()
 
     def _root_inv_decomposition(
-        self,
+        self: Float[LinearOperator, "*batch N N"],
         initial_vectors: Optional[torch.Tensor] = None,
         test_vectors: Optional[torch.Tensor] = None,
-    ) -> LinearOperator:
+    ) -> Union[Float[LinearOperator, "... N N"], Float[Tensor, "... N N"]]:
         r"""
         Returns the (usually low-rank) inverse root of a LinearOperator of a PSD matrix.
 
         ..note::
             This method is used internally by the related function
             :func:`~linear_operator.LinearOperator.root_inv_decomposition`, which does some additional work.
             Calling this method directly is discouraged.
@@ -728,28 +767,39 @@
                 if arg.dtype in (torch.float, torch.double, torch.half):
                     arg.requires_grad_(val)
         for arg in self._kwargs.values():
             if hasattr(arg, "requires_grad"):
                 if arg.dtype in (torch.float, torch.double, torch.half):
                     arg.requires_grad_(val)
 
-    def _solve(self, rhs: torch.Tensor, preconditioner: Callable, num_tridiag: int = 0) -> torch.Tensor:
+    def _solve(
+        self: Float[LinearOperator, "... N N"],
+        rhs: Float[torch.Tensor, "... N C"],
+        preconditioner: Optional[Callable[[Float[torch.Tensor, "... N C"]], Float[torch.Tensor, "... N C"]]] = None,
+        num_tridiag: Optional[int] = 0,
+    ) -> Union[
+        Float[torch.Tensor, "... N C"],
+        Tuple[
+            Float[torch.Tensor, "... N C"],
+            Float[torch.Tensor, "..."],  # Note that in case of a tuple the second term size depends on num_tridiag
+        ],
+    ]:
         r"""
         TODO
         """
         return utils.linear_cg(
             self._matmul,
             rhs,
             n_tridiag=num_tridiag,
             max_iter=settings.max_cg_iterations.value(),
             max_tridiag_iter=settings.max_lanczos_quadrature_iterations.value(),
             preconditioner=preconditioner,
         )
 
-    def _solve_preconditioner(self) -> Callable:
+    def _solve_preconditioner(self) -> Optional[Callable]:
         r"""
         (Optional) define a preconditioner :math:`\mathbf P` that can be used for linear systems,
         but not necessarily for log determinants. By default, this can call
         :meth:`~linear_operator.LinearOperator._preconditioner`.
 
         :return: a function which performs :math:`\mathbf P^{-1}(\cdot)`
         """
@@ -757,18 +807,15 @@
 
         if base_precond is not None:
             return base_precond
         elif linear_operator.beta_features.default_preconditioner.on():
             if hasattr(self, "_default_preconditioner_cache"):
                 U, S, Vt = self._default_preconditioner_cache
             else:
-                precond_basis_size = min(
-                    linear_operator.settings.max_preconditioner_size.value(),
-                    self.size(-1),
-                )
+                precond_basis_size = min(linear_operator.settings.max_preconditioner_size.value(), self.size(-1))
                 random_basis = torch.randn(
                     self.batch_shape + torch.Size((self.size(-2), precond_basis_size)),
                     device=self.device,
                     dtype=self.dtype,
                 )
                 projected_mat = self._matmul(random_basis)
                 proj_q = torch.linalg.qr(projected_mat)
@@ -804,26 +851,32 @@
         :param dim: The (positive valued) dimension to sum
         """
         from .sum_batch_linear_operator import SumBatchLinearOperator
 
         return SumBatchLinearOperator(self, block_dim=dim)
 
     @cached(name="svd")
-    def _svd(self) -> Tuple["LinearOperator", Tensor, "LinearOperator"]:
+    def _svd(
+        self: Float[LinearOperator, "*batch N N"]
+    ) -> Tuple[Float[LinearOperator, "*batch N N"], Float[Tensor, "... N"], Float[LinearOperator, "*batch N N"]]:
         """Method that allows implementing special-cased SVD computation. Should not be called directly"""
         # Using symeig is preferable here for psd LinearOperators.
         # Will need to overwrite this function for non-psd LinearOperators.
         evals, evecs = self._symeig(eigenvectors=True)
         signs = torch.sign(evals)
         U = evecs * signs.unsqueeze(-2)
         S = torch.abs(evals)
         V = evecs
         return U, S, V
 
-    def _symeig(self, eigenvectors: bool = False) -> Union[torch.Tensor, Tuple[torch.Tensor, "LinearOperator"]]:
+    def _symeig(
+        self: Float[LinearOperator, "*batch N N"],
+        eigenvectors: bool = False,
+        return_evals_as_lazy: Optional[bool] = False,
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         r"""
         Method that allows implementing special-cased symeig computation. Should not be called directly
         """
         from linear_operator.operators.dense_linear_operator import DenseLinearOperator
 
         if settings.verbose_linalg.on():
             settings.verbose_linalg.logger.debug(f"Running symeig on a matrix of size {self.shape}.")
@@ -836,15 +889,18 @@
         evals = evals.clamp_min(0.0).to(dtype=dtype)
         if eigenvectors:
             evecs = DenseLinearOperator(evecs.to(dtype=dtype))
         else:
             evecs = None
         return evals, evecs
 
-    def _t_matmul(self, rhs: torch.Tensor) -> LinearOperator:
+    def _t_matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[Tensor, "*batch2 M P"], Float[LinearOperator, "*batch2 M P"]],
+    ) -> Union[Float[LinearOperator, "... N P"], Float[Tensor, "... N P"]]:
         r"""
         Performs a transpose matrix multiplication :math:`\mathbf K^\top \mathbf M` with the
         (... x M x N) matrix :math:`\mathbf K` that this LinearOperator represents.
 
         ..note::
             This method is intended to be used only internally by various
             Functions that support backpropagation (e.g., :class:`Matmul`).
@@ -854,21 +910,25 @@
 
         :param rhs: the matrix :math:`\mathbf M` to multiply with.
         :return: :math:`\mathbf K^\top \mathbf M`
         """
         return self.mT._matmul(rhs)
 
     @_implements(torch.abs)
-    def abs(self) -> "LinearOperator":
+    def abs(self) -> LinearOperator:
         # Only implemented by some LinearOperator subclasses
         # We define it here so that we can map the torch function torch.abs to the LinearOperator method
         raise NotImplementedError(f"torch.abs({self.__class__.__name__}) is not implemented.")
 
     @_implements_symmetric(torch.add)
-    def add(self, other: Union[torch.Tensor, "LinearOperator"], alpha: float = None) -> LinearOperator:
+    def add(
+        self: Float[LinearOperator, "*batch M N"],
+        other: Union[Float[Tensor, "*batch M N"], Float[LinearOperator, "*batch M N"]],
+        alpha: float = None,
+    ) -> Float[LinearOperator, "*batch M N"]:
         r"""
         Each element of the tensor :attr:`other` is multiplied by the scalar :attr:`alpha`
         and added to each element of the :obj:`~linear_operator.operators.LinearOperator`.
         The resulting :obj:`~linear_operator.operators.LinearOperator` is returned.
 
         .. math::
             \text{out} = \text{self} + \text{alpha} ( \text{other} )
@@ -879,15 +939,18 @@
             is the linear operator and :math:`\mathbf O` is :attr:`other`.
         """
         if alpha is None:
             return self + other
         else:
             return self + alpha * other
 
-    def add_diagonal(self, diag: torch.Tensor) -> LinearOperator:
+    def add_diagonal(
+        self: Float[LinearOperator, "*batch N N"],
+        diag: Union[Float[torch.Tensor, "... N"], Float[torch.Tensor, "... 1"], Float[torch.Tensor, ""]],
+    ) -> Float[LinearOperator, "*batch N N"]:
         r"""
         Adds an element to the diagonal of the matrix.
 
         :param diag: Diagonal to add
         :return: :math:`\mathbf A + \text{diag}(\mathbf d)`, where :math:`\mathbf A` is the linear operator
             and :math:`\mathbf d` is the diagonal component
         """
@@ -926,36 +989,38 @@
                         self.shape, diag_shape
                     )
                 )
             diag_tensor = ConstantDiagLinearOperator(expanded_diag, diag_shape=self.shape[-1])
 
         return AddedDiagLinearOperator(self, diag_tensor)
 
-    def add_jitter(self, jitter_val: float = 1e-3) -> LinearOperator:
+    def add_jitter(
+        self: Float[LinearOperator, "*batch N N"], jitter_val: float = 1e-3
+    ) -> Float[LinearOperator, "*batch N N"]:
         r"""
         Adds jitter (i.e., a small diagonal component) to the matrix this
         LinearOperator represents.
         This is equivalent to calling :meth:`~linear_operator.operators.LinearOperator.add_diagonal`
         with a scalar tensor.
 
         :param jitter_val: The diagonal component to add
         :return: :math:`\mathbf A + \alpha (\mathbf I)`, where :math:`\mathbf A` is the linear operator
             and :math:`\alpha` is :attr:`jitter_val`.
         """
         diag = torch.tensor(jitter_val, dtype=self.dtype, device=self.device)
         return self.add_diagonal(diag)
 
     def add_low_rank(
-        self,
-        low_rank_mat: torch.Tensor,
+        self: Float[LinearOperator, "*batch N N"],
+        low_rank_mat: Union[Float[Tensor, "... N _"], Float[LinearOperator, "... N _"]],
         root_decomp_method: Optional[str] = None,
         root_inv_decomp_method: Optional[str] = None,
         generate_roots: Optional[bool] = True,
         **root_decomp_kwargs,
-    ) -> "SumLinearOperator":  # noqa F811
+    ) -> Float[LinearOperator, "*batch N N"]:  # returns SumLinearOperator
         r"""
         Adds a low rank matrix to the matrix that this LinearOperator represents, e.g.
         computes :math:`\mathbf A + \mathbf{BB}^\top`.
         We then update both the tensor and its root decomposition.
 
         We have access to, :math:`\mathbf L` and :math:`\mathbf M`
         where :math:`\mathbf A \approx \mathbf{LL}^\top`
@@ -1060,38 +1125,34 @@
         updated_inv_root = current_inv_root.mT.matmul(inner_inv_root)
 
         if return_triangular:
             updated_root = TriangularLinearOperator(updated_root)
             updated_inv_root = TriangularLinearOperator(updated_inv_root)
 
         add_to_cache(new_linear_op, "root_decomposition", RootLinearOperator(updated_root))
-        add_to_cache(
-            new_linear_op,
-            "root_inv_decomposition",
-            RootLinearOperator(updated_inv_root),
-        )
+        add_to_cache(new_linear_op, "root_inv_decomposition", RootLinearOperator(updated_inv_root))
 
         return new_linear_op
 
     @property
     def batch_dim(self) -> int:
         return len(self.batch_shape)
 
     @property
     def batch_shape(self) -> torch.Size:
         return self.shape[:-2]
 
     def cat_rows(
-        self,
-        cross_mat: torch.Tensor,
-        new_mat: torch.Tensor,
+        self: Float[LinearOperator, "... M N"],
+        cross_mat: Float[torch.Tensor, "... O N"],
+        new_mat: Float[torch.Tensor, "... O O"],
         generate_roots: bool = True,
         generate_inv_roots: bool = True,
         **root_decomp_kwargs,
-    ) -> LinearOperator:
+    ) -> Float[LinearOperator, "*batch M+O N+O"]:
         r"""
         Concatenates new rows and columns to the matrix that this LinearOperator represents, e.g.
 
         .. math::
             \mathbf C = \begin{bmatrix}
                 \mathbf A & \mathbf B^\top \\
                 \mathbf B & \mathbf D
@@ -1221,45 +1282,43 @@
                 new_inv_root = stable_pinverse(new_root).mT
             add_to_cache(
                 new_linear_op,
                 "root_inv_decomposition",
                 RootLinearOperator(to_linear_operator(new_inv_root)),
             )
 
-        add_to_cache(
-            new_linear_op,
-            "root_decomposition",
-            RootLinearOperator(to_linear_operator(new_root)),
-        )
+        add_to_cache(new_linear_op, "root_decomposition", RootLinearOperator(to_linear_operator(new_root)))
 
         return new_linear_op
 
     @_implements(torch.linalg.cholesky)
-    def cholesky(self, upper: bool = False) -> "TriangularLinearOperator":  # noqa F811
+    def cholesky(
+        self: Float[LinearOperator, "*batch N N"], upper: bool = False
+    ) -> Float[LinearOperator, "*batch N N"]:  # returns TriangularLinearOperator
         """
         Cholesky-factorizes the LinearOperator.
 
         :param upper: Upper triangular or lower triangular factor (default: False).
         :return: Cholesky factor (lower or upper triangular)
         """
         chol = self._cholesky(upper=False)
         if upper:
             chol = chol._transpose_nonbatch()
         return chol
 
     @_implements(torch.clone)
-    def clone(self) -> LinearOperator:
+    def clone(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         """
         Returns clone of the LinearOperator (with clones of all underlying tensors)
         """
         args = [arg.clone() if hasattr(arg, "clone") else arg for arg in self._args]
         kwargs = {key: val.clone() if hasattr(val, "clone") else val for key, val in self._kwargs.items()}
         return self.__class__(*args, **kwargs)
 
-    def cpu(self) -> LinearOperator:
+    def cpu(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         """
         Returns new LinearOperator identical to :attr:`self`, but on the CPU.
         """
         new_args = []
         new_kwargs = {}
         for arg in self._args:
             if hasattr(arg, "cpu"):
@@ -1269,15 +1328,17 @@
         for name, val in self._kwargs.items():
             if hasattr(val, "cpu"):
                 new_kwargs[name] = val.cpu()
             else:
                 new_kwargs[name] = val
         return self.__class__(*new_args, **new_kwargs)
 
-    def cuda(self, device_id: Optional[str] = None) -> LinearOperator:
+    def cuda(
+        self: Float[LinearOperator, "*batch M N"], device_id: Optional[str] = None
+    ) -> Float[LinearOperator, "*batch M N"]:
         """
         This method operates identically to :func:`torch.nn.Module.cuda`.
 
         :param device_id: Device ID of GPU to use.
         """
         new_args = []
         new_kwargs = {}
@@ -1290,39 +1351,45 @@
             if hasattr(val, "cuda"):
                 new_kwargs[name] = val.cuda(device_id)
             else:
                 new_kwargs[name] = val
         return self.__class__(*new_args, **new_kwargs)
 
     @property
-    def device(self) -> str:
+    def device(self) -> Optional[torch.device]:
         return self._args[0].device
 
-    def detach(self) -> LinearOperator:
+    def detach(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         """
         Removes the LinearOperator from the current computation graph.
         (In practice, this function removes all Tensors that make up the
         :obj:`~linear_operator.opeators.LinearOperator` from the computation graph.)
         """
-        return self.clone().detach_()
+        detached_args = [arg.detach() if hasattr(arg, "detach") else arg for arg in self._args]
+        detached_kwargs = dict(
+            (key, val.detach() if hasattr(val, "detach") else val) for key, val in self._kwargs.items()
+        )
+        return self.__class__(*detached_args, **detached_kwargs)
 
-    def detach_(self) -> LinearOperator:
+    def detach_(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         """
         An in-place version of :meth:`detach`.
         """
         for arg in self._args:
             if hasattr(arg, "detach"):
                 arg.detach_()
         for val in self._kwargs.values():
             if hasattr(val, "detach"):
                 val.detach_()
         return self
 
     @_implements(torch.diagonal)
-    def diagonal(self, offset: int = 0, dim1: int = -2, dim2: int = -1) -> torch.Tensor:
+    def diagonal(
+        self: Float[LinearOperator, "*batch N N"], offset: int = 0, dim1: int = -2, dim2: int = -1
+    ) -> Float[Tensor, "*batch N"]:
         r"""
         As :func:`torch.diagonal`, returns the diagonal of the matrix
         :math:`\mathbf A` this LinearOperator represents as a vector.
 
         .. note::
             This method is only implemented for when :attr:`dim1` and :attr:`dim2` are equal
             to -2 and -1, respectively, and :attr:`offset = 0`.
@@ -1340,15 +1407,17 @@
                 f"Got: offset={offset}, dim1={dim1}, dim2={dim2}."
             )
         elif not self.is_square:
             raise RuntimeError("LinearOperator#diagonal is only implemented for square operators.")
         return self._diagonal()
 
     @cached(name="diagonalization")
-    def diagonalization(self, method: Optional[str] = None) -> Tuple[torch.Tensor, torch.Tensor]:
+    def diagonalization(
+        self: Float[LinearOperator, "*batch N N"], method: Optional[str] = None
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         """
         Returns a (usually partial) diagonalization of a symmetric PSD matrix.
         Options are either "lanczos" or "symeig". "lanczos" runs Lanczos while
         "symeig" runs LinearOperator.symeig.
 
         :param method: Specify the method to use ("lanczos" or "symeig"). The method will be determined
             based on size if not specified.
@@ -1405,28 +1474,32 @@
         from .zero_linear_operator import ZeroLinearOperator
 
         if isinstance(other, ZeroLinearOperator):
             raise RuntimeError("Attempted to divide by a ZeroLinearOperator (divison by zero)")
 
         return self.mul(1.0 / other)
 
-    def double(self, device_id: Optional[str] = None) -> LinearOperator:
+    def double(
+        self: Float[LinearOperator, "*batch M N"], device_id: Optional[str] = None
+    ) -> Float[LinearOperator, "*batch M N"]:
         """
         This method operates identically to :func:`torch.Tensor.double`.
 
         :param device_id: Device ID of GPU to use.
         """
         return self.type(torch.double)
 
     @property
-    def dtype(self) -> torch.dtype:
+    def dtype(self) -> Optional[torch.dtype]:
         return self._args[0].dtype
 
     @_implements(torch.linalg.eigh)
-    def eigh(self) -> Tuple[torch.Tensor, "LinearOperator"]:
+    def eigh(
+        self: Float[LinearOperator, "*batch N N"]
+    ) -> Tuple[Float[Tensor, "*batch N"], Optional[Float[LinearOperator, "*batch N N"]]]:
         """
         Compute the symmetric eigendecomposition of the linear operator.
         This can be very slow for large tensors.
         Should be special-cased for tensors with particular structure.
 
         .. note::
             This method does NOT sort the eigenvalues.
@@ -1439,15 +1512,19 @@
             evals, evecs = pop_from_cache(self, "symeig", eigenvectors=True)
             return evals, None
         except CachingError:
             pass
         return self._symeig(eigenvectors=True)
 
     @_implements(torch.linalg.eigvalsh)
-    def eigvalsh(self) -> torch.Tensor:
+    def eigvalsh(
+        self: Float[LinearOperator, "*batch N N"]
+    ) -> Union[
+        Float[Tensor, "*batch N"], Tuple[Float[Tensor, "*batch N"], Optional[Float[LinearOperator, "*batch N N"]]]
+    ]:
         """
         Compute the eigenvalues of symmetric linear operator.
         This can be very slow for large tensors.
         Should be special-cased for tensors with particular structure.
 
         .. note::
             This method does NOT sort the eigenvalues.
@@ -1466,20 +1543,20 @@
         """
         Return a new LinearOperator representing the same one as this one, but with
         all lazily evaluated kernels actually evaluated.
         """
         return self.representation_tree()(*self.representation())
 
     @_implements(torch.exp)
-    def exp(self) -> "LinearOperator":
+    def exp(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         # Only implemented by some LinearOperator subclasses
         # We define it here so that we can map the torch function torch.exp to the LinearOperator method
         raise NotImplementedError(f"torch.exp({self.__class__.__name__}) is not implemented.")
 
-    def expand(self, *sizes: Union[torch.Size, Tuple[int, ...]]) -> LinearOperator:
+    def expand(self, *sizes: Union[torch.Size, int]) -> LinearOperator:
         r"""
         Returns a new view of the self
         :obj:`~linear_operator.operators.LinearOperator` with singleton
         dimensions expanded to a larger size.
 
         Passing -1 as the size for a dimension means not changing the size of
         that dimension.
@@ -1495,47 +1572,52 @@
         allocating new memory.
 
         :param sizes: the desired expanded size
         :return: The expanded LinearOperator
         """
         if len(sizes) == 1 and hasattr(sizes, "__iter__"):
             sizes = sizes[0]
-        if len(sizes) < 2 or tuple(sizes[-2:]) not in {
-            tuple(self.matrix_shape),
-            (-1, -1),
-        }:
+        if len(sizes) < 2 or tuple(sizes[-2:]) not in {tuple(self.matrix_shape), (-1, -1)}:
             raise RuntimeError(
                 "Invalid expand arguments {}. Currently, repeat only works to create repeated "
                 "batches of a 2D LinearOperator.".format(tuple(sizes))
             )
         elif all(isinstance(size, int) for size in sizes):
             shape = torch.Size(sizes)
         else:
             raise RuntimeError("Invalid arguments {} to expand.".format(sizes))
 
         res = self._expand_batch(batch_shape=shape[:-2])
         return res
 
-    def float(self, device_id: Optional[str] = None) -> LinearOperator:
+    def float(
+        self: Float[LinearOperator, "*batch M N"], device_id: Optional[str] = None
+    ) -> Float[LinearOperator, "*batch M N"]:
         """
         This method operates identically to :func:`torch.Tensor.float`.
 
         :param device_id: Device ID of GPU to use.
         """
         return self.type(torch.float)
 
-    def half(self, device_id: Optional[str] = None) -> LinearOperator:
+    def half(
+        self: Float[LinearOperator, "*batch M N"], device_id: Optional[str] = None
+    ) -> Float[LinearOperator, "*batch M N"]:
         """
         This method operates identically to :func:`torch.Tensor.half`.
 
         :param device_id: Device ID of GPU to use.
         """
         return self.type(torch.half)
 
-    def inv_quad(self, inv_quad_rhs: torch.Tensor, reduce_inv_quad: bool = True) -> torch.Tensor:
+    def inv_quad(
+        self: Float[LinearOperator, "*batch N N"],
+        inv_quad_rhs: Union[Float[Tensor, "*batch N M"], Float[Tensor, "*batch N"]],
+        reduce_inv_quad: bool = True,
+    ) -> Union[Float[Tensor, "*batch M"], Float[Tensor, " *batch"]]:
         r"""
         Computes an inverse quadratic form (w.r.t self) with several right hand sides, i.e:
 
         .. math::
            \text{tr}\left( \mathbf R^\top \mathbf A^{-1} \mathbf R \right),
 
         where :math:`\mathbf A` is the (positive definite) LinearOperator and :math:`\mathbf R`
@@ -1543,14 +1625,15 @@
 
         If :attr:`reduce_inv_quad` is set to false (and :attr:`inv_quad_rhs` is supplied),
         the function instead computes
 
         .. math::
            \text{diag}\left( \mathbf R^\top \mathbf A^{-1} \mathbf R \right).
 
+        :param input: :math:`\mathbf A` - the positive definite matrix (... X N X N)
         :param inv_quad_rhs: :math:`\mathbf R` - the right hand sides of the inverse quadratic term (... x N x M)
         :param reduce_inv_quad: Whether to compute
             :math:`\text{tr}\left( \mathbf R^\top \mathbf A^{-1} \mathbf R \right)`
             or :math:`\text{diag}\left( \mathbf R^\top \mathbf A^{-1} \mathbf R \right)`.
         :returns: The inverse quadratic term.
             If `reduce_inv_quad=True`, the inverse quadratic term is of shape (...). Otherwise, it is (... x M).
         """
@@ -1574,21 +1657,24 @@
         inv_quad_term = func(self.representation_tree(), *args)
 
         if reduce_inv_quad:
             inv_quad_term = inv_quad_term.sum(-1)
         return inv_quad_term
 
     def inv_quad_logdet(
-        self,
-        inv_quad_rhs: Optional[torch.Tensor] = None,
-        logdet: bool = False,
-        reduce_inv_quad: bool = True,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        self: Float[LinearOperator, "*batch N N"],
+        inv_quad_rhs: Optional[Union[Float[Tensor, "*batch N M"], Float[Tensor, "*batch N"]]] = None,
+        logdet: Optional[bool] = False,
+        reduce_inv_quad: Optional[bool] = True,
+    ) -> Tuple[
+        Optional[Union[Float[Tensor, "*batch M"], Float[Tensor, " *batch"], Float[Tensor, " 0"]]],
+        Optional[Float[Tensor, "..."]],
+    ]:
         r"""
-        Calls both :func:`inv_quad_logdet` and :func:`logdet` on a positive
+        Calls both :func:`inv_quad` and :func:`logdet` on a positive
         definite matrix (or batch) :math:`\mathbf A`.  However, calling this
         method is far more efficient and stable than calling each method
         independently.
 
         :param inv_quad_rhs: :math:`\mathbf R` - the right hand sides of the inverse quadratic term
         :param logdet: Whether or not to compute the
             logdet term :math:`\log \vert \mathbf A \vert`.
@@ -1689,43 +1775,46 @@
         logdet_term = logdet_term + logdet_p
 
         if inv_quad_term.numel() and reduce_inv_quad:
             inv_quad_term = inv_quad_term.sum(-1)
         return inv_quad_term, logdet_term
 
     @_implements(torch.inverse)
-    def inverse(self) -> "LinearOperator":
+    def inverse(self: Float[LinearOperator, "*batch N N"]) -> Float[LinearOperator, "*batch N N"]:
         # Only implemented by some LinearOperator subclasses
         # We define it here so that we can map the torch function torch.inverse to the LinearOperator method
         raise NotImplementedError(f"torch.inverse({self.__class__.__name__}) is not implemented.")
 
     @property
     def is_square(self) -> bool:
         return self.matrix_shape[0] == self.matrix_shape[1]
 
     @_implements_symmetric(torch.isclose)
     def isclose(self, other, rtol: float = 1e-05, atol: float = 1e-08, equal_nan: bool = False) -> Tensor:
         return self._isclose(other, rtol=rtol, atol=atol, equal_nan=equal_nan)
 
     @_implements(torch.log)
-    def log(self) -> "LinearOperator":
+    def log(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         # Only implemented by some LinearOperator subclasses
         # We define it here so that we can map the torch function torch.log to the LinearOperator method
         raise NotImplementedError(f"torch.log({self.__class__.__name__}) is not implemented.")
 
     @_implements(torch.logdet)
-    def logdet(self) -> torch.Tensor:
+    def logdet(self: Float[LinearOperator, "*batch M N"]) -> Float[Tensor, " *batch"]:
         r"""
         Computes the log determinant :math:`\log \vert \mathbf A \vert`.
         """
         _, res = self.inv_quad_logdet(inv_quad_rhs=None, logdet=True)
         return res
 
     @_implements(torch.matmul)
-    def matmul(self, other: Union[torch.Tensor, "LinearOperator"]) -> Union[torch.Tensor, "LinearOperator"]:
+    def matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        other: Union[Float[Tensor, "*batch2 N P"], Float[Tensor, "*batch2 N"], Float[LinearOperator, "*batch2 N P"]],
+    ) -> Union[Float[Tensor, "... M P"], Float[Tensor, "... M"], Float[LinearOperator, "... M P"]]:
         r"""
         Performs :math:`\mathbf A \mathbf B`, where :math:`\mathbf A \in
         \mathbb R^{M \times N}` is the LinearOperator and :math:`\mathbf B`
         is a right hand side :obj:`torch.Tensor` (or :obj:`~linear_operator.operators.LinearOperator`).
 
         :param other: :math:`\mathbf B` - the matrix or vector to multiply against.
         :return: The resulting of applying the linear operator to :math:`\mathbf B`.
@@ -1742,22 +1831,25 @@
         return Matmul.apply(self.representation_tree(), other, *self.representation())
 
     @property
     def matrix_shape(self) -> torch.Size:
         return torch.Size(self.shape[-2:])
 
     @property
-    def mT(self) -> LinearOperator:
+    def mT(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         """
         Alias of transpose(-1, -2)
         """
         return self.transpose(-1, -2)
 
     @_implements_symmetric(torch.mul)
-    def mul(self, other: Union[float, torch.Tensor, "LinearOperator"]) -> LinearOperator:
+    def mul(
+        self: Float[LinearOperator, "*batch M N"],
+        other: Union[float, Float[Tensor, "*batch2 M N"], Float[LinearOperator, "*batch2 M N"]],
+    ) -> Float[LinearOperator, "... M N"]:
         """
         Multiplies the matrix by a constant, or elementwise the matrix by another matrix.
 
         :param other: Constant or matrix to elementwise multiply by.
         :return: Another linear operator representing the result of the multiplication.
             If :obj:`other` was a constant (or batch of constants), this will likely be a
             :obj:`~linear_operator.operators.ConstantMulLinearOperator`. If :obj:`other` was
@@ -1800,22 +1892,22 @@
     @_implements(torch.numel)
     def numel(self) -> int:
         """
         Returns the number of elements.
         """
         return self.shape.numel()
 
-    def numpy(self) -> "numpy.ndarray":  # noqa F811
+    def numpy(self) -> np.ndarray:
         """
         Returns the LinearOperator as an dense numpy array.
         """
         return self.to_dense().detach().cpu().numpy()
 
     @_implements(torch.permute)
-    def permute(self, *dims: Tuple[int, ...]) -> LinearOperator:
+    def permute(self, *dims: Union[int, Tuple[int, ...]]) -> LinearOperator:
         """
         Returns a view of the original tensor with its dimensions permuted.
 
         :param dims: The desired ordering of dimensions.
         """
         # Unpack tuple
         if len(dims) == 1 and hasattr(dims, "__iter__"):
@@ -1840,16 +1932,19 @@
 
         if dims[-2:] != (num_dims - 2, num_dims - 1):
             raise ValueError("At the moment, cannot permute the non-batch dimensions of LinearOperators.")
 
         return self._permute_batch(*dims[:-2])
 
     def pivoted_cholesky(
-        self, rank: int, error_tol: Optional[float] = None, return_pivots: bool = False
-    ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
+        self: Float[LinearOperator, "*batch N N"],
+        rank: int,
+        error_tol: Optional[float] = None,
+        return_pivots: bool = False,
+    ) -> Union[Float[Tensor, "*batch N R"], Tuple[Float[Tensor, "*batch N R"], Int[Tensor, "*batch N"]]]:
         r"""
         Performs a partial pivoted Cholesky factorization of the (positive definite) LinearOperator.
         :math:`\mathbf L \mathbf L^\top = \mathbf K`.
         The partial pivoted Cholesky factor :math:`\mathbf L \in \mathbb R^{N \times \text{rank}}`
         forms a low rank approximation to the LinearOperator.
 
         The pivots are selected greedily, corresponding to the maximum diagonal element in the
@@ -1872,15 +1967,15 @@
         if return_pivots:
             return res, pivots
         else:
             return res
 
     # TODO: implement keepdim
     @_implements(torch.prod)
-    def prod(self, dim: int) -> Union["LinearOperator", torch.Tensor]:
+    def prod(self, dim: int) -> Union[LinearOperator, torch.Tensor]:
         r"""
         Returns the product of each row of :math:`\mathbf A` along the batch dimension :attr:`dim`.
 
             >>> linear_operator = DenseLinearOperator(torch.tensor([
                     [[2, 4], [1, 2]],
                     [[1, 1], [2., -1]],
                     [[2, 1], [1, 1.]],
@@ -1903,15 +1998,15 @@
             raise ValueError(
                 "At the moment, LinearOperator.prod only works on batch dimensions. "
                 "Got dim={} for LinearOperator of shape {}".format(orig_dim, self.shape)
             )
 
         return self._prod_batch(dim)
 
-    def repeat(self, *sizes: Union[torch.Size, Tuple[int, ...]]) -> LinearOperator:
+    def repeat(self, *sizes: Union[int, Tuple[int, ...]]) -> LinearOperator:
         """
         Repeats this tensor along the specified dimensions.
 
         Currently, this only works to create repeated batches of a 2D LinearOperator.
         I.e. all calls should be :attr:`linear_operator.repeat(*batch_sizes, 1, 1)`.
 
             >>> linear_operator = ToeplitzLinearOperator(torch.tensor([4. 1., 0.5]))
@@ -1938,15 +2033,15 @@
 
     # TODO: make this method private
     def representation(self) -> Tuple[torch.Tensor, ...]:
         """
         Returns the Tensors that are used to define the LinearOperator
         """
         representation = []
-        for arg in self._args:
+        for arg in itertools.chain(self._args, self._differentiable_kwargs.values()):
             if torch.is_tensor(arg):
                 representation.append(arg)
             elif hasattr(arg, "representation") and callable(arg.representation):  # Is it a LinearOperator?
                 representation += list(arg.representation())
             else:
                 raise RuntimeError("Representation of a LinearOperator should consist only of Tensors")
         return tuple(representation)
@@ -1985,26 +2080,29 @@
 
         :param val: Whether or not to require gradients.
         :return: self.
         """
         self._set_requires_grad(val)
         return self
 
-    def reshape(self, *sizes: Union[torch.Size, Tuple[int, ...]]) -> LinearOperator:
+    def reshape(self, *sizes: Union[torch.Size, int, Tuple[int, ...]]) -> LinearOperator:
         """
         Alias for expand
         """
         # While for regular tensors expand doesn't handle a leading non-existing -1 dimension,
         # reshape does. So we handle this conversion here.
         if len(sizes) == len(self.shape) + 1 and sizes[0] == -1:
             sizes = (1,) + sizes[1:]
         return self.expand(*sizes)
 
     @_implements_second_arg(torch.matmul)
-    def rmatmul(self, other: Union[torch.Tensor, "LinearOperator"]) -> Union[torch.Tensor, "LinearOperator"]:
+    def rmatmul(
+        self: Float[LinearOperator, "... M N"],
+        other: Union[Float[Tensor, "... P M"], Float[Tensor, "... M"], Float[LinearOperator, "... P M"]],
+    ) -> Union[Float[Tensor, "... P N"], Float[Tensor, "N"], Float[LinearOperator, "... P N"]]:
         r"""
         Performs :math:`\mathbf B \mathbf A`, where :math:`\mathbf A \in
         \mathbb R^{M \times N}` is the LinearOperator and :math:`\mathbf B`
         is a left hand side :obj:`torch.Tensor` (or :obj:`~linear_operator.operators.LinearOperator`).
 
         :param other: :math:`\mathbf B` - the matrix or vector that :math:`\mathbf A` will
             right multiply against.
@@ -2012,15 +2110,17 @@
             The return type will be the same as :attr:`other`'s type.
         """
         if other.ndim == 1:
             return self.mT.matmul(other)
         return self.mT.matmul(other.mT).mT
 
     @cached(name="root_decomposition")
-    def root_decomposition(self, method: Optional[str] = None) -> LinearOperator:
+    def root_decomposition(
+        self: Float[LinearOperator, "*batch N N"], method: Optional[str] = None
+    ) -> Float[LinearOperator, "*batch N N"]:
         r"""
         Returns a (usually low-rank) root decomposition linear operator of the PSD LinearOperator :math:`\mathbf A`.
         This can be used for sampling from a Gaussian distribution, or for obtaining a
         low-rank version of a matrix.
 
         :param method: Which method to use to perform the root decomposition. Choices are:
             "cholesky", "lanczos", "symeig", "pivoted_cholesky", or "svd".
@@ -2074,19 +2174,19 @@
         else:
             raise RuntimeError(f"Unknown root decomposition method '{method}'")
 
         return RootLinearOperator(root)
 
     @cached(name="root_inv_decomposition")
     def root_inv_decomposition(
-        self,
+        self: Float[LinearOperator, "*batch N N"],
         initial_vectors: Optional[torch.Tensor] = None,
         test_vectors: Optional[torch.Tensor] = None,
         method: Optional[str] = None,
-    ) -> LinearOperator:
+    ) -> Union[Float[LinearOperator, "... N N"], Float[Tensor, "... N N"]]:
         r"""
         Returns a (usually low-rank) inverse root decomposition linear operator
         of the PSD LinearOperator :math:`\mathbf A`.
         This can be used for sampling from a Gaussian distribution, or for obtaining a
         low-rank version of a matrix.
 
         The root_inv_decomposition is performed using a partial Lanczos tridiagonalization.
@@ -2173,19 +2273,23 @@
         """
         size = self._size()
         if dim is not None:
             return size[dim]
         return size
 
     @property
-    def shape(self):
-        return self.size()
+    def shape(self) -> torch.Size:
+        return self._size()
 
     @_implements(torch.linalg.solve)
-    def solve(self, right_tensor: torch.Tensor, left_tensor: Optional[torch.Tensor] = None) -> torch.Tensor:
+    def solve(
+        self: Float[LinearOperator, "... N N"],
+        right_tensor: Union[Float[Tensor, "... N P"], Float[Tensor, " N"]],
+        left_tensor: Optional[Float[Tensor, "... O N"]] = None,
+    ) -> Union[Float[Tensor, "... N P"], Float[Tensor, "... N"], Float[Tensor, "... O P"], Float[Tensor, "... O"]]:
         r"""
         Computes a linear solve (w.r.t self = :math:`\mathbf A`) with right hand side :math:`\mathbf R`.
         I.e. computes
 
         .. math::
            \begin{equation}
                \mathbf A^{-1} \mathbf R,
@@ -2231,19 +2335,15 @@
                 left_tensor,
                 right_tensor,
                 *self.representation(),
             )
 
     @_implements(torch.linalg.solve_triangular)
     def solve_triangular(
-        self,
-        rhs: torch.Tensor,
-        upper: bool,
-        left: bool = True,
-        unitriangular: bool = False,
+        self, rhs: torch.Tensor, upper: bool, left: bool = True, unitriangular: bool = False
     ) -> torch.Tensor:
         r"""
         Computes a triangular linear solve (w.r.t self = :math:`\mathbf A`) with right hand side :math:`\mathbf R`.
         If left=True, computes the soluton :math:`\mathbf X` to
 
         .. math::
            \begin{equation}
@@ -2267,20 +2367,24 @@
         :return: :math:`\mathbf A^{-1} \mathbf R` or :math:`\mathbf L \mathbf A^{-1} \mathbf R`.
         """
         # This function is only implemented by TriangularLinearOperator subclasses. We define it here so
         # that we can map the torch function torch.linalg.solve_triangular to the LinearOperator method.
         raise NotImplementedError(f"torch.linalg.solve_triangular({self.__class__.__name__}) is not implemented.")
 
     @_implements(torch.sqrt)
-    def sqrt(self) -> "LinearOperator":
+    def sqrt(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         # Only implemented by some LinearOperator subclasses
         # We define it here so that we can map the torch function torch.sqrt to the LinearOperator method
         raise NotImplementedError(f"torch.sqrt({self.__class__.__name__}) is not implemented.")
 
-    def sqrt_inv_matmul(self, rhs: torch.Tensor, lhs: Optional[torch.Tensor] = None) -> torch.Tensor:
+    def sqrt_inv_matmul(
+        self: Float[LinearOperator, "*batch N N"],
+        rhs: Float[Tensor, "*batch N P"],
+        lhs: Optional[Float[Tensor, "*batch O N"]] = None,
+    ) -> Union[Float[Tensor, "*batch N P"], Tuple[Float[Tensor, "*batch O P"], Float[Tensor, "*batch O"]]]:
         r"""
         If the LinearOperator :math:`\mathbf A` is positive definite,
         computes
 
         .. math::
            \begin{equation}
                \mathbf A^{-1/2} \mathbf R,
@@ -2315,15 +2419,15 @@
 
         if lhs is None:
             return sqrt_inv_matmul_res
         else:
             return sqrt_inv_matmul_res, inv_quad_res
 
     @_implements(torch.squeeze)
-    def squeeze(self, dim: int) -> Union["LinearOperator", torch.Tensor]:
+    def squeeze(self, dim: int) -> Union[LinearOperator, torch.Tensor]:
         """
         Removes the singleton dimension of a LinearOperator specifed by :attr:`dim`.
 
         :param dim: Which singleton dimension to remove.
         :return: The squeezed LinearOperator. Will be a :obj:`torch.Tensor` if the squeezed dimension
             was a matrix dimension; otherwise it will return a LinearOperator.
         """
@@ -2332,15 +2436,19 @@
         else:
             index = [_noop_index] * self.dim()
             index[dim] = 0
             index = tuple(index)
             return self[index]
 
     @_implements(torch.sub)
-    def sub(self, other: Union[torch.Tensor, "LinearOperator"], alpha: float = None) -> LinearOperator:
+    def sub(
+        self: Float[LinearOperator, "*batch M N"],
+        other: Union[Float[Tensor, "*batch M N"], Float[LinearOperator, "*batch M N"]],
+        alpha: float = None,
+    ) -> Float[LinearOperator, "*batch M N"]:
         r"""
         Each element of the tensor :attr:`other` is multiplied by the scalar :attr:`alpha`
         and subtracted to each element of the :obj:`~linear_operator.operators.LinearOperator`.
         The resulting :obj:`~linear_operator.operators.LinearOperator` is returned.
 
         .. math::
             \text{out} = \text{self} - \text{alpha} ( \text{other} )
@@ -2352,15 +2460,15 @@
         """
         if alpha is None:
             return self - other
         else:
             return self + (alpha * -1) * other
 
     @_implements(torch.sum)
-    def sum(self, dim: Optional[int] = None) -> Union["LinearOperator", torch.Tensor]:
+    def sum(self, dim: Optional[int] = None) -> Union[LinearOperator, torch.Tensor]:
         """
         Sum the LinearOperator across a dimension.
         The `dim` controls which batch dimension is summed over.
         If set to None, then sums all dimensions.
 
             >>> linear_operator = DenseLinearOperator(torch.tensor([
                     [[2, 4], [1, 2]],
@@ -2394,15 +2502,17 @@
             return (self.mT @ ones).squeeze(-1)
         # Otherwise: it's a batch dimension
         elif dim < self.dim():
             return self._sum_batch(dim)
         else:
             raise ValueError("Invalid dim ({}) for LinearOperator of size {}".format(orig_dim, self.shape))
 
-    def svd(self) -> Tuple["LinearOperator", torch.Tensor, "LinearOperator"]:
+    def svd(
+        self: Float[LinearOperator, "*batch N N"]
+    ) -> Tuple[Float[LinearOperator, "*batch N N"], Float[Tensor, "... N"], Float[LinearOperator, "*batch N N"]]:
         r"""
         Compute the SVD of the linear operator :math:`\mathbf A \in \mathbb R^{M \times N}`
         s.t. :math:`\mathbf A = \mathbf{U S V^\top}`.
         This can be very slow for large tensors.
         Should be special-cased for tensors with particular structure.
 
         .. note::
@@ -2413,44 +2523,44 @@
             - The singlar values :math:`\mathbf S` (... x min(M, N)),
             - The right singluar vectors :math:`\mathbf V` (... x N x N)),
         """
         return self._svd()
 
     @_implements(torch.linalg.svd)
     def _torch_linalg_svd(
-        self,
-    ) -> Tuple["LinearOperator", torch.Tensor, "LinearOperator"]:
+        self: Float[LinearOperator, "*batch N N"]
+    ) -> Tuple[Float[LinearOperator, "*batch N N"], Float[Tensor, "... N"], Float[LinearOperator, "*batch N N"]]:
         r"""
         A version of self.svd() that matches the torch.linalg.svd API.
 
         :returns:
             - The left singular vectors :math:`\mathbf U` (... x M, M),
             - The singlar values :math:`\mathbf S` (... x min(M, N)),
             - The right singluar vectors :math:`\mathbf V^\top` (... x N X N),
         """
         U, S, V = self._svd()
         return U, S, V.mT
 
     @property
-    def T(self) -> LinearOperator:
+    def T(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         """
         Alias of t()
         """
         return self.t()
 
-    def t(self) -> LinearOperator:
+    def t(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         """
         Alias of :meth:`~linear_operator.LinearOperator.transpose` for 2D LinearOperator.
         (Tranposes the two dimensions.)
         """
         if self.ndimension() != 2:
             raise RuntimeError("Cannot call t for more than 2 dimensions")
         return self.transpose(0, 1)
 
-    def to(self, *args, **kwargs) -> LinearOperator:
+    def to(self: Float[LinearOperator, "*batch M N"], *args, **kwargs) -> Float[LinearOperator, "*batch M N"]:
         """
         A device-agnostic method of moving the LinearOperator to the specified device or dtype.
         This method functions just like :meth:`torch.Tensor.to`.
 
         :return: New LinearOperator identical to self on specified device/dtype.
         """
         device, dtype = _to_helper(*args, **kwargs)
@@ -2466,15 +2576,15 @@
             if hasattr(val, "to"):
                 new_kwargs[name] = val.to(dtype=dtype, device=device)
             else:
                 new_kwargs[name] = val
         return self.__class__(*new_args, **new_kwargs)
 
     @cached
-    def to_dense(self) -> torch.Tensor:
+    def to_dense(self: Float[LinearOperator, "*batch M N"]) -> Float[Tensor, "*batch M N"]:
         """
         Explicitly evaluates the matrix this LinearOperator represents. This function
         should return a :obj:`torch.Tensor` storing an exact representation of this LinearOperator.
         """
         num_rows, num_cols = self.matrix_shape
 
         if num_rows < num_cols:
@@ -2522,15 +2632,15 @@
             res = self._transpose_nonbatch()
 
         else:
             raise RuntimeError("Cannot transpose batch dimension with non-batch dimension")
 
         return res
 
-    def type(self, dtype: torch.dtype) -> LinearOperator:
+    def type(self: LinearOperator, dtype: torch.dtype) -> LinearOperator:
         """
         A device-agnostic method of moving the LienarOperator to the specified dtype.
         This method operates similarly to :func:`torch.Tensor.dtype`.
 
         :param dtype: Target dtype.
         """
         attr_flag = _TYPES_DICT[dtype]
@@ -2569,16 +2679,18 @@
             raise ValueError(
                 "Can only unsqueeze batch dimensions of {} (size {}). Got "
                 "dim={}.".format(self.__class__.__name__, self.shape, dim)
             )
         res = self._unsqueeze_batch(positive_dim)
         return res
 
-    # TODO: repalce this method with something like sqrt_matmul.
-    def zero_mean_mvn_samples(self, num_samples: int) -> torch.Tensor:
+    # TODO: replace this method with something like sqrt_matmul.
+    def zero_mean_mvn_samples(
+        self: Float[LinearOperator, "*batch N N"], num_samples: int
+    ) -> Float[Tensor, "num_samples *batch N"]:
         r"""
         Assumes that the LinearOpeator :math:`\mathbf A` is a covariance
         matrix, or a batch of covariance matrices.
         Returns samples from a zero-mean MVN, defined by :math:`\mathcal N( \mathbf 0, \mathbf A)`.
 
         :param num_samples: Number of samples to draw.
         :return: Samples from MVN :math:`\mathcal N( \mathbf 0, \mathbf A)`.
@@ -2617,15 +2729,24 @@
                 dtype=self.dtype,
                 device=self.device,
             )
             samples = covar_root.matmul(base_samples).permute(-1, *range(self.dim() - 1)).contiguous()
 
         return samples
 
-    def __add__(self, other: Union[Tensor, LinearOperator, float]) -> LinearOperator:
+    def __sub__(
+        self: Float[LinearOperator, "... #M #N"],
+        other: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"], float],
+    ) -> Union[Float[LinearOperator, "... M N"], Float[Tensor, "... M N"]]:
+        return self + other.mul(-1)
+
+    def __add__(
+        self: Float[LinearOperator, "... #M #N"],
+        other: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"], float],
+    ) -> Union[Float[LinearOperator, "... M N"], Float[Tensor, "... M N"]]:
         from .added_diag_linear_operator import AddedDiagLinearOperator
         from .dense_linear_operator import to_linear_operator
         from .diag_linear_operator import DiagLinearOperator
         from .root_linear_operator import RootLinearOperator
         from .sum_linear_operator import SumLinearOperator
         from .zero_linear_operator import ZeroLinearOperator
 
@@ -2642,17 +2763,15 @@
             new_other = other if other.shape[:-2] == shape[:-2] else other._expand_batch(shape[:-2])
             return SumLinearOperator(new_self, new_other)
         elif isinstance(other, numbers.Number) and other == 0:
             return self
         else:
             return SumLinearOperator(self, other)
 
-    def __getitem__(
-        self, index: Tuple[Union[slice, torch.LongTensor, int, Ellipsis], ...]
-    ) -> Union[LinearOperator, torch.Tensor]:
+    def __getitem__(self, index: Union[IndexType, Tuple[IndexType, ...]]) -> Union[LinearOperator, torch.Tensor]:
         ndimension = self.ndimension()
 
         # Process the index
         index = index if isinstance(index, tuple) else (index,)
         index = tuple(torch.tensor(idx) if isinstance(idx, list) else idx for idx in index)
         index = tuple(idx.item() if torch.is_tensor(idx) and not len(idx.shape) else idx for idx in index)
 
@@ -2755,47 +2874,60 @@
         warnings.warn(
             f"Converting {self.__class__.__name__} into a dense torch.Tensor due to a torch.isclose call. "
             "This may incur substantial performance and memory penalties.",
             PerformanceWarning,
         )
         return torch.isclose(to_dense(self), to_dense(other), rtol=rtol, atol=atol, equal_nan=equal_nan)
 
-    def __matmul__(self, other: Union[torch.Tensor, LinearOperator]) -> Union[torch.Tensor, LinearOperator]:
+    def __matmul__(
+        self: Float[LinearOperator, "*batch M N"],
+        other: Union[
+            Float[torch.Tensor, "*batch2 N D"], Float[torch.Tensor, "N"], Float[LinearOperator, "*batch2 N D"]
+        ],
+    ) -> Union[Float[torch.Tensor, "... M D"], Float[torch.Tensor, "... M"], Float[LinearOperator, "... M D"]]:
         return self.matmul(other)
 
     @_implements_second_arg(torch.Tensor.matmul)
-    def __rmatmul__(self, other: Union[torch.Tensor, LinearOperator]) -> Union[torch.Tensor, LinearOperator]:
+    def __rmatmul__(
+        self: Float[LinearOperator, "... M N"],
+        other: Union[Float[Tensor, "... P M"], Float[Tensor, "... M"], Float[LinearOperator, "... P M"]],
+    ) -> Union[Float[Tensor, "... P N"], Float[Tensor, "... N"], Float[LinearOperator, "... P N"]]:
         return self.rmatmul(other)
 
     @_implements_second_arg(torch.Tensor.mul)
-    def __mul__(self, other: Union[torch.Tensor, LinearOperator, float]) -> LinearOperator:
+    def __mul__(
+        self: Float[LinearOperator, "*batch #M #N"],
+        other: Union[Float[torch.Tensor, "*batch2 #M #N"], Float[LinearOperator, "*batch2 #M #N"], float],
+    ) -> Float[LinearOperator, "... M N"]:
         return self.mul(other)
 
     @_implements_second_arg(torch.Tensor.add)
-    def __radd__(self, other: Union[torch.Tensor, LinearOperator, float]) -> LinearOperator:
+    def __radd__(
+        self: Float[LinearOperator, "*batch #M #N"],
+        other: Union[Float[torch.Tensor, "*batch2 #M #N"], Float[LinearOperator, "*batch2 #M #N"], float],
+    ) -> Float[LinearOperator, "... M N"]:
         return self + other
 
-    def __rmul__(self, other: Union[torch.Tensor, LinearOperator, float]) -> LinearOperator:
+    def __rmul__(
+        self: Float[LinearOperator, "*batch #M #N"],
+        other: Union[Float[torch.Tensor, "*batch2 #M #N"], Float[LinearOperator, "*batch2 #M #N"], float],
+    ) -> Float[LinearOperator, "... M N"]:
         return self.mul(other)
 
     @_implements_second_arg(torch.sub)
     @_implements_second_arg(torch.Tensor.sub)
-    def __rsub__(self, other: Union[torch.Tensor, LinearOperator, float]) -> LinearOperator:
+    def __rsub__(
+        self: Float[LinearOperator, "*batch #M #N"],
+        other: Union[Float[torch.Tensor, "*batch2 #M #N"], Float[LinearOperator, "*batch2 #M #N"], float],
+    ) -> Float[LinearOperator, "... M N"]:
         return self.mul(-1) + other
 
-    def __sub__(self, other: Union[torch.Tensor, LinearOperator, float]) -> LinearOperator:
-        return self + other.mul(-1)
-
     @classmethod
     def __torch_function__(
-        cls,
-        func: Callable,
-        types: Tuple[type, ...],
-        args: Tuple[Any, ...] = (),
-        kwargs: Dict[str, Any] = None,
+        cls, func: Callable, types: Tuple[type, ...], args: Tuple[Any, ...] = (), kwargs: Dict[str, Any] = None
     ) -> Any:
         if kwargs is None:
             kwargs = {}
 
         if not isinstance(args[0], cls):
             if func not in _HANDLED_SECOND_ARG_FUNCTIONS or not all(
                 issubclass(t, (torch.Tensor, LinearOperator)) for t in types
@@ -2827,15 +2959,15 @@
     components = name.split(".")
     obj = __import__(components[0])
     for component in components[1:]:
         obj = getattr(obj, component)
     return obj
 
 
-def to_dense(obj: Union[LinearOperator, torch.Tensor]) -> torch.Tensor:
+def to_dense(obj: Union[LinearOperator, Tensor]) -> Tensor:
     r"""
     A function which ensures that `obj` is a (normal) Tensor.
     - If `obj` is a Tensor, this function does nothing.
     - If `obj` is a LinearOperator, this function evaluates it.
     """
     if torch.is_tensor(obj):
         return obj
@@ -2843,8 +2975,8 @@
         return obj.to_dense()
     else:
         raise TypeError("object of class {} cannot be made into a Tensor".format(obj.__class__.__name__))
 
 
 _deprecate_renamed_methods(LinearOperator, inv_quad_log_det="inv_quad_logdet", log_det="logdet")
 
-__all__ = ["LinearOperator", "to_dense"]
+__all__ = ["LinearOperator", "to_dense", "IndexType"]
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/added_diag_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/added_diag_linear_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python3
 
+from __future__ import annotations
+
 import warnings
-from typing import Callable, Optional, Tuple, Union
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
 from torch import Tensor
 
 from .. import settings
 from ..utils.memoize import cached
 from ..utils.warnings import NumericalWarning
 from ._linear_operator import LinearOperator
 from .diag_linear_operator import ConstantDiagLinearOperator, DiagLinearOperator
@@ -29,18 +32,15 @@
 
     .. _Gardner et al., NeurIPS 2018:
         https://arxiv.org/abs/1809.11165
     """
 
     def __init__(
         self,
-        *linear_ops: Union[
-            Tuple[LinearOperator, DiagLinearOperator],
-            Tuple[DiagLinearOperator, LinearOperator],
-        ],
+        *linear_ops: Union[Tuple[LinearOperator, DiagLinearOperator], Tuple[DiagLinearOperator, LinearOperator]],
         preconditioner_override: Optional[Callable] = None,
     ):
         linear_ops = list(linear_ops)
         super(AddedDiagLinearOperator, self).__init__(*linear_ops, preconditioner_override=preconditioner_override)
         if len(linear_ops) > 2:
             raise RuntimeError("An AddedDiagLinearOperator can only have two components")
 
@@ -66,29 +66,38 @@
         self._noise = None
         self._piv_chol_self = None  # <- Doesn't need to be an attribute, but used for testing purposes
         self._precond_lt = None
         self._precond_logdet_cache = None
         self._q_cache = None
         self._r_cache = None
 
-    def _matmul(self, rhs: Tensor) -> Tensor:
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         return torch.addcmul(self._linear_op._matmul(rhs), self._diag_tensor._diag.unsqueeze(-1), rhs)
 
-    def add_diagonal(self, added_diag: Tensor) -> "AddedDiagLinearOperator":
-        return self.__class__(self._linear_op, self._diag_tensor.add_diagonal(added_diag))
-
-    def __add__(self, other: Union[Tensor, LinearOperator]) -> LinearOperator:
+    def add_diagonal(
+        self: Float[LinearOperator, "*batch N N"],
+        diag: Union[Float[torch.Tensor, "... N"], Float[torch.Tensor, "... 1"], Float[torch.Tensor, ""]],
+    ) -> Float[LinearOperator, "*batch N N"]:
+        return self.__class__(self._linear_op, self._diag_tensor.add_diagonal(diag))
+
+    def __add__(
+        self: Float[LinearOperator, "... #M #N"],
+        other: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"], float],
+    ) -> Union[Float[LinearOperator, "... M N"], Float[Tensor, "... M N"]]:
         from .diag_linear_operator import DiagLinearOperator
 
         if isinstance(other, DiagLinearOperator):
             return self.__class__(self._linear_op, self._diag_tensor + other)
         else:
             return self.__class__(self._linear_op + other, self._diag_tensor)
 
-    def _preconditioner(self) -> Tuple[Callable, "LinearOperator", torch.Tensor]:
+    def _preconditioner(self) -> Tuple[Optional[Callable], Optional[LinearOperator], Optional[torch.Tensor]]:
         r"""
         Here we use a partial pivoted Cholesky preconditioner:
 
         K \approx L L^T + D
 
         where L L^T is a low rank approximation, and D is a diagonal.
         We can compute the preconditioner's inverse using Woodbury
@@ -146,50 +155,56 @@
         if self._constant_diag:
             self._init_cache_for_constant_diag(eye, batch_shape, n, k)
         else:
             self._init_cache_for_non_constant_diag(eye, batch_shape, n)
 
         self._precond_lt = PsdSumLinearOperator(RootLinearOperator(self._piv_chol_self), self._diag_tensor)
 
-    def _init_cache_for_constant_diag(self, eye: Tensor, batch_shape: torch.Size, n: int, k: int):
+    def _init_cache_for_constant_diag(self, eye: Tensor, batch_shape: Union[torch.Size, List[int]], n: int, k: int):
         # We can factor out the noise for for both QR and solves.
         self._noise = self._noise.narrow(-2, 0, 1)
         self._q_cache, self._r_cache = torch.linalg.qr(
             torch.cat((self._piv_chol_self, self._noise.sqrt() * eye), dim=-2)
         )
         self._q_cache = self._q_cache[..., :n, :]
 
         # Use the matrix determinant lemma for the logdet, using the fact that R'R = L_k'L_k + s*I
         logdet = self._r_cache.diagonal(dim1=-1, dim2=-2).abs().log().sum(-1).mul(2)
         logdet = logdet + (n - k) * self._noise.squeeze(-2).squeeze(-1).log()
         self._precond_logdet_cache = logdet.view(*batch_shape) if len(batch_shape) else logdet.squeeze()
 
-    def _init_cache_for_non_constant_diag(self, eye: Tensor, batch_shape: torch.Size, n: int):
+    def _init_cache_for_non_constant_diag(self, eye: Tensor, batch_shape: Union[torch.Size, List[int]], n: int):
         # With non-constant diagonals, we cant factor out the noise as easily
         self._q_cache, self._r_cache = torch.linalg.qr(
             torch.cat((self._piv_chol_self / self._noise.sqrt(), eye), dim=-2)
         )
         self._q_cache = self._q_cache[..., :n, :] / self._noise.sqrt()
 
         # Use the matrix determinant lemma for the logdet, using the fact that R'R = L_k'L_k + s*I
         logdet = self._r_cache.diagonal(dim1=-1, dim2=-2).abs().log().sum(-1).mul(2)
         logdet -= (1.0 / self._noise).log().sum([-1, -2])
         self._precond_logdet_cache = logdet.view(*batch_shape) if len(batch_shape) else logdet.squeeze()
 
     @cached(name="svd")
-    def _svd(self) -> Tuple["LinearOperator", Tensor, "LinearOperator"]:
+    def _svd(
+        self: Float[LinearOperator, "*batch N N"]
+    ) -> Tuple[Float[LinearOperator, "*batch N N"], Float[Tensor, "... N"], Float[LinearOperator, "*batch N N"]]:
         if isinstance(self._diag_tensor, ConstantDiagLinearOperator):
             U, S_, V = self._linear_op.svd()
             S = S_ + self._diag_tensor._diagonal()
             return U, S, V
         return super()._svd()
 
-    def _symeig(self, eigenvectors: bool = False) -> Tuple[Tensor, Optional[LinearOperator]]:
+    def _symeig(
+        self: Float[LinearOperator, "*batch N N"],
+        eigenvectors: bool = False,
+        return_evals_as_lazy: Optional[bool] = False,
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         if isinstance(self._diag_tensor, ConstantDiagLinearOperator):
             evals_, evecs = self._linear_op._symeig(eigenvectors=eigenvectors)
             evals = evals_ + self._diag_tensor._diagonal()
             return evals, evecs
         return super()._symeig(eigenvectors=eigenvectors)
 
-    def evaluate_kernel(self) -> LinearOperator:
+    def evaluate_kernel(self):
         added_diag_linear_op = self.representation_tree()(*self.representation())
         return added_diag_linear_op._linear_op + added_diag_linear_op._diag_tensor
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/batch_repeat_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/batch_repeat_linear_operator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/env python3
+from __future__ import annotations
 
 import itertools
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
 from torch import Tensor
 
 from .. import settings
 from ..utils.broadcasting import _matmul_broadcast_shape
 from ..utils.memoize import cached
-from ._linear_operator import LinearOperator
+from ._linear_operator import IndexType, LinearOperator
 
 
 class BatchRepeatLinearOperator(LinearOperator):
     def __init__(self, base_linear_op, batch_repeat=torch.Size((1,))):
         if settings.debug.on():
             if not isinstance(batch_repeat, torch.Size):
                 raise RuntimeError(
@@ -33,77 +35,89 @@
             base_linear_op = base_linear_op.unsqueeze(0)
 
         super().__init__(base_linear_op, batch_repeat=batch_repeat)
         self.base_linear_op = base_linear_op
         self.batch_repeat = batch_repeat
 
     @cached(name="cholesky")
-    def _cholesky(self, upper=False):
+    def _cholesky(
+        self: Float[LinearOperator, "*batch N N"], upper: Optional[bool] = False
+    ) -> Float[LinearOperator, "*batch N N"]:
         from .triangular_linear_operator import TriangularLinearOperator
 
         res = self.base_linear_op.cholesky(upper=upper)._tensor
         res = res.repeat(*self.batch_repeat, 1, 1)
         return TriangularLinearOperator(res, upper=upper)
 
-    def _cholesky_solve(self, rhs, upper: bool = False):
+    def _cholesky_solve(
+        self: Float[LinearOperator, "*batch N N"],
+        rhs: Union[Float[LinearOperator, "*batch2 N M"], Float[Tensor, "*batch2 N M"]],
+        upper: Optional[bool] = False,
+    ) -> Union[Float[LinearOperator, "... N M"], Float[Tensor, "... N M"]]:
         # TODO: Figure out how to deal with this with TriangularLinearOperator if returned by _cholesky
         output_shape = _matmul_broadcast_shape(self.shape, rhs.shape)
         if rhs.shape != output_shape:
             rhs = rhs.expand(*output_shape)
 
         rhs = self._move_repeat_batches_to_columns(rhs, output_shape)
         res = self.base_linear_op._cholesky_solve(rhs, upper=upper)
         res = self._move_repeat_batches_back(res, output_shape)
         return res
 
-    def _compute_batch_repeat_size(self, current_batch_shape, desired_batch_shape):
+    def _compute_batch_repeat_size(
+        self, current_batch_shape: Union[torch.Size, List[int]], desired_batch_shape: Union[torch.Size, List[int]]
+    ) -> torch.Size:
         batch_repeat = torch.Size(
             desired_batch_size // current_batch_size
             for desired_batch_size, current_batch_size in zip(desired_batch_shape, current_batch_shape)
         )
         return batch_repeat
 
-    def _expand_batch(self, batch_shape):
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         padding_dims = torch.Size(tuple(1 for _ in range(max(len(batch_shape) + 2 - self.base_linear_op.dim(), 0))))
         current_batch_shape = padding_dims + self.base_linear_op.batch_shape
         return self.__class__(
-            self.base_linear_op,
-            batch_repeat=self._compute_batch_repeat_size(current_batch_shape, batch_shape),
+            self.base_linear_op, batch_repeat=self._compute_batch_repeat_size(current_batch_shape, batch_shape)
         )
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         # First remove any new batch indices that were added - they aren't necessary
         num_true_batch_indices = self.base_linear_op.dim() - 2
         batch_indices = batch_indices[len(batch_indices) - num_true_batch_indices :]
 
         # Now adjust the indices batch_indices that were repeated
         batch_indices = [
             batch_index.fmod(size) for batch_index, size in zip(batch_indices, self.base_linear_op.batch_shape)
         ]
 
         # Now call the sub _get_indices method
         res = self.base_linear_op._get_indices(row_index, col_index, *batch_indices)
         return res
 
-    def _getitem(self, row_index, col_index, *batch_indices):
+    def _getitem(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> LinearOperator:
         args = []
         kwargs = self.base_linear_op._kwargs
         num_base_batch_dims = len(self.base_linear_op.batch_shape)
 
         for arg in self.base_linear_op._args:
             if torch.is_tensor(arg) or isinstance(arg, LinearOperator):
                 arg_base_shape_len = max(arg.dim() - num_base_batch_dims, 0)
                 args.append(arg.repeat(*self.batch_repeat, *[1 for _ in range(arg_base_shape_len)]))
             else:
                 args.append(arg)
 
         new_linear_op = self.base_linear_op.__class__(*args, **kwargs)
         return new_linear_op._getitem(row_index, col_index, *batch_indices)
 
-    def _matmul(self, rhs):
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         output_shape = _matmul_broadcast_shape(self.shape, rhs.shape)
 
         # only attempt broadcasting if the non-batch dimensions are the same
         if self.is_square:
             if rhs.shape != output_shape:
                 rhs = rhs.expand(*output_shape)
 
@@ -175,71 +189,84 @@
         batch_dims = range(1, len(batch_repeat) * 2, 2)
         batch_matrix = batch_matrix.permute(*batch_dims, -2, -1, *repeat_dims).contiguous()
         batch_matrix = batch_matrix.view(*self.base_linear_op.batch_shape, output_shape[-2], -1)
 
         self.__batch_move_memo = output_shape, padded_base_batch_shape, batch_repeat
         return batch_matrix
 
-    def _permute_batch(self, *dims):
+    def _permute_batch(self, *dims: int) -> LinearOperator:
         new_batch_repeat = torch.Size(tuple(self.batch_repeat[dim] for dim in dims))
         res = self.__class__(self.base_linear_op._permute_batch(*dims), batch_repeat=new_batch_repeat)
         return res
 
-    def _bilinear_derivative(self, left_vectors, right_vectors):
+    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Optional[Tensor], ...]:
         if self.is_square:
-            left_output_shape = _matmul_broadcast_shape(self.shape, left_vectors.shape)
-            if left_output_shape != left_vectors.shape:
-                left_vectors = left_vectors.expand(left_output_shape)
-
-            right_output_shape = _matmul_broadcast_shape(self.shape, right_vectors.shape)
-            if right_output_shape != right_vectors.shape:
-                right_vectors = right_vectors.expand(right_output_shape)
+            left_output_shape = _matmul_broadcast_shape(self.shape, left_vecs.shape)
+            if left_output_shape != left_vecs.shape:
+                left_vecs = left_vecs.expand(left_output_shape)
+
+            right_output_shape = _matmul_broadcast_shape(self.shape, right_vecs.shape)
+            if right_output_shape != right_vecs.shape:
+                right_vecs = right_vecs.expand(right_output_shape)
 
-            left_vectors = self._move_repeat_batches_to_columns(left_vectors, left_output_shape)
-            right_vectors = self._move_repeat_batches_to_columns(right_vectors, right_output_shape)
+            left_vecs = self._move_repeat_batches_to_columns(left_vecs, left_output_shape)
+            right_vecs = self._move_repeat_batches_to_columns(right_vecs, right_output_shape)
 
-            return self.base_linear_op._bilinear_derivative(left_vectors, right_vectors)
+            return self.base_linear_op._bilinear_derivative(left_vecs, right_vecs)
         else:
-            return super()._bilinear_derivative(left_vectors, right_vectors)
+            return super()._bilinear_derivative(left_vecs, right_vecs)
 
-    def _root_decomposition(self):
+    def _root_decomposition(
+        self: Float[LinearOperator, "... N N"]
+    ) -> Union[Float[torch.Tensor, "... N N"], Float[LinearOperator, "... N N"]]:
         return self.base_linear_op._root_decomposition().repeat(*self.batch_repeat, 1, 1)
 
-    def _root_inv_decomposition(self, initial_vectors=None):
+    def _root_inv_decomposition(
+        self: Float[LinearOperator, "*batch N N"],
+        initial_vectors: Optional[torch.Tensor] = None,
+        test_vectors: Optional[torch.Tensor] = None,
+    ) -> Union[Float[LinearOperator, "... N N"], Float[Tensor, "... N N"]]:
         return self.base_linear_op._root_inv_decomposition().repeat(*self.batch_repeat, 1, 1)
 
-    def _size(self):
+    def _size(self) -> torch.Size:
         repeated_batch_shape = torch.Size(
             size * repeat for size, repeat in zip(self.base_linear_op.batch_shape, self.batch_repeat)
         )
         res = torch.Size(repeated_batch_shape + self.base_linear_op.matrix_shape)
         return res
 
-    def _transpose_nonbatch(self):
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         return self.__class__(self.base_linear_op._transpose_nonbatch(), batch_repeat=self.batch_repeat)
 
-    def _unsqueeze_batch(self, dim):
+    def _unsqueeze_batch(self, dim: int) -> LinearOperator:
         base_linear_op = self.base_linear_op
         batch_repeat = list(self.batch_repeat)
         batch_repeat.insert(dim, 1)
         batch_repeat = torch.Size(batch_repeat)
         # If the dim only adds a new padded dimension, then we're done
         # Otherwise we have to also unsqueeze the base_linear_op
         base_unsqueeze_dim = dim - (len(self.base_linear_op.batch_shape) - len(self.base_linear_op.batch_shape))
         if base_unsqueeze_dim > 0:
             base_linear_op = base_linear_op._unsqueeze_batch(base_unsqueeze_dim)
         return self.__class__(base_linear_op, batch_repeat=batch_repeat)
 
-    def add_jitter(self, jitter_val=1e-3):
-        return self.__class__(
-            self.base_linear_op.add_jitter(jitter_val=jitter_val),
-            batch_repeat=self.batch_repeat,
-        )
-
-    def inv_quad_logdet(self, inv_quad_rhs=None, logdet=False, reduce_inv_quad=True):
+    def add_jitter(
+        self: Float[LinearOperator, "*batch N N"], jitter_val: float = 1e-3
+    ) -> Float[LinearOperator, "*batch N N"]:
+        return self.__class__(self.base_linear_op.add_jitter(jitter_val=jitter_val), batch_repeat=self.batch_repeat)
+
+    def inv_quad_logdet(
+        self: Float[LinearOperator, "*batch N N"],
+        inv_quad_rhs: Optional[Union[Float[Tensor, "*batch N M"], Float[Tensor, "*batch N"]]] = None,
+        logdet: Optional[bool] = False,
+        reduce_inv_quad: Optional[bool] = True,
+    ) -> Tuple[
+        Optional[Union[Float[Tensor, "*batch M"], Float[Tensor, " *batch"], Float[Tensor, " 0"]]],
+        Optional[Float[Tensor, "..."]],
+    ]:
         if not self.is_square:
             raise RuntimeError(
                 "inv_quad_logdet only operates on (batches of) square (positive semi-definite) LinearOperators. "
                 "Got a {} of size {}.".format(self.__class__.__name__, self.size())
             )
 
         if inv_quad_rhs is not None:
@@ -270,15 +297,15 @@
                 inv_quad_term = inv_quad_term.sum(-1)
 
         if logdet_term is not None and logdet_term.numel():
             logdet_term = logdet_term.repeat(*self.batch_repeat)
 
         return inv_quad_term, logdet_term
 
-    def repeat(self, *sizes):
+    def repeat(self, *sizes: Union[int, Tuple[int, ...]]) -> LinearOperator:
         if len(sizes) < 3 or tuple(sizes[-2:]) != (1, 1):
             raise RuntimeError(
                 "Invalid repeat arguments {}. Currently, repeat only works to create repeated "
                 "batches of a 2D LinearOperator.".format(tuple(sizes))
             )
 
         padded_batch_repeat = tuple(1 for _ in range(len(sizes) - 2 - len(self.batch_repeat))) + self.batch_repeat
@@ -287,20 +314,26 @@
             batch_repeat=torch.Size(
                 orig_repeat_size * new_repeat_size
                 for orig_repeat_size, new_repeat_size in zip(padded_batch_repeat, sizes[:-2])
             ),
         )
 
     @cached(name="svd")
-    def _svd(self) -> Tuple["LinearOperator", Tensor, "LinearOperator"]:
+    def _svd(
+        self: Float[LinearOperator, "*batch N N"]
+    ) -> Tuple[Float[LinearOperator, "*batch N N"], Float[Tensor, "... N"], Float[LinearOperator, "*batch N N"]]:
         U_, S_, V_ = self.base_linear_op.svd()
         U = U_.repeat(*self.batch_repeat, 1, 1)
         S = S_.repeat(*self.batch_repeat, 1)
         V = V_.repeat(*self.batch_repeat, 1, 1)
         return U, S, V
 
-    def _symeig(self, eigenvectors: bool = False) -> Tuple[Tensor, Optional[LinearOperator]]:
+    def _symeig(
+        self: Float[LinearOperator, "*batch N N"],
+        eigenvectors: bool = False,
+        return_evals_as_lazy: Optional[bool] = False,
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         evals, evecs = self.base_linear_op._symeig(eigenvectors=eigenvectors)
         evals = evals.repeat(*self.batch_repeat, 1)
         if eigenvectors:
             evecs = evecs.repeat(*self.batch_repeat, 1, 1)
         return evals, evecs
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/block_diag_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/block_interleaved_linear_operator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,138 +1,141 @@
 #!/usr/bin/env python3
-
-from abc import ABCMeta
-from typing import Optional, Tuple
+from typing import Callable, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
 from torch import Tensor
 
 from ..utils.memoize import cached
-from ._linear_operator import LinearOperator
+from ._linear_operator import IndexType, LinearOperator
 from .block_linear_operator import BlockLinearOperator
 
 
-# metaclass of BlockDiagLinearOperator, overwrites behavior of constructor call
-# _MetaBlockDiagLinearOperator(base_linear_op, block_dim=-3) to return a DiagLinearOperator
-# if base_linear_op is a DiagLinearOperator itself
-class _MetaBlockDiagLinearOperator(ABCMeta):
-    def __call__(cls, base_linear_op: LinearOperator, block_dim=-3):
-        from .diag_linear_operator import DiagLinearOperator
-
-        if cls is BlockDiagLinearOperator and isinstance(base_linear_op, DiagLinearOperator):
-            if block_dim != -3:
-                raise NotImplementedError(
-                    "Passing a base_linear_op of type DiagLinearOperator to the constructor of "
-                    f"BlockDiagLinearOperator with block_dim = {block_dim} != -3 is not supported."
-                )
-            else:
-                diag = base_linear_op._diag.flatten(-2, -1)  # flatten last two dimensions of diag
-                return DiagLinearOperator(diag)
-        else:
-            return type.__call__(cls, base_linear_op, block_dim)
-
-
-class BlockDiagLinearOperator(BlockLinearOperator, metaclass=_MetaBlockDiagLinearOperator):
+class BlockInterleavedLinearOperator(BlockLinearOperator):
     """
     Represents a lazy tensor that is the block diagonal of square matrices.
     The :attr:`block_dim` attribute specifies which dimension of the base LinearOperator
     specifies the blocks.
     For example, (with `block_dim=-3` a `k x n x n` tensor represents `k` `n x n` blocks (a `kn x kn` matrix).
     A `b x k x n x n` tensor represents `k` `b x n x n` blocks (a `b x kn x kn` batch matrix).
 
     Args:
         :attr:`base_linear_op` (LinearOperator or Tensor):
             Must be at least 3 dimensional.
         :attr:`block_dim` (int):
             The dimension that specifies the blocks.
     """
 
-    def __init__(self, base_linear_op, block_dim=-3):
-        super().__init__(base_linear_op, block_dim)
-        # block diagonal is restricted to have square diagonal blocks
-        if self.base_linear_op.shape[-1] != self.base_linear_op.shape[-2]:
-            raise RuntimeError(
-                "base_linear_op must be a batch of square matrices, but non-batch dimensions are "
-                f"{base_linear_op.shape[-2:]}"
-            )
-
     @property
-    def num_blocks(self):
+    def num_blocks(self) -> int:
         return self.base_linear_op.size(-3)
 
     def _add_batch_dim(self, other):
         *batch_shape, num_rows, num_cols = other.shape
         batch_shape = list(batch_shape)
 
-        batch_shape.append(self.num_blocks)
-        other = other.view(*batch_shape, num_rows // self.num_blocks, num_cols)
+        batch_shape.append(num_rows // self.num_blocks)
+        other = other.view(*batch_shape, self.num_blocks, num_cols)
+        other = other.transpose(-2, -3).contiguous()
         return other
 
     @cached(name="cholesky")
-    def _cholesky(self, upper=False):
+    def _cholesky(
+        self: Float[LinearOperator, "*batch N N"], upper: Optional[bool] = False
+    ) -> Float[LinearOperator, "*batch N N"]:
         from .triangular_linear_operator import TriangularLinearOperator
 
         chol = self.__class__(self.base_linear_op.cholesky(upper=upper))
         return TriangularLinearOperator(chol, upper=upper)
 
-    def _cholesky_solve(self, rhs, upper: bool = False):
+    def _cholesky_solve(
+        self: Float[LinearOperator, "*batch N N"],
+        rhs: Union[Float[LinearOperator, "*batch2 N M"], Float[Tensor, "*batch2 N M"]],
+        upper: Optional[bool] = False,
+    ) -> Union[Float[LinearOperator, "... N M"], Float[Tensor, "... N M"]]:
         rhs = self._add_batch_dim(rhs)
         res = self.base_linear_op._cholesky_solve(rhs, upper=upper)
         res = self._remove_batch_dim(res)
         return res
 
-    def _diagonal(self):
-        res = self.base_linear_op._diagonal().contiguous()
-        return res.view(*self.batch_shape, self.size(-1))
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
+        block_diag = self.base_linear_op._diagonal()
+        return block_diag.mT.contiguous().view(*block_diag.shape[:-2], -1)
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         # Figure out what block the row/column indices belong to
-        row_index_block = torch.div(row_index, self.base_linear_op.size(-2), rounding_mode="floor")
-        col_index_block = torch.div(col_index, self.base_linear_op.size(-1), rounding_mode="floor")
+        row_index_block = row_index.fmod(self.base_linear_op.size(-3))
+        col_index_block = col_index.fmod(self.base_linear_op.size(-3))
 
         # Find the row/col index within each block
-        row_index = row_index.fmod(self.base_linear_op.size(-2))
-        col_index = col_index.fmod(self.base_linear_op.size(-1))
+        row_index = torch.div(row_index, self.base_linear_op.size(-3), rounding_mode="floor")
+        col_index = torch.div(col_index, self.base_linear_op.size(-3), rounding_mode="floor")
 
         # If the row/column blocks do not agree, then we have off diagonal elements
         # These elements should be zeroed out
         res = self.base_linear_op._get_indices(row_index, col_index, *batch_indices, row_index_block)
         res = res * torch.eq(row_index_block, col_index_block).type_as(res)
         return res
 
     def _remove_batch_dim(self, other):
+        other = other.transpose(-2, -3).contiguous()
         shape = list(other.shape)
-        del shape[-3]
+        del shape[-2]
         shape[-2] *= self.num_blocks
         other = other.reshape(*shape)
         return other
 
-    def _root_decomposition(self):
+    def _root_decomposition(
+        self: Float[LinearOperator, "... N N"]
+    ) -> Union[Float[torch.Tensor, "... N N"], Float[LinearOperator, "... N N"]]:
         return self.__class__(self.base_linear_op._root_decomposition())
 
-    def _root_inv_decomposition(self, initial_vectors=None):
+    def _root_inv_decomposition(
+        self: Float[LinearOperator, "*batch N N"],
+        initial_vectors: Optional[torch.Tensor] = None,
+        test_vectors: Optional[torch.Tensor] = None,
+    ) -> Union[Float[LinearOperator, "... N N"], Float[Tensor, "... N N"]]:
         return self.__class__(self.base_linear_op._root_inv_decomposition(initial_vectors))
 
-    def _size(self):
+    def _size(self) -> torch.Size:
         shape = list(self.base_linear_op.shape)
         shape[-2] *= shape[-3]
         shape[-1] *= shape[-3]
         del shape[-3]
         return torch.Size(shape)
 
-    def _solve(self, rhs, preconditioner, num_tridiag=0):
+    def _solve(
+        self: Float[LinearOperator, "... N N"],
+        rhs: Float[torch.Tensor, "... N C"],
+        preconditioner: Optional[Callable[[Float[torch.Tensor, "... N C"]], Float[torch.Tensor, "... N C"]]] = None,
+        num_tridiag: Optional[int] = 0,
+    ) -> Union[
+        Float[torch.Tensor, "... N C"],
+        Tuple[
+            Float[torch.Tensor, "... N C"],
+            Float[torch.Tensor, "..."],  # Note that in case of a tuple the second term size depends on num_tridiag
+        ],
+    ]:
         if num_tridiag:
             return super()._solve(rhs, preconditioner, num_tridiag=num_tridiag)
         else:
             rhs = self._add_batch_dim(rhs)
             res = self.base_linear_op._solve(rhs, preconditioner, num_tridiag=None)
             res = self._remove_batch_dim(res)
             return res
 
-    def inv_quad_logdet(self, inv_quad_rhs=None, logdet=False, reduce_inv_quad=True):
+    def inv_quad_logdet(
+        self: Float[LinearOperator, "*batch N N"],
+        inv_quad_rhs: Optional[Union[Float[Tensor, "*batch N M"], Float[Tensor, "*batch N"]]] = None,
+        logdet: Optional[bool] = False,
+        reduce_inv_quad: Optional[bool] = True,
+    ) -> Tuple[
+        Optional[Union[Float[Tensor, "*batch M"], Float[Tensor, " *batch"], Float[Tensor, " 0"]]],
+        Optional[Float[Tensor, "..."]],
+    ]:
         if inv_quad_rhs is not None:
             inv_quad_rhs = self._add_batch_dim(inv_quad_rhs)
         inv_quad_res, logdet_res = self.base_linear_op.inv_quad_logdet(
             inv_quad_rhs, logdet, reduce_inv_quad=reduce_inv_quad
         )
         if inv_quad_res is not None and inv_quad_res.numel():
             if reduce_inv_quad:
@@ -140,41 +143,7 @@
                 inv_quad_res = inv_quad_res.sum(-1)
             else:
                 inv_quad_res = inv_quad_res.view(*self.base_linear_op.batch_shape, inv_quad_res.size(-1))
                 inv_quad_res = inv_quad_res.sum(-2)
         if logdet_res is not None and logdet_res.numel():
             logdet_res = logdet_res.view(*logdet_res.shape).sum(-1)
         return inv_quad_res, logdet_res
-
-    def matmul(self, other):
-        from .diag_linear_operator import DiagLinearOperator
-
-        # this is trivial if we multiply two BlockDiagLinearOperator with matching block sizes
-        if isinstance(other, BlockDiagLinearOperator) and self.base_linear_op.shape == other.base_linear_op.shape:
-            return BlockDiagLinearOperator(self.base_linear_op @ other.base_linear_op)
-        # special case if we have a DiagLinearOperator
-        if isinstance(other, DiagLinearOperator):
-            # matmul is going to be cheap because of the special casing in DiagLinearOperator
-            diag_reshape = other._diag.view(*self.base_linear_op.shape[:-1])
-            diag = DiagLinearOperator(diag_reshape)
-            return BlockDiagLinearOperator(self.base_linear_op @ diag)
-        return super().matmul(other)
-
-    @cached(name="svd")
-    def _svd(self) -> Tuple["LinearOperator", Tensor, "LinearOperator"]:
-        U, S, V = self.base_linear_op.svd()
-        # Doesn't make much sense to sort here, o/w we lose the structure
-        S = S.reshape(*S.shape[:-2], S.shape[-2:].numel())
-        # can assume that block_dim is -3 here
-        U = self.__class__(U)
-        V = self.__class__(V)
-        return U, S, V
-
-    def _symeig(self, eigenvectors: bool = False) -> Tuple[Tensor, Optional[LinearOperator]]:
-        evals, evecs = self.base_linear_op._symeig(eigenvectors=eigenvectors)
-        # Doesn't make much sense to sort here, o/w we lose the structure
-        evals = evals.reshape(*evals.shape[:-2], evals.shape[-2:].numel())
-        if eigenvectors:
-            evecs = self.__class__(evecs)  # can assume that block_dim is -3 here
-        else:
-            evecs = None
-        return evals, evecs
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/block_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/block_linear_operator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #!/usr/bin/env python3
 
 from abc import abstractmethod
+from typing import List, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
+from torch import Tensor
 
 from ..utils.getitem import _is_noop_index, _noop_index
-from ._linear_operator import LinearOperator
+from ._linear_operator import IndexType, LinearOperator
 from .dense_linear_operator import to_linear_operator
 
 
 class BlockLinearOperator(LinearOperator):
     """
     An abstract LinearOperator class for block tensors.
     Subclasses will determine how the different blocks are layed out
@@ -51,42 +54,36 @@
         super(BlockLinearOperator, self).__init__(to_linear_operator(base_linear_op))
         self.base_linear_op = base_linear_op
 
     @abstractmethod
     def _add_batch_dim(self, other):
         raise NotImplementedError
 
-    def _expand_batch(self, batch_shape):
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         batch_shape = torch.Size((*batch_shape, self.base_linear_op.size(-3)))
         res = self.__class__(self.base_linear_op._expand_batch(batch_shape))
         return res
 
-    def _getitem(self, row_index, col_index, *batch_indices):
+    def _getitem(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> LinearOperator:
         # First the easy case: just batch indexing
         if _is_noop_index(row_index) and _is_noop_index(col_index):
             return self.__class__(self.base_linear_op._getitem(row_index, col_index, *batch_indices, _noop_index))
 
         # If either of the dimensions are indices, it's too complicated - go with the base case
         if not isinstance(row_index, slice) or not isinstance(col_index, slice):
             # It's too complicated to deal with tensor indices in this case - we'll use the super method
             return super()._getitem(row_index, col_index, *batch_indices)
 
         # Now we know that row_index and col_index
         num_blocks = self.num_blocks
         num_rows, num_cols = self.matrix_shape
-        row_start, row_end, row_step = (
-            row_index.start or 0,
-            row_index.stop or num_rows,
-            row_index.step,
-        )
-        col_start, col_end, col_step = (
-            col_index.start or 0,
-            col_index.stop or num_cols,
-            col_index.step,
-        )
+        row_start, row_end, row_step = row_index.start or 0, row_index.stop or num_rows, row_index.step
+        col_start, col_end, col_step = col_index.start or 0, col_index.stop or num_cols, col_index.step
 
         # If we have a step, it's too complicated - go with the base case
         if row_step is not None or col_step is not None:
             return super()._getitem(row_index, col_index, *batch_indices)
 
         # Let's make sure that the slice dimensions perfectly correspond with the number of
         # outputs per input that we have
@@ -100,71 +97,78 @@
 
         # Now we can try the super call!
         new_base_linear_op = self.base_linear_op._getitem(row_index, col_index, *batch_indices)
 
         # Now construct a kernel with those indices
         return self.__class__(new_base_linear_op, block_dim=-3)
 
-    def _matmul(self, rhs):
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         isvector = rhs.ndimension() == 1
         if isvector:
             rhs = rhs.unsqueeze(1)
 
         rhs = self._add_batch_dim(rhs)
         res = self.base_linear_op._matmul(rhs)
         res = self._remove_batch_dim(res)
 
         if isvector:
             res = res.squeeze(-1)
         return res
 
-    def _bilinear_derivative(self, left_vecs, right_vecs):
+    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Optional[Tensor], ...]:
         if left_vecs.ndim == 1:
             left_vecs = left_vecs.unsqueeze(-1)
             right_vecs = right_vecs.unsqueeze(-1)
         # deal with left_vecs having batch dimensions
         elif left_vecs.size(-1) != right_vecs.size(-1):
             left_vecs = left_vecs.unsqueeze(-1)
         left_vecs = self._add_batch_dim(left_vecs)
         right_vecs = self._add_batch_dim(right_vecs)
         res = self.base_linear_op._bilinear_derivative(left_vecs, right_vecs)
         return res
 
-    def _permute_batch(self, *dims):
+    def _permute_batch(self, *dims: int) -> LinearOperator:
         if torch.is_tensor(self.base_linear_op):
             base_linear_op = self.base_linear_op.permute(*dims, -3, -2, -1)
         else:
             base_linear_op = self.base_linear_op._permute_batch(*dims, self.base_linear_op.dim() - 3)
         res = self.__class__(base_linear_op)
         return res
 
-    def _unsqueeze_batch(self, dim):
+    def _unsqueeze_batch(self, dim: int) -> LinearOperator:
         if torch.is_tensor(self.base_linear_op):
             base_linear_op = self.base_linear_op.unsqueeze(dim)
         else:
             base_linear_op = self.base_linear_op._unsqueeze_batch(dim)
         res = self.__class__(base_linear_op)
         return res
 
     @abstractmethod
     def _remove_batch_dim(self, other):
         raise NotImplementedError
 
-    def _mul_constant(self, other):
+    def _mul_constant(
+        self: Float[LinearOperator, "*batch M N"], other: Union[float, torch.Tensor]
+    ) -> Float[LinearOperator, "*batch M N"]:
         # We're using a custom method here - the constant mul is applied to the base_lazy tensor
         # This preserves the block structure
         from .constant_mul_linear_operator import ConstantMulLinearOperator
 
         return self.__class__(ConstantMulLinearOperator(self.base_linear_op, other))
 
-    def _transpose_nonbatch(self):
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         base_op = self.base_linear_op
         if isinstance(base_op, LinearOperator):
             new_base_op = base_op._transpose_nonbatch()
         else:
             new_base_op = base_op.transpose(-1, -2)
         return self.__class__(new_base_op)
 
-    def zero_mean_mvn_samples(self, num_samples):
+    def zero_mean_mvn_samples(
+        self: Float[LinearOperator, "*batch N N"], num_samples: int
+    ) -> Float[Tensor, "num_samples *batch N"]:
         res = self.base_linear_op.zero_mean_mvn_samples(num_samples)
         res = self._remove_batch_dim(res.unsqueeze(-1)).squeeze(-1)
         return res
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/cat_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/cat_linear_operator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
-from typing import Tuple, Union
+from typing import List, Optional, Sequence, Tuple, Union
 
 import torch
+from jaxtyping import Float
+from torch import Tensor
 
 from ..utils.broadcasting import _matmul_broadcast_shape
 from ..utils.deprecation import bool_compat
 from ..utils.generic import _to_helper
 from ..utils.getitem import _noop_index
-from ._linear_operator import LinearOperator, to_dense
+from ._linear_operator import IndexType, LinearOperator, to_dense
 from .dense_linear_operator import DenseLinearOperator, to_linear_operator
 
 
 def cat(inputs, dim=0, output_device=None):
     if all(torch.is_tensor(i) for i in inputs):
         return torch.cat(inputs, dim=dim)
 
@@ -94,22 +96,18 @@
         for tsr_idx, (start_idx, end_idx) in enumerate(zip(cat_dim_cum_sizes[:-1], cat_dim_cum_sizes[1:])):
             idx_to_tensor_idx[start_idx.item() : end_idx.item()].fill_(tsr_idx)
 
         self.cat_dim_sizes = cat_dim_sizes
         self.cat_dim_cum_sizes = cat_dim_cum_sizes
         self.idx_to_tensor_idx = idx_to_tensor_idx
         self._shape = torch.Size(
-            (
-                *rep_tensor.shape[:positive_dim],
-                cat_dim_cum_sizes[-1].item(),
-                *rep_tensor.shape[positive_dim + 1 :],
-            )
+            (*rep_tensor.shape[:positive_dim], cat_dim_cum_sizes[-1].item(), *rep_tensor.shape[positive_dim + 1 :])
         )
 
-    def _split_slice(self, slice_idx):
+    def _split_slice(self, slice_idx: slice) -> Tuple[Sequence[int], List[slice]]:
         """
         Splits a slice(a, b, None) in to a list of slices [slice(a1, b1, None), slice(a2, b2, None), ...]
         so that each slice in the list slices in to a single tensor that we have concatenated with this LinearOperator.
         """
         if slice_idx.step is not None:
             # TODO: Add support for this eventually.
             raise RuntimeError("Slicing a CatLinearOperator with a step is not currently supported!")
@@ -129,15 +127,15 @@
             first_slice = slice(first_tensor_start_index, None, None)
             last_slice = slice(None, last_tensor_stop_index, None)
             return (
                 list(range(first_tensor_idx, last_tensor_idx + 1)),
                 [first_slice] + [_noop_index] * num_middle_tensors + [last_slice],
             )
 
-    def _diagonal(self):
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
         if self.cat_dim == -2:
             res = []
             curr_col = 0
             for t in self.linear_ops:
                 n_rows, n_cols = t.shape[-2:]
                 rows = torch.arange(0, n_rows, dtype=torch.long, device=t.device)
                 cols = torch.arange(curr_col, curr_col + n_rows, dtype=torch.long, device=t.device)
@@ -151,21 +149,20 @@
                 n_rows, n_cols = t.shape[-2:]
                 rows = torch.arange(curr_row, curr_row + n_cols, dtype=torch.long, device=t.device)
                 cols = torch.arange(0, n_cols, dtype=torch.long, device=t.device)
                 curr_row += n_cols
                 res.append(t[..., rows, cols].to(self.device))
             res = torch.cat(res, dim=-1)
         else:
-            res = torch.cat(
-                [t._diagonal().to(self.device) for t in self.linear_ops],
-                dim=self.cat_dim + 1,
-            )
+            res = torch.cat([t._diagonal().to(self.device) for t in self.linear_ops], dim=self.cat_dim + 1)
         return res
 
-    def _expand_batch(self, batch_shape):
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         batch_dim = self.cat_dim + 2
         if batch_dim < 0:
             if batch_shape[batch_dim] != self.batch_shape[batch_dim]:
                 raise RuntimeError(
                     f"Trying to expand a CatLinearOperator in dimension {self.cat_dim}, but this is the concatenated "
                     f"dimension.\nCurrent shape: {self.shape} - expanded shape: {batch_shape + self.matrix_shape}."
                 )
@@ -175,15 +172,15 @@
                 sub_batch_shape[batch_dim] = linear_op.shape[self.cat_dim]
                 linear_ops.append(linear_op._expand_batch(sub_batch_shape))
         else:
             linear_ops = [linear_op._expand_batch(batch_shape) for linear_op in self.linear_ops]
         res = self.__class__(*linear_ops, dim=self.cat_dim, output_device=self.output_device)
         return res
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         indices = [*batch_indices, row_index, col_index]
         target_shape = torch.broadcast_shapes(*[index.shape for index in indices])
         indices = [index.expand(target_shape).reshape(-1) for index in indices]
         cat_dim_indices = indices[self.cat_dim]
 
         # Find out for which indices we switch to different tensors
         target_tensors = self.idx_to_tensor_idx[cat_dim_indices]
@@ -218,20 +215,15 @@
             return res_list[0].view(target_shape).to(self.device)
         else:
             # Explicitly move tensors to one device as torch.cat no longer moves tensors:
             # https://github.com/pytorch/pytorch/issues/35045
             res_list = [linear_op.to(self.device) for linear_op in res_list]
             return torch.cat(res_list).view(target_shape)
 
-    def _getitem(
-        self,
-        row_index: Union[slice, torch.LongTensor],
-        col_index: Union[slice, torch.LongTensor],
-        *batch_indices: Tuple[Union[int, slice, torch.LongTensor], ...],
-    ) -> LinearOperator:
+    def _getitem(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> LinearOperator:
         indices = [*batch_indices, row_index, col_index]
         cat_dim_indices = indices[self.cat_dim]
 
         # If any of the (non-cat_dim) batch indices are ints, make sure that we appropriately update the cat_dim
         updated_cat_dim = self.cat_dim
         if self.cat_dim < -2:
             batch_indices_below_cat_dim = batch_indices[self.cat_dim + 3 :]
@@ -304,15 +296,18 @@
         # Process the list
         if len(res_list) == 1:
             return res_list[0].to(self.output_device)
         else:
             res = self.__class__(*res_list, dim=updated_cat_dim, output_device=self.output_device)
             return res
 
-    def _matmul(self, rhs):
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         output_device = self.device if self.device is not None else rhs.device
         # make a copy of `rhs` on each device
         rhs_ = []
         for d in self.devices:
             if d != rhs.device:
                 rhs_.append(rhs.to(d))
             else:
@@ -347,69 +342,73 @@
                 curr_idx += size
             # copy result back to output device
             res_list = [x.to(output_device) for x in res_list]
             res = torch.cat(res_list, dim=self.cat_dim)
 
         return res
 
-    def _permute_batch(self, *dims):
+    def _permute_batch(self, *dims: int) -> LinearOperator:
         linear_ops = [linear_op._permute_batch(*dims) for linear_op in self.linear_ops]
         if self.cat_dim < -2:
             positive_cat_dim = self.dim() + self.cat_dim
             new_cat_dim = dims.index(positive_cat_dim)
         else:
             new_cat_dim = self.cat_dim
         return self.__class__(*linear_ops, dim=new_cat_dim, output_device=self.output_device)
 
-    def _size(self):
+    def _size(self) -> torch.Size:
         return self._shape
 
-    def _transpose_nonbatch(self):
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         if self.cat_dim == -2:
             new_dim = -1
         elif self.cat_dim == -1:
             new_dim = -2
         else:
             new_dim = self.cat_dim
         return self.__class__(
-            *[t._transpose_nonbatch() for t in self.linear_ops],
-            dim=new_dim,
-            output_device=self.output_device,
+            *[t._transpose_nonbatch() for t in self.linear_ops], dim=new_dim, output_device=self.output_device
         )
 
-    def _unsqueeze_batch(self, dim):
+    def _unsqueeze_batch(self, dim: int) -> LinearOperator:
         cat_dim = self.dim() + self.cat_dim
         linear_ops = [linear_op._unsqueeze_batch(dim) for linear_op in self.linear_ops]
         res = self.__class__(
-            *linear_ops,
-            dim=(cat_dim + 1 if dim <= cat_dim else cat_dim),
-            output_device=self.output_device,
+            *linear_ops, dim=(cat_dim + 1 if dim <= cat_dim else cat_dim), output_device=self.output_device
         )
         return res
 
-    def to_dense(self):
+    def to_dense(self: Float[LinearOperator, "*batch M N"]) -> Float[Tensor, "*batch M N"]:
         return torch.cat([to_dense(L) for L in self.linear_ops], dim=self.cat_dim)
 
-    def inv_quad_logdet(self, inv_quad_rhs=None, logdet=False, reduce_inv_quad=True):
+    def inv_quad_logdet(
+        self: Float[LinearOperator, "*batch N N"],
+        inv_quad_rhs: Optional[Union[Float[Tensor, "*batch N M"], Float[Tensor, "*batch N"]]] = None,
+        logdet: Optional[bool] = False,
+        reduce_inv_quad: Optional[bool] = True,
+    ) -> Tuple[
+        Optional[Union[Float[Tensor, "*batch M"], Float[Tensor, " *batch"], Float[Tensor, " 0"]]],
+        Optional[Float[Tensor, "..."]],
+    ]:
         res = super().inv_quad_logdet(inv_quad_rhs, logdet, reduce_inv_quad)
         return tuple(r.to(self.device) for r in res)
 
     @property
-    def device(self):
+    def device(self) -> Optional[torch.device]:
         return self.output_device
 
     @property
-    def devices(self):
+    def devices(self) -> List[torch.device]:
         return [t.device for t in self.linear_ops]
 
     @property
-    def device_count(self):
+    def device_count(self) -> int:
         return len(set(self.devices))
 
-    def to(self, *args, **kwargs):
+    def to(self: Float[LinearOperator, "*batch M N"], *args, **kwargs) -> Float[LinearOperator, "*batch M N"]:
         """
         Returns a new CatLinearOperator with device as the output_device and dtype
         as the dtype.
         Warning: this does not move the LinearOperators in this CatLinearOperator to
         device.
         """
         device, dtype = _to_helper(*args, **kwargs)
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/interpolated_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/interpolated_linear_operator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
-from typing import Tuple, Union
+from typing import List, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
+from torch import Tensor
 
 from ..utils import sparse
 from ..utils.broadcasting import _pad_with_singletons
 from ..utils.getitem import _noop_index
 from ..utils.interpolation import left_interp, left_t_interp
-from ._linear_operator import LinearOperator
+from ._linear_operator import IndexType, LinearOperator
 from .dense_linear_operator import DenseLinearOperator, to_linear_operator
 from .diag_linear_operator import DiagLinearOperator
 from .root_linear_operator import RootLinearOperator
 
 
 class InterpolatedLinearOperator(LinearOperator):
     def _check_args(
-        self,
-        base_linear_op,
-        left_interp_indices,
-        left_interp_values,
-        right_interp_indices,
-        right_interp_values,
+        self, base_linear_op, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
     ):
         if left_interp_indices.size() != left_interp_values.size():
             return "Expected left_interp_indices ({}) to have the same size as left_interp_values ({})".format(
                 left_interp_indices.size(), left_interp_values.size()
             )
         if right_interp_indices.size() != right_interp_values.size():
             return "Expected right_interp_indices ({}) to have the same size as right_interp_values ({})".format(
@@ -58,98 +55,80 @@
             num_rows = base_linear_op.size(-2)
             left_interp_indices = torch.arange(0, num_rows, dtype=torch.long, device=base_linear_op.device)
             left_interp_indices.unsqueeze_(-1)
             left_interp_indices = left_interp_indices.expand(*base_linear_op.batch_shape, num_rows, 1)
 
         if left_interp_values is None:
             left_interp_values = torch.ones(
-                left_interp_indices.size(),
-                dtype=base_linear_op.dtype,
-                device=base_linear_op.device,
+                left_interp_indices.size(), dtype=base_linear_op.dtype, device=base_linear_op.device
             )
 
         if right_interp_indices is None:
             num_cols = base_linear_op.size(-1)
             right_interp_indices = torch.arange(0, num_cols, dtype=torch.long, device=base_linear_op.device)
             right_interp_indices.unsqueeze_(-1)
             right_interp_indices = right_interp_indices.expand(*base_linear_op.batch_shape, num_cols, 1)
 
         if right_interp_values is None:
             right_interp_values = torch.ones(
-                right_interp_indices.size(),
-                dtype=base_linear_op.dtype,
-                device=base_linear_op.device,
+                right_interp_indices.size(), dtype=base_linear_op.dtype, device=base_linear_op.device
             )
 
         if left_interp_indices.shape[:-2] != base_linear_op.batch_shape:
             try:
                 base_linear_op = base_linear_op._expand_batch(left_interp_indices.shape[:-2])
             except RuntimeError:
                 raise RuntimeError(
                     "interp size ({}) is incompatible with base_linear_op size ({}). ".format(
                         right_interp_indices.size(), base_linear_op.size()
                     )
                 )
 
         super(InterpolatedLinearOperator, self).__init__(
-            base_linear_op,
-            left_interp_indices,
-            left_interp_values,
-            right_interp_indices,
-            right_interp_values,
+            base_linear_op, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
         )
         self.base_linear_op = base_linear_op
         self.left_interp_indices = left_interp_indices
         self.left_interp_values = left_interp_values
         self.right_interp_indices = right_interp_indices
         self.right_interp_values = right_interp_values
 
-    def _approx_diagonal(self):
+    def _approx_diagonal(self: Float[LinearOperator, "*batch N N"]) -> Float[torch.Tensor, "*batch N"]:
         base_diag_root = self.base_linear_op._diagonal().sqrt()
-        left_res = left_interp(
-            self.left_interp_indices,
-            self.left_interp_values,
-            base_diag_root.unsqueeze(-1),
-        )
-        right_res = left_interp(
-            self.right_interp_indices,
-            self.right_interp_values,
-            base_diag_root.unsqueeze(-1),
-        )
+        left_res = left_interp(self.left_interp_indices, self.left_interp_values, base_diag_root.unsqueeze(-1))
+        right_res = left_interp(self.right_interp_indices, self.right_interp_values, base_diag_root.unsqueeze(-1))
         res = left_res * right_res
         return res.squeeze(-1)
 
-    def _diagonal(self):
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
         if isinstance(self.base_linear_op, RootLinearOperator) and isinstance(
             self.base_linear_op.root, DenseLinearOperator
         ):
             left_interp_vals = left_interp(
-                self.left_interp_indices,
-                self.left_interp_values,
-                self.base_linear_op.root.to_dense(),
+                self.left_interp_indices, self.left_interp_values, self.base_linear_op.root.to_dense()
             )
             right_interp_vals = left_interp(
-                self.right_interp_indices,
-                self.right_interp_values,
-                self.base_linear_op.root.to_dense(),
+                self.right_interp_indices, self.right_interp_values, self.base_linear_op.root.to_dense()
             )
             return (left_interp_vals * right_interp_vals).sum(-1)
         else:
             return super(InterpolatedLinearOperator, self)._diagonal()
 
-    def _expand_batch(self, batch_shape):
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         return self.__class__(
             self.base_linear_op._expand_batch(batch_shape),
             self.left_interp_indices.expand(*batch_shape, *self.left_interp_indices.shape[-2:]),
             self.left_interp_values.expand(*batch_shape, *self.left_interp_values.shape[-2:]),
             self.right_interp_indices.expand(*batch_shape, *self.right_interp_indices.shape[-2:]),
             self.right_interp_values.expand(*batch_shape, *self.right_interp_values.shape[-2:]),
         )
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         left_interp_indices = self.left_interp_indices.__getitem__((*batch_indices, row_index)).unsqueeze(-2)
         right_interp_indices = self.right_interp_indices.__getitem__((*batch_indices, col_index)).unsqueeze(-1)
         base_vals = self.base_linear_op._get_indices(
             left_interp_indices,
             right_interp_indices,
             *[batch_index.view(*batch_index.shape, 1, 1) for batch_index in batch_indices],
         )
@@ -157,20 +136,15 @@
         left_interp_values = self.left_interp_values.__getitem__((*batch_indices, row_index)).unsqueeze(-2)
         right_interp_values = self.right_interp_values.__getitem__((*batch_indices, col_index)).unsqueeze(-1)
         interp_values = left_interp_values * right_interp_values
 
         res = (base_vals * interp_values).sum([-2, -1])
         return res
 
-    def _getitem(
-        self,
-        row_index: Union[slice, torch.LongTensor],
-        col_index: Union[slice, torch.LongTensor],
-        *batch_indices: Tuple[Union[int, slice, torch.LongTensor], ...],
-    ) -> LinearOperator:
+    def _getitem(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> LinearOperator:
         # Handle batch dimensions
         # Construt a new LinearOperator
         base_linear_op = self.base_linear_op
         left_interp_indices = self.left_interp_indices
         left_interp_values = self.left_interp_values
         right_interp_indices = self.right_interp_indices
         right_interp_values = self.right_interp_values
@@ -208,15 +182,18 @@
             left_interp_values,
             right_interp_indices,
             right_interp_values,
             **self._kwargs,
         )
         return res
 
-    def _matmul(self, rhs):
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         # Get sparse tensor representations of left/right interp matrices
         left_interp_t = self._sparse_left_interp_t(self.left_interp_indices, self.left_interp_values)
         right_interp_t = self._sparse_right_interp_t(self.right_interp_indices, self.right_interp_values)
 
         if rhs.ndimension() == 1:
             is_vector = True
             rhs = rhs.unsqueeze(-1)
@@ -234,26 +211,31 @@
         res = sparse.bdsmm(left_interp_mat, base_res)
 
         # Squeeze if necessary
         if is_vector:
             res = res.squeeze(-1)
         return res
 
-    def _mul_constant(self, other):
+    def _mul_constant(
+        self: Float[LinearOperator, "*batch M N"], other: Union[float, torch.Tensor]
+    ) -> Float[LinearOperator, "*batch M N"]:
         # We're using a custom method here - the constant mul is applied to the base_lazy tensor
         # This preserves the interpolated structure
         return self.__class__(
             self.base_linear_op._mul_constant(other),
             self.left_interp_indices,
             self.left_interp_values,
             self.right_interp_indices,
             self.right_interp_values,
         )
 
-    def _t_matmul(self, rhs):
+    def _t_matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[Tensor, "*batch2 M P"], Float[LinearOperator, "*batch2 M P"]],
+    ) -> Union[Float[LinearOperator, "... N P"], Float[Tensor, "... N P"]]:
         # Get sparse tensor representations of left/right interp matrices
         left_interp_t = self._sparse_left_interp_t(self.left_interp_indices, self.left_interp_values)
         right_interp_t = self._sparse_right_interp_t(self.right_interp_indices, self.right_interp_values)
 
         if rhs.ndimension() == 1:
             is_vector = True
             rhs = rhs.unsqueeze(-1)
@@ -271,15 +253,15 @@
         res = sparse.bdsmm(right_interp_mat, base_res)
 
         # Squeeze if necessary
         if is_vector:
             res = res.squeeze(-1)
         return res
 
-    def _bilinear_derivative(self, left_vecs, right_vecs):
+    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Optional[Tensor], ...]:
         # Get sparse tensor representations of left/right interp matrices
         left_interp_t = self._sparse_left_interp_t(self.left_interp_indices, self.left_interp_values)
         right_interp_t = self._sparse_right_interp_t(self.right_interp_indices, self.right_interp_values)
 
         if left_vecs.ndimension() == 1:
             left_vecs = left_vecs.unsqueeze(1)
             right_vecs = right_vecs.unsqueeze(1)
@@ -338,20 +320,20 @@
                 left_values_grad,
                 torch.zeros_like(self.right_interp_indices),
                 right_values_grad,
             ]
         )
         return res
 
-    def _size(self):
+    def _size(self) -> torch.Size:
         return torch.Size(
             self.base_linear_op.batch_shape + (self.left_interp_indices.size(-2), self.right_interp_indices.size(-2))
         )
 
-    def _transpose_nonbatch(self):
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         res = self.__class__(
             self.base_linear_op.mT,
             self.right_interp_indices,
             self.right_interp_values,
             self.left_interp_indices,
             self.left_interp_values,
             **self._kwargs,
@@ -362,41 +344,37 @@
         if hasattr(self, "_sparse_left_interp_t_memo"):
             if torch.equal(self._left_interp_indices_memo, left_interp_indices_tensor) and torch.equal(
                 self._left_interp_values_memo, left_interp_values_tensor
             ):
                 return self._sparse_left_interp_t_memo
 
         left_interp_t = sparse.make_sparse_from_indices_and_values(
-            left_interp_indices_tensor,
-            left_interp_values_tensor,
-            self.base_linear_op.size()[-2],
+            left_interp_indices_tensor, left_interp_values_tensor, self.base_linear_op.size()[-2]
         )
         self._left_interp_indices_memo = left_interp_indices_tensor
         self._left_interp_values_memo = left_interp_values_tensor
         self._sparse_left_interp_t_memo = left_interp_t
         return self._sparse_left_interp_t_memo
 
     def _sparse_right_interp_t(self, right_interp_indices_tensor, right_interp_values_tensor):
         if hasattr(self, "_sparse_right_interp_t_memo"):
             if torch.equal(self._right_interp_indices_memo, right_interp_indices_tensor) and torch.equal(
                 self._right_interp_values_memo, right_interp_values_tensor
             ):
                 return self._sparse_right_interp_t_memo
 
         right_interp_t = sparse.make_sparse_from_indices_and_values(
-            right_interp_indices_tensor,
-            right_interp_values_tensor,
-            self.base_linear_op.size()[-1],
+            right_interp_indices_tensor, right_interp_values_tensor, self.base_linear_op.size()[-1]
         )
         self._right_interp_indices_memo = right_interp_indices_tensor
         self._right_interp_values_memo = right_interp_values_tensor
         self._sparse_right_interp_t_memo = right_interp_t
         return self._sparse_right_interp_t_memo
 
-    def _sum_batch(self, dim):
+    def _sum_batch(self, dim: int) -> LinearOperator:
         left_interp_indices = self.left_interp_indices
         left_interp_values = self.left_interp_values
         right_interp_indices = self.right_interp_indices
         right_interp_values = self.right_interp_values
 
         # Increase interpolation indices appropriately
         left_factor = torch.arange(0, left_interp_indices.size(dim), dtype=torch.long, device=self.device)
@@ -406,87 +384,82 @@
         right_factor = torch.arange(0, right_interp_indices.size(dim), dtype=torch.long, device=self.device)
         right_factor = _pad_with_singletons(right_factor, 0, self.dim() - dim - 1)
         right_factor = right_factor * self.base_linear_op.size(-1)
         right_interp_indices = right_interp_indices.add(right_factor)
 
         # Rearrange the indices and values
         permute_order = (*range(0, dim), *range(dim + 1, self.dim()), dim)
-        left_shape = (
-            *left_interp_indices.shape[:dim],
-            *left_interp_indices.shape[dim + 1 : -1],
-            -1,
-        )
-        right_shape = (
-            *right_interp_indices.shape[:dim],
-            *right_interp_indices.shape[dim + 1 : -1],
-            -1,
-        )
+        left_shape = (*left_interp_indices.shape[:dim], *left_interp_indices.shape[dim + 1 : -1], -1)
+        right_shape = (*right_interp_indices.shape[:dim], *right_interp_indices.shape[dim + 1 : -1], -1)
         left_interp_indices = left_interp_indices.permute(permute_order).reshape(left_shape)
         left_interp_values = left_interp_values.permute(permute_order).reshape(left_shape)
         right_interp_indices = right_interp_indices.permute(permute_order).reshape(right_shape)
         right_interp_values = right_interp_values.permute(permute_order).reshape(right_shape)
 
         # Make the base_lazy tensor block diagonal
         from .block_diag_linear_operator import BlockDiagLinearOperator
 
         block_diag = BlockDiagLinearOperator(self.base_linear_op, block_dim=dim)
 
         # Finally! We have an interpolated lazy tensor again
         return InterpolatedLinearOperator(
-            block_diag,
-            left_interp_indices,
-            left_interp_values,
-            right_interp_indices,
-            right_interp_values,
+            block_diag, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
         )
 
-    def double(self, device_id=None):
+    def double(
+        self: Float[LinearOperator, "*batch M N"], device_id: Optional[str] = None
+    ) -> Float[LinearOperator, "*batch M N"]:
         # We need to ensure that the indices remain integers.
         new_lt = super().double(device_id=device_id)
         new_lt.left_interp_indices = new_lt.left_interp_indices.type(torch.int64)
         new_lt.right_interp_indices = new_lt.right_interp_indices.type(torch.int64)
         return new_lt
 
-    def matmul(self, tensor):
+    def matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        other: Union[Float[Tensor, "*batch2 N P"], Float[Tensor, "*batch2 N"], Float[LinearOperator, "*batch2 N P"]],
+    ) -> Union[Float[Tensor, "... M P"], Float[Tensor, "... M"], Float[LinearOperator, "... M P"]]:
         # We're using a custom matmul here, because it is significantly faster than
         # what we get from the function factory.
         # The _matmul_closure is optimized for repeated calls, such as for _solve
 
-        if isinstance(tensor, DiagLinearOperator):
+        if isinstance(other, DiagLinearOperator):
             # if we know the rhs is diagonal this is easy
-            new_right_interp_values = self.right_interp_values * tensor._diag.unsqueeze(-1)
+            new_right_interp_values = self.right_interp_values * other._diag.unsqueeze(-1)
             return InterpolatedLinearOperator(
                 base_linear_op=self.base_linear_op,
                 left_interp_indices=self.left_interp_indices,
                 left_interp_values=self.left_interp_values,
                 right_interp_indices=self.right_interp_indices,
                 right_interp_values=new_right_interp_values,
             )
 
-        if tensor.ndimension() == 1:
+        if other.ndimension() == 1:
             is_vector = True
-            tensor = tensor.unsqueeze(-1)
+            other = other.unsqueeze(-1)
         else:
             is_vector = False
 
         # right_interp^T * tensor
         base_size = self.base_linear_op.size(-1)
-        right_interp_res = left_t_interp(self.right_interp_indices, self.right_interp_values, tensor, base_size)
+        right_interp_res = left_t_interp(self.right_interp_indices, self.right_interp_values, other, base_size)
 
         # base_linear_op * right_interp^T * tensor
         base_res = self.base_linear_op.matmul(right_interp_res)
 
         # left_interp * base_linear_op * right_interp^T * tensor
         res = left_interp(self.left_interp_indices, self.left_interp_values, base_res)
 
         # Squeeze if necessary
         if is_vector:
             res = res.squeeze(-1)
         return res
 
-    def zero_mean_mvn_samples(self, num_samples):
+    def zero_mean_mvn_samples(
+        self: Float[LinearOperator, "*batch N N"], num_samples: int
+    ) -> Float[Tensor, "num_samples *batch N"]:
         base_samples = self.base_linear_op.zero_mean_mvn_samples(num_samples)
         batch_iter = tuple(range(1, base_samples.dim()))
         base_samples = base_samples.permute(*batch_iter, 0)
         res = left_interp(self.left_interp_indices, self.left_interp_values, base_samples).contiguous()
         batch_iter = tuple(range(res.dim() - 1))
         return res.permute(-1, *batch_iter).contiguous()
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 
-from typing import Optional, Tuple
+from typing import Callable, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
 from torch import Tensor
 
 from .. import settings
 from ._linear_operator import LinearOperator
 from .added_diag_linear_operator import AddedDiagLinearOperator
 from .diag_linear_operator import ConstantDiagLinearOperator, DiagLinearOperator
 from .kronecker_product_linear_operator import KroneckerProductDiagLinearOperator, KroneckerProductLinearOperator
@@ -55,25 +56,33 @@
             self.linear_op = linear_ops[0]
         else:
             raise RuntimeError(
                 "One of the LinearOperators input to AddedDiagLinearOperator must be a DiagLinearOperator!"
             )
         self._diag_is_constant = isinstance(self.diag_tensor, ConstantDiagLinearOperator)
 
-    def inv_quad_logdet(self, inv_quad_rhs=None, logdet=False, reduce_inv_quad=True):
+    def inv_quad_logdet(
+        self: Float[LinearOperator, "*batch N N"],
+        inv_quad_rhs: Optional[Union[Float[Tensor, "*batch N M"], Float[Tensor, "*batch N"]]] = None,
+        logdet: Optional[bool] = False,
+        reduce_inv_quad: Optional[bool] = True,
+    ) -> Tuple[
+        Optional[Union[Float[Tensor, "*batch M"], Float[Tensor, " *batch"], Float[Tensor, " 0"]]],
+        Optional[Float[Tensor, "..."]],
+    ]:
         if inv_quad_rhs is not None:
             inv_quad_term, _ = super().inv_quad_logdet(
                 inv_quad_rhs=inv_quad_rhs, logdet=False, reduce_inv_quad=reduce_inv_quad
             )
         else:
             inv_quad_term = None
         logdet_term = self._logdet() if logdet else None
         return inv_quad_term, logdet_term
 
-    def _logdet(self):
+    def _logdet(self: Float[LinearOperator, "*batch N N"]) -> Float[Tensor, " *batch"]:
         if self._diag_is_constant:
             # symeig requires computing the eigenvectors for it to be differentiable
             evals, _ = self.linear_op._symeig(eigenvectors=True)
             evals_plus_diag = evals + self.diag_tensor._diagonal()
             return torch.log(evals_plus_diag).sum(dim=-1)
         if self.shape[-1] >= settings.max_cholesky_size.value() and isinstance(
             self.diag_tensor, KroneckerProductDiagLinearOperator
@@ -109,19 +118,30 @@
                     _, evals_plus_i, _ = _symmetrize_kpadlt_constructor(lt, dlt)
 
                 diag_term = self.diag_tensor.logdet()
                 return diag_term + evals_plus_i.logdet()
 
         return super().inv_quad_logdet(logdet=True)[1]
 
-    def _preconditioner(self):
+    def _preconditioner(self) -> Tuple[Optional[Callable], Optional[LinearOperator], Optional[torch.Tensor]]:
         # solves don't use CG so don't waste time computing it
         return None, None, None
 
-    def _solve(self, rhs, preconditioner=None, num_tridiag=0):
+    def _solve(
+        self: Float[LinearOperator, "... N N"],
+        rhs: Float[torch.Tensor, "... N C"],
+        preconditioner: Optional[Callable[[Float[torch.Tensor, "... N C"]], Float[torch.Tensor, "... N C"]]] = None,
+        num_tridiag: Optional[int] = 0,
+    ) -> Union[
+        Float[torch.Tensor, "... N C"],
+        Tuple[
+            Float[torch.Tensor, "... N C"],
+            Float[torch.Tensor, "..."],  # Note that in case of a tuple the second term size depends on num_tridiag
+        ],
+    ]:
 
         rhs_dtype = rhs.dtype
 
         # we perform the solve in double for numerical stability issues
         symeig_dtype = settings._linalg_dtype_symeig.value()
 
         # if the diagonal is constant, we can solve this using the Kronecker-structured eigendecomposition
@@ -194,15 +214,17 @@
             res3 = evecs.matmul(res2)
             res = dlt_inv_root.matmul(res3)
             return res.to(rhs_dtype)
 
         # in all other cases we fall back to the default
         return super()._solve(rhs, preconditioner=preconditioner, num_tridiag=num_tridiag)
 
-    def _root_decomposition(self):
+    def _root_decomposition(
+        self: Float[LinearOperator, "... N N"]
+    ) -> Union[Float[torch.Tensor, "... N N"], Float[LinearOperator, "... N N"]]:
         if self._diag_is_constant:
             evals, q_matrix = self.linear_op.diagonalization()
             updated_evals = DiagLinearOperator((evals + self.diag_tensor._diagonal()).pow(0.5))
             return MatmulLinearOperator(q_matrix, updated_evals)
 
         dlt = self.diag_tensor
         lt = self.linear_op
@@ -225,15 +247,19 @@
             dlt_root = dlt.sqrt()
             _, evals_p_i, evecs = _symmetrize_kpadlt_constructor(lt, dlt)
             evals_p_i_root = DiagLinearOperator(evals_p_i._diagonal().sqrt())
             return MatmulLinearOperator(dlt_root, MatmulLinearOperator(evecs, evals_p_i_root))
 
         return super()._root_decomposition()
 
-    def _root_inv_decomposition(self, initial_vectors=None):
+    def _root_inv_decomposition(
+        self: Float[LinearOperator, "*batch N N"],
+        initial_vectors: Optional[torch.Tensor] = None,
+        test_vectors: Optional[torch.Tensor] = None,
+    ) -> Union[Float[LinearOperator, "... N N"], Float[Tensor, "... N N"]]:
         if self._diag_is_constant:
             evals, q_matrix = self.linear_op.diagonalization()
             inv_sqrt_evals = DiagLinearOperator((evals + self.diag_tensor._diagonal()).pow(-0.5))
             return MatmulLinearOperator(q_matrix, inv_sqrt_evals)
 
         dlt = self.diag_tensor
         lt = self.linear_op
@@ -256,23 +282,30 @@
             dlt_sqrt, evals_p_i, evecs = _symmetrize_kpadlt_constructor(lt, dlt)
             dlt_inv_root = dlt_sqrt.inverse()
             evals_p_i_root = DiagLinearOperator(evals_p_i._diagonal().reciprocal().sqrt())
             return MatmulLinearOperator(dlt_inv_root, MatmulLinearOperator(evecs, evals_p_i_root))
 
         return super()._root_inv_decomposition(initial_vectors=initial_vectors)
 
-    def _symeig(self, eigenvectors: bool = False) -> Tuple[Tensor, Optional[LinearOperator]]:
+    def _symeig(
+        self: Float[LinearOperator, "*batch N N"],
+        eigenvectors: bool = False,
+        return_evals_as_lazy: Optional[bool] = False,
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         # return_evals_as_lazy is a flag to return the eigenvalues as a lazy tensor
         # which is useful for root decompositions here (see the root_decomposition
         # method above)
         if self._diag_is_constant:
             evals, evecs = self.linear_op._symeig(eigenvectors=eigenvectors)
             evals = evals + self.diag_tensor.diag_values
 
             return evals, evecs
         return super()._symeig(eigenvectors=eigenvectors)
 
-    def __add__(self, other):
+    def __add__(
+        self: Float[LinearOperator, "... #M #N"],
+        other: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"], float],
+    ) -> Union[Float[LinearOperator, "... M N"], Float[Tensor, "... M N"]]:
         if isinstance(other, ConstantDiagLinearOperator) and self._diag_is_constant:
             # the other cases have only partial implementations
             return KroneckerProductAddedDiagLinearOperator(self.linear_op, self.diag_tensor + other)
         return super().__add__(other)
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/kronecker_product_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/kronecker_product_linear_operator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python3
 
 import operator
 from functools import reduce
-from typing import Optional, Tuple
+from typing import Callable, List, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
 from torch import Tensor
 
 from .. import settings
 from ..utils.broadcasting import _matmul_broadcast_shape
 from ..utils.memoize import cached
-from ._linear_operator import LinearOperator
+from ._linear_operator import IndexType, LinearOperator
 from .dense_linear_operator import to_linear_operator
 from .diag_linear_operator import ConstantDiagLinearOperator, DiagLinearOperator
 from .triangular_linear_operator import _TriangularLinearOperatorBase, TriangularLinearOperator
 
 
 def _kron_diag(*lts) -> Tensor:
     """Compute diagonal of a KroneckerProductLinearOperator from the diagonals of the constituiting tensors"""
@@ -57,52 +58,67 @@
         factor = factor.view(*output_batch_shape, linear_op.size(-1), -1, num_cols).transpose(-3, -2)
         res = factor.reshape(*output_batch_shape, -1, num_cols)
     return res
 
 
 class KroneckerProductLinearOperator(LinearOperator):
     r"""
-    Returns the Kronecker product of the given lazy tensors
+    Given linearOperators :math:`\boldsymbol K_1, \ldots, \boldsymbol K_P`,
+    this LinearOperator represents the Kronecker product :math:`\boldsymbol K_1 \otimes \ldots \otimes \boldsymbol K_P`.
 
-    Args:
-        :`linear_ops`: List of lazy tensors
+    :param linear_ops: :math:`\boldsymbol K_1, \ldots, \boldsymbol K_P`: the LinearOperators in the Kronecker product.
     """
 
-    def __init__(self, *linear_ops):
+    def __init__(self, *linear_ops: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"]]):
         try:
             linear_ops = tuple(to_linear_operator(linear_op) for linear_op in linear_ops)
         except TypeError:
             raise RuntimeError("KroneckerProductLinearOperator is intended to wrap lazy tensors.")
-        for prev_linear_op, curr_linear_op in zip(linear_ops[:-1], linear_ops[1:]):
-            if prev_linear_op.batch_shape != curr_linear_op.batch_shape:
-                raise RuntimeError(
-                    "KroneckerProductLinearOperator expects lazy tensors with the "
-                    "same batch shapes. Got {}.".format([lv.batch_shape for lv in linear_ops])
-                )
+
+        # Make batch shapes the same for all operators
+        try:
+            batch_broadcast_shape = torch.broadcast_shapes(*(linear_op.batch_shape for linear_op in linear_ops))
+        except RuntimeError:
+            raise RuntimeError(
+                "Batch shapes of LinearOperators "
+                f"({', '.join([str(tuple(linear_op.shape)) for linear_op in linear_ops])}) "
+                "are incompatible for a Kronecker product."
+            )
+
+        if len(batch_broadcast_shape):  # Otherwise all linear_ops are non-batch, and we don't need to expand
+            # NOTE: we must explicitly call requires_grad on each of these arguments
+            # for the automatic _bilinear_derivative to work in torch.autograd.Functions
+            linear_ops = [
+                linear_op._expand_batch(batch_broadcast_shape).requires_grad_(linear_op.requires_grad)
+                for linear_op in linear_ops
+            ]
+
         super().__init__(*linear_ops)
         self.linear_ops = linear_ops
 
-    def __add__(self, other):
+    def __add__(
+        self: Float[LinearOperator, "... #M #N"],
+        other: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"], float],
+    ) -> Union[Float[LinearOperator, "... M N"], Float[Tensor, "... M N"]]:
         if isinstance(other, (KroneckerProductDiagLinearOperator, ConstantDiagLinearOperator)):
             from .kronecker_product_added_diag_linear_operator import KroneckerProductAddedDiagLinearOperator
 
             return KroneckerProductAddedDiagLinearOperator(self, other)
         if isinstance(other, KroneckerProductLinearOperator):
             from .sum_kronecker_linear_operator import SumKroneckerLinearOperator
 
             return SumKroneckerLinearOperator(self, other)
         if isinstance(other, DiagLinearOperator):
             return self.add_diagonal(other._diagonal())
         return super().__add__(other)
 
-    def add_diagonal(self, diag):
-        r"""
-        Adds a diagonal to a KroneckerProductLinearOperator
-        """
-
+    def add_diagonal(
+        self: Float[LinearOperator, "*batch N N"],
+        diag: Union[Float[torch.Tensor, "... N"], Float[torch.Tensor, "... 1"], Float[torch.Tensor, ""]],
+    ) -> Float[LinearOperator, "*batch N N"]:
         from .kronecker_product_added_diag_linear_operator import KroneckerProductAddedDiagLinearOperator
 
         if not self.is_square:
             raise RuntimeError("add_diag only defined for square matrices")
 
         diag_shape = diag.shape
         if len(diag_shape) == 0:
@@ -120,48 +136,62 @@
                         self.shape, diag_shape
                     )
                 )
             diag_tensor = DiagLinearOperator(expanded_diag)
 
         return KroneckerProductAddedDiagLinearOperator(self, diag_tensor)
 
-    def diagonalization(self, method: Optional[str] = None):
+    def diagonalization(
+        self: Float[LinearOperator, "*batch N N"], method: Optional[str] = None
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         if method is None:
             method = "symeig"
         return super().diagonalization(method=method)
 
     @cached
-    def inverse(self):
+    def inverse(self: Float[LinearOperator, "*batch N N"]) -> Float[LinearOperator, "*batch N N"]:
         # here we use that (A \kron B)^-1 = A^-1 \kron B^-1
         # TODO: Investigate under what conditions computing individual individual inverses makes sense
         inverses = [lt.inverse() for lt in self.linear_ops]
         return self.__class__(*inverses)
 
-    def inv_quad_logdet(self, inv_quad_rhs=None, logdet=False, reduce_inv_quad=True):
+    def inv_quad_logdet(
+        self: Float[LinearOperator, "*batch N N"],
+        inv_quad_rhs: Optional[Union[Float[Tensor, "*batch N M"], Float[Tensor, "*batch N"]]] = None,
+        logdet: Optional[bool] = False,
+        reduce_inv_quad: Optional[bool] = True,
+    ) -> Tuple[
+        Optional[Union[Float[Tensor, "*batch M"], Float[Tensor, " *batch"], Float[Tensor, " 0"]]],
+        Optional[Float[Tensor, "..."]],
+    ]:
         if inv_quad_rhs is not None:
             inv_quad_term, _ = super().inv_quad_logdet(
                 inv_quad_rhs=inv_quad_rhs, logdet=False, reduce_inv_quad=reduce_inv_quad
             )
         else:
             inv_quad_term = None
         logdet_term = self._logdet() if logdet else None
         return inv_quad_term, logdet_term
 
     @cached(name="cholesky")
-    def _cholesky(self, upper=False):
+    def _cholesky(
+        self: Float[LinearOperator, "*batch N N"], upper: Optional[bool] = False
+    ) -> Float[LinearOperator, "*batch N N"]:
         chol_factors = [lt.cholesky(upper=upper) for lt in self.linear_ops]
         return KroneckerProductTriangularLinearOperator(*chol_factors, upper=upper)
 
-    def _diagonal(self):
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
         return _kron_diag(*self.linear_ops)
 
-    def _expand_batch(self, batch_shape):
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         return self.__class__(*[linear_op._expand_batch(batch_shape) for linear_op in self.linear_ops])
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         row_factor = self.size(-2)
         col_factor = self.size(-1)
 
         res = None
         for linear_op in self.linear_ops:
             sub_row_size = linear_op.size(-2)
             sub_col_size = linear_op.size(-1)
@@ -173,15 +203,26 @@
                 torch.div(col_index, col_factor, rounding_mode="floor").fmod(sub_col_size),
                 *batch_indices,
             )
             res = sub_res if res is None else (sub_res * res)
 
         return res
 
-    def _solve(self, rhs, preconditioner=None, num_tridiag=0):
+    def _solve(
+        self: Float[LinearOperator, "... N N"],
+        rhs: Float[torch.Tensor, "... N C"],
+        preconditioner: Optional[Callable[[Float[torch.Tensor, "... N C"]], Float[torch.Tensor, "... N C"]]] = None,
+        num_tridiag: Optional[int] = 0,
+    ) -> Union[
+        Float[torch.Tensor, "... N C"],
+        Tuple[
+            Float[torch.Tensor, "... N C"],
+            Float[torch.Tensor, "..."],  # Note that in case of a tuple the second term size depends on num_tridiag
+        ],
+    ]:
         # Computes solve by exploiting the identity (A \kron B)^-1 = A^-1 \kron B^-1
         # we perform the solve first before worrying about any tridiagonal matrices
 
         tsr_shapes = [q.size(-1) for q in self.linear_ops]
         n_rows = rhs.size(-2)
         batch_shape = torch.broadcast_shapes(self.shape[:-2], rhs.shape[:-2])
         perm_batch = tuple(range(len(batch_shape)))
@@ -209,76 +250,90 @@
         # if _inv_matmul is called, we ignore the eigenvalue handling
         # this is efficient because of the structure of the lazy tensor
         res = self._solve(rhs=right_tensor)
         if left_tensor is not None:
             res = left_tensor @ res
         return res
 
-    def _logdet(self):
+    def _logdet(self: Float[LinearOperator, "*batch M N"]) -> Float[Tensor, " *batch"]:
         evals, _ = self.diagonalization()
         logdet = evals.clamp(min=1e-7).log().sum(-1)
         return logdet
 
-    def _matmul(self, rhs):
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         is_vec = rhs.ndimension() == 1
         if is_vec:
             rhs = rhs.unsqueeze(-1)
 
         res = _matmul(self.linear_ops, self.shape, rhs.contiguous())
 
         if is_vec:
             res = res.squeeze(-1)
         return res
 
     @cached(name="root_decomposition")
-    def root_decomposition(self, method: Optional[str] = None):
+    def root_decomposition(
+        self: Float[LinearOperator, "*batch N N"], method: Optional[str] = None
+    ) -> Float[LinearOperator, "*batch N N"]:
         from linear_operator.operators import RootLinearOperator
 
         # return a dense root decomposition if the matrix is small
         if self.shape[-1] <= settings.max_cholesky_size.value():
             return super().root_decomposition(method=method)
 
         root_list = [lt.root_decomposition(method=method).root for lt in self.linear_ops]
         kronecker_root = KroneckerProductLinearOperator(*root_list)
         return RootLinearOperator(kronecker_root)
 
     @cached(name="root_inv_decomposition")
-    def root_inv_decomposition(self, method=None, initial_vectors=None, test_vectors=None):
+    def root_inv_decomposition(
+        self: Float[LinearOperator, "*batch N N"],
+        initial_vectors: Optional[torch.Tensor] = None,
+        test_vectors: Optional[torch.Tensor] = None,
+        method: Optional[str] = None,
+    ) -> Union[Float[LinearOperator, "... N N"], Float[Tensor, "... N N"]]:
         from linear_operator.operators import RootLinearOperator
 
         # return a dense root decomposition if the matrix is small
         if self.shape[-1] <= settings.max_cholesky_size.value():
             return super().root_inv_decomposition()
 
         root_list = [lt.root_inv_decomposition().root for lt in self.linear_ops]
         kronecker_root = KroneckerProductLinearOperator(*root_list)
         return RootLinearOperator(kronecker_root)
 
     @cached(name="size")
-    def _size(self):
+    def _size(self) -> torch.Size:
         left_size = _prod(linear_op.size(-2) for linear_op in self.linear_ops)
         right_size = _prod(linear_op.size(-1) for linear_op in self.linear_ops)
         return torch.Size((*self.linear_ops[0].batch_shape, left_size, right_size))
 
     @cached(name="svd")
-    def _svd(self) -> Tuple[LinearOperator, Tensor, LinearOperator]:
+    def _svd(
+        self: Float[LinearOperator, "*batch N N"]
+    ) -> Tuple[Float[LinearOperator, "*batch N N"], Float[Tensor, "... N"], Float[LinearOperator, "*batch N N"]]:
         U, S, V = [], [], []
         for lt in self.linear_ops:
             U_, S_, V_ = lt.svd()
             U.append(U_)
             S.append(S_)
             V.append(V_)
         S = KroneckerProductLinearOperator(*[DiagLinearOperator(S_) for S_ in S])._diagonal()
         U = KroneckerProductLinearOperator(*U)
         V = KroneckerProductLinearOperator(*V)
         return U, S, V
 
     def _symeig(
-        self, eigenvectors: bool = False, return_evals_as_lazy: bool = False
-    ) -> Tuple[Tensor, Optional[LinearOperator]]:
+        self: Float[LinearOperator, "*batch N N"],
+        eigenvectors: bool = False,
+        return_evals_as_lazy: Optional[bool] = False,
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         # return_evals_as_lazy is a flag to return the eigenvalues as a lazy tensor
         # which is useful for root decompositions here (see the root_decomposition
         # method above)
         evals, evecs = [], []
         for lt in self.linear_ops:
             evals_, evecs_ = lt._symeig(eigenvectors=eigenvectors)
             evals.append(evals_)
@@ -290,66 +345,80 @@
 
         if eigenvectors:
             evecs = KroneckerProductLinearOperator(*evecs)
         else:
             evecs = None
         return evals, evecs
 
-    def _t_matmul(self, rhs):
+    def _t_matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[Tensor, "*batch2 M P"], Float[LinearOperator, "*batch2 M P"]],
+    ) -> Union[Float[LinearOperator, "... N P"], Float[Tensor, "... N P"]]:
         is_vec = rhs.ndimension() == 1
         if is_vec:
             rhs = rhs.unsqueeze(-1)
 
         res = _t_matmul(self.linear_ops, self.shape, rhs.contiguous())
 
         if is_vec:
             res = res.squeeze(-1)
         return res
 
-    def _transpose_nonbatch(self):
-        return self.__class__(
-            *(linear_op._transpose_nonbatch() for linear_op in self.linear_ops),
-            **self._kwargs,
-        )
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
+        return self.__class__(*(linear_op._transpose_nonbatch() for linear_op in self.linear_ops), **self._kwargs)
 
 
 class KroneckerProductTriangularLinearOperator(KroneckerProductLinearOperator, _TriangularLinearOperatorBase):
     def __init__(self, *linear_ops, upper=False):
         if not all(isinstance(lt, TriangularLinearOperator) for lt in linear_ops):
             raise RuntimeError(
                 "Components of KroneckerProductTriangularLinearOperator must be TriangularLinearOperator."
             )
         super().__init__(*linear_ops)
         self.upper = upper
 
     @cached
-    def inverse(self):
+    def inverse(self: Float[LinearOperator, "*batch N N"]) -> Float[LinearOperator, "*batch N N"]:
         # here we use that (A \kron B)^-1 = A^-1 \kron B^-1
         inverses = [lt.inverse() for lt in self.linear_ops]
         return self.__class__(*inverses, upper=self.upper)
 
     @cached(name="cholesky")
-    def _cholesky(self, upper=False):
+    def _cholesky(
+        self: Float[LinearOperator, "*batch N N"], upper: Optional[bool] = False
+    ) -> Float[LinearOperator, "*batch N N"]:
         raise NotImplementedError("_cholesky not applicable to triangular lazy tensors")
 
-    def _cholesky_solve(self, rhs, upper=False):
+    def _cholesky_solve(
+        self: Float[LinearOperator, "*batch N N"],
+        rhs: Union[Float[LinearOperator, "*batch2 N M"], Float[Tensor, "*batch2 N M"]],
+        upper: Optional[bool] = False,
+    ) -> Union[Float[LinearOperator, "... N M"], Float[Tensor, "... N M"]]:
         if upper:
             # res = (U.T @ U)^-1 @ v = U^-1 @ U^-T @ v
             w = self._transpose_nonbatch().solve(rhs)
             res = self.solve(w)
         else:
             # res = (L @ L.T)^-1 @ v = L^-T @ L^-1 @ v
             w = self.solve(rhs)
             res = self._transpose_nonbatch().solve(w)
         return res
 
-    def _symeig(self, eigenvectors: bool = False) -> Tuple[Tensor, Optional[LinearOperator]]:
+    def _symeig(
+        self: Float[LinearOperator, "*batch N N"],
+        eigenvectors: bool = False,
+        return_evals_as_lazy: Optional[bool] = False,
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         raise NotImplementedError("_symeig not applicable to triangular lazy tensors")
 
-    def solve(self, right_tensor, left_tensor=None):
+    def solve(
+        self: Float[LinearOperator, "... N N"],
+        right_tensor: Union[Float[Tensor, "... N P"], Float[Tensor, " N"]],
+        left_tensor: Optional[Float[Tensor, "... O N"]] = None,
+    ) -> Union[Float[Tensor, "... N P"], Float[Tensor, "... N"], Float[Tensor, "... O P"], Float[Tensor, "... O"]]:
         # For triangular components, using triangular-triangular substition should generally be good
         return self._inv_matmul(right_tensor=right_tensor, left_tensor=left_tensor)
 
 
 class KroneckerProductDiagLinearOperator(DiagLinearOperator, KroneckerProductTriangularLinearOperator):
     r"""
     Represents the kronecker product of multiple DiagonalLinearOperators
@@ -361,35 +430,52 @@
 
     def __init__(self, *linear_ops: Tuple[DiagLinearOperator, ...]):
         if not all(isinstance(lt, DiagLinearOperator) for lt in linear_ops):
             raise RuntimeError("Components of KroneckerProductDiagLinearOperator must be DiagLinearOperator.")
         super(KroneckerProductTriangularLinearOperator, self).__init__(*linear_ops)
         self.upper = False
 
-    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Tensor, ...]:
+    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Optional[Tensor], ...]:
         return KroneckerProductTriangularLinearOperator._bilinear_derivative(self, left_vecs, right_vecs)
 
     @cached(name="cholesky")
-    def _cholesky(self, upper: bool = False) -> "KroneckerProductDiagLinearOperator":
+    def _cholesky(
+        self: Float[LinearOperator, "*batch N N"], upper: Optional[bool] = False
+    ) -> Float[LinearOperator, "*batch N N"]:
         chol_factors = [lt.cholesky(upper=upper) for lt in self.linear_ops]
         return KroneckerProductDiagLinearOperator(*chol_factors)
 
     @property
-    def _diag(self) -> Tensor:
+    def _diag(self: Float[LinearOperator, "*batch N N"]) -> Float[Tensor, "*batch N"]:
         return _kron_diag(*self.linear_ops)
 
-    def _expand_batch(self, batch_shape: torch.Size) -> "KroneckerProductTriangularLinearOperator":
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         return KroneckerProductTriangularLinearOperator._expand_batch(self, batch_shape)
 
-    def _mul_constant(self, constant: Tensor) -> "KroneckerProductTriangularLinearOperator":
-        return DiagLinearOperator(self._diag * constant.unsqueeze(-1))
+    def _mul_constant(
+        self: Float[LinearOperator, "*batch M N"], other: Union[float, torch.Tensor]
+    ) -> Float[LinearOperator, "*batch M N"]:
+        return DiagLinearOperator(self._diag * other.unsqueeze(-1))
+
+    def _size(self) -> torch.Size:
+        # Though the super._size method works, this is more efficient
+        diag_shapes = [linear_op._diag.shape for linear_op in self.linear_ops]
+        batch_shape = torch.broadcast_shapes(*[diag_shape[:-1] for diag_shape in diag_shapes])
+        N = 1
+        for diag_shape in diag_shapes:
+            N *= diag_shape[-1]
+        return torch.Size([*batch_shape, N, N])
 
     def _symeig(
-        self, eigenvectors: bool = False, return_evals_as_lazy: bool = False
-    ) -> Tuple[Tensor, Optional[LinearOperator]]:
+        self: Float[LinearOperator, "*batch N N"],
+        eigenvectors: bool = False,
+        return_evals_as_lazy: Optional[bool] = False,
+    ) -> Tuple[Float[Tensor, "*batch M"], Optional[Float[LinearOperator, "*batch N M"]]]:
         # return_evals_as_lazy is a flag to return the eigenvalues as a lazy tensor
         # which is useful for root decompositions here (see the root_decomposition
         # method above)
         evals, evecs = [], []
         for lt in self.linear_ops:
             evals_, evecs_ = lt._symeig(eigenvectors=eigenvectors)
             evals.append(evals_)
@@ -401,33 +487,33 @@
 
         if eigenvectors:
             evecs = KroneckerProductDiagLinearOperator(*evecs)
         else:
             evecs = None
         return evals, evecs
 
-    def abs(self) -> "KroneckerProductDiagLinearOperator":
+    def abs(self) -> LinearOperator:
         """
         Returns a DiagLinearOperator with the absolute value of all diagonal entries.
         """
         return self.__class__(*[lt.abs() for lt in self.linear_ops])
 
-    def exp(self) -> "KroneckerProductDiagLinearOperator":
+    def exp(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         raise NotImplementedError(f"torch.exp({self.__class__.__name__}) is not implemented.")
 
     @cached
-    def inverse(self) -> "KroneckerProductDiagLinearOperator":
+    def inverse(self: Float[LinearOperator, "*batch N N"]) -> Float[LinearOperator, "*batch N N"]:
         """
         Returns the inverse of the DiagLinearOperator.
         """
         # here we use that (A \kron B)^-1 = A^-1 \kron B^-1
         inverses = [lt.inverse() for lt in self.linear_ops]
         return self.__class__(*inverses)
 
-    def log(self) -> "KroneckerProductDiagLinearOperator":
+    def log(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         raise NotImplementedError(f"torch.log({self.__class__.__name__}) is not implemented.")
 
-    def sqrt(self) -> "KroneckerProductDiagLinearOperator":
+    def sqrt(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch M N"]:
         """
         Returns a DiagLinearOperator with the square root of all diagonal entries.
         """
         return self.__class__(*[lt.sqrt() for lt in self.linear_ops])
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/usr/bin/env python3
+from typing import Callable, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
+from torch import Tensor
 
 from ..utils.cholesky import psd_safe_cholesky
 from ..utils.memoize import cached
 from . import to_dense
+from ._linear_operator import LinearOperator
 from .added_diag_linear_operator import AddedDiagLinearOperator
 from .diag_linear_operator import ConstantDiagLinearOperator, DiagLinearOperator
 from .low_rank_root_linear_operator import LowRankRootLinearOperator
 from .sum_batch_linear_operator import SumBatchLinearOperator
 
 
 class LowRankRootAddedDiagLinearOperator(AddedDiagLinearOperator):
@@ -36,65 +40,86 @@
         C = ConstantDiagLinearOperator(torch.ones(*V.batch_shape, 1, device=V.device, dtype=V.dtype), V.shape[-2])
 
         cap_mat = to_dense(C + V.matmul(A_inv.matmul(U)))
         chol_cap_mat = psd_safe_cholesky(cap_mat)
 
         return chol_cap_mat
 
-    def _mul_constant(self, constant):
+    def _mul_constant(
+        self: Float[LinearOperator, "*batch M N"], other: Union[float, torch.Tensor]
+    ) -> Float[LinearOperator, "*batch M N"]:
         # We have to over-ride this here for the case where the constant is negative
-        if constant > 0:
-            res = super()._mul_constant(constant)
+        if other > 0:
+            res = super()._mul_constant(other)
         else:
-            res = AddedDiagLinearOperator(
-                self._linear_op._mul_constant(constant),
-                self._diag_tensor._mul_constant(constant),
-            )
+            res = AddedDiagLinearOperator(self._linear_op._mul_constant(other), self._diag_tensor._mul_constant(other))
         return res
 
-    def _preconditioner(self):
+    def _preconditioner(self) -> Tuple[Optional[Callable], Optional[LinearOperator], Optional[torch.Tensor]]:
         return None, None, None
 
-    def _solve(self, rhs, preconditioner=None, num_tridiag=0):
+    def _solve(
+        self: Float[LinearOperator, "... N N"],
+        rhs: Float[torch.Tensor, "... N C"],
+        preconditioner: Optional[Callable[[Float[torch.Tensor, "... N C"]], Float[torch.Tensor, "... N C"]]] = None,
+        num_tridiag: Optional[int] = 0,
+    ) -> Union[
+        Float[torch.Tensor, "... N C"],
+        Tuple[
+            Float[torch.Tensor, "... N C"],
+            Float[torch.Tensor, "..."],  # Note that in case of a tuple the second term size depends on num_tridiag
+        ],
+    ]:
         A_inv = self._diag_tensor.inverse()  # This is fine since it's a DiagLinearOperator
         U = self._linear_op.root
         V = self._linear_op.root.mT
         chol_cap_mat = self.chol_cap_mat
 
         res = V.matmul(A_inv.matmul(rhs))
         res = torch.cholesky_solve(res, chol_cap_mat)
         res = A_inv.matmul(U.matmul(res))
 
         solve = A_inv.matmul(rhs) - res
 
         return solve
 
-    def _solve_preconditioner(self):
+    def _solve_preconditioner(self) -> Optional[Callable]:
         return None
 
-    def _sum_batch(self, dim):
+    def _sum_batch(self, dim: int) -> LinearOperator:
         return SumBatchLinearOperator(self, dim)
 
     def _logdet(self):
         chol_cap_mat = self.chol_cap_mat
         logdet_cap_mat = 2 * torch.diagonal(chol_cap_mat, offset=0, dim1=-2, dim2=-1).log().sum(-1)
         logdet_A = self._diag_tensor.logdet()
         logdet_term = logdet_cap_mat + logdet_A
 
         return logdet_term
 
-    def __add__(self, other):
+    def __add__(
+        self: Float[LinearOperator, "... #M #N"],
+        other: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"], float],
+    ) -> Union[Float[LinearOperator, "... M N"], Float[Tensor, "... M N"]]:
         from .diag_linear_operator import DiagLinearOperator
 
         if isinstance(other, DiagLinearOperator):
             return self.__class__(self._linear_op, self._diag_tensor + other)
         else:
             return AddedDiagLinearOperator(self._linear_op + other, self._diag_tensor)
 
-    def inv_quad_logdet(self, inv_quad_rhs=None, logdet=False, reduce_inv_quad=True):
+    def inv_quad_logdet(
+        self: Float[LinearOperator, "*batch N N"],
+        inv_quad_rhs: Optional[Union[Float[Tensor, "*batch N M"], Float[Tensor, "*batch N"]]] = None,
+        logdet: Optional[bool] = False,
+        reduce_inv_quad: Optional[bool] = True,
+    ) -> Tuple[
+        Optional[Union[Float[Tensor, "*batch M"], Float[Tensor, " *batch"], Float[Tensor, " 0"]]],
+        Optional[Float[Tensor, "..."]],
+    ]:
         if not self.is_square:
             raise RuntimeError(
                 "inv_quad_logdet only operates on (batches of) square (positive semi-definite) LinearOperators. "
                 "Got a {} of size {}.".format(self.__class__.__name__, self.size())
             )
 
         if inv_quad_rhs is not None:
@@ -126,15 +151,19 @@
                 inv_quad_term = inv_quad_term.sum(dim=-1)
 
         if logdet:
             logdet_term = self._logdet()
 
         return inv_quad_term, logdet_term
 
-    def solve(self, right_tensor, left_tensor=None):
+    def solve(
+        self: Float[LinearOperator, "... N N"],
+        right_tensor: Union[Float[Tensor, "... N P"], Float[Tensor, " N"]],
+        left_tensor: Optional[Float[Tensor, "... O N"]] = None,
+    ) -> Union[Float[Tensor, "... N P"], Float[Tensor, "... N"], Float[Tensor, "... O P"], Float[Tensor, "... O"]]:
         if not self.is_square:
             raise RuntimeError(
                 "solve only operates on (batches of) square (positive semi-definite) LinearOperators. "
                 "Got a {} of size {}.".format(self.__class__.__name__, self.size())
             )
 
         if self.dim() == 2 and right_tensor.dim() == 1:
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/low_rank_root_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/low_rank_root_linear_operator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 #!/usr/bin/env python3
+from typing import Union
 
+import torch
+from jaxtyping import Float
+from torch import Tensor
+
+from ._linear_operator import LinearOperator
 from .root_linear_operator import RootLinearOperator
 
 
 class LowRankRootLinearOperator(RootLinearOperator):
     """
     Very thin wrapper around RootLinearOperator that denotes that the tensor specifically represents a low rank
     decomposition of a full rank matrix.
 
     The rationale for this class existing is that we can create LowRankAddedDiagLinearOperator without having to
     write custom _getitem, _get_indices, etc, leading to much better code reuse.
     """
 
-    def add_diagonal(self, diag):
+    def add_diagonal(
+        self: Float[LinearOperator, "*batch N N"],
+        diag: Union[Float[torch.Tensor, "... N"], Float[torch.Tensor, "... 1"], Float[torch.Tensor, ""]],
+    ) -> Float[LinearOperator, "*batch N N"]:
         from .diag_linear_operator import ConstantDiagLinearOperator, DiagLinearOperator
         from .low_rank_root_added_diag_linear_operator import LowRankRootAddedDiagLinearOperator
 
         if not self.is_square:
             raise RuntimeError("add_diag only defined for square matrices")
 
         diag_shape = diag.shape
@@ -35,15 +44,18 @@
                         self.shape, diag_shape
                     )
                 )
             diag_tensor = DiagLinearOperator(expanded_diag)
 
         return LowRankRootAddedDiagLinearOperator(self, diag_tensor)
 
-    def __add__(self, other):
+    def __add__(
+        self: Float[LinearOperator, "... #M #N"],
+        other: Union[Float[Tensor, "... #M #N"], Float[LinearOperator, "... #M #N"], float],
+    ) -> Union[Float[LinearOperator, "... M N"], Float[Tensor, "... M N"]]:
         from .diag_linear_operator import DiagLinearOperator
         from .low_rank_root_added_diag_linear_operator import LowRankRootAddedDiagLinearOperator
 
         if isinstance(other, DiagLinearOperator):
             return LowRankRootAddedDiagLinearOperator(self, other)
         else:
             return super().__add__(other)
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/matmul_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/matmul_linear_operator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 #!/usr/bin/env python3
 
+from typing import List, Optional, Tuple, Union
+
 import torch
+from jaxtyping import Float
+from torch import Tensor
 
 from ..utils.broadcasting import _matmul_broadcast_shape, _pad_with_singletons
 from ..utils.getitem import _noop_index
 from ..utils.memoize import cached
-from ._linear_operator import LinearOperator
+from ._linear_operator import IndexType, LinearOperator
 from .dense_linear_operator import DenseLinearOperator, to_linear_operator
 from .diag_linear_operator import DiagLinearOperator
 
 
 def _inner_repeat(tensor, amt):
     return tensor.unsqueeze(-1).repeat(amt, 1).squeeze(-1)
 
@@ -37,21 +41,22 @@
         else:
             self.left_linear_op = left_linear_op
         if right_linear_op.batch_shape != batch_shape:
             self.right_linear_op = right_linear_op._expand_batch(batch_shape)
         else:
             self.right_linear_op = right_linear_op
 
-    def _expand_batch(self, batch_shape):
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         return self.__class__(
-            self.left_linear_op._expand_batch(batch_shape),
-            self.right_linear_op._expand_batch(batch_shape),
+            self.left_linear_op._expand_batch(batch_shape), self.right_linear_op._expand_batch(batch_shape)
         )
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         row_index = row_index.unsqueeze(-1)
         col_index = col_index.unsqueeze(-1)
         batch_indices = tuple(batch_index.unsqueeze(-1) for batch_index in batch_indices)
         inner_index = torch.arange(0, self.left_linear_op.size(-1), device=self.device)
         inner_index = _pad_with_singletons(inner_index, row_index.dim() - 1, 0)
 
         left_tensor = self.left_linear_op._get_indices(
@@ -59,69 +64,69 @@
         )
         right_tensor = self.right_linear_op._get_indices(
             inner_index, col_index, *batch_indices[-len(self.right_linear_op.batch_shape) :]
         )
         res = (left_tensor * right_tensor).sum(-1)
         return res
 
-    def _diagonal(self):
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
         if isinstance(self.left_linear_op, DenseLinearOperator) and isinstance(
             self.right_linear_op, DenseLinearOperator
         ):
             return (self.left_linear_op.tensor * self.right_linear_op.tensor.mT).sum(-1)
         elif isinstance(self.left_linear_op, DiagLinearOperator) or isinstance(
             self.right_linear_op, DiagLinearOperator
         ):
             return self.left_linear_op._diagonal() * self.right_linear_op._diagonal()
         else:
             return super()._diagonal()
 
-    def _getitem(self, row_index, col_index, *batch_indices):
+    def _getitem(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> LinearOperator:
         # Make sure we're not generating more memory with our "efficient" method
         if torch.is_tensor(row_index) and torch.is_tensor(col_index):
             num_indices = row_index.numel()
             if num_indices > self.matrix_shape.numel():
                 return to_linear_operator(self.to_dense())._getitem(row_index, col_index, *batch_indices)
 
         left_tensor = self.left_linear_op._getitem(row_index, _noop_index, *batch_indices)
         right_tensor = self.right_linear_op._getitem(_noop_index, col_index, *batch_indices)
 
         res = MatmulLinearOperator(left_tensor, right_tensor)
         return res
 
-    def _matmul(self, right_linear_op):
-        return self.left_linear_op._matmul(self.right_linear_op._matmul(right_linear_op))
-
-    def _t_matmul(self, right_linear_op):
-        return self.right_linear_op._t_matmul(self.left_linear_op._t_matmul(right_linear_op))
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
+        return self.left_linear_op._matmul(self.right_linear_op._matmul(rhs))
+
+    def _t_matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[Tensor, "*batch2 M P"], Float[LinearOperator, "*batch2 M P"]],
+    ) -> Union[Float[LinearOperator, "... N P"], Float[Tensor, "... N P"]]:
+        return self.right_linear_op._t_matmul(self.left_linear_op._t_matmul(rhs))
 
-    def _bilinear_derivative(self, left_vecs, right_vecs):
+    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Optional[Tensor], ...]:
         if left_vecs.ndimension() == 1:
             left_vecs = left_vecs.unsqueeze(1)
             right_vecs = right_vecs.unsqueeze(1)
         right_vecs_times_right_linear_op = self.right_linear_op._matmul(right_vecs)
         left_vecs_times_left_linear_op_t = self.left_linear_op._t_matmul(left_vecs)
         left_grad = self.left_linear_op._bilinear_derivative(left_vecs, right_vecs_times_right_linear_op)
         right_grad = self.right_linear_op._bilinear_derivative(left_vecs_times_left_linear_op_t, right_vecs)
 
         left_grad = (left_grad,) if not isinstance(left_grad, tuple) else left_grad
         right_grad = (right_grad,) if not isinstance(right_grad, tuple) else right_grad
         return left_grad + right_grad
 
-    def _permute_batch(self, *dims):
-        return self.__class__(
-            self.left_linear_op._permute_batch(*dims),
-            self.right_linear_op._permute_batch(*dims),
-        )
+    def _permute_batch(self, *dims: int) -> LinearOperator:
+        return self.__class__(self.left_linear_op._permute_batch(*dims), self.right_linear_op._permute_batch(*dims))
 
-    def _size(self):
+    def _size(self) -> torch.Size:
         return _matmul_broadcast_shape(self.left_linear_op.shape, self.right_linear_op.shape)
 
-    def _transpose_nonbatch(self, *args):
-        return self.__class__(
-            self.right_linear_op._transpose_nonbatch(),
-            self.left_linear_op._transpose_nonbatch(),
-        )
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
+        return self.__class__(self.right_linear_op._transpose_nonbatch(), self.left_linear_op._transpose_nonbatch())
 
     @cached
-    def to_dense(self):
+    def to_dense(self: Float[LinearOperator, "*batch M N"]) -> Float[Tensor, "*batch M N"]:
         return torch.matmul(self.left_linear_op.to_dense(), self.right_linear_op.to_dense())
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/mul_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/mul_linear_operator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/usr/bin/env python3
+from typing import List, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
+from torch import Tensor
 
 from ..utils.broadcasting import _matmul_broadcast_shape
 from ..utils.memoize import cached
-from ._linear_operator import LinearOperator
+from ._linear_operator import IndexType, LinearOperator
+from .linear_operator_representation_tree import LinearOperatorRepresentationTree
 from .root_linear_operator import RootLinearOperator
 
 
 class MulLinearOperator(LinearOperator):
     def _check_args(self, left_linear_op, right_linear_op):
         if not isinstance(left_linear_op, LinearOperator) or not isinstance(right_linear_op, LinearOperator):
             return "MulLinearOperator expects two LinearOperators."
@@ -29,24 +33,27 @@
             left_linear_op = left_linear_op.root_decomposition()
         if not isinstance(right_linear_op, RootLinearOperator):
             right_linear_op = right_linear_op.root_decomposition()
         super().__init__(left_linear_op, right_linear_op)
         self.left_linear_op = left_linear_op
         self.right_linear_op = right_linear_op
 
-    def _diagonal(self):
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
         res = self.left_linear_op._diagonal() * self.right_linear_op._diagonal()
         return res
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         left_res = self.left_linear_op._get_indices(row_index, col_index, *batch_indices)
         right_res = self.right_linear_op._get_indices(row_index, col_index, *batch_indices)
         return left_res * right_res
 
-    def _matmul(self, rhs):
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         output_shape = _matmul_broadcast_shape(self.shape, rhs.shape)
         output_batch_shape = output_shape[:-2]
 
         is_vector = False
         if rhs.ndimension() == 1:
             rhs = rhs.unsqueeze(1)
             is_vector = True
@@ -66,24 +73,26 @@
             res = left_res.mul_(left_root.unsqueeze(-1)).sum(-2)
         # This is the case where we're not doing a root decomposition, because the matrix is too small
         else:  # Dead?
             res = (self.left_linear_op.to_dense() * self.right_linear_op.to_dense()).matmul(rhs)
         res = res.squeeze(-1) if is_vector else res
         return res
 
-    def _mul_constant(self, constant):
-        if constant > 0:
-            res = self.__class__(self.left_linear_op._mul_constant(constant), self.right_linear_op)
+    def _mul_constant(
+        self: Float[LinearOperator, "*batch M N"], other: Union[float, torch.Tensor]
+    ) -> Float[LinearOperator, "*batch M N"]:
+        if other > 0:
+            res = self.__class__(self.left_linear_op._mul_constant(other), self.right_linear_op)
         else:
             # Negative constants can screw up the root_decomposition
             # So we'll do a standard _mul_constant
-            res = super()._mul_constant(constant)
+            res = super()._mul_constant(other)
         return res
 
-    def _bilinear_derivative(self, left_vecs, right_vecs):
+    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Optional[Tensor], ...]:
         if left_vecs.ndimension() == 1:
             left_vecs = left_vecs.unsqueeze(1)
             right_vecs = right_vecs.unsqueeze(1)
 
         *batch_shape, n, num_vecs = left_vecs.size()
 
         if isinstance(self.right_linear_op, RootLinearOperator):
@@ -114,33 +123,34 @@
 
         left_factor = left_factor.view(*batch_shape, n, num_vecs * left_rank)
         right_factor = right_factor.view(*batch_shape, n, num_vecs * left_rank)
         right_deriv_args = self.right_linear_op._bilinear_derivative(left_factor, right_factor)
 
         return tuple(list(left_deriv_args) + list(right_deriv_args))
 
-    def _expand_batch(self, batch_shape):
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         return self.__class__(
-            self.left_linear_op._expand_batch(batch_shape),
-            self.right_linear_op._expand_batch(batch_shape),
+            self.left_linear_op._expand_batch(batch_shape), self.right_linear_op._expand_batch(batch_shape)
         )
 
     @cached
-    def to_dense(self):
+    def to_dense(self: Float[LinearOperator, "*batch M N"]) -> Float[Tensor, "*batch M N"]:
         return self.left_linear_op.to_dense() * self.right_linear_op.to_dense()
 
-    def _size(self):
+    def _size(self) -> torch.Size:
         return self.left_linear_op.size()
 
-    def _transpose_nonbatch(self):
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         # mul.linear_op only works with symmetric matrices
         return self
 
-    def representation(self):
+    def representation(self) -> Tuple[torch.Tensor, ...]:
         """
         Returns the Tensors that are used to define the LinearOperator
         """
         res = super(MulLinearOperator, self).representation()
         return res
 
-    def representation_tree(self):
+    def representation_tree(self) -> LinearOperatorRepresentationTree:
         return super(MulLinearOperator, self).representation_tree()
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/permutation_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/permutation_linear_operator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,54 @@
-from typing import Optional, Tuple
+from typing import Callable, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
 from torch import Tensor
 
 from ._linear_operator import LinearOperator
 
 
 class AbstractPermutationLinearOperator(LinearOperator):
     r"""Abstract base class for permutation operators.
     Incorporates 1) square shape, 2) common input shape checking, and
     3) the fact that permutation matrices' transposes are their inverses.
     """
 
-    def inverse(self):
+    def inverse(self: Float[LinearOperator, "*batch N N"]) -> Float[LinearOperator, "*batch N N"]:
         return self._transpose_nonbatch()
 
-    def _solve(self, rhs: Tensor):
+    def _solve(
+        self: Float[LinearOperator, "... N N"],
+        rhs: Float[torch.Tensor, "... N C"],
+        preconditioner: Optional[Callable[[Float[torch.Tensor, "... N C"]], Float[torch.Tensor, "... N C"]]] = None,
+        num_tridiag: Optional[int] = 0,
+    ) -> Union[
+        Float[torch.Tensor, "... N C"],
+        Tuple[
+            Float[torch.Tensor, "... N C"],
+            Float[torch.Tensor, "..."],  # Note that in case of a tuple the second term size depends on num_tridiag
+        ],
+    ]:
         self._matmul_check_shape(rhs)
         return self.inverse() @ rhs
 
     def _matmul_check_shape(self, rhs: Tensor) -> None:
         if rhs.shape[-2] != self.shape[-1]:
             raise ValueError(
                 f"{rhs.shape[0] = } incompatible with first dimensions of"
                 f"permutation operator with shape {self.shape}."
             )
 
     def _matmul_batch_shape(self, rhs: Tensor) -> torch.Size:
         return torch.broadcast_shapes(self.batch_shape, rhs.shape[:-2])
 
+    @property
+    def dtype(self) -> Optional[torch.dtype]:
+        return self._dtype
+
 
 class PermutationLinearOperator(AbstractPermutationLinearOperator):
     r"""LinearOperator that lazily represents a permutation matrix with O(n) memory.
     Upon left-multiplication, it permutes the first non-batch dimension of a tensor.
 
     Args:
         - perm: A permutation tensor with which to permute the first non-batch
@@ -72,17 +88,21 @@
                     raise ValueError(
                         f"Invalid perm-inv_perm input, index {i} missing or not at "
                         f"correct index for permutation with {perm.shape = }."
                     )
 
         self.perm = perm
         self.inv_perm = inv_perm
+        self._dtype = torch.float32
         super().__init__(perm, inv_perm, validate_args=validate_args)
 
-    def _matmul(self, rhs: Tensor) -> Tensor:
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         # input rhs is guaranteed to be at least two-dimensional due to matmul implementation
         self._matmul_check_shape(rhs)
 
         # batch broadcasting logic
         batch_shape = self._matmul_batch_shape(rhs)
         expanded_rhs = rhs.expand(*batch_shape, *rhs.shape[-2:])
         ndim = expanded_rhs.ndim
@@ -107,15 +127,15 @@
             )
             for i, n in enumerate(batch_shape)
         )
 
     def _size(self) -> torch.Size:
         return torch.Size((*self.perm.shape, self.perm.shape[-1]))
 
-    def _transpose_nonbatch(self):
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         return PermutationLinearOperator(perm=self.inv_perm, inv_perm=self.perm, validate_args=False)
 
     def to_sparse(self) -> Tensor:
         """Returns a sparse CSR tensor that represents the PermutationLinearOperator."""
         # crow_indices[i] is index where values of row i begin
         return torch.sparse_csr_tensor(
             crow_indices=torch.arange(self.shape[-1] + 1).expand(*self.batch_shape, -1).contiguous(),
@@ -139,30 +159,34 @@
 
     def __init__(self, m: int):
         if m < 1:
             raise ValueError(f"m = {m} has to be a positive integer.")
         super().__init__(m=m)
         self.n = m * m  # size of implicitly represented linear operator
         self.m = m  # (m, m) is size of the reshaped input which is transposed
-        self._dtype = type(m)
+        # self._dtype = type(m)
+        self._dtype = torch.float32
 
-    def _matmul(self, rhs: Tensor) -> Tensor:
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         self._matmul_check_shape(rhs)
         return rhs.unflatten(dim=-2, sizes=(self.m, self.m)).transpose(-3, -2).flatten(start_dim=-3, end_dim=-2)
 
     def _size(self) -> torch.Size:
         return torch.Size((self.n, self.n))
 
-    def _transpose_nonbatch(self):
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         return self
 
     @property
-    def dtype(self):
+    def dtype(self) -> Optional[torch.dtype]:
         return self._dtype
 
-    def type(self, dtype: torch.dtype) -> LinearOperator:
+    def type(self: LinearOperator, dtype: torch.dtype) -> LinearOperator:
         self._dtype = dtype
         return self
 
     @property
-    def device(self):
+    def device(self) -> Optional[torch.device]:
         return None
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/sum_batch_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/sum_batch_linear_operator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python3
 
 import torch
+from jaxtyping import Float
+from torch import Tensor
 
 from ..utils.broadcasting import _pad_with_singletons
 from ..utils.getitem import _noop_index
+from ._linear_operator import IndexType, LinearOperator
 from .block_linear_operator import BlockLinearOperator
 
 
 class SumBatchLinearOperator(BlockLinearOperator):
     """
     Represents a lazy tensor that is actually the sum of several lazy tensors blocks.
     The :attr:`block_dim` attribute specifies which dimension of the base LinearOperator
@@ -26,36 +29,36 @@
         shape = list(other.shape)
         expand_shape = list(other.shape)
         shape.insert(-2, 1)
         expand_shape.insert(-2, self.base_linear_op.size(-3))
         other = other.reshape(*shape).expand(*expand_shape)
         return other
 
-    def _diagonal(self):
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
         diag = self.base_linear_op._diagonal().sum(-2)
         return diag
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         # Create an extra index for the summed dimension
         sum_index = torch.arange(0, self.base_linear_op.size(-3), device=self.device)
         sum_index = _pad_with_singletons(sum_index, row_index.dim(), 0)
         row_index = row_index.unsqueeze(-1)
         col_index = col_index.unsqueeze(-1)
         batch_indices = [index.unsqueeze(-1) for index in batch_indices]
 
         res = self.base_linear_op._get_indices(row_index, col_index, *batch_indices, sum_index)
         return res.sum(-1)
 
-    def _getitem(self, row_index, col_index, *batch_indices):
+    def _getitem(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> LinearOperator:
         res = self.base_linear_op._getitem(row_index, col_index, *batch_indices, _noop_index)
         return self.__class__(res, **self._kwargs)
 
     def _remove_batch_dim(self, other):
         return other.sum(-3)
 
-    def _size(self):
+    def _size(self) -> torch.Size:
         shape = list(self.base_linear_op.shape)
         del shape[-3]
         return torch.Size(shape)
 
-    def to_dense(self):
+    def to_dense(self: Float[LinearOperator, "*batch M N"]) -> Float[Tensor, "*batch M N"]:
         return self.base_linear_op.to_dense().sum(dim=-3)  # BlockLinearOperators always use dim3 for the block_dim
```

### Comparing `linear_operator-0.4.0/linear_operator/operators/toeplitz_linear_operator.py` & `linear_operator-0.5.0/linear_operator/operators/toeplitz_linear_operator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #!/usr/bin/env python3
+from typing import List, Optional, Tuple, Union
 
 import torch
+from jaxtyping import Float
+from torch import Tensor
 
 from ..utils.toeplitz import sym_toeplitz_derivative_quadratic_form, sym_toeplitz_matmul
-from ._linear_operator import LinearOperator
+from ._linear_operator import IndexType, LinearOperator
 
 
 class ToeplitzLinearOperator(LinearOperator):
     def __init__(self, column):
         """
         Args:
             :attr: `column` (Tensor)
@@ -15,50 +18,60 @@
                 Toeplitz matrix with `column` as its first column.
                 If `column` is `b_1 x b_2 x ... x b_k x n`, then this represents a batch
                 `b_1 x b_2 x ... x b_k` of Toeplitz matrices.
         """
         super(ToeplitzLinearOperator, self).__init__(column)
         self.column = column
 
-    def _diagonal(self):
+    def _diagonal(self: Float[LinearOperator, "... M N"]) -> Float[torch.Tensor, "... N"]:
         diag_term = self.column[..., 0]
         if self.column.ndimension() > 1:
             diag_term = diag_term.unsqueeze(-1)
         return diag_term.expand(*self.column.size())
 
-    def _expand_batch(self, batch_shape):
+    def _expand_batch(
+        self: Float[LinearOperator, "... M N"], batch_shape: Union[torch.Size, List[int]]
+    ) -> Float[LinearOperator, "... M N"]:
         return self.__class__(self.column.expand(*batch_shape, self.column.size(-1)))
 
-    def _get_indices(self, row_index, col_index, *batch_indices):
+    def _get_indices(self, row_index: IndexType, col_index: IndexType, *batch_indices: IndexType) -> torch.Tensor:
         toeplitz_indices = (row_index - col_index).fmod(self.size(-1)).abs().long()
         return self.column[(*batch_indices, toeplitz_indices)]
 
-    def _matmul(self, rhs):
+    def _matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[torch.Tensor, "*batch2 N C"], Float[torch.Tensor, "*batch2 N"]],
+    ) -> Union[Float[torch.Tensor, "... M C"], Float[torch.Tensor, "... M"]]:
         return sym_toeplitz_matmul(self.column, rhs)
 
-    def _t_matmul(self, rhs):
+    def _t_matmul(
+        self: Float[LinearOperator, "*batch M N"],
+        rhs: Union[Float[Tensor, "*batch2 M P"], Float[LinearOperator, "*batch2 M P"]],
+    ) -> Union[Float[LinearOperator, "... N P"], Float[Tensor, "... N P"]]:
         # Matrix is symmetric
         return self._matmul(rhs)
 
-    def _bilinear_derivative(self, left_vecs, right_vecs):
+    def _bilinear_derivative(self, left_vecs: Tensor, right_vecs: Tensor) -> Tuple[Optional[Tensor], ...]:
         if left_vecs.ndimension() == 1:
             left_vecs = left_vecs.unsqueeze(1)
             right_vecs = right_vecs.unsqueeze(1)
 
         res = sym_toeplitz_derivative_quadratic_form(left_vecs, right_vecs)
 
         # Collapse any expanded broadcast dimensions
         if res.dim() > self.column.dim():
             res = res.view(-1, *self.column.shape).sum(0)
 
         return (res,)
 
-    def _size(self):
+    def _size(self) -> torch.Size:
         return torch.Size((*self.column.shape, self.column.size(-1)))
 
-    def _transpose_nonbatch(self):
+    def _transpose_nonbatch(self: Float[LinearOperator, "*batch M N"]) -> Float[LinearOperator, "*batch N M"]:
         return ToeplitzLinearOperator(self.column)
 
-    def add_jitter(self, jitter_val=1e-3):
+    def add_jitter(
+        self: Float[LinearOperator, "*batch N N"], jitter_val: float = 1e-3
+    ) -> Float[LinearOperator, "*batch N N"]:
         jitter = torch.zeros_like(self.column)
         jitter.narrow(-1, 0, 1).fill_(jitter_val)
         return ToeplitzLinearOperator(self.column.add(jitter))
```

### Comparing `linear_operator-0.4.0/linear_operator/settings.py` & `linear_operator-0.5.0/linear_operator/settings.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/test/base_test_case.py` & `linear_operator-0.5.0/linear_operator/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/test/linear_operator_test_case.py` & `linear_operator-0.5.0/linear_operator/test/linear_operator_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/usr/bin/env python3
 
+import logging
 import math
+import traceback
 from abc import abstractmethod
 from itertools import combinations, product
 from unittest.mock import MagicMock, patch
 
 import torch
 
 import linear_operator
 from linear_operator.operators import DenseLinearOperator, DiagLinearOperator, to_dense
 from linear_operator.settings import linalg_dtypes
 from linear_operator.utils.errors import CachingError
 from linear_operator.utils.memoize import get_from_cache
-from linear_operator.utils.warnings import PerformanceWarning
 
+from ..utils.warnings import PerformanceWarning
 from .base_test_case import BaseTestCase
 
 
 class RectangularLinearOperatorTestCase(BaseTestCase):
 
     tolerances = {
         "matmul": {"rtol": 1e-3},
@@ -80,14 +82,17 @@
 
     def test_add(self):
         linear_op = self.create_linear_op()
         evaluated = self.evaluate_linear_op(linear_op)
 
         rhs = torch.randn(linear_op.shape)
         # Test operator functionality
+        a = (linear_op + rhs).to_dense()
+        b = evaluated + rhs
+        self.assertAllClose(a, b)
         self.assertAllClose((linear_op + rhs).to_dense(), evaluated + rhs)
         self.assertAllClose((rhs + linear_op).to_dense(), evaluated + rhs)
         # Test __torch_function__ functionality
         self.assertAllClose(torch.add(linear_op, rhs).to_dense(), evaluated + rhs)
         self.assertAllClose(torch.add(rhs, linear_op).to_dense(), evaluated + rhs)
 
         rhs = torch.randn(linear_op.matrix_shape)
@@ -606,14 +611,15 @@
 
     def test_add_diagonal(self):
         linear_op = self.create_linear_op()
         evaluated = self.evaluate_linear_op(linear_op)
 
         other_diag = torch.tensor(1.5)
         res = linear_operator.add_diagonal(linear_op, other_diag).to_dense()
+
         actual = evaluated + torch.eye(evaluated.size(-1)).view(
             *[1 for _ in range(linear_op.dim() - 2)], evaluated.size(-1), evaluated.size(-1)
         ).repeat(*linear_op.batch_shape, 1, 1).mul(1.5)
         self.assertAllClose(res, actual)
 
         other_diag = torch.tensor([1.5])
         res = linear_operator.add_diagonal(linear_op, other_diag).to_dense()
@@ -635,15 +641,14 @@
             for i in range(other_diag.size(-1)):
                 actual[..., i, i] = actual[..., i, i] + other_diag[..., i]
             self.assertAllClose(res, actual, **self.tolerances["diag"])
 
     def test_add_jitter(self):
         linear_op = self.create_linear_op()
         evaluated = self.evaluate_linear_op(linear_op)
-
         res = linear_operator.add_jitter(linear_op, 0.4).to_dense()
         actual = evaluated + torch.eye(evaluated.size(-1)).mul_(0.4)
         self.assertAllClose(res, actual)
 
     def test_add_low_rank(self):
         linear_op = self.create_linear_op()
         linear_op = self.create_linear_op()
@@ -690,15 +695,19 @@
             new_point = torch.rand(*batch_shape, *linear_op.shape[:-2], 1, 1)
 
             # we need to expand here to be able to concat (this happens automatically in cat_rows)
             cat_col1 = torch.cat((evaluated.expand(*batch_shape, *evaluated.shape), new_rows), dim=-2)
             cat_col2 = torch.cat((new_rows.mT, new_point), dim=-2)
 
             concatenated_lt = torch.cat((cat_col1, cat_col2), dim=-1)
-            new_lt = linear_op.cat_rows(new_rows, new_point)
+            try:
+                new_lt = linear_op.cat_rows(new_rows, new_point)
+            except Exception:
+                msg = traceback.format_exc()
+                logging.warning(msg)
 
             # check that the concatenation is okay
             self.assertAllClose(new_lt.to_dense(), concatenated_lt)
 
             # check that the root approximation is close
             rhs = torch.randn(linear_op.size(-1) + 1)
             concat_rhs = concatenated_lt.matmul(rhs)
@@ -843,15 +852,15 @@
         self.assertEqual(expanded_op.shape, expanded_shape)
         # dealing with -1 shapes
         expanded_op = linear_op.expand(*linear_op.shape[:-2], -1, -1)
         self.assertEqual(expanded_op.shape, linear_op.shape)
         # check that error is raised if incompatible expand shape
         expand_args = (*linear_op.shape[:-2], 4, 5)
         expected_msg = r"Invalid expand arguments \({}\)".format(", ".join(str(a) for a in expand_args))
-        with self.assertRaisesRegex(RuntimeError, expected_msg):
+        with self.assertRaisesRegex((TypeError, RuntimeError), expected_msg):
             linear_op.expand(*expand_args)
 
     def test_reshape(self):
         # reshape is mostly an alias for expand, we just need to check the handling of a leading -1 dim
         linear_op = self.create_linear_op()
         expanded_op = linear_op.reshape(-1, *linear_op.shape)
         self.assertEqual(expanded_op.shape, torch.Size([1]) + linear_op.shape)
@@ -896,15 +905,15 @@
         self.assertFalse(torch.any(is_close[..., 0, 0]))
         is_close[..., 0, 0] = True
         self.assertTrue(torch.all(is_close))
 
     def test_logdet(self):
         tolerances = self.tolerances["logdet"]
 
-        linear_op = self.create_linear_op()
+        linear_op = self.create_linear_op().detach()
         linear_op_copy = linear_op.detach().clone()
         linear_op.requires_grad_(True)
         linear_op_copy.requires_grad_(True)
         evaluated = self.evaluate_linear_op(linear_op_copy)
         evaluated.register_hook(self._ensure_symmetric_grad)
 
         # Add a diagonal
@@ -961,15 +970,19 @@
 
     def test_diagonalization(self, symeig=False):
         _wrapped_lanczos = MagicMock(wraps=linear_operator.utils.lanczos.lanczos_tridiag)
         with patch("linear_operator.utils.lanczos.lanczos_tridiag", new=_wrapped_lanczos) as lanczos_mock:
             linear_op = self.create_linear_op()
             test_mat = torch.randn(*linear_op.batch_shape, linear_op.size(-1), 5)
             with linear_operator.settings.max_cholesky_size(math.inf if symeig else 0):
-                evals, evecs = linear_op.diagonalization()
+                try:
+                    evals, evecs = linear_op.diagonalization()
+                except Exception:
+                    msg = traceback.format_exc()
+                    logging.warning(msg)
                 evecs = evecs.to_dense()
                 approx = evecs.matmul(torch.diag_embed(evals)).matmul(evecs.mT)
                 res = approx.matmul(test_mat)
                 actual = linear_op.matmul(test_mat)
                 self.assertAllClose(res, actual, rtol=0.05)
 
             # Make sure that we're calling the correct function
```

### Comparing `linear_operator-0.4.0/linear_operator/test/utils.py` & `linear_operator-0.5.0/linear_operator/test/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if self.size() != other.size():
         raise RuntimeError(
             "Size mismatch between self ({self}) and other ({other})".format(self=self.size(), other=other.size())
         )
     return torch.max((self - other).abs()) <= epsilon
 
 
-def get_cuda_max_memory_allocations() -> int:
+def get_cuda_max_memory_allocations() -> torch.Tensor:
     """Get the `max_memory_allocated` for each cuda device"""
     return torch.tensor([torch.cuda.max_memory_allocated(i) for i in range(torch.cuda.device_count())])
 
 
 @contextmanager
 def least_used_cuda_device() -> Generator:
     """Contextmanager for automatically selecting the cuda device
```

### Comparing `linear_operator-0.4.0/linear_operator/utils/__init__.py` & `linear_operator-0.5.0/linear_operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/broadcasting.py` & `linear_operator-0.5.0/linear_operator/utils/broadcasting.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/cholesky.py` & `linear_operator-0.5.0/linear_operator/utils/cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/contour_integral_quad.py` & `linear_operator-0.5.0/linear_operator/utils/contour_integral_quad.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/deprecation.py` & `linear_operator-0.5.0/linear_operator/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/generic.py` & `linear_operator-0.5.0/linear_operator/utils/generic.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/getitem.py` & `linear_operator-0.5.0/linear_operator/utils/getitem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
-from typing import Tuple, Union
+from typing import Any, Iterable, Tuple, Union
 
 import torch
 
 from .. import settings
 from .broadcasting import _pad_with_singletons
 
+# EllipsisType is only available in Python 3.10+
+IndexType = Union[type(Ellipsis), slice, Iterable[int], torch.LongTensor, int]
+
 # A slice that does nothing to a dimension
 _noop_index = slice(None, None, None)
 
 
 def _compute_getitem_size(
-    obj: Union[torch.Tensor, "LinearOperator"],  # noqa F821
-    indices: Tuple[Union[slice, torch.LongTensor, int], ...],  # noqa F811
+    obj: Union[torch.Tensor, Any],
+    indices: IndexType,  # Forward references not supported - obj: Union[torch.Tensor, "LinearOperator"]
 ) -> torch.Size:
     """
     Given an object and a tuple of indices, computes the final size of the
     Indices is a tuple containing ints, slices, and tensors
 
     .. note::
         The length of indices must match the dimensionality of obj
@@ -89,16 +92,16 @@
     if tensor_idx is not None:
         final_shape = final_shape[:tensor_idx] + list(tensor_idx_shape) + final_shape[tensor_idx:]
 
     return torch.Size(final_shape)
 
 
 def _convert_indices_to_tensors(
-    obj: Union[torch.Tensor, "LinearOperator"],  # noqa F821
-    indices: Tuple[Union[slice, torch.LongTensor, int], ...],  # noqa F811
+    obj: Union[torch.Tensor, Any],
+    indices: IndexType,  # Forward references not supported - obj: Union[torch.Tensor, "LinearOperator"]
 ) -> Tuple[torch.LongTensor, ...]:
     """
     Given an index made up of tensors/slices/ints, returns a tensor-only index that has the
     same outcome as the original index (when applied to the obj)
 
     .. note::
         The length of indices must match the dimensionality of obj
```

### Comparing `linear_operator-0.4.0/linear_operator/utils/interpolation.py` & `linear_operator-0.5.0/linear_operator/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/lanczos.py` & `linear_operator-0.5.0/linear_operator/utils/lanczos.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/linear_cg.py` & `linear_operator-0.5.0/linear_operator/utils/linear_cg.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/memoize.py` & `linear_operator-0.5.0/linear_operator/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/minres.py` & `linear_operator-0.5.0/linear_operator/utils/minres.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/permutation.py` & `linear_operator-0.5.0/linear_operator/utils/permutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 import torch
 
 
 def apply_permutation(
-    matrix: Union["LinearOperator", torch.Tensor],  # noqa: F821
+    matrix: Union[Any, torch.Tensor],  # Union["LinearOperator", torch.Tensor]
     left_permutation: Optional[torch.Tensor] = None,
     right_permutation: Optional[torch.Tensor] = None,
 ):
     r"""
     Applies a left and/or right (partial) permutation to a given matrix :math:`\mathbf K`:
 
     .. math::
```

### Comparing `linear_operator-0.4.0/linear_operator/utils/pinverse.py` & `linear_operator-0.5.0/linear_operator/utils/pinverse.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/qr.py` & `linear_operator-0.5.0/linear_operator/utils/qr.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/sparse.py` & `linear_operator-0.5.0/linear_operator/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/stochastic_lq.py` & `linear_operator-0.5.0/linear_operator/utils/stochastic_lq.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator/utils/toeplitz.py` & `linear_operator-0.5.0/linear_operator/utils/toeplitz.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/linear_operator.egg-info/PKG-INFO` & `linear_operator-0.5.0/linear_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-operator
-Version: 0.4.0
+Version: 0.5.0
 Summary: A linear operator implementation, primarily designed for finite-dimensional positive definite operators (i.e. kernel matrices).
 Home-page: UNKNOWN
 Author: Geoff Pleiss
 Author-email: gpleiss@gmail.com
 License: MIT
 Project-URL: Documentation, https://linear_operator.readthedocs.io
 Project-URL: Source, https://github.com/cornellius-gp/linear_operator/
```

### Comparing `linear_operator-0.4.0/linear_operator.egg-info/SOURCES.txt` & `linear_operator-0.5.0/linear_operator.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,22 @@
 .conda/meta.yaml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/documentation_examples.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/other.md
 .github/ISSUE_TEMPLATE/refactor.md
 .github/workflows/deploy.yml
+.github/workflows/pull_request.yml
+.github/workflows/push_to_main.yml
+.github/workflows/run_linter.yml
 .github/workflows/run_test_suite.yml
+.github/workflows/run_type_checked_test_suite.yml
+.hooks/check_type_hints.sh
+.hooks/propagate_type_hints.py
+.hooks/propagate_type_hints.sh
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/about.rst
 docs/source/composition_decoration_operators.rst
 docs/source/conf.py
 docs/source/converting.rst
@@ -63,14 +70,15 @@
 linear_operator/operators/chol_linear_operator.py
 linear_operator/operators/constant_mul_linear_operator.py
 linear_operator/operators/dense_linear_operator.py
 linear_operator/operators/diag_linear_operator.py
 linear_operator/operators/identity_linear_operator.py
 linear_operator/operators/interpolated_linear_operator.py
 linear_operator/operators/keops_linear_operator.py
+linear_operator/operators/kernel_linear_operator.py
 linear_operator/operators/kronecker_product_added_diag_linear_operator.py
 linear_operator/operators/kronecker_product_linear_operator.py
 linear_operator/operators/linear_operator_representation_tree.py
 linear_operator/operators/low_rank_root_added_diag_linear_operator.py
 linear_operator/operators/low_rank_root_linear_operator.py
 linear_operator/operators/matmul_linear_operator.py
 linear_operator/operators/mul_linear_operator.py
@@ -82,14 +90,15 @@
 linear_operator/operators/sum_linear_operator.py
 linear_operator/operators/toeplitz_linear_operator.py
 linear_operator/operators/triangular_linear_operator.py
 linear_operator/operators/zero_linear_operator.py
 linear_operator/test/__init__.py
 linear_operator/test/base_test_case.py
 linear_operator/test/linear_operator_test_case.py
+linear_operator/test/type_checking_test_case.py
 linear_operator/test/utils.py
 linear_operator/utils/__init__.py
 linear_operator/utils/broadcasting.py
 linear_operator/utils/cholesky.py
 linear_operator/utils/contour_integral_quad.py
 linear_operator/utils/deprecation.py
 linear_operator/utils/errors.py
@@ -126,14 +135,15 @@
 test/operators/test_cat_linear_operator.py
 test/operators/test_chol_linear_operator.py
 test/operators/test_constant_mul_linear_operator.py
 test/operators/test_dense_linear_operator.py
 test/operators/test_diag_linear_operator.py
 test/operators/test_identity_linear_operator.py
 test/operators/test_interpolated_linear_operator.py
+test/operators/test_kernel_linear_operator.py
 test/operators/test_kronecker_product_added_diag_linear_operator.py
 test/operators/test_kronecker_product_linear_operator.py
 test/operators/test_low_rank_root_added_diag_linear_operator.py
 test/operators/test_low_rank_root_linear_operator.py
 test/operators/test_matmul_linear_operator.py
 test/operators/test_mul_linear_operator.py
 test/operators/test_permutation_linear_operator.py
```

### Comparing `linear_operator-0.4.0/setup.py` & `linear_operator-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     if torch.__version__ >= torch_min:
         install_requires = []
 except ImportError:
     pass
 
 # Other requirements
-install_requires += ["scipy"]
+install_requires += ["scipy", "jaxtyping>=0.2.9", "typeguard~=2.13.3"]
 
 
 # Get version
 def find_version(*file_paths):
     try:
         with io.open(os.path.join(os.path.dirname(__file__), *file_paths), encoding="utf8") as fp:
             version_file = fp.read()
@@ -73,11 +73,11 @@
         "Programming Language :: Python :: 3",
     ],
     packages=find_packages(exclude=["test", "test.*"]),
     python_requires=">=3.8",
     install_requires=install_requires,
     extras_require={
         "dev": ["ufmt", "twine", "pre-commit"],
-        "test": ["flake8==5.0.4", "flake8-print==5.0.0"],
+        "test": ["flake8==5.0.4", "flake8-print==5.0.0", "pytest"],
     },
     test_suite="test",
 )
```

### Comparing `linear_operator-0.4.0/test/functions/test_diagonalization.py` & `linear_operator-0.5.0/test/functions/test_diagonalization.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/functions/test_dsmm.py` & `linear_operator-0.5.0/test/functions/test_dsmm.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/functions/test_inv_quad.py` & `linear_operator-0.5.0/test/functions/test_inv_quad.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/functions/test_inv_quad_logdet.py` & `linear_operator-0.5.0/test/functions/test_inv_quad_logdet.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/functions/test_matmul.py` & `linear_operator-0.5.0/test/functions/test_matmul.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/functions/test_pivoted_cholesky.py` & `linear_operator-0.5.0/test/functions/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/functions/test_root_decomposition.py` & `linear_operator-0.5.0/test/functions/test_root_decomposition.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/functions/test_solve.py` & `linear_operator-0.5.0/test/functions/test_solve.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_added_diag_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_batch_repeat_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_batch_repeat_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_block_diag_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_block_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_block_interleaved_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_block_interleaved_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_cat_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_cat_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_chol_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_chol_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_constant_mul_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_constant_mul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_dense_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_dense_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_diag_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_identity_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_identity_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_interpolated_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_interpolated_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_kronecker_product_added_diag_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_kronecker_product_added_diag_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     DiagLinearOperator,
     KroneckerProductAddedDiagLinearOperator,
     KroneckerProductDiagLinearOperator,
     KroneckerProductLinearOperator,
 )
 from linear_operator.test.linear_operator_test_case import LinearOperatorTestCase
 
+# requires typeguard 3.1+
+# import typeguard
+# import pytest
+# @pytest.fixture(autouse=True)
+# def suppress_typeguard():
+#    yield typeguard.suppress_type_checks()
+
 
 class TestKroneckerProductAddedDiagLinearOperator(unittest.TestCase, LinearOperatorTestCase):
     # this lazy tensor has an explicit inverse so we don't need to run these
     skip_slq_tests = True
     tolerances = {
         **LinearOperatorTestCase.tolerances,
         # eigh (used in Kronecker algebra) yields less precise solves
```

### Comparing `linear_operator-0.4.0/test/operators/test_kronecker_product_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_kronecker_product_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_low_rank_root_added_diag_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_low_rank_root_added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_low_rank_root_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_low_rank_root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_matmul_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_matmul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_mul_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_mul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_permutation_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_permutation_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 #!/usr/bin/env python3
 
 import unittest
 
 import torch
 
+from packaging import version
+
 from linear_operator.operators import PermutationLinearOperator, TransposePermutationLinearOperator
 
 
 class TestPermutationLinearOperator(unittest.TestCase):
     def test_permutation_linear_operator(self):
-        with self.assertRaisesRegex(ValueError, "perm is not a Tensor."):
-            PermutationLinearOperator([1, 3, 5])
+        # Type checking handles this
+        # with self.assertRaisesRegex(ValueError, "perm is not a Tensor."):
+        #   PermutationLinearOperator([1, 3, 5])
 
         with self.assertRaisesRegex(ValueError, "Invalid perm*"):
             PermutationLinearOperator(torch.tensor([1, 3, 5]))
 
         with self.assertRaisesRegex(ValueError, "Invalid perm*"):
             PermutationLinearOperator(torch.tensor([0, 2, 1]), torch.tensor([0, 1, 2]))
 
@@ -29,20 +32,20 @@
             torch.randperm(n),
             torch.cat(tuple(torch.randperm(n).unsqueeze(0) for _ in range(b1)), dim=0),
         ]
         operators = [PermutationLinearOperator(perm) for perm in permutations]
         right_hand_sides = [torch.randn(n)] + [torch.randn(*batch_shape, n, 4) for batch_shape in batch_shapes]
 
         for P in operators:
-            if torch.__version__ > "1.12":
+            if version.parse(torch.__version__) > version.parse("1.12"):
                 D = P.to_dense()
                 S = P.to_sparse()
                 self.assertTrue(isinstance(S, torch.Tensor))
                 self.assertTrue(S.layout == torch.sparse_csr)
-                self.assertTrue(torch.equal(D, S.to_dense()))
+                self.assertTrue(torch.equal(D, S.to_dense().to(D.dtype)))
 
             for x in right_hand_sides:
                 batch_shape = torch.broadcast_shapes(P.batch_shape, x.shape[:-2])
                 expanded_x = x.expand(*batch_shape, *x.shape[-2:]).contiguous()
                 self.assertTrue(P._matmul_batch_shape(x) == batch_shape)
                 y = P @ x
```

### Comparing `linear_operator-0.4.0/test/operators/test_psd_sum_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_psd_sum_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_root_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_sum_batch_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_sum_batch_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_sum_kronecker_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_sum_kronecker_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_sum_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_sum_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_toeplitz_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_toeplitz_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_triangular_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_triangular_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/operators/test_zero_linear_operator.py` & `linear_operator-0.5.0/test/operators/test_zero_linear_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     def test_matmul(self):
         zero = ZeroLinearOperator(5, 4, 3)
         lazy_square = ZeroLinearOperator(5, 3, 3)
         actual = torch.zeros(5, 4, 3)
         product = zero.matmul(lazy_square)
         self.assertTrue(approx_equal(product, actual))
 
-        tensor_square = torch.eye(3, dtype=int).repeat(5, 1, 1)
+        tensor_square = torch.eye(3, dtype=float).repeat(5, 1, 1)
         product = zero._matmul(tensor_square)
         self.assertTrue(approx_equal(product, actual))
         self.assertEqual(product.dtype, tensor_square.dtype)
 
         tensor_square = torch.eye(4).repeat(5, 1, 1)
         actual = torch.zeros(5, 3, 4)
         product = zero._t_matmul(tensor_square)
```

### Comparing `linear_operator-0.4.0/test/test_settings.py` & `linear_operator-0.5.0/test/test_settings.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_cholesky.py` & `linear_operator-0.5.0/test/utils/test_cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_generic.py` & `linear_operator-0.5.0/test/utils/test_generic.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_getitem.py` & `linear_operator-0.5.0/test/utils/test_getitem.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_interpolation.py` & `linear_operator-0.5.0/test/utils/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_lanczos.py` & `linear_operator-0.5.0/test/utils/test_lanczos.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_linear_cg.py` & `linear_operator-0.5.0/test/utils/test_linear_cg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python3
 
 import os
 import random
 import unittest
+import warnings
 
 import torch
 
 from linear_operator.utils.linear_cg import linear_cg
+from linear_operator.utils.warnings import NumericalWarning
 
 
 class TestLinearCG(unittest.TestCase):
     def setUp(self):
         if os.getenv("UNLOCK_SEED") is None or os.getenv("UNLOCK_SEED").lower() == "false":
             self.rng_state = torch.get_rng_state()
             torch.manual_seed(0)
@@ -65,23 +67,25 @@
         size = 10
         matrix = torch.randn(size, size, dtype=torch.float64)
         matrix = matrix.matmul(matrix.mT)
         matrix.div_(matrix.norm())
         matrix.add_(torch.eye(matrix.size(-1), dtype=torch.float64).mul_(1e-1))
 
         rhs = torch.randn(size, 50, dtype=torch.float64)
-        solves, t_mats = linear_cg(
-            matrix.matmul,
-            rhs=rhs,
-            n_tridiag=5,
-            max_tridiag_iter=10,
-            max_iter=size,
-            tolerance=0,
-            eps=1e-15,
-        )
+        with warnings.catch_warnings(record=True) as ws:
+            solves, t_mats = linear_cg(
+                matrix.matmul,
+                rhs=rhs,
+                n_tridiag=5,
+                max_tridiag_iter=10,
+                max_iter=size,
+                tolerance=0,
+                eps=1e-15,
+            )
+            self.assertTrue(any(issubclass(w.category, NumericalWarning) for w in ws))
 
         # Check cg
         matrix_chol = torch.linalg.cholesky(matrix)
         actual = torch.cholesky_solve(rhs, matrix_chol)
         self.assertTrue(torch.allclose(solves, actual, atol=1e-3, rtol=1e-4))
 
         # Check tridiag
@@ -111,23 +115,25 @@
         size = 10
         matrix = torch.randn(batch, size, size, dtype=torch.float64)
         matrix = matrix.matmul(matrix.mT)
         matrix.div_(matrix.norm())
         matrix.add_(torch.eye(matrix.size(-1), dtype=torch.float64).mul_(1e-1))
 
         rhs = torch.randn(batch, size, 10, dtype=torch.float64)
-        solves, t_mats = linear_cg(
-            matrix.matmul,
-            rhs=rhs,
-            n_tridiag=8,
-            max_iter=size,
-            max_tridiag_iter=10,
-            tolerance=0,
-            eps=1e-30,
-        )
+        with warnings.catch_warnings(record=True) as ws:
+            solves, t_mats = linear_cg(
+                matrix.matmul,
+                rhs=rhs,
+                n_tridiag=8,
+                max_iter=size,
+                max_tridiag_iter=10,
+                tolerance=0,
+                eps=1e-30,
+            )
+            self.assertTrue(any(issubclass(w.category, NumericalWarning) for w in ws))
 
         # Check cg
         matrix_chol = torch.linalg.cholesky(matrix)
         actual = torch.cholesky_solve(rhs, matrix_chol)
         self.assertTrue(torch.allclose(solves, actual, atol=1e-3, rtol=1e-4))
 
         # Check tridiag
```

### Comparing `linear_operator-0.4.0/test/utils/test_minres.py` & `linear_operator-0.5.0/test/utils/test_minres.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_permutation.py` & `linear_operator-0.5.0/test/utils/test_permutation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_sparse.py` & `linear_operator-0.5.0/test/utils/test_sparse.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.4.0/test/utils/test_toeplitz.py` & `linear_operator-0.5.0/test/utils/test_toeplitz.py`

 * *Files identical despite different names*

