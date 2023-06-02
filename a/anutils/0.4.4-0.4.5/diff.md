# Comparing `tmp/anutils-0.4.4.tar.gz` & `tmp/anutils-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anutils-0.4.4.tar", last modified: Sun May 14 18:24:37 2023, max compression
+gzip compressed data, was "anutils-0.4.5.tar", last modified: Fri Jun  2 05:38:02 2023, max compression
```

## Comparing `anutils-0.4.4.tar` & `anutils-0.4.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1799 2022-06-15 05:53:11.000000 anutils-0.4.4/.gitignore
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2863 2023-05-14 18:24:37.812678 anutils-0.4.4/PKG-INFO
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2372 2023-05-07 16:11:39.000000 anutils-0.4.4/README.md
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-14 18:24:37.812678 anutils-0.4.4/setup.cfg
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      901 2023-05-14 18:24:05.000000 anutils-0.4.4/setup.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       43 2023-05-14 06:23:19.000000 anutils-0.4.4/src/anutils/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      556 2023-05-14 06:17:33.000000 anutils-0.4.4/src/anutils/exceptions.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/mlutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-11 06:32:55.000000 anutils-0.4.4/src/anutils/mlutils/__init__.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2498 2023-05-11 06:32:47.000000 anutils-0.4.4/src/anutils/mlutils/mlutils.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/scutils/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      215 2023-05-14 06:31:30.000000 anutils-0.4.4/src/anutils/scutils/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     7738 2023-05-14 06:11:56.000000 anutils-0.4.4/src/anutils/scutils/annotation.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/scutils/data/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       39 2023-05-11 06:31:57.000000 anutils-0.4.4/src/anutils/scutils/data/__init__.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     3942 2023-05-11 06:33:02.000000 anutils-0.4.4/src/anutils/scutils/data/data.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1539 2023-04-18 21:48:37.000000 anutils-0.4.4/src/anutils/scutils/data/h5ad2mtx.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1211 2023-04-10 19:26:07.000000 anutils-0.4.4/src/anutils/scutils/data/mtx2rds.R
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/scutils/external/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       68 2023-05-11 06:31:45.000000 anutils-0.4.4/src/anutils/scutils/external/__init__.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/src/anutils/scutils/external/integration/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      297 2023-05-11 14:19:55.000000 anutils-0.4.4/src/anutils/scutils/external/integration/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1707 2023-05-05 18:26:12.000000 anutils-0.4.4/src/anutils/scutils/external/integration/harmony.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2809 2023-04-20 06:33:17.000000 anutils-0.4.4/src/anutils/scutils/external/integration/harmony_matrix.R
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      577 2023-05-06 07:55:23.000000 anutils-0.4.4/src/anutils/scutils/external/integration/integration.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3414 2023-05-11 14:37:17.000000 anutils-0.4.4/src/anutils/scutils/external/integration/scalex.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2187 2023-05-06 07:55:52.000000 anutils-0.4.4/src/anutils/scutils/external/integration/scvi.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4242 2023-05-09 06:26:37.000000 anutils-0.4.4/src/anutils/scutils/external/integration/seurat.R
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1578 2023-05-06 07:50:07.000000 anutils-0.4.4/src/anutils/scutils/external/integration/seurat.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    17278 2023-05-12 08:10:32.000000 anutils-0.4.4/src/anutils/scutils/plotting.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     7833 2023-05-05 13:05:09.000000 anutils-0.4.4/src/anutils/scutils/preprocessing.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils/scutils/resources/
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/src/anutils/scutils/resources/gene_sets/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      556 2023-05-12 15:00:19.000000 anutils-0.4.4/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/src/anutils/scutils/sc_cuda/
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      116 2023-05-11 06:30:39.000000 anutils-0.4.4/src/anutils/scutils/sc_cuda/__init__.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    29119 2023-04-20 13:48:41.000000 anutils-0.4.4/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2503 2023-04-20 13:50:49.000000 anutils-0.4.4/src/anutils/scutils/sc_cuda/scanpy_cuda.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4564 2023-03-12 12:33:33.000000 anutils-0.4.4/src/anutils/scutils/sc_cuda/scib_cuda.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       91 2023-05-14 05:41:26.000000 anutils-0.4.4/src/anutils/scutils/settings.py
--rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1229 2023-05-11 02:41:54.000000 anutils-0.4.4/src/anutils/scutils/utils.py
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)    10831 2023-05-14 06:13:42.000000 anutils-0.4.4/src/anutils/utils.py
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.808678 anutils-0.4.4/src/anutils.egg-info/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2863 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/PKG-INFO
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1401 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/SOURCES.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)        1 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/dependency_links.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)       73 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/requires.txt
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)        8 2023-05-14 18:24:37.000000 anutils-0.4.4/src/anutils.egg-info/top_level.txt
-drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-05-14 18:24:37.812678 anutils-0.4.4/tests/
--rwx------   0 ningweixi  (7191) zhangqflab  (9018)      581 2022-06-17 11:20:29.000000 anutils-0.4.4/tests/run_tests.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.960394 anutils-0.4.5/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1799 2022-06-15 05:53:11.000000 anutils-0.4.5/.gitignore
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2863 2023-06-02 05:38:02.960394 anutils-0.4.5/PKG-INFO
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2372 2023-05-25 12:50:22.000000 anutils-0.4.5/README.md
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-06-02 05:38:02.960394 anutils-0.4.5/setup.cfg
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      901 2023-06-02 05:37:32.000000 anutils-0.4.5/setup.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.956394 anutils-0.4.5/src/
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.956394 anutils-0.4.5/src/anutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       43 2023-05-14 06:23:19.000000 anutils-0.4.5/src/anutils/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      556 2023-05-14 06:17:33.000000 anutils-0.4.5/src/anutils/exceptions.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.956394 anutils-0.4.5/src/anutils/mlutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       38 2023-05-11 06:32:55.000000 anutils-0.4.5/src/anutils/mlutils/__init__.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2506 2023-05-25 06:06:48.000000 anutils-0.4.5/src/anutils/mlutils/mlutils.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.956394 anutils-0.4.5/src/anutils/scutils/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      215 2023-05-14 06:31:30.000000 anutils-0.4.5/src/anutils/scutils/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     8060 2023-05-15 14:34:04.000000 anutils-0.4.5/src/anutils/scutils/annotation.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.956394 anutils-0.4.5/src/anutils/scutils/data/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       39 2023-05-11 06:31:57.000000 anutils-0.4.5/src/anutils/scutils/data/__init__.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     3942 2023-05-11 06:33:02.000000 anutils-0.4.5/src/anutils/scutils/data/data.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1635 2023-05-22 08:45:38.000000 anutils-0.4.5/src/anutils/scutils/data/h5ad2mtx.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1211 2023-04-10 19:26:07.000000 anutils-0.4.5/src/anutils/scutils/data/mtx2rds.R
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.956394 anutils-0.4.5/src/anutils/scutils/external/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       68 2023-05-11 06:31:45.000000 anutils-0.4.5/src/anutils/scutils/external/__init__.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.960394 anutils-0.4.5/src/anutils/scutils/external/integration/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      297 2023-05-11 14:19:55.000000 anutils-0.4.5/src/anutils/scutils/external/integration/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1707 2023-05-05 18:26:12.000000 anutils-0.4.5/src/anutils/scutils/external/integration/harmony.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2806 2023-05-22 08:54:01.000000 anutils-0.4.5/src/anutils/scutils/external/integration/harmony_matrix.R
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      577 2023-05-06 07:55:23.000000 anutils-0.4.5/src/anutils/scutils/external/integration/integration.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     3460 2023-05-23 07:45:20.000000 anutils-0.4.5/src/anutils/scutils/external/integration/scalex.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2187 2023-05-06 07:55:52.000000 anutils-0.4.5/src/anutils/scutils/external/integration/scvi.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4251 2023-05-22 08:54:21.000000 anutils-0.4.5/src/anutils/scutils/external/integration/seurat.R
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1578 2023-05-06 07:50:07.000000 anutils-0.4.5/src/anutils/scutils/external/integration/seurat.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    23710 2023-05-25 05:37:16.000000 anutils-0.4.5/src/anutils/scutils/plotting.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     8287 2023-05-29 02:17:55.000000 anutils-0.4.5/src/anutils/scutils/preprocessing.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.956394 anutils-0.4.5/src/anutils/scutils/resources/
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.960394 anutils-0.4.5/src/anutils/scutils/resources/gene_sets/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      556 2023-05-12 15:00:19.000000 anutils-0.4.5/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.960394 anutils-0.4.5/src/anutils/scutils/sc_cuda/
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)      116 2023-05-11 06:30:39.000000 anutils-0.4.5/src/anutils/scutils/sc_cuda/__init__.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)    29119 2023-04-20 13:48:41.000000 anutils-0.4.5/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     2503 2023-04-20 13:50:49.000000 anutils-0.4.5/src/anutils/scutils/sc_cuda/scanpy_cuda.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     4564 2023-03-12 12:33:33.000000 anutils-0.4.5/src/anutils/scutils/sc_cuda/scib_cuda.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)       91 2023-05-14 05:41:26.000000 anutils-0.4.5/src/anutils/scutils/settings.py
+-rw-r--r--   0 ningweixi  (7191) zhangqflab  (9018)     1491 2023-05-23 11:54:01.000000 anutils-0.4.5/src/anutils/scutils/utils.py
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)    10831 2023-05-14 06:13:42.000000 anutils-0.4.5/src/anutils/utils.py
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.956394 anutils-0.4.5/src/anutils.egg-info/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     2863 2023-06-02 05:38:02.000000 anutils-0.4.5/src/anutils.egg-info/PKG-INFO
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)     1401 2023-06-02 05:38:02.000000 anutils-0.4.5/src/anutils.egg-info/SOURCES.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)        1 2023-06-02 05:38:02.000000 anutils-0.4.5/src/anutils.egg-info/dependency_links.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)       73 2023-06-02 05:38:02.000000 anutils-0.4.5/src/anutils.egg-info/requires.txt
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)        8 2023-06-02 05:38:02.000000 anutils-0.4.5/src/anutils.egg-info/top_level.txt
+drwxr-xr-x   0 ningweixi  (7191) zhangqflab  (9018)        0 2023-06-02 05:38:02.960394 anutils-0.4.5/tests/
+-rwx------   0 ningweixi  (7191) zhangqflab  (9018)      581 2022-06-17 11:20:29.000000 anutils-0.4.5/tests/run_tests.py
```

### Comparing `anutils-0.4.4/.gitignore` & `anutils-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/PKG-INFO` & `anutils-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,22 @@
 Metadata-Version: 2.1
 Name: anutils
-Version: 0.4.4
+Version: 0.4.5
 Summary: ml and single cell utils.
 Home-page: https://github.com/AaronNing/anutils
 Author: Aaron Ning
 Author-email: aaronning98@gmail.com
 License: MIT
 Keywords: anutils
 
 anutils
 =======
 
 ML and single cell analysis utils.
 
-installation
-------------
-
-::
-
-   pip install anutils
-
-**NOTE**: To use ``anutils.scutils.sc_cuda``, you need to install rapids
-first. see `rapids.ai <https://rapids.ai/start.html>`__ for details. For
-example, to install rapids on a linux machine with cuda 11, you can run:
-
-.. code:: bash
-
-   pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
-   pip install cuml-cu11 --extra-index-url=https://pypi.nvidia.com
-   pip install cugraph-cu11 --extra-index-url=https://pypi.nvidia.com
-
 usage
 -----
 
 general utils: ``anutils.*``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ``anutls.glimpse`` is similar to ``dplyr::glimpse`` in R, but enhanced
@@ -99,7 +82,24 @@
 -----------------------
 
 .. code:: python
 
    import anutils.mlutils as ml
 
    # to be added
+
+installation
+------------
+
+::
+
+   pip install anutils
+
+**NOTE**: To use ``anutils.scutils.sc_cuda``, you need to install rapids
+first. see `rapids.ai <https://rapids.ai/start.html>`__ for details. For
+example, to install rapids on a linux machine with cuda 11, you can run:
+
+.. code:: bash
+
+   pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
+   pip install cuml-cu11 --extra-index-url=https://pypi.nvidia.com
+   pip install cugraph-cu11 --extra-index-url=https://pypi.nvidia.com
```

### Comparing `anutils-0.4.4/README.md` & `anutils-0.4.5/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,10 @@
 # anutils
 ML and single cell analysis utils.  
 
-## installation
-```
-pip install anutils
-```
-**NOTE**: To use `anutils.scutils.sc_cuda`, you need to install rapids first. see [rapids.ai](https://rapids.ai/start.html) for details. For example, to install rapids on a linux machine with cuda 11, you can run:  
-```bash
-pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
-pip install cuml-cu11 --extra-index-url=https://pypi.nvidia.com
-pip install cugraph-cu11 --extra-index-url=https://pypi.nvidia.com
-```
-
 ## usage
 
 ### general utils: `anutils.*`
 
 `anutls.glimpse` is similar to `dplyr::glimpse` in R, but enhanced in:
 - display the index
 - when passing `show_unique=True`, display the number of unique values for each column
@@ -70,7 +59,18 @@
 
 ## machine learning utils:
 ```python
 import anutils.mlutils as ml
 
 # to be added
 ```
+
+## installation
+```
+pip install anutils
+```
+**NOTE**: To use `anutils.scutils.sc_cuda`, you need to install rapids first. see [rapids.ai](https://rapids.ai/start.html) for details. For example, to install rapids on a linux machine with cuda 11, you can run:  
+```bash
+pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
+pip install cuml-cu11 --extra-index-url=https://pypi.nvidia.com
+pip install cugraph-cu11 --extra-index-url=https://pypi.nvidia.com
+```
```

### Comparing `anutils-0.4.4/setup.py` & `anutils-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     from pypandoc import convert_file
     long_description = convert_file('README.md', 'rst')
 except:
     long_description = ''
 
 setup(
     name='anutils',
-    version='0.4.4',
+    version='0.4.5',
     license='MIT',
     author="Aaron Ning",
     author_email='aaronning98@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
 
     # If any package contains *.r files, include them:
```

### Comparing `anutils-0.4.4/src/anutils/exceptions.py` & `anutils-0.4.5/src/anutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/mlutils/mlutils.py` & `anutils-0.4.5/src/anutils/mlutils/mlutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
+
 from anutils.utils import flatten
 
 
 def plot_learning_curve(data: pd.DataFrame,
                         keys: list,
-                        suptitle='',
+                        suptitle: str = '',
                         save: str = None,
                         style: str = 'default'):
     r"""
     data: dict of curves
     keys: list specifying the plot structures. E.g., [['tl', 'vl], ['ta', 'va']] means two subplots. 
     """
     plt.style.use(style)
```

### Comparing `anutils-0.4.4/src/anutils/scutils/annotation.py` & `anutils-0.4.5/src/anutils/scutils/annotation.py`

 * *Files 5% similar despite different names*

```diff
@@ -145,14 +145,24 @@
                        frameon=False,
                        colorbar_loc=None,
                        wspace=0)
         dfs.append((g, df))
     return dfs
 
 
+def gsea(gene_list, gene_sets='GO_Biological_Process_2021', **enrichr_kwargs):
+    import gseapy as gp
+    from gseapy.plot import barplot
+    # perform enrichment analysis
+    enr = gp.enrichr(gene_list=gene_list, gene_sets=gene_sets, **enrichr_kwargs)
+    # plot
+    barplot(enr.res2d, title=gene_sets)
+    return enr
+
+
 def score_genes_cell_cycle(adata, copy=False, **scanpy_score_genes_kwargs):
     """score cell cycle genes
     
     Cell cycle genes are from [Tirosh et al, 2015](https://doi.org/10.1126/science.aad0501).
     
     See [this notebook from scanpy](https://nbviewer.org/github/theislab/scanpy_usage/blob/master/180209_cell_cycle/cell_cycle.ipynb) for details.
```

### Comparing `anutils-0.4.4/src/anutils/scutils/data/data.py` & `anutils-0.4.5/src/anutils/scutils/data/data.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/data/h5ad2mtx.py` & `anutils-0.4.5/src/anutils/scutils/data/h5ad2mtx.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,38 @@
 import numpy as np
 import pandas as pd
 import scanpy as sc
 from scipy.io import mmwrite
 from scipy.sparse import csr_matrix
 
 
-def h5ad2mtx(adata: sc.AnnData, outdir, filed='integer'):
+def h5ad2mtx(adata: sc.AnnData, outdir, field='integer', layer=None):
     """
     field: 'integer' or 'real'
     """
+
+    adata = adata.copy()
+
+    if layer is not None:
+        adata.X = adata.layers[layer]
+
     if os.path.exists(outdir):
         print("Output directory already exists. Overwriting...")
     else:
         os.makedirs(outdir)
     adata.X = csr_matrix(adata.X)
-    
+
     print("checking adata.X...")
-    if filed == 'integer':
+    if field == 'integer':
         if (adata.X - adata.X.astype(int)).nnz > 0:
             print("WARNING: adata.X contains non-integer values. Converting to integer...")
             adata.X = adata.X.astype(int)
-    
+
     print("writing mtx files...")
-    mmwrite(outdir + '/matrix.mtx', csr_matrix(adata.X), field=filed)
+    mmwrite(outdir + '/matrix.mtx', csr_matrix(adata.X), field=field)
     adata.obs.to_csv(outdir + "/metadata.txt", sep='\t')
     pd.DataFrame(adata.var_names).to_csv(outdir + "/features.txt",
                                          sep='\t',
                                          header=None,
                                          index=0)
     print("Done.")
```

### Comparing `anutils-0.4.4/src/anutils/scutils/data/mtx2rds.R` & `anutils-0.4.5/src/anutils/scutils/data/mtx2rds.R`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/external/integration/harmony.py` & `anutils-0.4.5/src/anutils/scutils/external/integration/harmony.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/external/integration/harmony_matrix.R` & `anutils-0.4.5/src/anutils/scutils/external/integration/harmony_matrix.R`

 * *Files 12% similar despite different names*

```diff
@@ -37,34 +37,35 @@
 parser$add_argument("--max_iter_harmony", type = "double", required = FALSE, default = 10, help = "Max iteration of harmony")
 parser$add_argument("--max_iter_cluster", type = "double", required = FALSE, default = 200, help = "Max iteration of cluster")
 parser$add_argument("--epsilon_cluster", type = "double", required = FALSE, default = 1e-05, help = "Epsilon of cluster")
 parser$add_argument("--epsilon_harmony", type = "double", required = FALSE, default = 1e-04, help = "Epsilon of harmony")
 args <- parser$parse_args()
 
 # Read data
-message('Reading data...')
-data <- read.table(args$input_file, sep = '\t')
-metadata <- read.table(args$metadata_file, sep = '\t', header = 1, row.names = 1)
+message("Reading data...")
+data <- read.table(args$input_file, sep = "\t")
+metadata <- read.table(args$metadata_file, sep = "\t", header = 1, row.names = 1)
 
-cat('shape of adata: ', dim(data), '\n')
-cat('there are ', length(unique(metadata[[args$batch_key]])), ' batches\n')
+cat("shape of adata: ", dim(data), "\n")
+cat("there are ", length(unique(metadata[[args$batch_key]])), " batches\n")
 
 # Run Harmony
-message('Running Harmony...')
+message("Running Harmony...")
 data.harmony <- HarmonyMatrix(
-    data, metadata, args$batch_key, do_pca = FALSE, 
-    theta = args$theta, 
-    lambda = args$lambda, 
-    sigma = args$sigma, 
-    tau = args$tau, 
-    max.iter.harmony = args$max_iter_harmony, 
-    max.iter.cluster = args$max_iter_cluster, 
-    epsilon.cluster = args$epsilon_cluster, 
+    data, metadata, args$batch_key,
+    do_pca = FALSE,
+    theta = args$theta,
+    lambda = args$lambda,
+    sigma = args$sigma,
+    tau = args$tau,
+    max.iter.harmony = args$max_iter_harmony,
+    max.iter.cluster = args$max_iter_cluster,
+    epsilon.cluster = args$epsilon_cluster,
     epsilon.harmony = args$epsilon_harmony
 )
 
 # Write data
-message('Writing data...')
-cat('Writing data to ', args$output_file, '\n')
-write.table(data.harmony, file = args$output_file, sep = '\t', row.names = FALSE, col.names = FALSE)
+message("Writing data...")
+cat("Writing data to ", args$output_file, "\n")
+write.table(data.harmony, file = args$output_file, sep = "\t", row.names = FALSE, col.names = FALSE)
 
-message('Done.')
+message("Done.")
```

### Comparing `anutils-0.4.4/src/anutils/scutils/external/integration/integration.py` & `anutils-0.4.5/src/anutils/scutils/external/integration/integration.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/external/integration/scalex.py` & `anutils-0.4.5/src/anutils/scutils/external/integration/scalex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 def scalex(
+    #TODO: extract default params from scalex
     adata,
     batch,
     output_path=None,
     return_model=False,
     seed=0,
-    lr=1e-3,
+    lr=2e-4,
     max_iteration=30000,
     batch_size=64,
     hidden_dim=1024,
     latent_dim=10,
     verbose=False,
     batch_scale=True,
     key_added='X_scalex',
```

### Comparing `anutils-0.4.4/src/anutils/scutils/external/integration/scvi.py` & `anutils-0.4.5/src/anutils/scutils/external/integration/scvi.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/external/integration/seurat.R` & `anutils-0.4.5/src/anutils/scutils/external/integration/seurat.R`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 suppressPackageStartupMessages(library(argparse))
 suppressPackageStartupMessages(library(Seurat))
 suppressPackageStartupMessages(library(scater))
 suppressPackageStartupMessages(library(future))
 suppressPackageStartupMessages(library(Matrix))
 suppressPackageStartupMessages(library(future.apply))
 
-parser <- ArgumentParser(description='Seurat_v3 for the integrative analysis of multi-batch single-cell transcriptomic profiles')
-parser$add_argument("-i", "--input_path", type="character", help="Path contains RNA data")
-parser$add_argument("-o", "--output_path", type="character", default='/home/tiankang/SCALEX/results/Seurat_v3', help="Output path")
-parser$add_argument("-mf", "--minFeatures", type="integer", default=600, help="Remove cells with less than minFeatures features")
-parser$add_argument("-mc", "--minCells", type="integer", default=3, help="Remove features with less than minCells cells")
-parser$add_argument("-nt", "--n_top_features", type="integer", default=2000, help="N highly variable features")
-parser$add_argument("-nj", "--n_jobs", type="integer", default=1, help="Number of jobs")
-parser$add_argument("--batch_key", type="character", default='batch', help="Batch key")
-parser$add_argument("--k_anchor", type="integer", default=5, help="k.anchor")
-parser$add_argument("--k_filter", type="integer", default=200, help="k.filter")
-parser$add_argument("--k_score", type="integer", default=30, help="k.score")
+parser <- ArgumentParser(description = "Seurat_v3 for the integrative analysis of multi-batch single-cell transcriptomic profiles")
+parser$add_argument("-i", "--input_path", type = "character", help = "Path contains RNA data")
+parser$add_argument("-o", "--output_path", type = "character", default = "/home/tiankang/SCALEX/results/Seurat_v3", help = "Output path")
+parser$add_argument("-mf", "--minFeatures", type = "integer", default = 600, help = "Remove cells with less than minFeatures features")
+parser$add_argument("-mc", "--minCells", type = "integer", default = 3, help = "Remove features with less than minCells cells")
+parser$add_argument("-nt", "--n_top_features", type = "integer", default = 2000, help = "N highly variable features")
+parser$add_argument("-nj", "--n_jobs", type = "integer", default = 1, help = "Number of jobs")
+parser$add_argument("--batch_key", type = "character", default = "batch", help = "Batch key")
+parser$add_argument("--k_anchor", type = "integer", default = 5, help = "k.anchor")
+parser$add_argument("--k_filter", type = "integer", default = 200, help = "k.filter")
+parser$add_argument("--k_score", type = "integer", default = 30, help = "k.score")
 args <- parser$parse_args()
 
-plan("multiprocess", workers = args$n_jobs)
+plan("multisession", workers = args$n_jobs)
 options(future.globals.maxSize = 100000 * 1024^2, warn = -1)
 
 # Read data
-message('Reading data...')
-data <- readMM(paste(args$input_path, '/matrix.mtx', sep=''))
-genes <- read.table(paste(args$input_path, '/features.txt', sep=''), sep='\t')
-metadata <- read.csv(paste(args$input_path, '/metadata.txt', sep=''), sep='\t')
-row.names(metadata) <- metadata[,1]
-metadata <- metadata[,-1]
-metadata[[args$batch_key]] = as.character(metadata[[args$batch_key]])
+message("Reading data...")
+data <- readMM(paste(args$input_path, "/matrix.mtx", sep = ""))
+genes <- read.table(paste(args$input_path, "/features.txt", sep = ""), sep = "\t")
+metadata <- read.csv(paste(args$input_path, "/metadata.txt", sep = ""), sep = "\t")
+row.names(metadata) <- metadata[, 1]
+metadata <- metadata[, -1]
+metadata[[args$batch_key]] <- as.character(metadata[[args$batch_key]])
 data <- t(data)
-colnames(data) <- row.names(metadata) 
-row.names(data) <- genes[,1]
+colnames(data) <- row.names(metadata)
+row.names(data) <- genes[, 1]
 
-message('CreateSeuratObject...')
-adata <- CreateSeuratObject(as(data, "sparseMatrix"), 
-                           meta.data = metadata,
-                           min.cells = args$minCells, 
-                           min.features = args$minFeatures)
+message("CreateSeuratObject...")
+adata <- CreateSeuratObject(as(data, "sparseMatrix"),
+    meta.data = metadata,
+    min.cells = args$minCells,
+    min.features = args$minFeatures
+)
 
-cat('shape of adata: ', dim(adata), '\n')
-cat('there are ', length(unique(metadata[[args$batch_key]])), ' batches\n')
+cat("shape of adata: ", dim(adata), "\n")
+cat("there are ", length(unique(metadata[[args$batch_key]])), " batches\n")
 
 # PP and integration
 adata.list <- SplitObject(adata, split.by = args$batch_key)
 
-message('Preprocessing each batch...')
+message("Preprocessing each batch...")
 adata.list <- future_lapply(X = adata.list, FUN = function(x) {
     # calculate percent.mito
     # x <- PercentageFeatureSet(x, pattern = "^MT-", col.name = "percent.mito")
     x <- NormalizeData(x, verbose = FALSE)
     x <- FindVariableFeatures(x, nfeatures = args$n_top_features, selection.method = "vst", verbose = FALSE)
     # x <- ScaleData(x, verbose = FALSE, vars.to.regress = c('nUMI', 'percent.mito'))
 }, future.seed = TRUE)
 
-message('SelectIntegrationFeatures...')
+message("SelectIntegrationFeatures...")
 features <- SelectIntegrationFeatures(object.list = adata.list)
 
-message('PCA each batch...')
+message("PCA each batch...")
 adata.list <- future_lapply(X = adata.list, FUN = function(x) {
     x <- ScaleData(x, features = features, verbose = FALSE)
     x <- RunPCA(x, features = features, verbose = FALSE)
 }, future.seed = TRUE)
 
-message('FindIntegrationAnchors...')
-adata.anchors <- FindIntegrationAnchors(object.list = adata.list, dims = 1:30, verbose = FALSE, reduction = 'rpca')
+message("FindIntegrationAnchors...")
+adata.anchors <- FindIntegrationAnchors(object.list = adata.list, dims = 1:30, verbose = FALSE, reduction = "rpca")
 
-message('IntegrateData...')
+message("IntegrateData...")
 adata.integrated <- IntegrateData(anchorset = adata.anchors, dims = 1:30, verbose = FALSE)
 
-message('RunPCA...')
+message("RunPCA...")
 adata.integrated <- ScaleData(adata.integrated, verbose = FALSE)
 adata.integrated <- RunPCA(adata.integrated, npcs = 50, verbose = FALSE)
 
 # write outputs
-if (!file.exists(args$output_path)){
-    dir.create(file.path(args$output_path),recursive = TRUE)
+if (!file.exists(args$output_path)) {
+    dir.create(file.path(args$output_path), recursive = TRUE)
 }
-message('Writing outputs...')
-cat('Writing pcs to ', args$output_path, '/pcs.txt\n', sep='')
-cat('Writing meta to ', args$output_path, '/meta.txt\n', sep = '')
-write.table(adata.integrated@meta.data[,-1:-3], paste0(args$output_path, '/meta.txt'), sep = '\t')
-write.table(adata.integrated@reductions$pca@cell.embeddings, paste0(args$output_path, '/pcs.txt'), sep = '\t')
+message("Writing outputs...")
+cat("Writing pcs to ", args$output_path, "/pcs.txt\n", sep = "")
+cat("Writing meta to ", args$output_path, "/meta.txt\n", sep = "")
+write.table(adata.integrated@meta.data[, -1:-3], paste0(args$output_path, "/meta.txt"), sep = "\t")
+write.table(adata.integrated@reductions$pca@cell.embeddings, paste0(args$output_path, "/pcs.txt"), sep = "\t")
 
-message('Done!')
+message("Done!")
```

### Comparing `anutils-0.4.4/src/anutils/scutils/external/integration/seurat.py` & `anutils-0.4.5/src/anutils/scutils/external/integration/seurat.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/plotting.py` & `anutils-0.4.5/src/anutils/scutils/plotting.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,41 +2,61 @@
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import seaborn as sns
+from scanpy._utils import _check_use_raw
 from statannotations.Annotator import Annotator
 
+from anutils.scutils.utils import _get_df_or_adata_obs
 from anutils.utils import Silent
 
 
 def init_fig_params():
     plt.rcParams['axes.unicode_minus'] = False
     plt.rc('font', family='Helvetica')
     plt.rcParams['pdf.fonttype'] = 42
     # sc.settings.verbosity = 3  # verbosity: errors (0), warnings (1), info (2), hints (3)
     # sc.logging.print_header()
     sc.set_figure_params(dpi=120, facecolor='w', frameon=True, figsize=(4, 4))
     # %config InlineBackend.figure_format='retina'
     # %matplotlib inline
 
 
+def subplots(ncols, nrows, subfigsize=None, wspace=None, hspace=None, **subplots_kwargs):
+    """`plt.subplots` with `figsize` calculated from `ncols`, `nrows`, `subfigsize`, `wspace`, `hspace`
+    """
+    if subfigsize is None:
+        subfigsize = mpl.rcParams['figure.figsize']
+    if wspace is None:
+        wspace = mpl.rcParams['figure.subplot.wspace']
+    if hspace is None:
+        hspace = mpl.rcParams['figure.subplot.hspace']
+    figsize = (subfigsize[0] * (ncols + wspace * (ncols - 1)),
+               subfigsize[1] * (nrows + hspace * (nrows - 1)))
+    fig, axes = plt.subplots(ncols=ncols, nrows=nrows, figsize=figsize, **subplots_kwargs)
+    fig.subplots_adjust(wspace=wspace, hspace=hspace)
+    return fig, axes
+
+
 def embeddings(adata,
                basis=None,
                *,
                groupby,
                replicate_key=None,
                groups_order=None,
                add_bg=False,
                ncols=None,
                figsize=None,
                zoom=False,
                return_fig_axes=False,
+               wspace=None,
+               hspace=None,
                **embedding_kwargs):
     """plot embeddings of adata grouped by group_adata_by
 
     Parameters
     ----------
     groupby : str or list of str
         column(s) in adata.obs. if a list, they will be concatenated with '::' as the group key
@@ -45,15 +65,15 @@
     groups_order : iterable, optional
         a ordered list of keys in `adata.obs[groupby]`, by default None
     add_bg : bool, optional
         whether to add umap background (from other groups), by default False
     ncols : int, optional
         ncols, by default 3
     figsize : 2 length tuple, optional
-        figsize, by default `(5 * ncols, 5 * nrows)`
+        figsize of each embedding, by default None
     zoom : bool, optional
         whether to zoom each umap plot, by default False, which means the xlim and ylim will be the same for all plots
     return_fig_axes : bool, optional
         whether to return the fig and axes, by default False
     embedding_kwargs : dict
         kwargs for sc.pl.embedding. `adata` is required. if `basis` is not provided, `X_umap` will be used.
 
@@ -61,96 +81,107 @@
     -------
     fig
         the fig object
     """
     if basis is None:
         basis = 'X_umap'
 
-    # reorder
+    # handle groupby
     if isinstance(groupby, str):
         pass
     else:  # iterable
         groupby = '::'.join(groupby)
         adata.obs[groupby] = adata.obs[list(groupby.split('::'))].apply(lambda x: '::'.join(x),
                                                                         axis=1)
-    indices = adata.obs.groupby(groupby).indices
+    group_indices_dict = adata.obs.groupby(groupby).indices
     if groups_order is None:
-        groups_order = indices.keys()
-    indices = {k: indices[k] for k in groups_order}
-    if ncols is None:
-        ncols = min(4, len(indices))
-    # plot
-    N = adata.obs[groupby].nunique()
-    nrows = (N - 1) // ncols + 1
-    if figsize is None:
-        figsize = (5 * ncols, 5 * nrows)
-    fig, axes = plt.subplots(ncols=ncols, nrows=nrows, figsize=figsize)
+        groups_order = group_indices_dict.keys()
+    group_indices_dict = {k: group_indices_dict[k] for k in groups_order}
 
+    # handle color
     if 'color' in embedding_kwargs:
         if isinstance(embedding_kwargs['color'], str):
             embedding_kwargs['color'] = [embedding_kwargs['color']]
-        # freeze the colors for categorical variables to make sure the colors are
-        # the same for different plots. (scanpy will change the colors for categorical
-        # variables if the number of categories changes when subseting the adata)
-        # sc.pl.embedding(**embedding_kwargs, show=False)
 
-    for i, (k, v) in enumerate(indices.items()):
-        ad = adata[v, :]
+    # now plot
+    if ncols is None:
+        ncols = min(4, len(group_indices_dict))
+    N = adata.obs[groupby].nunique()
+    nrows = (N - 1) // ncols + 1
+    fig, axes = subplots(
+        ncols=ncols,
+        nrows=nrows,
+        subfigsize=figsize,
+        wspace=wspace,
+        hspace=hspace,
+    )
+
+    for i_group, (group, group_idcs) in enumerate(group_indices_dict.items()):
+        ad = adata[group_idcs, :]
+
         # scanpy changes the number of categories when subseting the adata, so we need
         # to reset the categories
         if 'color' in embedding_kwargs:
             for c in embedding_kwargs['color']:
                 if c not in ad.obs.columns:
                     # might be a gene name
                     continue
                 # if it is categorical
                 if adata.obs[c].dtype.name == 'category':
+                    # reset the categories to the original categories
                     ad.obs[c].cat.set_categories(adata.obs[c].cat.categories, inplace=True)
 
-        title = k
+        title = group
         if replicate_key is not None:
             title += f' (n={ad.obs[replicate_key].nunique()})'
+
         kwargs = embedding_kwargs.copy()
+
+        # background umap
         if add_bg:
             _ = sc.pl.embedding(
                 adata,
                 basis=basis,
-                ax=axes.flatten()[i],
+                ax=axes.flatten()[i_group],
                 show=False,
             )
+
+        # foreground umap
         _ = sc.pl.embedding(
             ad,
             basis=basis,
             **kwargs,
-            ax=axes.flatten()[i],
+            ax=axes.flatten()[i_group],
             show=False,
             title=title,
         )
 
     # remove empty axes
-    while i < ncols * nrows - 1:
-        i += 1
-        axes.flatten()[i].axis('off')
-
+    while i_group < ncols * nrows - 1:
+        i_group += 1
+        axes.flatten()[i_group].axis('off')
+
+    # adjust axes lims to make them equal
+    # maybe use `sharex=True, sharey=True` in `plt.subplots`?
+    # need to test.
     if not zoom:
         axes_used = axes.flatten()[:N]
-        # adjust axes lims to make them equal
         xlims = np.array([ax.get_xlim() for ax in axes_used.flat])
         ylims = np.array([ax.get_ylim() for ax in axes_used.flat])
         xlims = np.array([xlims[:, 0].min(), xlims[:, 1].max()])
         ylims = np.array([ylims[:, 0].min(), ylims[:, 1].max()])
         for ax in axes_used.flat:
             ax.set_xlim(xlims)
             ax.set_ylim(ylims)
 
     # fig.tight_layout()
     return (fig, axes) if return_fig_axes else None
 
 
-def change_bar_width(ax, new_value):
+def _change_bar_width(ax, new_value):
     for patch in ax.patches:
         current_width = patch.get_width()
         diff = current_width - new_value
 
         # we change the bar width
         patch.set_width(new_value)
 
@@ -221,14 +252,15 @@
     legend_fontsize=None,
     legend_ncols=2,
     label_fontsize=None,
     label_pad=None,
     label_rotation=45,
     return_df=False,
     add_counts=True,
+    add_counts_text=True,
     hspace=0.1,
     counts_height_ratio=.25,
     counts_color='#154c79',
 ):
     """plot the composition of a categorical variable `hue` in different groups of `x`
 
     Parameters
@@ -254,24 +286,15 @@
         axes
 
     Raises
     ------
     ValueError
         data must be a pandas.DataFrame or an anndata.AnnData
     """
-    if type(data).__name__ == 'DataFrame':
-        df: pd.DataFrame = data
-    elif type(data).__name__ == 'AnnData':
-        df: pd.DataFrame = data.obs
-    else:
-        raise ValueError('data must be a pandas.DataFrame or an anndata.AnnData')
-    
-    if figsize is None:
-        # get the scanpy default figsize
-        sc.set_figure_params
+    df = _get_df_or_adata_obs(data)
 
     counts_df: pd.DataFrame = df.groupby(x)[hue].value_counts().unstack()
     if x_subset is None:
         x_subset = counts_df.index
     if hue_subset is None:
         hue_subset = counts_df.columns
     counts_df = counts_df.loc[x_subset, hue_subset]
@@ -286,40 +309,74 @@
             nrows=2,
             ncols=1,
             sharex=True,
             gridspec_kw={'height_ratios': [counts_height_ratio, 1 - counts_height_ratio]},
             figsize=figsize,
         )
         fig.subplots_adjust(hspace=hspace)
-        
+
         # plot counts
         ax = counts.plot.bar(ax=ax1, color=counts_color, width=bar_width)
         ax.set_ylabel('Cell counts', fontsize=label_fontsize)
-        ax.set_yticklabels(ax.get_yticklabels(), fontsize=label_fontsize)
+        # set fontsize of the counts plot
+        ax.tick_params(labelsize=label_fontsize)
+
+        if add_counts_text:
+            # Add counts above the two bar graphs
+            highest_height = 0
+            highest_txt = None
+            for rect in ax.patches:
+                barx = rect.get_x()
+                barw = rect.get_width()
+                barh = rect.get_height()
+                txt = ax.text(barx + barw / 2.0,
+                              barh,
+                              f'{barh:.0f}',
+                              ha='center',
+                              va='bottom',
+                              fontsize=label_fontsize)
+                if barh > highest_height:
+                    highest_height = barh
+                    highest_txt = txt
+            # adjust the ylim of the counts plot to make sure the counts text is visible
+            # by adding font height to the ylim
+            txtbb = highest_txt.get_window_extent(
+                renderer=fig.canvas.get_renderer()).transformed(ax.transData.inverted())
+            ax.set_ylim(ax.get_ylim()[0], ax.get_ylim()[1] + txtbb.height * 1.5)
+
     else:
         fig, ax2 = plt.subplots(1, 1, figsize=figsize)
 
     # plot composition
-    ax: plt.Axes = comp_df.plot.bar(ax=ax2, stacked=True, figsize=figsize, color=hue_colors)
+    ax: plt.Axes = comp_df.plot.bar(ax=ax2,
+                                    stacked=True,
+                                    figsize=figsize,
+                                    color=hue_colors,
+                                    width=bar_width)
     ax.set_xticklabels(ax.get_xticklabels(), fontsize=label_fontsize, rotation=label_rotation)
     ax.set_yticklabels(ax.get_yticklabels(), fontsize=label_fontsize)
     ax.set_ylabel('Relative celltype abundacy(%)', fontsize=label_fontsize)
     ax.set_xlabel('', fontsize=label_fontsize, labelpad=label_pad)
     legend_params = {
         'loc': 'center left',
         'bbox_to_anchor': (1.01, 0.5),
         'fontsize': legend_fontsize,
         'ncol': legend_ncols,
         'frameon': False,
         'markerscale': 100,
     }
     ax.legend(**legend_params)
 
-    change_bar_width(ax, bar_width)
-    
+    # remove grid
+    for ax in fig.axes:
+        ax.grid(False)
+
+    # adjust the figure to make sure all ylabels and xlabels are visible
+    #TODO
+
     return (ax1, ax2) if not return_df else ((ax1, ax2), comp_df)
 
 
 def get_cmap_colors(cmap, n, alpha=1, pad=1):
     colors = getattr(mpl.cm, cmap)(np.linspace(start=0, stop=1, num=n + 2 * pad), alpha=alpha)
     if pad > 0:
         colors = colors[pad:-pad]
@@ -370,21 +427,131 @@
         for i, item in enumerate(group_items[g]):
             item_colors[item] = group_colors[g][i]
     item_colors = {k: item_colors[k] for k in items}
     colors = list(item_colors.values())
     return colors
 
 
+def barplot_with_pvals_by_group(
+    data,
+    x,
+    y,
+    groupby,
+    add_legend=None,
+    figsize=None,
+    return_fig_axes=False,
+    ncols=None,
+    wspace=None,
+    hspace=None,
+    x_order=None,
+    groups_order=None,
+    pairs=None,
+    verbose=False,
+    palette=None,
+    add_swarmplot=True,
+    showfliers=True,
+    simple_format=True,
+    test='t-test_ind',
+    text_format='star',
+):
+    """sns.barplot with p-values, grouped by groupby
+    
+    Recommended to use with figsize = (1.5, 2)
+    """
+    if hasattr(data, 'obs') and y not in data.obs.columns:
+        data = data.obs.join(sc.get.obs_df(data, keys=[y], use_raw=True))
+
+    df = _get_df_or_adata_obs(data)
+
+    # handle x_order
+    if x_order is None:
+        x_order = sorted(df[x].unique())
+
+    # handle groupby
+    if isinstance(groupby, str):
+        pass
+    else:  # iterable
+        groupby = '::'.join(groupby)
+        df[groupby] = df[list(groupby.split('::'))].apply(lambda x: '::'.join(x), axis=1)
+    group_indices_dict = df.groupby(groupby).indices
+    if groups_order is None:
+        groups_order = group_indices_dict.keys()
+    group_indices_dict = {k: group_indices_dict[k] for k in groups_order}
+
+    # handle add_legend
+    if add_legend is None:
+        add_legend = simple_format
+
+    # now plot
+    if ncols is None:
+        ncols = min(4, len(group_indices_dict))
+    N = df[groupby].nunique()
+    if add_legend:
+        N += 1
+    nrows = (N - 1) // ncols + 1
+    if figsize is None:
+        figsize = (1.5, 2)
+
+    fig, axes = subplots(
+        ncols=ncols,
+        nrows=nrows,
+        subfigsize=figsize,
+        wspace=wspace,
+        hspace=hspace,
+    )
+
+    for i_group, (group, group_idcs) in enumerate(group_indices_dict.items()):
+        group_df = df.iloc[group_idcs, :]
+
+        barplot_with_pvals(
+            data=group_df,
+            x=x,
+            y=y,
+            x_order=x_order,
+            pairs=pairs,
+            verbose=verbose,
+            ax=axes.flatten()[i_group],
+            title=group,
+            palette=palette,
+            add_swarmplot=add_swarmplot,
+            showfliers=showfliers,
+            simple_format=simple_format,
+            test=test,
+            text_format=text_format,
+        )
+
+    # remove empty axes
+    while i_group < ncols * nrows - 1:
+        i_group += 1
+        axes.flatten()[i_group].axis('off')
+
+    # add legend
+    if add_legend:
+        patch_names = x_order
+        patch_colors = [patch.get_facecolor() for patch in axes.flatten()[0].patches]
+        color_dict = dict(zip(patch_names, patch_colors))
+        plot_legend(axes.flatten()[-1], color_dict=color_dict)
+
+    # remove grid
+    for ax in fig.axes:
+        ax.grid(False)
+
+    # fig.tight_layout()
+
+    return (fig, axes) if return_fig_axes else None
+
+
 def barplot_with_pvals(data,
                        x,
                        y,
-                       order=None,
+                       x_order=None,
                        pairs=None,
                        verbose=True,
                        ax=None,
+                       title=None,
                        palette=None,
                        add_swarmplot=True,
                        showfliers=True,
                        simple_format=False,
                        test='t-test_ind',
                        text_format='star'):
     """sns.barplot with p-values
@@ -421,81 +588,93 @@
         see `statannotations.Annotator.Annotator`, by default 'star'
 
     Returns
     -------
     Axes
         ax
     """
-    if order is None:
-        order = sorted(data[x].unique())
+    if hasattr(data, 'obs') and y not in data.obs.columns:
+        data = data.obs.join(sc.get.obs_df(data, keys=[y], use_raw=True))
+
+    data = _get_df_or_adata_obs(data)
+
+    if x_order is None:
+        x_order = sorted(data[x].unique())
     if pairs is None:
-        pairs = list(combinations(order, 2))
+        pairs = list(combinations(x_order, 2))
     if simple_format:
         showfliers = False
 
     ax = sns.boxplot(
-        data=data[data[x].isin(order)],
+        data=data[data[x].isin(x_order)],
         x=x,
         y=y,
         ax=ax,
-        order=order,
+        order=x_order,
         linewidth=1,
         width=.4,
         saturation=1,
         showfliers=showfliers,
         palette=palette,
     )
     if add_swarmplot:
         # if too many points, do not add swarmplot
         if data.groupby(x).size().max() > 100:
             print('Too many points, not adding swarmplot.')
             add_swarmplot = False
         else:
-            ax = sns.swarmplot(data=data[data[x].isin(order)],
+            ax = sns.swarmplot(data=data[data[x].isin(x_order)],
                                x=x,
                                y=y,
                                ax=ax,
-                               order=order,
+                               order=x_order,
                                edgecolor='k',
                                palette=palette,
                                alpha=.9,
                                size=3,
                                linewidth=0.5)
     ax.grid(False)
     if simple_format:
-        ax.set_xlabel(y)
+        if title is not None:
+            ax.set_xlabel(title)
+        else:
+            ax.set_xlabel(y)
         # ax.set_ylabel('Percentage')
         ax.set_ylabel('')
         # ax.set_xticks([])
         ax.tick_params(bottom=False, labelbottom=False)
+    else:
+        if title is not None:
+            ax.set_title(title)
     ax.spines[['top', 'right']].set_visible(False)
     ax.tick_params(labelsize=8)
-    if verbose:
-        annotator = Annotator(ax, pairs, data=data, x=x, y=y, order=order)
-        annotator.configure(test='t-test_ind',
-                            text_format='star',
-                            loc='inside',
-                            show_test_name=False,
-                            line_width=1)
-        annotator.apply_and_annotate()
-    else:
-        with Silent('stdout'):
-            annotator = Annotator(ax, pairs, data=data, x=x, y=y, order=order)
+    if len(pairs) > 0:
+        if verbose:
+            annotator = Annotator(ax, pairs, data=data, x=x, y=y, order=x_order)
             annotator.configure(test=test,
                                 text_format=text_format,
-                                loc='outside',
+                                loc='inside',
                                 show_test_name=False,
                                 line_width=1)
             annotator.apply_and_annotate()
+        else:
+            with Silent('stdout'):
+                annotator = Annotator(ax, pairs, data=data, x=x, y=y, order=x_order)
+                annotator.configure(test=test,
+                                    text_format=text_format,
+                                    loc='inside',
+                                    show_test_name=False,
+                                    line_width=1)
+                annotator.apply_and_annotate()
     return ax
 
 
 def plot_legend(
     ax,
-    color_map,
+    color_dict,
     ncol=1,
     title='',
     marker='s',
     loc='lower right',
 ):
     """plot legend on an ax.
 
@@ -517,17 +696,58 @@
     Axes
         ax
     """
     from matplotlib.lines import Line2D
 
     # plt.figure(figsize=figsize)
     legend_TN = [
-        Line2D([0], [0], color=color, label=c, marker=marker) for c, color in color_map.items()
+        Line2D([0], [0], color=color, label=c, marker=marker)
+        for c, color in color_dict.items()
     ]
     ax.legend(handles=legend_TN,
               ncol=ncol,
               frameon=False,
               title=title,
               prop={'size': 10},
               loc=loc)
     ax.axis('off')
-    return ax
+    return ax
+
+
+def embedding_region(adata: sc.AnnData,
+                     basis=None,
+                     *,
+                     groupby,
+                     color,
+                     metric='mean',
+                     ax=None,
+                     layer=None,
+                     use_raw=False,
+                     **embedding_kwargs):
+    """plot embedding with color representing metrics of groups
+    """
+    if basis is None:
+        basis = 'X_umap'
+
+    assert metric in ['mean', 'median']
+
+    adata._sanitize()
+    use_raw = _check_use_raw(adata, use_raw)
+    if isinstance(color, str):
+        keys = [color]
+    else:
+        keys = color
+    obs_df = sc.get.obs_df(adata, keys=[groupby] + keys, layer=layer, use_raw=use_raw)
+
+    if metric == 'mean':
+        group_metric = obs_df.groupby(groupby).mean()
+    elif metric == 'median':
+        group_metric = obs_df.groupby(groupby).median()
+    obs_metric = group_metric.loc[obs_df[groupby].values, keys]
+
+    keys = [f'{metric}_{key}_by_{groupby}' for key in keys]
+    obs_metric.columns = keys
+
+    ad = adata.copy()
+    ad.obs = obs_metric
+
+    sc.pl.embedding(ad, basis=basis, color=keys, ax=ax, **embedding_kwargs)
```

### Comparing `anutils-0.4.4/src/anutils/scutils/preprocessing.py` & `anutils-0.4.5/src/anutils/scutils/preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 def rna_preprocess(adata,
                    min_features=150,
                    min_cells=3,
                    pct_counts_mt=20,
                    target_sum=None,
                    log1p=True,
                    n_top_features=None,
+                   batch_key=None,
                    remove_doublets=False,
                    transform=None,
                    inplace=True):
     """
     scRNA-seq data preprocess
     """
     if not inplace:
@@ -68,18 +69,18 @@
 
     sc.pp.normalize_total(adata, target_sum=target_sum)
     if log1p:
         sc.pp.log1p(adata)
     adata.raw = adata
     if n_top_features is not None:
         if type(n_top_features) == int:
-            if n_top_features > 0:
-                sc.pp.highly_variable_genes(adata, n_top_genes=n_top_features, subset=True)
-            else:
-                raise ValueError("Illegal n_top_features input!")
+            sc.pp.highly_variable_genes(adata,
+                                        n_top_genes=n_top_features,
+                                        subset=True,
+                                        batch_key=batch_key)
         elif type(n_top_features) == str:
             n_top_features = np.loadtxt(n_top_features, dtype=str)
             idx = [i for i, g in enumerate(n_top_features) if g in adata.var_names]
             adata = adata[:, idx]
     if transform:
         if sc.settings.verbosity > 1:
             print('transform...')
@@ -121,29 +122,43 @@
     return adata if not inplace else None
 
 
 def qc_glance(ad, groupby=None, rotation=90):
     ad.var['mt'] = ad.var_names.str.startswith(tuple(
         ['ERCC', 'MT-', 'mt-']))  # annotate the group of mitochondrial genes as 'mt'
     sc.pp.calculate_qc_metrics(ad, qc_vars=['mt'], percent_top=None, log1p=True, inplace=True)
-    sc.pl.violin(ad, ['total_counts', 'n_genes_by_counts', 'pct_counts_mt'],
-                 groupby=groupby,
-                 rotation=rotation)
-    sc.pl.violin(ad, ['log1p_total_counts', 'log1p_n_genes_by_counts', 'log1p_total_counts_mt'],
-                 groupby=groupby,
-                 rotation=rotation)
+    qc_plots(ad, groupby=groupby, rotation=rotation)
+
+
+def qc_plots(ad,
+             groupby=None,
+             rotation=90,
+             qc_keys=('total_counts', 'n_genes_by_counts', 'pct_counts_mt'),
+             log1p=True):
+    keys = qc_keys
+    sc.pl.violin(ad, keys, groupby=groupby, rotation=rotation)
+    if log1p:
+        keys = ['log1p_' + key for key in keys]
+        # check keys exist, if not, print message and skip
+        for key in keys:
+            if key not in ad.obs.columns:
+                print(f'key `{key}` not found in `adata.obs.columns`, skip violin plot')
+                break
+        else:
+            sc.pl.violin(ad, keys, groupby=groupby, rotation=rotation)
+
     sc.pl.scatter(ad, x='total_counts', y='n_genes_by_counts', color='pct_counts_mt')
 
 
 def qc_outliers(
-    ad,
-    groupby=None,
-    rotation=90,
-    nmads=5,
-    qc_keys=['log1p_total_counts', 'log1p_n_genes_by_counts', 'log1p_total_counts_mt'],
+        ad,
+        groupby=None,
+        rotation=90,
+        nmads=5,
+        qc_keys=('log1p_total_counts', 'log1p_n_genes_by_counts', 'log1p_total_counts_mt'),
 ):
     """identify outliers with values out of nmads * median absolute deviation (MAD) range
     
     add key `is_outlier` to `adata.obs` and plot violin plots with outliers highlighted
 
     Parameters
     ----------
```

### Comparing `anutils-0.4.4/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt` & `anutils-0.4.5/src/anutils/scutils/resources/gene_sets/regev_lab_cell_cycle_genes.txt`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py` & `anutils-0.4.5/src/anutils/scutils/sc_cuda/rapids_scanpy_funcs.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/sc_cuda/scanpy_cuda.py` & `anutils-0.4.5/src/anutils/scutils/sc_cuda/scanpy_cuda.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/sc_cuda/scib_cuda.py` & `anutils-0.4.5/src/anutils/scutils/sc_cuda/scib_cuda.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils/scutils/utils.py` & `anutils-0.4.5/src/anutils/scutils/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import pandas as pd
+
+
 def filter_batches_with_too_few_samples(adata,
                                         batch_key,
                                         min_samples,
                                         inplace=True,
                                         copy=False,
-                                        verbose=True
-                                        ):
+                                        verbose=True):
     """
     params:
     ---
     adata: AnnData
         AnnData object
     batch_key: str
         key in `adata.obs` to use for batch
@@ -27,7 +29,17 @@
         print(f'Filtering batches with fewer than {min_samples} samples:')
         print(batch_sizes[batch_sizes < min_samples])
     if inplace:
         adata._inplace_subset_obs(adata.obs[batch_key].isin(batches_to_keep))
     else:
         adata = adata[adata.obs[batch_key].isin(batches_to_keep)]
     return adata if copy else None
+
+
+def _get_df_or_adata_obs(data) -> pd.DataFrame:
+    if type(data).__name__ == 'DataFrame':
+        df = data
+    elif type(data).__name__ == 'AnnData':
+        df = data.obs
+    else:
+        raise ValueError('data must be a pandas.DataFrame or an anndata.AnnData')
+    return df
```

### Comparing `anutils-0.4.4/src/anutils/utils.py` & `anutils-0.4.5/src/anutils/utils.py`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/src/anutils.egg-info/PKG-INFO` & `anutils-0.4.5/src/anutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,22 @@
 Metadata-Version: 2.1
 Name: anutils
-Version: 0.4.4
+Version: 0.4.5
 Summary: ml and single cell utils.
 Home-page: https://github.com/AaronNing/anutils
 Author: Aaron Ning
 Author-email: aaronning98@gmail.com
 License: MIT
 Keywords: anutils
 
 anutils
 =======
 
 ML and single cell analysis utils.
 
-installation
-------------
-
-::
-
-   pip install anutils
-
-**NOTE**: To use ``anutils.scutils.sc_cuda``, you need to install rapids
-first. see `rapids.ai <https://rapids.ai/start.html>`__ for details. For
-example, to install rapids on a linux machine with cuda 11, you can run:
-
-.. code:: bash
-
-   pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
-   pip install cuml-cu11 --extra-index-url=https://pypi.nvidia.com
-   pip install cugraph-cu11 --extra-index-url=https://pypi.nvidia.com
-
 usage
 -----
 
 general utils: ``anutils.*``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ``anutls.glimpse`` is similar to ``dplyr::glimpse`` in R, but enhanced
@@ -99,7 +82,24 @@
 -----------------------
 
 .. code:: python
 
    import anutils.mlutils as ml
 
    # to be added
+
+installation
+------------
+
+::
+
+   pip install anutils
+
+**NOTE**: To use ``anutils.scutils.sc_cuda``, you need to install rapids
+first. see `rapids.ai <https://rapids.ai/start.html>`__ for details. For
+example, to install rapids on a linux machine with cuda 11, you can run:
+
+.. code:: bash
+
+   pip install cudf-cu11 dask-cudf-cu11 --extra-index-url=https://pypi.nvidia.com
+   pip install cuml-cu11 --extra-index-url=https://pypi.nvidia.com
+   pip install cugraph-cu11 --extra-index-url=https://pypi.nvidia.com
```

### Comparing `anutils-0.4.4/src/anutils.egg-info/SOURCES.txt` & `anutils-0.4.5/src/anutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anutils-0.4.4/tests/run_tests.py` & `anutils-0.4.5/tests/run_tests.py`

 * *Files identical despite different names*

