# Comparing `tmp/pyperformance-1.0.7.tar.gz` & `tmp/pyperformance-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperformance-1.0.7.tar", last modified: Sun Apr 23 06:21:09 2023, max compression
+gzip compressed data, was "pyperformance-1.0.8.tar", last modified: Fri Jun  2 11:47:16 2023, max compression
```

## Comparing `pyperformance-1.0.7.tar` & `pyperformance-1.0.8.tar`

### file list

```diff
@@ -1,539 +1,556 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.877154 pyperformance-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-23 06:20:54.000000 pyperformance-1.0.7/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-23 06:20:54.000000 pyperformance-1.0.7/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-23 06:20:54.000000 pyperformance-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-23 06:21:09.877154 pyperformance-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-23 06:20:54.000000 pyperformance-1.0.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/TODO.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.801153 pyperformance-1.0.7/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_2to3/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_2to3/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_async_generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_async_generators/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_async_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_async_tree/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_asyncio_tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_asyncio_tcp/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_chameleon/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_chameleon/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_chaos/
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_chaos/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_comprehensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_comprehensions/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_concurrent_imap/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_concurrent_imap/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_coroutines/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_coroutines/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_coverage/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_crypto_pyaes/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_crypto_pyaes/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_dask/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_deepcopy/
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_deepcopy/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_deltablue/
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_deltablue/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_django_template/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_django_template/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_docutils/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_docutils/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_dulwich_log/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_dulwich_log/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_fannkuch/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_fannkuch/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_float/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_float/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_gc_collect/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_gc_collect/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_gc_traversal/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_gc_traversal/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_generators/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_genshi/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_genshi/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_go/
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_go/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_hexiom/
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_hexiom/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_hg_startup/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_hg_startup/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_html5lib/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_html5lib/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_json_dumps/
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_json_dumps/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_json_loads/
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_json_loads/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_logging/
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_logging/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_mako/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_mako/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_mdp/
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_mdp/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_meteor_contest/
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_meteor_contest/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_nbody/
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_nbody/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_nqueens/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_nqueens/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pathlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pathlib/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pickle/
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pickle/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pidigits/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pidigits/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pprint/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pprint/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pyflate/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pyflate/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_python_startup/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_python_startup/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_raytrace/
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_raytrace/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_regex_compile/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_compile/bm_regex_effbot.py
--rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_compile/bm_regex_v8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_compile/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_regex_dna/
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_dna/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_regex_effbot/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_effbot/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_regex_v8/
--rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_v8/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_richards/
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_richards/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_scimark/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_scimark/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_spectral_norm/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_spectral_norm/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sqlalchemy_declarative/
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sqlalchemy_imperative/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sqlglot/
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sqlglot/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sqlite_synth/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sqlite_synth/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sympy/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sympy/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_telco/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_telco/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_tomli_loads/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_tomli_loads/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_tomli_loads/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_tornado_http/
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_tornado_http/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_unpack_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_unpack_sequence/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_xml_etree/
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_xml_etree/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    20221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/benchmarks.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/cpython_results_2017.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/custom_benchmarks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/images/bm_chaos.png
--rw-r--r--   0 runner    (1001) docker     (123)    55274 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/images/bm_raytrace.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    48901 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/images/html5lib.png
--rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/images/sympy_sum.png
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_benchmark_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_benchmark_selections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_pyproject_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_pythoninfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/compile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/data-files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/MANIFEST
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.801153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/__init__.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/signals.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/template_loader.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15786 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_generators/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed.toml
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization.toml
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/bm_asyncio_tcp_ssl.toml
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chaos/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chaos/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_comprehensions/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_comprehensions/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_concurrent_imap/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_concurrent_imap/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coroutines/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coroutines/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deepcopy/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deepcopy/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deltablue/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deltablue/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.801153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16986 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/
--rw-r--r--   0 runner    (1001) docker     (123)   113263 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35463 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt
--rw-r--r--   0 runner    (1001) docker     (123)    98603 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36399 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32543 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/
--rw-r--r--   0 runner    (1001) docker     (123)   132076 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt
--rw-r--r--   0 runner    (1001) docker     (123)    51188 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt
--rw-r--r--   0 runner    (1001) docker     (123)   117454 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/
--rw-r--r--   0 runner    (1001) docker     (123)    64502 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.837154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-black.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-white.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/default.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/happy_monkey.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-black.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-white.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-all.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-breaks.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-covers.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-cuts.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-empty.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-objects.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-black.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-white.png
--rw-r--r--   0 runner    (1001) docker     (123)    62611 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt
--rw-r--r--   0 runner    (1001) docker     (123)    38313 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.837154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.837154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap-scaling.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-scaling.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.swf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/pens.mp4
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title-scaling.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.837154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.801153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/ORIG_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/config
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/exclude
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/bind_modules
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/master
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/zero_timeout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/packs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/
--rw-r--r--   0 runner    (1001) docker     (123)   247416 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx
--rw-r--r--   0 runner    (1001) docker     (123)  1774473 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_fannkuch/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_fannkuch/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_float/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_float/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_collect/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_collect/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_traversal/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_traversal/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_generators/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_go/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_go/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hexiom/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hexiom/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/data/
--rw-r--r--   0 runner    (1001) docker     (123)   133837 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_dumps/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_dumps/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_loads/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_loads/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_logging/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_logging/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mdp/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mdp/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_meteor_contest/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_meteor_contest/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nbody/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nbody/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nqueens/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nqueens/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pathlib/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pathlib/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_dict.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_list.toml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_pure_python.toml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_list.toml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_pure_python.toml
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pidigits/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pidigits/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pprint/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pprint/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/data/
--rw-r--r--   0 runner    (1001) docker     (123)    67562 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/bm_python_startup_no_site.toml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_raytrace/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_raytrace/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py
--rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_dna/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_dna/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_effbot/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_effbot/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_v8/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_v8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_richards/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_richards/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_scimark/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_scimark/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_spectral_norm/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_spectral_norm/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlite_synth/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlite_synth/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/data/
--rw-r--r--   0 runner    (1001) docker     (123)   160000 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/data/
--rw-r--r--   0 runner    (1001) docker     (123) 16824157 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.873154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.877154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_unpack_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_unpack_sequence/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.877154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_xml_etree/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_xml_etree/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/venv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 06:20:55.000000 pyperformance-1.0.7/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-23 06:20:55.000000 pyperformance-1.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 06:21:09.877154 pyperformance-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.674830 pyperformance-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-02 11:46:55.000000 pyperformance-1.0.8/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-02 11:46:55.000000 pyperformance-1.0.8/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 11:46:55.000000 pyperformance-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-02 11:47:16.674830 pyperformance-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-02 11:46:55.000000 pyperformance-1.0.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/TODO.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.542829 pyperformance-1.0.8/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_2to3/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_async_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_async_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_async_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_async_tree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_asyncio_tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_asyncio_tcp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_chameleon/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_chameleon/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_chaos/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_comprehensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_comprehensions/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_concurrent_imap/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_concurrent_imap/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_coroutines/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_coroutines/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_coverage/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_crypto_pyaes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_crypto_pyaes/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_dask/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_deepcopy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_deepcopy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_deltablue/
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_deltablue/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_django_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_django_template/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_docutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_docutils/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_dulwich_log/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_dulwich_log/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_fannkuch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_fannkuch/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_float/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_float/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_gc_collect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_gc_collect/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_gc_traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_gc_traversal/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_genshi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_genshi/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.558829 pyperformance-1.0.8/benchmarks/bm_go/
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_go/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_hexiom/
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_hexiom/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_hg_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_hg_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_html5lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_html5lib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_json_dumps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_json_dumps/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_json_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_json_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_logging/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_mako/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_mako/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_mdp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_mdp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_meteor_contest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_meteor_contest/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_nbody/
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_nbody/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_nqueens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_nqueens/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pathlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pathlib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pickle/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pidigits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pidigits/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pprint/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_pyflate/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_pyflate/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_python_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_python_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.562829 pyperformance-1.0.8/benchmarks/bm_raytrace/
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_raytrace/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_regex_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_compile/bm_regex_effbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_compile/bm_regex_v8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_compile/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_regex_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_dna/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_regex_effbot/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_effbot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_regex_v8/
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_regex_v8/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_richards/
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_richards/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_richards_super/
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_richards_super/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_scimark/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_scimark/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_spectral_norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_spectral_norm/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sqlalchemy_declarative/
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sqlalchemy_imperative/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sqlglot/
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sqlglot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sqlite_synth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sqlite_synth/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.570829 pyperformance-1.0.8/benchmarks/bm_sympy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_sympy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_telco/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_telco/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_tomli_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_tomli_loads/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_tomli_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_tornado_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_tornado_http/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_typing_runtime_protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_typing_runtime_protocols/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_unpack_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_unpack_sequence/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/benchmarks/bm_xml_etree/
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-02 11:46:55.000000 pyperformance-1.0.8/benchmarks/bm_xml_etree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.574829 pyperformance-1.0.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20403 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/cpython_results_2017.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/custom_benchmarks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.578829 pyperformance-1.0.8/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/images/bm_chaos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55274 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/images/bm_raytrace.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    48901 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/images/html5lib.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/images/sympy_sum.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-06-02 11:46:55.000000 pyperformance-1.0.8/doc/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.582829 pyperformance-1.0.8/pyperformance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_benchmark_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_benchmark_selections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_pyproject_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_pythoninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.542829 pyperformance-1.0.8/pyperformance/data-files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.582829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/MANIFEST
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.582829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.542829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.586829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/__init__.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/signals.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/template_loader.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15786 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.586829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_generators/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.586829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_cpu_io_mixed.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_io.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_memoization.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.586829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/bm_asyncio_tcp_ssl.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_key.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chaos/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_comprehensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_comprehensions/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_concurrent_imap/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_concurrent_imap/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coroutines/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coroutines/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.590829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deepcopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deepcopy/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deltablue/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deltablue/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.546829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.594829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.598830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16986 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.598830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)   113263 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35463 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    98603 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.598830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.598830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36399 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32543 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.602830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/
+-rw-r--r--   0 runner    (1001) docker     (123)   132076 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.602830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    51188 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   117454 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.606830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    64502 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.606830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/default.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/happy_monkey.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-all.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-breaks.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-covers.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-cuts.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62611 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38313 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.606830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.610830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.swf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/pens.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.610830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.546829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.610830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/ORIG_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/config
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/exclude
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.546829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.546829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/bind_modules
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/master
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/zero_timeout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.550829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/packs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.614830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/
+-rw-r--r--   0 runner    (1001) docker     (123)   247416 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx
+-rw-r--r--   0 runner    (1001) docker     (123)  1774473 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.550829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.550829 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_fannkuch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_fannkuch/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_float/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_float/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_collect/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_collect/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.618830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_traversal/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_generators/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_go/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_go/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hexiom/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hexiom/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.622830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   133837 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_dumps/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_dumps/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_loads/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_logging/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mdp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_meteor_contest/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_meteor_contest/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.626830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nbody/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nbody/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nqueens/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nqueens/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pathlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pathlib/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_dict.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_list.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_pure_python.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_list.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_pure_python.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pidigits/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pidigits/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pprint/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.630830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    67562 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.634830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/bm_python_startup_no_site.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.634830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_raytrace/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_raytrace/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.638830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.638830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_dna/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_effbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_effbot/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_v8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards_super/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards_super/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards_super/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_scimark/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_scimark/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_spectral_norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_spectral_norm/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.642830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlite_synth/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlite_synth/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   160000 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.646830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 16824157 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.670830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.670830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.674830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_unpack_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_unpack_sequence/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.674830 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_xml_etree/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_xml_etree/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.674830 pyperformance-1.0.8/pyperformance/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyperformance/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:47:16.582829 pyperformance-1.0.8/pyperformance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 11:47:16.000000 pyperformance-1.0.8/pyperformance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-02 11:46:55.000000 pyperformance-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-02 11:46:55.000000 pyperformance-1.0.8/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-02 11:46:55.000000 pyperformance-1.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:47:16.674830 pyperformance-1.0.8/setup.cfg
```

### Comparing `pyperformance-1.0.7/AUTHORS` & `pyperformance-1.0.8/AUTHORS`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/COPYING` & `pyperformance-1.0.8/COPYING`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/MANIFEST.in` & `pyperformance-1.0.8/MANIFEST.in`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 include requirements.in
 include requirements.txt
 
 include doc/*.rst doc/images/*.png doc/images/*.jpg
 include doc/conf.py doc/Makefile doc/make.bat
 
 include pyperformance/*.py
-include pyperformance/data-files/requirements.txt
+include pyperformance/requirements/requirements.txt
 include pyperformance/data-files/benchmarks/MANIFEST
 include pyperformance/data-files/benchmarks/bm_*/*.toml
 include pyperformance/data-files/benchmarks/bm_*/*.py
 include pyperformance/data-files/benchmarks/bm_*/requirements.txt
+include pyperformance/data-files/benchmarks/bm_*/*.pem
 recursive-include pyperformance/data-files/benchmarks/bm_*/data *
 recursive-exclude pyperformance/tests *
```

### Comparing `pyperformance-1.0.7/PKG-INFO` & `pyperformance-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperformance
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python benchmark suite
 Author: Collin Winter, Jeffrey Yasskin
 License: MIT
 Project-URL: Homepage, https://github.com/python/pyperformance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyperformance-1.0.7/README.rst` & `pyperformance-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/TODO.rst` & `pyperformance-1.0.8/TODO.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_async_generators/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_async_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_async_tree/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_async_tree/run_benchmark.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 Benchmark for async tree workload, which calls asyncio.gather() on a tree
 (6 levels deep, 6 branches per level) with the leaf nodes simulating some
 (potentially) async work (depending on the benchmark variant). Benchmark
 variants include:
 
 1) "none": No actual async work in the async tree.
 2) "io": All leaf nodes simulate async IO workload (async sleep 50ms).
-3) "memoization": All leaf nodes simulate async IO workload with 90% of 
+3) "memoization": All leaf nodes simulate async IO workload with 90% of
                   the data memoized
-4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and 
-                   the other half simulate the same workload as the 
+4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and
+                   the other half simulate the same workload as the
                    "memoization" variant.
+
+All variants also have an "eager" flavor that uses
+the asyncio eager task factory (if available).
 """
 
 
 import asyncio
 import math
 import random
 
@@ -53,24 +56,40 @@
             *[self.recurse(recurse_level - 1) for _ in range(NUM_RECURSE_BRANCHES)]
         )
 
     async def run(self):
         await self.recurse(NUM_RECURSE_LEVELS)
 
 
+class EagerMixin:
+    async def run(self):
+        loop = asyncio.get_running_loop()
+        if hasattr(asyncio, 'eager_task_factory'):
+            loop.set_task_factory(asyncio.eager_task_factory)
+        return await super().run()
+
+
 class NoneAsyncTree(AsyncTree):
     async def workload_func(self):
         return
 
 
+class EagerAsyncTree(EagerMixin, NoneAsyncTree):
+    pass
+
+
 class IOAsyncTree(AsyncTree):
     async def workload_func(self):
         await self.mock_io_call()
 
 
+class EagerIOAsyncTree(EagerMixin, IOAsyncTree):
+    pass
+
+
 class MemoizationAsyncTree(AsyncTree):
     async def workload_func(self):
         # deterministic random, seed set in AsyncTree.__init__()
         data = random.randint(1, 100)
 
         if data <= MEMOIZABLE_PERCENTAGE:
             if self.cache.get(data):
@@ -78,24 +97,32 @@
 
             self.cache[data] = True
 
         await self.mock_io_call()
         return data
 
 
+class EagerMemoizationAsyncTree(EagerMixin, MemoizationAsyncTree):
+    pass
+
+
 class CpuIoMixedAsyncTree(MemoizationAsyncTree):
     async def workload_func(self):
         # deterministic random, seed set in AsyncTree.__init__()
         if random.random() < CPU_PROBABILITY:
             # mock cpu-bound call
             return math.factorial(FACTORIAL_N)
         else:
             return await MemoizationAsyncTree.workload_func(self)
 
 
+class EagerCpuIoMixedAsyncTree(EagerMixin, CpuIoMixedAsyncTree):
+    pass
+
+
 def add_metadata(runner):
     runner.metadata["description"] = "Async tree workloads."
     runner.metadata["async_tree_recurse_levels"] = NUM_RECURSE_LEVELS
     runner.metadata["async_tree_recurse_branches"] = NUM_RECURSE_BRANCHES
     runner.metadata["async_tree_random_seed"] = RANDOM_SEED
     runner.metadata["async_tree_io_sleep_time"] = IO_SLEEP_TIME
     runner.metadata["async_tree_memoizable_percentage"] = MEMOIZABLE_PERCENTAGE
@@ -111,35 +138,38 @@
     parser.add_argument(
         "benchmark",
         choices=BENCHMARKS,
         help="""\
 Determines which benchmark to run. Options:
 1) "none": No actual async work in the async tree.
 2) "io": All leaf nodes simulate async IO workload (async sleep 50ms).
-3) "memoization": All leaf nodes simulate async IO workload with 90% of 
+3) "memoization": All leaf nodes simulate async IO workload with 90% of
                   the data memoized
-4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and 
-                   the other half simulate the same workload as the 
+4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and
+                   the other half simulate the same workload as the
                    "memoization" variant.
 """,
     )
 
 
 BENCHMARKS = {
     "none": NoneAsyncTree,
+    "eager": EagerAsyncTree,
     "io": IOAsyncTree,
+    "eager_io": EagerIOAsyncTree,
     "memoization": MemoizationAsyncTree,
+    "eager_memoization": EagerMemoizationAsyncTree,
     "cpu_io_mixed": CpuIoMixedAsyncTree,
+    "eager_cpu_io_mixed": EagerCpuIoMixedAsyncTree,
 }
 
 
 if __name__ == "__main__":
     runner = pyperf.Runner(add_cmdline_args=add_cmdline_args)
     add_metadata(runner)
     add_parser_args(runner.argparser)
     args = runner.parse_args()
     benchmark = args.benchmark
 
     async_tree_class = BENCHMARKS[benchmark]
     async_tree = async_tree_class()
     runner.bench_async_func(f"async_tree_{benchmark}", async_tree.run)
-
```

### Comparing `pyperformance-1.0.7/benchmarks/bm_asyncio_tcp/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_asyncio_tcp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_chameleon/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_chameleon/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_chaos/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_chaos/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_comprehensions/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_comprehensions/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_concurrent_imap/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_concurrent_imap/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_coroutines/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_coroutines/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_coverage/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_coverage/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_crypto_pyaes/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_crypto_pyaes/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_dask/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_dask/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_deepcopy/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_deepcopy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_deltablue/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_deltablue/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_django_template/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_django_template/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_docutils/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_docutils/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_dulwich_log/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_dulwich_log/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_fannkuch/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_fannkuch/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_float/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_float/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_gc_collect/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_gc_collect/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_gc_traversal/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_gc_traversal/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_generators/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_genshi/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_genshi/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_go/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_go/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_hexiom/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_hexiom/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_hg_startup/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_hg_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_html5lib/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_html5lib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_json_dumps/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_json_dumps/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_json_loads/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_json_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_logging/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_logging/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_mako/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_mako/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_mdp/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_mdp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_meteor_contest/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_meteor_contest/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_nbody/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_nbody/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_nqueens/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_nqueens/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_pathlib/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_pathlib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_pickle/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_pickle/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_pidigits/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_pidigits/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_pprint/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_pprint/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_pyflate/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_pyflate/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_python_startup/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_python_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_raytrace/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_raytrace/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_regex_compile/bm_regex_effbot.py` & `pyperformance-1.0.8/benchmarks/bm_regex_compile/bm_regex_effbot.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_regex_compile/bm_regex_v8.py` & `pyperformance-1.0.8/benchmarks/bm_regex_compile/bm_regex_v8.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_regex_compile/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_regex_compile/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_regex_dna/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_regex_dna/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_regex_effbot/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_regex_effbot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_regex_v8/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_regex_v8/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_richards/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_richards/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_scimark/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_scimark/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_spectral_norm/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_spectral_norm/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_sqlglot/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_sqlglot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_sqlite_synth/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_sqlite_synth/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_sympy/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_sympy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_telco/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_telco/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_tomli_loads/generate_data.py` & `pyperformance-1.0.8/benchmarks/bm_tomli_loads/generate_data.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_tomli_loads/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_tomli_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_tornado_http/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_tornado_http/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_unpack_sequence/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_unpack_sequence/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/benchmarks/bm_xml_etree/run_benchmark.py` & `pyperformance-1.0.8/benchmarks/bm_xml_etree/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/Makefile` & `pyperformance-1.0.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/benchmarks.rst` & `pyperformance-1.0.8/doc/benchmarks.rst`

 * *Files 2% similar despite different names*

```diff
@@ -62,20 +62,23 @@
 
 Async workload benchmark, which calls ``asyncio.gather()`` on a tree (6 levels deep,
 6 branches per level) with the leaf nodes simulating some [potentially] async work
 (depending on the benchmark variant). Available variants:
 
 * ``async_tree``: no actual async work at any leaf node.
 * ``async_tree_io``: all leaf nodes simulate async IO workload (async sleep 50ms).
-* ``async_tree_memoization``: all leaf nodes simulate async IO workload with 90% of 
+* ``async_tree_memoization``: all leaf nodes simulate async IO workload with 90% of
   the data memoized.
 * ``async_tree_cpu_io_mixed``: half of the leaf nodes simulate CPU-bound workload
-  (``math.factorial(500)``) and the other half simulate the same workload as the 
+  (``math.factorial(500)``) and the other half simulate the same workload as the
   ``async_tree_memoization`` variant.
 
+These benchmarks also have an "eager" flavor that uses asyncio eager task factory,
+if available.
+
 
 chameleon
 ---------
 
 Render a template using the ``chameleon`` module to create an HTML table of 500
 lignes and 10 columns.
```

### Comparing `pyperformance-1.0.7/doc/changelog.rst` & `pyperformance-1.0.8/doc/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 Changelog
 =========
 
+Version 1.0.8 (2023-06-02)
+-------------
+
+* Move the main requirements.txt file to pyperformance/requirements
+  so that dependabot can only run on that one file
+* Update dependencies of benchmarks not to specify setuptools
+* On older versions of Python, skip benchmarks that use features
+  introduced in newer Python versions
+* Support ``--inherit-environ`` when reusing a venv
+* Use tomllib/tomli over toml
+* Update MANIFEST.in to include cert files for asyncio_tcp_ssl benchmark
+* Fix undefined variable issue when raising VenvPipInstallFailedError
+* Add mypy config; run mypy in CI
+* Fix typo of str.partition from _pyproject_toml.py
+* Add  version of Richards benchmark that uses super()
+* Add a benchmark for runtime-checkable protocols
+* Extend async tree benchmarks to cover eager task execution
+
 Version 1.0.7 (2023-04-22)
 -------------
 
 * Upgrade pyperf from 2.5.0 to 2.6.0
 * Clean unused imports and other small code details
 * Migrage to the pyproject.toml based project
 * Fix the django_template benchmark due to lack of distutils
```

### Comparing `pyperformance-1.0.7/doc/conf.py` & `pyperformance-1.0.8/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/cpython_results_2017.rst` & `pyperformance-1.0.8/doc/cpython_results_2017.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/custom_benchmarks.rst` & `pyperformance-1.0.8/doc/custom_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/images/bm_chaos.png` & `pyperformance-1.0.8/doc/images/bm_chaos.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/images/bm_raytrace.jpg` & `pyperformance-1.0.8/doc/images/bm_raytrace.jpg`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/images/html5lib.png` & `pyperformance-1.0.8/doc/images/html5lib.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/images/sympy_sum.png` & `pyperformance-1.0.8/doc/images/sympy_sum.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/index.rst` & `pyperformance-1.0.8/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/make.bat` & `pyperformance-1.0.8/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/doc/usage.rst` & `pyperformance-1.0.8/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/__init__.py` & `pyperformance-1.0.8/pyperformance/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 import sys
 
 
-VERSION = (1, 0, 7)
+VERSION = (1, 0, 8)
 __version__ = '.'.join(map(str, VERSION))
 
 
 PKG_ROOT = os.path.dirname(__file__)
 DATA_DIR = os.path.join(PKG_ROOT, 'data-files')
 
 
@@ -30,17 +30,17 @@
 
 
 def _is_devel_install():
     # pip install -e <path-to-git-checkout> will do a "devel" install.
     # This means it creates a link back to the checkout instead
     # of copying the files.
     try:
-        import toml
+        import packaging
     except ModuleNotFoundError:
         return False
-    sitepackages = os.path.dirname(os.path.dirname(toml.__file__))
+    sitepackages = os.path.dirname(os.path.dirname(packaging.__file__))
     if os.path.isdir(os.path.join(sitepackages, 'pyperformance')):
         return False
     if not os.path.exists(os.path.join(sitepackages, 'pyperformance.egg-link')):
         # XXX Check the contents?
         return False
     return True
```

### Comparing `pyperformance-1.0.7/pyperformance/_benchmark.py` & `pyperformance-1.0.8/pyperformance/_benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from collections import namedtuple
 import os
 import os.path
 import sys
 
 import pyperf
+from packaging.specifiers import SpecifierSet
 
 from . import _utils, _benchmark_metadata
 
 
 def check_name(name):
     _utils.check_name('_' + name)
 
@@ -160,29 +161,32 @@
     def runscript(self):
         return self._get_metadata_value('runscript', None)
 
     @property
     def extra_opts(self):
         return self._get_metadata_value('extra_opts', ())
 
+    @property
+    def python(self):
+        return SpecifierSet(self._get_metadata_value("python", ""))
+
     # Other metadata keys:
     # * base
-    # * python
     # * dependencies
     # * requirements
 
     def run(self, python, runid=None, pyperf_opts=None, *,
             venv=None,
             verbose=False,
             ):
         if venv and python == sys.executable:
             python = venv.python
 
         if not runid:
-            from ..run import get_run_id
+            from .run import get_run_id
             runid = get_run_id(python, self)
 
         runscript = self.runscript
         bench = _run_perf_script(
             python,
             runscript,
             runid,
```

### Comparing `pyperformance-1.0.7/pyperformance/_benchmark_metadata.py` & `pyperformance-1.0.8/pyperformance/_benchmark_metadata.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/_benchmark_selections.py` & `pyperformance-1.0.8/pyperformance/_benchmark_selections.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/_manifest.py` & `pyperformance-1.0.8/pyperformance/_manifest.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/_pip.py` & `pyperformance-1.0.8/pyperformance/_pip.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/_pyproject_toml.py` & `pyperformance-1.0.8/pyperformance/_pyproject_toml.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 import re
 import urllib.parse
 
 import packaging.requirements
 import packaging.specifiers
 import packaging.utils
 import packaging.version
-import toml
+
+try:
+    import tomllib  # type: ignore[import] # tomllib doesn't exist on 3.7-3.10
+except ImportError:
+    import tomli as tomllib
 
 from ._utils import check_name
 
 
 NAME_RE = re.compile('^([A-Z0-9]|[A-Z0-9][A-Z0-9._-]*[A-Z0-9])$', re.IGNORECASE)
 
 
@@ -36,27 +40,27 @@
     return text
 
 
 def parse_entry_point(text):
     # See:
     #  * https://packaging.python.org/specifications/entry-points/#data-model
     #  * https://www.python.org/dev/peps/pep-0517/#source-trees
-    module, sep, qualname = text.parition(':')
+    module, sep, qualname = text.partition(':')
     if all(p.isidentifier() for p in module.split('.')):
         if not sep or all(p.isidentifier() for p in qualname.split('.')):
             return module, qualname
 
     raise ValueError(f'invalid entry point {text!r}')
 
 
 def parse_pyproject_toml(text, rootdir, name=None, *,
                          tools=None,
                          requirefiles=True,
                          ):
-    data = toml.loads(text)
+    data = tomllib.loads(text)
     unused = list(data)
 
     for section, normalize in SECTIONS.items():
         try:
             secdata = data[section]
         except KeyError:
             data[section] = None
```

### Comparing `pyperformance-1.0.7/pyperformance/_python.py` & `pyperformance-1.0.8/pyperformance/_python.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/_pythoninfo.py` & `pyperformance-1.0.8/pyperformance/_pythoninfo.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/_utils.py` & `pyperformance-1.0.8/pyperformance/_utils.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/_venv.py` & `pyperformance-1.0.8/pyperformance/_venv.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,17 +211,17 @@
             self.python,
             info=self.info,
             downloaddir=downloaddir or self.root,
             env=self._env,
             upgrade=upgrade,
         )
         if ec != 0:
-            raise VenvPipInstallFailedError(root, ec)
+            raise VenvPipInstallFailedError(self.root, ec)
         elif not _pip.is_pip_installed(self.python, env=self._env):
-            raise VenvPipInstallFailedError(root, 0, "pip doesn't work")
+            raise VenvPipInstallFailedError(self.root, 0, "pip doesn't work")
 
         if installer:
             # Upgrade installer dependencies (setuptools, ...)
             ec, _, _ = _pip.ensure_installer(
                 self.python,
                 env=self._env,
                 upgrade=True,
```

### Comparing `pyperformance-1.0.7/pyperformance/cli.py` & `pyperformance-1.0.8/pyperformance/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,19 +237,23 @@
             continue
         name = parsed.name if kind == 'benchmark' else parsed
         if name in manifest.groups and op == '-':
             raise ValueError(f'negative groups not supported: -{parsed.name}')
 
     # Get the selections.
     selected = []
+    this_python_version = ".".join(map(str, sys.version_info[:3]))
     for bench in _benchmark_selections.iter_selections(manifest, parsed_infos):
         if isinstance(bench, str):
             logging.warning(f"no benchmark named {bench!r}")
             continue
-        selected.append(bench)
+        # Filter out any benchmarks that can't be run on the Python version we're running
+        if this_python_version in bench.python:
+            selected.append(bench)
+
     return selected
 
 
 def _main():
     if not is_installed():
         # Always require a local checkout to be installed.
         print('ERROR: pyperformance should not be run without installing first')
```

### Comparing `pyperformance-1.0.7/pyperformance/commands.py` & `pyperformance-1.0.8/pyperformance/commands.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/compare.py` & `pyperformance-1.0.8/pyperformance/compare.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/compile.py` & `pyperformance-1.0.8/pyperformance/compile.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/MANIFEST` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/MANIFEST`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 name	metafile
 2to3	<local>
 async_generators	<local>
 async_tree	<local>
 async_tree_cpu_io_mixed	<local:async_tree>
 async_tree_io	<local:async_tree>
 async_tree_memoization	<local:async_tree>
+async_tree_eager	<local:async_tree>
+async_tree_eager_cpu_io_mixed	<local:async_tree>
+async_tree_eager_io	<local:async_tree>
+async_tree_eager_memoization	<local:async_tree>
 asyncio_tcp	<local>
 asyncio_tcp_ssl	<local:asyncio_tcp>
 concurrent_imap	<local>
 coroutines	<local>
 coverage	<local>
 gc_traversal	<local>
 gc_collect	<local>
@@ -54,24 +58,26 @@
 python_startup_no_site	<local:python_startup>
 raytrace	<local>
 regex_compile	<local>
 regex_dna	<local>
 regex_effbot	<local>
 regex_v8	<local>
 richards	<local>
+richards_super	<local>
 scimark	<local>
 spectral_norm	<local>
 sqlalchemy_declarative	<local>
 sqlalchemy_imperative	<local>
 sqlglot	<local>
 sqlite_synth	<local>
 sympy	<local>
 telco	<local>
 tomli_loads	<local>
 tornado_http	<local>
+typing_runtime_protocols	<local>
 unpack_sequence	<local>
 unpickle	<local:pickle>
 unpickle_list	<local:pickle>
 unpickle_pure_python	<local:pickle>
 xml_etree	<local>
```

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 Benchmark for async tree workload, which calls asyncio.gather() on a tree
 (6 levels deep, 6 branches per level) with the leaf nodes simulating some
 (potentially) async work (depending on the benchmark variant). Benchmark
 variants include:
 
 1) "none": No actual async work in the async tree.
 2) "io": All leaf nodes simulate async IO workload (async sleep 50ms).
-3) "memoization": All leaf nodes simulate async IO workload with 90% of 
+3) "memoization": All leaf nodes simulate async IO workload with 90% of
                   the data memoized
-4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and 
-                   the other half simulate the same workload as the 
+4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and
+                   the other half simulate the same workload as the
                    "memoization" variant.
+
+All variants also have an "eager" flavor that uses
+the asyncio eager task factory (if available).
 """
 
 
 import asyncio
 import math
 import random
 
@@ -53,24 +56,40 @@
             *[self.recurse(recurse_level - 1) for _ in range(NUM_RECURSE_BRANCHES)]
         )
 
     async def run(self):
         await self.recurse(NUM_RECURSE_LEVELS)
 
 
+class EagerMixin:
+    async def run(self):
+        loop = asyncio.get_running_loop()
+        if hasattr(asyncio, 'eager_task_factory'):
+            loop.set_task_factory(asyncio.eager_task_factory)
+        return await super().run()
+
+
 class NoneAsyncTree(AsyncTree):
     async def workload_func(self):
         return
 
 
+class EagerAsyncTree(EagerMixin, NoneAsyncTree):
+    pass
+
+
 class IOAsyncTree(AsyncTree):
     async def workload_func(self):
         await self.mock_io_call()
 
 
+class EagerIOAsyncTree(EagerMixin, IOAsyncTree):
+    pass
+
+
 class MemoizationAsyncTree(AsyncTree):
     async def workload_func(self):
         # deterministic random, seed set in AsyncTree.__init__()
         data = random.randint(1, 100)
 
         if data <= MEMOIZABLE_PERCENTAGE:
             if self.cache.get(data):
@@ -78,24 +97,32 @@
 
             self.cache[data] = True
 
         await self.mock_io_call()
         return data
 
 
+class EagerMemoizationAsyncTree(EagerMixin, MemoizationAsyncTree):
+    pass
+
+
 class CpuIoMixedAsyncTree(MemoizationAsyncTree):
     async def workload_func(self):
         # deterministic random, seed set in AsyncTree.__init__()
         if random.random() < CPU_PROBABILITY:
             # mock cpu-bound call
             return math.factorial(FACTORIAL_N)
         else:
             return await MemoizationAsyncTree.workload_func(self)
 
 
+class EagerCpuIoMixedAsyncTree(EagerMixin, CpuIoMixedAsyncTree):
+    pass
+
+
 def add_metadata(runner):
     runner.metadata["description"] = "Async tree workloads."
     runner.metadata["async_tree_recurse_levels"] = NUM_RECURSE_LEVELS
     runner.metadata["async_tree_recurse_branches"] = NUM_RECURSE_BRANCHES
     runner.metadata["async_tree_random_seed"] = RANDOM_SEED
     runner.metadata["async_tree_io_sleep_time"] = IO_SLEEP_TIME
     runner.metadata["async_tree_memoizable_percentage"] = MEMOIZABLE_PERCENTAGE
@@ -111,35 +138,38 @@
     parser.add_argument(
         "benchmark",
         choices=BENCHMARKS,
         help="""\
 Determines which benchmark to run. Options:
 1) "none": No actual async work in the async tree.
 2) "io": All leaf nodes simulate async IO workload (async sleep 50ms).
-3) "memoization": All leaf nodes simulate async IO workload with 90% of 
+3) "memoization": All leaf nodes simulate async IO workload with 90% of
                   the data memoized
-4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and 
-                   the other half simulate the same workload as the 
+4) "cpu_io_mixed": Half of the leaf nodes simulate CPU-bound workload and
+                   the other half simulate the same workload as the
                    "memoization" variant.
 """,
     )
 
 
 BENCHMARKS = {
     "none": NoneAsyncTree,
+    "eager": EagerAsyncTree,
     "io": IOAsyncTree,
+    "eager_io": EagerIOAsyncTree,
     "memoization": MemoizationAsyncTree,
+    "eager_memoization": EagerMemoizationAsyncTree,
     "cpu_io_mixed": CpuIoMixedAsyncTree,
+    "eager_cpu_io_mixed": EagerCpuIoMixedAsyncTree,
 }
 
 
 if __name__ == "__main__":
     runner = pyperf.Runner(add_cmdline_args=add_cmdline_args)
     add_metadata(runner)
     add_parser_args(runner.argparser)
     args = runner.parse_args()
     benchmark = args.benchmark
 
     async_tree_class = BENCHMARKS[benchmark]
     async_tree = async_tree_class()
     runner.bench_async_func(f"async_tree_{benchmark}", async_tree.run)
-
```

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py` & `pyperformance-1.0.8/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/run.py` & `pyperformance-1.0.8/pyperformance/run.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.7/pyperformance/venv.py` & `pyperformance-1.0.8/pyperformance/venv.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import os.path
 import sys
 
 import pyperformance
 from . import _utils, _pip, _venv
 
 
-REQUIREMENTS_FILE = os.path.join(pyperformance.DATA_DIR, 'requirements.txt')
+REQUIREMENTS_FILE = os.path.join(
+    os.path.dirname(__file__), 'requirements', 'requirements.txt'
+)
 PYPERF_OPTIONAL = ['psutil']
 
 
 class Requirements(object):
 
     @classmethod
     def from_file(cls, filename):
@@ -167,36 +169,39 @@
         # Display the pip version
         _pip.run_pip('--version', python=self.python, env=self._env)
 
         return self
 
     @classmethod
     def ensure(cls, root, python=None, *,
+               inherit_environ=None,
                upgrade=False,
                **kwargs
                ):
         exists = _venv.venv_exists(root)
         if upgrade == 'oncreate':
             upgrade = not exists
         elif upgrade == 'onexists':
             upgrade = exists
         elif isinstance(upgrade, str):
             raise NotImplementedError(upgrade)
 
         if exists:
             self = super().ensure(root)
+            self.inherit_environ = inherit_environ
             if upgrade:
                 self.upgrade_pip()
             else:
                 self.ensure_pip(upgrade=False)
             return self
         else:
             return cls.create(
                 root,
                 python,
+                inherit_environ=inherit_environ,
                 upgrade=upgrade,
                 **kwargs
             )
 
     def __init__(self, root, *, base=None, inherit_environ=None):
         super().__init__(root, base=base)
         self.inherit_environ = inherit_environ or None
```

### Comparing `pyperformance-1.0.7/pyperformance.egg-info/PKG-INFO` & `pyperformance-1.0.8/pyperformance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperformance
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python benchmark suite
 Author: Collin Winter, Jeffrey Yasskin
 License: MIT
 Project-URL: Homepage, https://github.com/python/pyperformance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyperformance-1.0.7/pyperformance.egg-info/SOURCES.txt` & `pyperformance-1.0.8/pyperformance.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -51,25 +51,27 @@
 benchmarks/bm_regex_compile/bm_regex_effbot.py
 benchmarks/bm_regex_compile/bm_regex_v8.py
 benchmarks/bm_regex_compile/run_benchmark.py
 benchmarks/bm_regex_dna/run_benchmark.py
 benchmarks/bm_regex_effbot/run_benchmark.py
 benchmarks/bm_regex_v8/run_benchmark.py
 benchmarks/bm_richards/run_benchmark.py
+benchmarks/bm_richards_super/run_benchmark.py
 benchmarks/bm_scimark/run_benchmark.py
 benchmarks/bm_spectral_norm/run_benchmark.py
 benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
 benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
 benchmarks/bm_sqlglot/run_benchmark.py
 benchmarks/bm_sqlite_synth/run_benchmark.py
 benchmarks/bm_sympy/run_benchmark.py
 benchmarks/bm_telco/run_benchmark.py
 benchmarks/bm_tomli_loads/generate_data.py
 benchmarks/bm_tomli_loads/run_benchmark.py
 benchmarks/bm_tornado_http/run_benchmark.py
+benchmarks/bm_typing_runtime_protocols/run_benchmark.py
 benchmarks/bm_unpack_sequence/run_benchmark.py
 benchmarks/bm_xml_etree/run_benchmark.py
 doc/Makefile
 doc/benchmarks.rst
 doc/changelog.rst
 doc/conf.py
 doc/cpython_results_2017.rst
@@ -101,15 +103,14 @@
 pyperformance/venv.py
 pyperformance.egg-info/PKG-INFO
 pyperformance.egg-info/SOURCES.txt
 pyperformance.egg-info/dependency_links.txt
 pyperformance.egg-info/entry_points.txt
 pyperformance.egg-info/requires.txt
 pyperformance.egg-info/top_level.txt
-pyperformance/data-files/requirements.txt
 pyperformance/data-files/benchmarks/MANIFEST
 pyperformance/data-files/benchmarks/bm_2to3/pyproject.toml
 pyperformance/data-files/benchmarks/bm_2to3/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_2to3/data/2to3/README.txt
 pyperformance/data-files/benchmarks/bm_2to3/data/2to3/__init__.py.txt
 pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt
 pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt
@@ -118,21 +119,27 @@
 pyperformance/data-files/benchmarks/bm_2to3/data/2to3/signals.py.txt
 pyperformance/data-files/benchmarks/bm_2to3/data/2to3/template_loader.py.txt
 pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt
 pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt
 pyperformance/data-files/benchmarks/bm_async_generators/pyproject.toml
 pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed.toml
+pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager.toml
+pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_cpu_io_mixed.toml
+pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_io.toml
+pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_eager_memoization.toml
 pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io.toml
 pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization.toml
 pyperformance/data-files/benchmarks/bm_async_tree/pyproject.toml
 pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_asyncio_tcp/bm_asyncio_tcp_ssl.toml
 pyperformance/data-files/benchmarks/bm_asyncio_tcp/pyproject.toml
 pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py
+pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_cert.pem
+pyperformance/data-files/benchmarks/bm_asyncio_tcp/ssl_key.pem
 pyperformance/data-files/benchmarks/bm_chameleon/pyproject.toml
 pyperformance/data-files/benchmarks/bm_chameleon/requirements.txt
 pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_chaos/pyproject.toml
 pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_comprehensions/pyproject.toml
 pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py
@@ -338,14 +345,16 @@
 pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_regex_effbot/pyproject.toml
 pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_regex_v8/pyproject.toml
 pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_richards/pyproject.toml
 pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py
+pyperformance/data-files/benchmarks/bm_richards_super/pyproject.toml
+pyperformance/data-files/benchmarks/bm_richards_super/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_scimark/pyproject.toml
 pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_spectral_norm/pyproject.toml
 pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/pyproject.toml
 pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/requirements.txt
 pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
@@ -367,11 +376,14 @@
 pyperformance/data-files/benchmarks/bm_tomli_loads/pyproject.toml
 pyperformance/data-files/benchmarks/bm_tomli_loads/requirements.txt
 pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml
 pyperformance/data-files/benchmarks/bm_tornado_http/pyproject.toml
 pyperformance/data-files/benchmarks/bm_tornado_http/requirements.txt
 pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py
+pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/pyproject.toml
+pyperformance/data-files/benchmarks/bm_typing_runtime_protocols/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_unpack_sequence/pyproject.toml
 pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_xml_etree/pyproject.toml
-pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
+pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
+pyperformance/requirements/requirements.txt
```

### Comparing `pyperformance-1.0.7/pyproject.toml` & `pyperformance-1.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -55,25 +55,52 @@
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python',
 ]
 requires-python = ">=3.7"
-dependencies = ["pyperf", "toml", "packaging"]
+dependencies = [
+    "pyperf",
+    "tomli; python_version < '3.11'",
+    "packaging",
+]
 
 [project.optional-dependencies]
 dev = [
     'tox',
+    'mypy==1.2.0',
+    'tomli',  # Needed even on 3.11+ for typechecking with mypy
 ]
 
 [project.scripts]
 pyperformance = "pyperformance.cli:main"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages]
 find = {}  # Scanning implicit namespaces is active by default
 
 [tool.setuptools.dynamic]
 version = {attr = "pyperformance.__version__"}
+
+[tool.mypy]
+python_version = "3.7"
+pretty = true
+enable_error_code = "ignore-without-code"
+disallow_any_generics = true
+strict_concatenate = true
+warn_redundant_casts = true
+warn_unused_ignores = true
+warn_unused_configs = true
+files = [
+    'pyperformance/',
+]
+exclude = [
+    'pyperformance/data-files/',
+    'pyperformance/tests/'
+]
+
+[[tool.mypy.overrides]]
+module = "pyperf"
+ignore_missing_imports = true
```

### Comparing `pyperformance-1.0.7/requirements.in` & `pyperformance-1.0.8/requirements.in`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # pyperformance dependencies
 # --------------------------
 
 pyperf
 
 # for benchmark metadata:
 packaging
-toml
+tomli; python_version < '3.11'
 
 
 # Optional dependencies
 # ---------------------
 #
 # The list of optional dependencies is hardcoded in pyperformance/venv.py
```

