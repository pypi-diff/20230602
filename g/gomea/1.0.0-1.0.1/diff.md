# Comparing `tmp/gomea-1.0.0.tar.gz` & `tmp/gomea-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gomea-1.0.0.tar", last modified: Wed May 10 09:48:55 2023, max compression
+gzip compressed data, was "gomea-1.0.1.tar", last modified: Thu Jun  1 20:45:10 2023, max compression
```

## Comparing `gomea-1.0.0.tar` & `gomea-1.0.1.tar`

### file list

```diff
@@ -1,70 +1,458 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.127649 gomea-1.0.0/
--rw-r--r--   0 runner     (501) staff       (20)     1069 2023-05-10 09:47:57.000000 gomea-1.0.0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       94 2023-05-10 09:47:57.000000 gomea-1.0.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)      681 2023-05-10 09:48:55.127199 gomea-1.0.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      358 2023-05-10 09:47:57.000000 gomea-1.0.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.102932 gomea-1.0.0/gomea/
--rw-r--r--   0 runner     (501) staff       (20)     5009 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/EmbeddedFitness.pxi
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/__init__.pxd
--rw-r--r--   0 runner     (501) staff       (20)      255 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1961 2023-05-10 09:48:48.000000 gomea-1.0.0/gomea/discrete.h
--rw-r--r--   0 runner     (501) staff       (20)     1064 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/discrete.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3812 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/discrete.pyx
--rw-r--r--   0 runner     (501) staff       (20)     1954 2023-05-10 09:48:50.000000 gomea-1.0.0/gomea/fitness.h
--rw-r--r--   0 runner     (501) staff       (20)     5364 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/fitness.pxd
--rw-r--r--   0 runner     (501) staff       (20)     9720 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/fitness.pyx
--rw-r--r--   0 runner     (501) staff       (20)      916 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/linkage.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3195 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/linkage.pyx
--rw-r--r--   0 runner     (501) staff       (20)      523 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/output.pxd
--rw-r--r--   0 runner     (501) staff       (20)     2038 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/output.pyx
--rw-r--r--   0 runner     (501) staff       (20)     1982 2023-05-10 09:48:54.000000 gomea-1.0.0/gomea/real_valued.h
--rw-r--r--   0 runner     (501) staff       (20)     1289 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/real_valued.pxd
--rw-r--r--   0 runner     (501) staff       (20)     3413 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/real_valued.pyx
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.091211 gomea-1.0.0/gomea/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.110506 gomea-1.0.0/gomea/src/common/
--rw-r--r--   0 runner     (501) staff       (20)      537 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/common/gomea_defs.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1365 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/common/linkage_config.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4312 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/common/linkage_model.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1108 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/common/output_statistics.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1662 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/common/partial_solution.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2771 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/common/solution.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.115224 gomea-1.0.0/gomea/src/discrete/
--rw-r--r--   0 runner     (501) staff       (20)     2022 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/discrete/Config.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1927 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/discrete/Population.hpp
--rw-r--r--   0 runner     (501) staff       (20)      251 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/discrete/gomea.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1784 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/discrete/gomeaIMS.hpp
--rw-r--r--   0 runner     (501) staff       (20)      793 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/discrete/shared.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1516 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/discrete/utils.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.120354 gomea-1.0.0/gomea/src/fitness/
--rw-r--r--   0 runner     (501) staff       (20)      962 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/bbo_fitness.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2112 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/benchmarks-discrete.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2194 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/benchmarks-rv.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3810 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/fitness.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1786 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/gbo_fitness.hpp
--rw-r--r--   0 runner     (501) staff       (20)      711 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/py_bbo_fitness.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1046 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/py_gbo_fitness.hpp
--rw-r--r--   0 runner     (501) staff       (20)      454 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/your_fitness_discrete.hpp
--rw-r--r--   0 runner     (501) staff       (20)      533 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/fitness/your_fitness_realvalued.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.124988 gomea-1.0.0/gomea/src/real_valued/
--rw-r--r--   0 runner     (501) staff       (20)     3406 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/real_valued/Config.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5364 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/real_valued/distribution.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5242 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/real_valued/linkage_model.hpp
--rw-r--r--   0 runner     (501) staff       (20)      791 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/real_valued/partial_solutionRV.hpp
--rw-r--r--   0 runner     (501) staff       (20)     4373 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/real_valued/population.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3237 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/real_valued/rv-gomea.hpp
--rw-r--r--   0 runner     (501) staff       (20)      451 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/real_valued/solutionRV.hpp
--rw-r--r--   0 runner     (501) staff       (20)     2779 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/real_valued/tools.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.126587 gomea-1.0.0/gomea/src/utils/
--rw-r--r--   0 runner     (501) staff       (20)      235 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/utils/embed.hpp
--rw-r--r--   0 runner     (501) staff       (20)      914 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/utils/time.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1206 2023-05-10 09:47:57.000000 gomea-1.0.0/gomea/src/utils/tools.hpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-05-10 09:48:55.106330 gomea-1.0.0/gomea.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      681 2023-05-10 09:48:55.000000 gomea-1.0.0/gomea.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1638 2023-05-10 09:48:55.000000 gomea-1.0.0/gomea.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-10 09:48:55.000000 gomea-1.0.0/gomea.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-05-10 09:48:54.000000 gomea-1.0.0/gomea.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)       19 2023-05-10 09:48:55.000000 gomea-1.0.0/gomea.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2023-05-10 09:48:55.000000 gomea-1.0.0/gomea.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      118 2023-05-10 09:47:57.000000 gomea-1.0.0/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-05-10 09:48:55.127755 gomea-1.0.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3833 2023-05-10 09:47:57.000000 gomea-1.0.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.911494 gomea-1.0.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1069 2023-06-01 20:44:17.000000 gomea-1.0.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      112 2023-06-01 20:44:17.000000 gomea-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     4242 2023-06-01 20:45:10.911038 gomea-1.0.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3919 2023-06-01 20:44:17.000000 gomea-1.0.1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.635284 gomea-1.0.1/gomea/
+-rw-r--r--   0 runner     (501) staff       (20)     5009 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/EmbeddedFitness.pxi
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/__init__.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      255 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1064 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/discrete.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3812 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/discrete.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     5364 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/fitness.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     9720 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/fitness.pyx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.591026 gomea-1.0.1/gomea/lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.664872 gomea-1.0.1/gomea/lib/Eigen/
+-rw-r--r--   0 runner     (501) staff       (20)     1161 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Cholesky
+-rw-r--r--   0 runner     (501) staff       (20)     1900 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/CholmodSupport
+-rw-r--r--   0 runner     (501) staff       (20)    12799 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Core
+-rw-r--r--   0 runner     (501) staff       (20)      122 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Dense
+-rw-r--r--   0 runner     (501) staff       (20)       35 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Eigen
+-rw-r--r--   0 runner     (501) staff       (20)     1777 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Eigenvalues
+-rw-r--r--   0 runner     (501) staff       (20)     1940 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Geometry
+-rw-r--r--   0 runner     (501) staff       (20)      829 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Householder
+-rw-r--r--   0 runner     (501) staff       (20)     2083 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner     (501) staff       (20)      894 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Jacobi
+-rw-r--r--   0 runner     (501) staff       (20)     1389 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/KLUSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1268 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/LU
+-rw-r--r--   0 runner     (501) staff       (20)      991 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/MetisSupport
+-rw-r--r--   0 runner     (501) staff       (20)     2451 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/OrderingMethods
+-rw-r--r--   0 runner     (501) staff       (20)     1751 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/PaStiXSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1116 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/PardisoSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1272 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/QR
+-rw-r--r--   0 runner     (501) staff       (20)      900 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner     (501) staff       (20)     1162 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/SPQRSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1584 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/SVD
+-rw-r--r--   0 runner     (501) staff       (20)      888 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/Sparse
+-rw-r--r--   0 runner     (501) staff       (20)     1235 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/SparseCholesky
+-rw-r--r--   0 runner     (501) staff       (20)     2240 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/SparseCore
+-rw-r--r--   0 runner     (501) staff       (20)     1814 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/SparseLU
+-rw-r--r--   0 runner     (501) staff       (20)     1195 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/SparseQR
+-rw-r--r--   0 runner     (501) staff       (20)      797 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/StdDeque
+-rw-r--r--   0 runner     (501) staff       (20)      726 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/StdList
+-rw-r--r--   0 runner     (501) staff       (20)      803 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/StdVector
+-rw-r--r--   0 runner     (501) staff       (20)     2243 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/SuperLUSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1382 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.590779 gomea-1.0.1/gomea/lib/Eigen/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.666592 gomea-1.0.1/gomea/lib/Eigen/src/Cholesky/
+-rw-r--r--   0 runner     (501) staff       (20)    24934 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner     (501) staff       (20)    18760 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner     (501) staff       (20)     3974 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.667232 gomea-1.0.1/gomea/lib/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    25441 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.721477 gomea-1.0.1/gomea/lib/Eigen/src/Core/
+-rw-r--r--   0 runner     (501) staff       (20)    19214 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner     (501) staff       (20)    16782 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner     (501) staff       (20)     8217 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7018 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner     (501) staff       (20)     2738 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner     (501) staff       (20)    41673 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    12488 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner     (501) staff       (20)    14075 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    18648 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner     (501) staff       (20)     4429 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner     (501) staff       (20)     5981 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner     (501) staff       (20)     6990 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner     (501) staff       (20)    63841 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner     (501) staff       (20)     4745 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner     (501) staff       (20)     7909 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)    36282 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     8256 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     3937 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     5551 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner     (501) staff       (20)    31529 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    24484 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    25360 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner     (501) staff       (20)     9870 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner     (501) staff       (20)    14670 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)      988 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)    11654 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner     (501) staff       (20)     5841 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     4909 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner     (501) staff       (20)     5759 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner     (501) staff       (20)    21679 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)    38812 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    11543 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)     8238 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner     (501) staff       (20)     9620 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner     (501) staff       (20)     3503 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner     (501) staff       (20)     7256 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner     (501) staff       (20)    11281 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    60784 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)     7156 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)    24343 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    23856 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     2520 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner     (501) staff       (20)     3620 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner     (501) staff       (20)    12884 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner     (501) staff       (20)     9207 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner     (501) staff       (20)    20748 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    49193 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7336 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner     (501) staff       (20)    53832 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner     (501) staff       (20)     7756 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner     (501) staff       (20)    19195 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner     (501) staff       (20)    17821 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner     (501) staff       (20)     5656 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner     (501) staff       (20)    17033 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner     (501) staff       (20)     4284 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner     (501) staff       (20)     7522 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner     (501) staff       (20)     6143 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner     (501) staff       (20)    14999 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner     (501) staff       (20)     1697 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     6837 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner     (501) staff       (20)     9368 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner     (501) staff       (20)     6170 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     8700 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner     (501) staff       (20)    21641 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner     (501) staff       (20)     4212 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner     (501) staff       (20)     2765 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner     (501) staff       (20)    17606 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner     (501) staff       (20)    13567 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner     (501) staff       (20)    38277 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     3488 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner     (501) staff       (20)    35168 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner     (501) staff       (20)    11997 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.569591 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.724560 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner     (501) staff       (20)    15223 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     8102 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    64608 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     2564 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.727365 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner     (501) staff       (20)    17160 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    13344 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    87891 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     2134 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.731599 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner     (501) staff       (20)    16540 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     2323 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)   119355 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     9490 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner     (501) staff       (20)    24820 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxr-xr-x   0 runner     (501) staff       (20)   102394 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.732457 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner     (501) staff       (20)    17317 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/CUDA/Complex.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.737854 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner     (501) staff       (20)    26903 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner     (501) staff       (20)     5251 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner     (501) staff       (20)    67696 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)     3770 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner     (501) staff       (20)    35534 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner     (501) staff       (20)     1746 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner     (501) staff       (20)     3746 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.740929 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner     (501) staff       (20)     2695 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    57047 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     2256 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.566110 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.741812 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner     (501) staff       (20)      691 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.744120 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner     (501) staff       (20)    17541 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    16159 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    33615 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.748501 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner     (501) staff       (20)    22503 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     6815 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner     (501) staff       (20)     3083 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)   189525 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    51286 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.751300 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner     (501) staff       (20)    14251 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     6765 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    64465 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.753179 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    21200 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     1351 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.758473 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner     (501) staff       (20)     7428 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner     (501) staff       (20)    12539 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    27786 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    21856 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner     (501) staff       (20)     2626 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.760296 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner     (501) staff       (20)    16728 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     8024 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    36894 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.765097 gomea-1.0.1/gomea/lib/Eigen/src/Core/functors/
+-rw-r--r--   0 runner     (501) staff       (20)     6686 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)    20921 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)     8334 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)     4998 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)      607 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)    40146 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.779805 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/
+-rw-r--r--   0 runner     (501) staff       (20)   108448 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner     (501) staff       (20)    20104 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    15948 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner     (501) staff       (20)     6936 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     5106 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    21724 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     6368 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     5582 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner     (501) staff       (20)    21354 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    11570 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     9958 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     5209 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     6164 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     4126 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner     (501) staff       (20)    20987 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    13867 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    14722 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)    10571 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    14678 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     6707 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     5882 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.791178 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner     (501) staff       (20)    23156 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner     (501) staff       (20)    19876 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner     (501) staff       (20)    21931 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     4892 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner     (501) staff       (20)    15555 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner     (501) staff       (20)     6696 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner     (501) staff       (20)    10949 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/IntegralConstant.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     4268 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner     (501) staff       (20)    52909 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner     (501) staff       (20)    46661 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    29336 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner     (501) staff       (20)       85 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner     (501) staff       (20)     1024 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner     (501) staff       (20)     1432 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner     (501) staff       (20)    10676 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner     (501) staff       (20)    12003 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner     (501) staff       (20)    35762 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.800246 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner     (501) staff       (20)    12559 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    17274 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner     (501) staff       (20)     4178 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    22970 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    17176 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)     9716 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    14349 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner     (501) staff       (20)     5575 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner     (501) staff       (20)    23640 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner     (501) staff       (20)    21078 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    35182 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)     4104 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    22764 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.808884 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/
+-rw-r--r--   0 runner     (501) staff       (20)    18939 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner     (501) staff       (20)     8403 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner     (501) staff       (20)     3624 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner     (501) staff       (20)    20726 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner     (501) staff       (20)    11962 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner     (501) staff       (20)     8955 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner     (501) staff       (20)     9812 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner     (501) staff       (20)    34367 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner     (501) staff       (20)     6862 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner     (501) staff       (20)     8063 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     6724 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner     (501) staff       (20)    61930 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner     (501) staff       (20)     7664 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner     (501) staff       (20)     6190 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.809386 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner     (501) staff       (20)     5945 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Geometry/arch/Geometry_SIMD.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.811426 gomea-1.0.1/gomea/lib/Eigen/src/Householder/
+-rw-r--r--   0 runner     (501) staff       (20)     4784 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner     (501) staff       (20)     5365 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner     (501) staff       (20)    23611 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.816704 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner     (501) staff       (20)     6771 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner     (501) staff       (20)     6850 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner     (501) staff       (20)     8887 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner     (501) staff       (20)    15036 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner     (501) staff       (20)    14940 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner     (501) staff       (20)    13379 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7349 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner     (501) staff       (20)     4212 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.817370 gomea-1.0.1/gomea/lib/Eigen/src/Jacobi/
+-rw-r--r--   0 runner     (501) staff       (20)    16383 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.817944 gomea-1.0.1/gomea/lib/Eigen/src/KLUSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    11555 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.822867 gomea-1.0.1/gomea/lib/Eigen/src/LU/
+-rw-r--r--   0 runner     (501) staff       (20)     3439 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner     (501) staff       (20)    32383 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner     (501) staff       (20)    15727 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)    22069 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner     (501) staff       (20)     3555 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.823480 gomea-1.0.1/gomea/lib/Eigen/src/LU/arch/
+-rw-r--r--   0 runner     (501) staff       (20)    13693 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/LU/arch/InverseSize4.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.824029 gomea-1.0.1/gomea/lib/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner     (501) staff       (20)     4588 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.826252 gomea-1.0.1/gomea/lib/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner     (501) staff       (20)    16105 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner     (501) staff       (20)    61681 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner     (501) staff       (20)     5248 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.826791 gomea-1.0.1/gomea/lib/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    22249 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.827756 gomea-1.0.1/gomea/lib/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    20092 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.832828 gomea-1.0.1/gomea/lib/Eigen/src/QR/
+-rw-r--r--   0 runner     (501) staff       (20)    25498 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)     4662 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    23429 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner     (501) staff       (20)    26768 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)    14641 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)     2993 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.833788 gomea-1.0.1/gomea/lib/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    11826 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.837934 gomea-1.0.1/gomea/lib/Eigen/src/SVD/
+-rw-r--r--   0 runner     (501) staff       (20)    54214 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner     (501) staff       (20)    32988 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner     (501) staff       (20)     5099 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    14743 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    15957 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.839612 gomea-1.0.1/gomea/lib/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner     (501) staff       (20)    24216 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner     (501) staff       (20)     5830 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.859218 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/
+-rw-r--r--   0 runner     (501) staff       (20)    10670 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     8743 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner     (501) staff       (20)    13166 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     2191 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    11368 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner     (501) staff       (20)    24360 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner     (501) staff       (20)     6485 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner     (501) staff       (20)    13606 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    25524 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     4757 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)    13256 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     5808 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     3080 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner     (501) staff       (20)     1107 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner     (501) staff       (20)    12589 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner     (501) staff       (20)    57475 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    17451 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7329 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner     (501) staff       (20)     7593 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     1699 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner     (501) staff       (20)    15600 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner     (501) staff       (20)    25889 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner     (501) staff       (20)     4424 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     8704 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner     (501) staff       (20)     3175 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner     (501) staff       (20)     6437 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner     (501) staff       (20)     6827 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner     (501) staff       (20)    14832 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     8127 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner     (501) staff       (20)     9657 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.870460 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/
+-rw-r--r--   0 runner     (501) staff       (20)    33316 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner     (501) staff       (20)     4303 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)     7602 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner     (501) staff       (20)    12837 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     2049 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner     (501) staff       (20)     6712 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     6584 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner     (501) staff       (20)     3681 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner     (501) staff       (20)    10217 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner     (501) staff       (20)     4181 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner     (501) staff       (20)     5723 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     8485 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     9028 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner     (501) staff       (20)     4979 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner     (501) staff       (20)     4545 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.871093 gomea-1.0.1/gomea/lib/Eigen/src/SparseQR/
+-rw-r--r--   0 runner     (501) staff       (20)    29167 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.873211 gomea-1.0.1/gomea/lib/Eigen/src/StlSupport/
+-rw-r--r--   0 runner     (501) staff       (20)     4730 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner     (501) staff       (20)     4155 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner     (501) staff       (20)     5338 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     2809 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.873752 gomea-1.0.1/gomea/lib/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    34324 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.874453 gomea-1.0.1/gomea/lib/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    24456 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.882655 gomea-1.0.1/gomea/lib/Eigen/src/misc/
+-rw-r--r--   0 runner     (501) staff       (20)     2913 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner     (501) staff       (20)     2742 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner     (501) staff       (20)     1748 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner     (501) staff       (20)    30560 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner     (501) staff       (20)     7834 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner     (501) staff       (20)  1058369 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner     (501) staff       (20)      474 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.888398 gomea-1.0.1/gomea/lib/Eigen/src/plugins/
+-rw-r--r--   0 runner     (501) staff       (20)    14060 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)    21431 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)    59020 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner     (501) staff       (20)     4828 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     6089 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)    12283 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner     (501) staff       (20)     6387 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     3350 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     6915 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/Eigen/src/plugins/ReshapedMethods.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.889618 gomea-1.0.1/gomea/lib/cxxopts-3.1.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1055 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/cxxopts-3.1.1/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     8555 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/cxxopts-3.1.1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.890136 gomea-1.0.1/gomea/lib/cxxopts-3.1.1/include/
+-rw-r--r--   0 runner     (501) staff       (20)    57387 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/lib/cxxopts-3.1.1/include/cxxopts.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      916 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/linkage.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3195 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/linkage.pyx
+-rw-r--r--   0 runner     (501) staff       (20)      523 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/output.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2038 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/output.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     1289 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/real_valued.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3413 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/real_valued.pyx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.596065 gomea-1.0.1/gomea/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.893757 gomea-1.0.1/gomea/src/common/
+-rw-r--r--   0 runner     (501) staff       (20)      537 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/common/gomea_defs.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1365 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/common/linkage_config.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4312 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/common/linkage_model.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1108 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/common/output_statistics.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1662 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/common/partial_solution.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2771 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/common/solution.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.898108 gomea-1.0.1/gomea/src/discrete/
+-rw-r--r--   0 runner     (501) staff       (20)     2022 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/discrete/Config.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1927 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/discrete/Population.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      251 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/discrete/gomea.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1784 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/discrete/gomeaIMS.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      793 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/discrete/shared.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1516 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/discrete/utils.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.903708 gomea-1.0.1/gomea/src/fitness/
+-rw-r--r--   0 runner     (501) staff       (20)      962 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/bbo_fitness.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2112 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/benchmarks-discrete.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2194 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/benchmarks-rv.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3810 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/fitness.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1786 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/gbo_fitness.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      711 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/py_bbo_fitness.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1046 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/py_gbo_fitness.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      454 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/your_fitness_discrete.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      533 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/fitness/your_fitness_realvalued.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.908602 gomea-1.0.1/gomea/src/real_valued/
+-rw-r--r--   0 runner     (501) staff       (20)     3406 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/real_valued/Config.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5364 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/real_valued/distribution.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5242 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/real_valued/linkage_model.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      791 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/real_valued/partial_solutionRV.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     4373 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/real_valued/population.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3237 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/real_valued/rv-gomea.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      451 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/real_valued/solutionRV.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     2779 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/real_valued/tools.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.910397 gomea-1.0.1/gomea/src/utils/
+-rw-r--r--   0 runner     (501) staff       (20)      235 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/utils/embed.hpp
+-rw-r--r--   0 runner     (501) staff       (20)      914 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/utils/time.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1206 2023-06-01 20:44:17.000000 gomea-1.0.1/gomea/src/utils/tools.hpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-06-01 20:45:10.646760 gomea-1.0.1/gomea.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     4242 2023-06-01 20:45:10.000000 gomea-1.0.1/gomea.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    16938 2023-06-01 20:45:10.000000 gomea-1.0.1/gomea.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-01 20:45:10.000000 gomea-1.0.1/gomea.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-06-01 20:45:09.000000 gomea-1.0.1/gomea.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)       19 2023-06-01 20:45:10.000000 gomea-1.0.1/gomea.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2023-06-01 20:45:10.000000 gomea-1.0.1/gomea.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      118 2023-06-01 20:44:17.000000 gomea-1.0.1/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-06-01 20:45:10.911606 gomea-1.0.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3774 2023-06-01 20:44:17.000000 gomea-1.0.1/setup.py
```

### Comparing `gomea-1.0.0/LICENSE` & `gomea-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/EmbeddedFitness.pxi` & `gomea-1.0.1/gomea/EmbeddedFitness.pxi`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/discrete.pxd` & `gomea-1.0.1/gomea/discrete.pxd`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/discrete.pyx` & `gomea-1.0.1/gomea/discrete.pyx`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/fitness.pxd` & `gomea-1.0.1/gomea/fitness.pxd`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/fitness.pyx` & `gomea-1.0.1/gomea/fitness.pyx`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/linkage.pxd` & `gomea-1.0.1/gomea/linkage.pxd`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/linkage.pyx` & `gomea-1.0.1/gomea/linkage.pyx`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/output.pxd` & `gomea-1.0.1/gomea/output.pxd`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/output.pyx` & `gomea-1.0.1/gomea/output.pyx`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/real_valued.pxd` & `gomea-1.0.1/gomea/real_valued.pxd`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/real_valued.pyx` & `gomea-1.0.1/gomea/real_valued.pyx`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/common/gomea_defs.hpp` & `gomea-1.0.1/gomea/src/common/gomea_defs.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/common/linkage_config.hpp` & `gomea-1.0.1/gomea/src/common/linkage_config.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/common/linkage_model.hpp` & `gomea-1.0.1/gomea/src/common/linkage_model.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/common/output_statistics.hpp` & `gomea-1.0.1/gomea/src/common/output_statistics.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/common/partial_solution.hpp` & `gomea-1.0.1/gomea/src/common/partial_solution.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/common/solution.hpp` & `gomea-1.0.1/gomea/src/common/solution.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/discrete/Config.hpp` & `gomea-1.0.1/gomea/src/discrete/Config.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/discrete/Population.hpp` & `gomea-1.0.1/gomea/src/discrete/Population.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/discrete/gomeaIMS.hpp` & `gomea-1.0.1/gomea/src/discrete/gomeaIMS.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/discrete/shared.hpp` & `gomea-1.0.1/gomea/src/discrete/shared.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/discrete/utils.hpp` & `gomea-1.0.1/gomea/src/discrete/utils.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/fitness/bbo_fitness.hpp` & `gomea-1.0.1/gomea/src/fitness/bbo_fitness.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/fitness/benchmarks-discrete.hpp` & `gomea-1.0.1/gomea/src/fitness/benchmarks-discrete.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/fitness/benchmarks-rv.hpp` & `gomea-1.0.1/gomea/src/fitness/benchmarks-rv.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/fitness/fitness.hpp` & `gomea-1.0.1/gomea/src/fitness/fitness.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/fitness/gbo_fitness.hpp` & `gomea-1.0.1/gomea/src/fitness/gbo_fitness.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/fitness/py_bbo_fitness.hpp` & `gomea-1.0.1/gomea/src/fitness/py_bbo_fitness.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/fitness/py_gbo_fitness.hpp` & `gomea-1.0.1/gomea/src/fitness/py_gbo_fitness.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/fitness/your_fitness_realvalued.hpp` & `gomea-1.0.1/gomea/src/fitness/your_fitness_realvalued.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/real_valued/Config.hpp` & `gomea-1.0.1/gomea/src/real_valued/Config.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/real_valued/distribution.hpp` & `gomea-1.0.1/gomea/src/real_valued/distribution.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/real_valued/linkage_model.hpp` & `gomea-1.0.1/gomea/src/real_valued/linkage_model.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/real_valued/partial_solutionRV.hpp` & `gomea-1.0.1/gomea/src/real_valued/partial_solutionRV.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/real_valued/population.hpp` & `gomea-1.0.1/gomea/src/real_valued/population.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/real_valued/rv-gomea.hpp` & `gomea-1.0.1/gomea/src/real_valued/rv-gomea.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/real_valued/tools.hpp` & `gomea-1.0.1/gomea/src/real_valued/tools.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/utils/time.hpp` & `gomea-1.0.1/gomea/src/utils/time.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/gomea/src/utils/tools.hpp` & `gomea-1.0.1/gomea/src/utils/tools.hpp`

 * *Files identical despite different names*

### Comparing `gomea-1.0.0/setup.py` & `gomea-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 VERSION_MAJOR = 1
 VERSION_MINOR = 0
-VERSION_PATCH = 0
+VERSION_PATCH = 1
 VERSION_STRING = '%s.%s.%s' % (VERSION_MAJOR, VERSION_MINOR, VERSION_PATCH)
 __version__ = VERSION_STRING
 
 from setuptools import Extension, setup, find_namespace_packages
 from Cython.Build import cythonize
 import sys
 import glob
@@ -46,23 +46,23 @@
                 compile_args.extend(['/O2'])
                 link_args.extend(['/O2'])
 
 extensions = []
 
 extensions.append( Extension("gomea.discrete",
         ["gomea/discrete.pyx"] + glob.glob("gomea/src/discrete/*.cpp") + common_src + fitness_src,
-        include_dirs = ["."] + ["lib/cxxopts-3.1.1/include/"] + [np.get_include()],
+        include_dirs = ["."] + ["gomea/lib/cxxopts-3.1.1/include/"] + [np.get_include()],
         language="c++",
         extra_compile_args=compile_args,
         extra_link_args=link_args)
 )
 
 extensions.append( Extension("gomea.real_valued",
         ["gomea/real_valued.pyx"] + glob.glob("gomea/src/real_valued/*.cpp") + common_src + fitness_src,
-        include_dirs = ["."] + ["lib/Eigen"] + [np.get_include()],
+        include_dirs = ["."] + ["gomea/lib/Eigen"] + [np.get_include()],
         language="c++",
         extra_compile_args=compile_args,
         extra_link_args=link_args,
         library_dirs=[],
         extra_objects=[])
 )
 
@@ -96,20 +96,17 @@
     author = 'Anton Bouter',
     author_email = 'Anton.Bouter@cwi.nl',
     url = 'https://github.com/abouter/gomea',
     version = __version__,
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages=["gomea"],
+    include_package_data=True,
     include_dirs=["gomea"],
     ext_modules = cythonize(extensions,
         include_path = ["."] + [np.get_include()],
         gdb_debug = debug_mode,
         language_level = "3"),
     install_requires=["numpy>=1.23.0","tqdm"],
-    include_package_data=True,
-    package_data = {
-        'gomea': ['*.pxd', '*.hpp', '*.h']
-    },
     zip_safe = False
 )
```

