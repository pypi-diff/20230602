# Comparing `tmp/pyoscode-1.0.2.tar.gz` & `tmp/pyoscode-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyoscode-1.0.2.tar", last modified: Thu Dec  3 16:53:47 2020, max compression
+gzip compressed data, was "pyoscode-1.1.2.tar", last modified: Thu Jun  1 22:07:19 2023, max compression
```

## Comparing `pyoscode-1.0.2.tar` & `pyoscode-1.1.2.tar`

### file list

```diff
@@ -1,365 +1,415 @@
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.649786 pyoscode-1.0.2/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)       84 2020-12-03 15:27:24.000000 pyoscode-1.0.2/MANIFEST.in
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    11883 2020-12-03 16:53:47.649786 pyoscode-1.0.2/PKG-INFO
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8559 2020-12-03 16:53:29.000000 pyoscode-1.0.2/README.rst
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.525786 pyoscode-1.0.2/include/
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.533785 pyoscode-1.0.2/include/Eigen/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1129 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Cholesky
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1900 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/CholmodSupport
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17361 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Core
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      122 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Dense
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)       35 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Eigen
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1763 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Eigenvalues
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2050 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Geometry
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      874 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Householder
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2083 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/IterativeLinearSolvers
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      939 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Jacobi
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1374 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/LU
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      991 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/MetisSupport
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2483 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/OrderingMethods
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1676 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/PaStiXSupport
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1116 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/PardisoSupport
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1258 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/QR
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      940 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/QtAlignedMalloc
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1162 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/SPQRSupport
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1570 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/SVD
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      919 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/Sparse
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1371 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/SparseCholesky
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2240 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/SparseCore
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1713 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/SparseLU
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1222 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/SparseQR
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      797 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/StdDeque
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      726 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/StdList
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      803 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/StdVector
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2243 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/SuperLUSupport
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1382 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/UmfPackSupport
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.525786 pyoscode-1.0.2/include/Eigen/src/
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.537785 pyoscode-1.0.2/include/Eigen/src/Cholesky/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    24254 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Cholesky/LDLT.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17834 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Cholesky/LLT.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3974 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.537785 pyoscode-1.0.2/include/Eigen/src/CholmodSupport/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    22307 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.585786 pyoscode-1.0.2/include/Eigen/src/Core/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12218 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Array.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8179 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/ArrayBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6775 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/ArrayWrapper.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2720 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Assign.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    38120 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/AssignEvaluator.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12221 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Assign_MKL.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    13910 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/BandMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    18064 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Block.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4249 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/BooleanRedux.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5689 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/CommaInitializer.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6970 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/ConditionEstimator.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    61293 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/CoreEvaluators.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4525 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/CoreIterators.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7593 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/CwiseBinaryOp.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    31424 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/CwiseNullaryOp.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8256 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/CwiseTernaryOp.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3877 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/CwiseUnaryOp.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5282 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/CwiseUnaryView.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    27420 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/DenseBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    24212 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/DenseCoeffsBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    21959 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/DenseStorage.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9507 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Diagonal.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12666 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/DiagonalMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      970 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/DiagonalProduct.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    11392 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Dot.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5619 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/EigenBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4769 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/ForceAlignedAccess.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5705 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Fuzzy.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    21119 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/GeneralProduct.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    22185 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/GenericPacketMath.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10222 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/GlobalFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7076 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/IO.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3519 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Inverse.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6655 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Map.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10621 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/MapBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    40859 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/MathFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2776 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/MathFunctionsImpl.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    19170 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Matrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    22375 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/MatrixBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3400 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/NestByValue.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3582 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/NoAlias.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9234 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/NumTraits.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    21646 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/PermutationMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    45040 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/PlainObjectBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7149 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Product.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    48917 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/ProductEvaluators.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6379 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Random.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17832 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Redux.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12729 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Ref.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5595 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Replicate.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4200 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/ReturnByValue.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7073 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Reverse.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6020 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Select.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14135 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/SelfAdjointView.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1909 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6795 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Solve.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9031 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/SolveTriangular.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4365 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/SolverBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7686 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/StableNorm.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3865 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Stride.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2683 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Swap.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14777 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Transpose.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14396 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Transpositions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    37234 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/TriangularMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3462 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/VectorBlock.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    29441 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/VectorwiseOp.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8074 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/Visitor.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.525786 pyoscode-1.0.2/include/Eigen/src/Core/arch/
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.585786 pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    19305 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/Complex.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17776 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    27570 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1194 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.589786 pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX512/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15827 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    50915 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.589786 pyoscode-1.0.2/include/Eigen/src/Core/arch/AltiVec/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17722 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10797 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    37102 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.601786 pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4240 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/Complex.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    21057 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/Half.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2387 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10744 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    35462 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5509 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.601786 pyoscode-1.0.2/include/Eigen/src/Core/arch/Default/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1746 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/Default/Settings.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.601786 pyoscode-1.0.2/include/Eigen/src/Core/arch/NEON/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17570 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/NEON/Complex.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2846 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    27880 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.601786 pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    20720 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/Complex.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    18888 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/MathFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    35047 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1726 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.605786 pyoscode-1.0.2/include/Eigen/src/Core/arch/ZVector/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15259 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/ZVector/Complex.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4418 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    32283 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.605786 pyoscode-1.0.2/include/Eigen/src/Core/functors/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6284 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    18081 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/functors/BinaryFunctors.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8229 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/functors/NullaryFunctors.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4184 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/functors/StlFunctors.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      607 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/functors/TernaryFunctors.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    27944 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/functors/UnaryFunctors.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.609786 pyoscode-1.0.2/include/Eigen/src/Core/products/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    81106 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    18478 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15188 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6746 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4730 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    26736 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6053 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4905 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/Parallelizer.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    19632 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10614 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9901 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4903 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6105 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointProduct.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4066 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    19345 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    13238 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14216 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9895 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    13979 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6024 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5741 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularSolverVector.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.613786 pyoscode-1.0.2/include/Eigen/src/Core/util/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15722 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/BlasUtil.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    21579 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/Constants.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3564 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14150 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/ForwardDeclarations.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3970 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/MKL_support.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    36377 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/Macros.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    39712 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/Memory.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    18481 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/Meta.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)       85 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/NonMPL2.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      809 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10284 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/StaticAssert.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    34198 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Core/util/XprHelper.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.617786 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12558 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17021 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4178 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    22944 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/EigenSolver.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17191 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9715 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14351 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5679 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    23586 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/RealQZ.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    20268 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/RealSchur.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3650 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    33674 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4378 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    22444 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.617786 pyoscode-1.0.2/include/Eigen/src/Geometry/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14815 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/AlignedBox.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8415 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/AngleAxis.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3639 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/EulerAngles.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    20539 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/Homogeneous.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    11961 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/Hyperplane.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8949 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/OrthoMethods.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8308 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/ParametrizedLine.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    31688 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/Quaternion.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6877 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/Rotation2D.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8063 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/RotationBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6324 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/Scaling.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    60514 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/Transform.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7773 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/Translation.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6191 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/Umeyama.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.617786 pyoscode-1.0.2/include/Eigen/src/Geometry/arch/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5387 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.617786 pyoscode-1.0.2/include/Eigen/src/Householder/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4481 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Householder/BlockHouseholder.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5345 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Householder/Householder.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    20603 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Householder/HouseholderSequence.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6763 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7253 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9184 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15062 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15234 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    11527 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7762 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4158 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/Jacobi/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14888 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/Jacobi/Jacobi.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/LU/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3057 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/LU/Determinant.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    32803 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/LU/FullPivLU.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15068 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/LU/InverseImpl.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    21478 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/LU/PartialPivLU.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3555 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/LU/arch/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    13669 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/LU/arch/Inverse_SSE.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/MetisSupport/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4588 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/MetisSupport/MetisSupport.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/OrderingMethods/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    16396 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/OrderingMethods/Amd.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    62266 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5229 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/OrderingMethods/Ordering.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/PaStiXSupport/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    22220 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/PardisoSupport/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    20032 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/QR/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    24881 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/QR/ColPivHouseholderQR.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4662 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    20805 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    25478 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/QR/FullPivHouseholderQR.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14022 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/QR/HouseholderQR.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2993 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.621786 pyoscode-1.0.2/include/Eigen/src/SPQRSupport/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    11405 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.629786 pyoscode-1.0.2/include/Eigen/src/SVD/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    47664 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SVD/BDCSVD.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    32949 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SVD/JacobiSVD.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5009 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12650 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SVD/SVDBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15957 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SVD/UpperBidiagonalization.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.629786 pyoscode-1.0.2/include/Eigen/src/SparseCholesky/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    24010 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6898 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.633786 pyoscode-1.0.2/include/Eigen/src/SparseCore/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10532 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/AmbiVector.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8164 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/CompressedStorage.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12655 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2191 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8080 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseAssign.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    25592 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseBlock.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6485 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseColEtree.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12720 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    25840 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4711 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12487 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5808 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3080 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseDot.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1107 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseFuzzy.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    12589 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseMap.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    52349 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17923 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7329 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparsePermutation.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7049 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseProduct.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1699 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseRedux.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    15492 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseRef.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    25670 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4424 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseSolverBase.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8741 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3175 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseTranspose.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6437 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseTriangularView.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6602 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseUtil.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    14831 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseVector.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8110 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseView.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9657 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseCore/TriangularSolver.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.637786 pyoscode-1.0.2/include/Eigen/src/SparseLU/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    27923 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4303 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLUImpl.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7601 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4974 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10022 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2049 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6712 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6582 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3681 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    10216 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4181 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5723 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     8486 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9028 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4979 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4545 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2889 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.637786 pyoscode-1.0.2/include/Eigen/src/SparseQR/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    28084 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SparseQR/SparseQR.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.637786 pyoscode-1.0.2/include/Eigen/src/StlSupport/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5117 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/StlSupport/StdDeque.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4147 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/StlSupport/StdList.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5330 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/StlSupport/StdVector.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2809 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/StlSupport/details.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.637786 pyoscode-1.0.2/include/Eigen/src/SuperLUSupport/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    34341 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.637786 pyoscode-1.0.2/include/Eigen/src/UmfPackSupport/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17202 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.645786 pyoscode-1.0.2/include/Eigen/src/misc/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2913 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/misc/Image.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2742 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/misc/Kernel.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     1748 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/misc/RealSvd2x2.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    30560 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/misc/blas.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     7834 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/misc/lapack.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)  1058368 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/misc/lapacke.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      474 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/misc/lapacke_mangling.h
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.645786 pyoscode-1.0.2/include/Eigen/src/plugins/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    13132 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    16929 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    37403 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/plugins/BlockMethods.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4828 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     5621 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     6375 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2937 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     4450 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/interpolator.hpp
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9453 2020-10-08 10:29:22.000000 pyoscode-1.0.2/include/rksolver.hpp
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    17555 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/solver.hpp
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2754 2020-10-07 14:00:56.000000 pyoscode-1.0.2/include/system.hpp
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    30690 2020-11-09 12:19:29.000000 pyoscode-1.0.2/include/wkbsolver.hpp
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.645786 pyoscode-1.0.2/pyoscode/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     3921 2020-10-07 17:18:02.000000 pyoscode-1.0.2/pyoscode/__init__.py
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     9797 2020-10-07 14:00:56.000000 pyoscode-1.0.2/pyoscode/_pyoscode.cpp
--rw-r--r--   0 fruzsina  (1000) fruzsina  (1000)      916 2020-06-04 13:31:15.000000 pyoscode-1.0.2/pyoscode/_pyoscode.hpp
--rw-r--r--   0 fruzsina  (1000) fruzsina  (1000)       81 2020-06-04 13:31:15.000000 pyoscode-1.0.2/pyoscode/_python.hpp
-drwxrwxr-x   0 fruzsina  (1000) fruzsina  (1000)        0 2020-12-03 16:53:47.649786 pyoscode-1.0.2/pyoscode.egg-info/
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    11883 2020-12-03 16:53:47.000000 pyoscode-1.0.2/pyoscode.egg-info/PKG-INFO
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)    13207 2020-12-03 16:53:47.000000 pyoscode-1.0.2/pyoscode.egg-info/SOURCES.txt
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)        1 2020-12-03 16:53:47.000000 pyoscode-1.0.2/pyoscode.egg-info/dependency_links.txt
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      103 2020-12-03 16:53:47.000000 pyoscode-1.0.2/pyoscode.egg-info/requires.txt
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)       19 2020-12-03 16:53:47.000000 pyoscode-1.0.2/pyoscode.egg-info/top_level.txt
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)      107 2020-12-03 15:30:10.000000 pyoscode-1.0.2/pyproject.toml
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)       38 2020-12-03 16:53:47.649786 pyoscode-1.0.2/setup.cfg
--rw-rw-r--   0 fruzsina  (1000) fruzsina  (1000)     2230 2020-12-03 16:52:29.000000 pyoscode-1.0.2/setup.py
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:19.057240 pyoscode-1.1.2/
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.405786 pyoscode-1.1.2/.github/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      400 2022-03-28 16:31:24.000000 pyoscode-1.1.2/.github/pull_request_template.md
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.411222 pyoscode-1.1.2/.github/workflows/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1109 2023-03-10 20:33:47.000000 pyoscode-1.1.2/.github/workflows/python-package.yml
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      184 2021-11-24 19:50:23.000000 pyoscode-1.1.2/.gitignore
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      575 2021-11-24 19:50:23.000000 pyoscode-1.1.2/.readthedocs.yml
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1109 2022-02-15 01:53:05.000000 pyoscode-1.1.2/Dockerfile
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.422293 pyoscode-1.1.2/JOSS-paper/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6212 2021-11-24 19:50:23.000000 pyoscode-1.1.2/JOSS-paper/paper.bib
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5648 2021-11-24 19:50:23.000000 pyoscode-1.1.2/JOSS-paper/paper.md
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1557 2021-11-24 19:50:23.000000 pyoscode-1.1.2/LICENSE
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10662 2023-06-01 22:07:19.026922 pyoscode-1.1.2/PKG-INFO
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9605 2023-06-01 21:55:57.000000 pyoscode-1.1.2/README.rst
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.505851 pyoscode-1.1.2/examples/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1572 2023-03-10 20:33:47.000000 pyoscode-1.1.2/examples/airy.py
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5408 2022-03-28 16:31:24.000000 pyoscode-1.1.2/examples/burst.cpp
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)   601037 2022-08-12 21:56:21.000000 pyoscode-1.1.2/examples/cosmology.ipynb
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.586036 pyoscode-1.1.2/examples/images/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)  1197382 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/airy.png
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)   123960 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/bingo-singlek-k1e-5-ref.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2395 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/bingo-singlek-k1e-5.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    33313 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/cambridge.png
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    83867 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/caplogo.svg
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)  2993802 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/cmb.png
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    25046 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/kavli.jpg
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    13472 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/rkwkb-single-k1e-5.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17131 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/singlek-kd-bd-2a.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)   121994 2021-11-24 19:50:23.000000 pyoscode-1.1.2/examples/images/singlek-kd-bg-2a-ref.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)   619964 2021-11-24 19:51:12.000000 pyoscode-1.1.2/examples/introduction_to_pyoscode.ipynb
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      972 2022-02-09 17:32:27.000000 pyoscode-1.1.2/examples/plot_burst.py
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)   481085 2021-11-24 19:51:12.000000 pyoscode-1.1.2/examples/pyoscode_scipy.ipynb
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1423 2021-11-24 19:51:12.000000 pyoscode-1.1.2/examples/test-rk.py
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.612428 pyoscode-1.1.2/include/
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.880530 pyoscode-1.1.2/include/Eigen/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1129 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Cholesky
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1900 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/CholmodSupport
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17361 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Core
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      122 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Dense
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)       35 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Eigen
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1763 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Eigenvalues
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2050 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Geometry
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      874 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Householder
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2083 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/IterativeLinearSolvers
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      939 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Jacobi
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1374 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/LU
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      991 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/MetisSupport
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2483 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/OrderingMethods
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1676 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/PaStiXSupport
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1116 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/PardisoSupport
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1258 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/QR
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      940 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/QtAlignedMalloc
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1162 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/SPQRSupport
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1570 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/SVD
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      919 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/Sparse
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1371 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/SparseCholesky
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2240 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/SparseCore
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1713 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/SparseLU
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1222 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/SparseQR
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      797 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/StdDeque
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      726 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/StdList
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      803 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/StdVector
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2243 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/SuperLUSupport
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1382 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/UmfPackSupport
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.251978 pyoscode-1.1.2/include/Eigen/src/
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.896972 pyoscode-1.1.2/include/Eigen/src/Cholesky/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    24254 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Cholesky/LDLT.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17834 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Cholesky/LLT.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3974 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.902483 pyoscode-1.1.2/include/Eigen/src/CholmodSupport/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    22307 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.260576 pyoscode-1.1.2/include/Eigen/src/Core/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12218 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Array.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8179 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/ArrayBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6775 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/ArrayWrapper.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2720 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Assign.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    38120 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/AssignEvaluator.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12221 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Assign_MKL.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    13910 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/BandMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    18064 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Block.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4249 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/BooleanRedux.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5689 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/CommaInitializer.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6970 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/ConditionEstimator.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    61293 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/CoreEvaluators.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4525 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/CoreIterators.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7593 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/CwiseBinaryOp.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    31424 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/CwiseNullaryOp.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8256 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/CwiseTernaryOp.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3877 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/CwiseUnaryOp.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5282 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/CwiseUnaryView.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    27420 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/DenseBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    24212 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/DenseCoeffsBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    21959 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/DenseStorage.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9507 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Diagonal.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12666 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/DiagonalMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      970 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/DiagonalProduct.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    11392 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Dot.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5619 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/EigenBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4769 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/ForceAlignedAccess.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5705 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Fuzzy.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    21119 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/GeneralProduct.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    22185 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/GenericPacketMath.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10222 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/GlobalFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7076 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/IO.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3519 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Inverse.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6655 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Map.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10621 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/MapBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    40859 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/MathFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2776 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/MathFunctionsImpl.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    19170 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Matrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    22375 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/MatrixBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3400 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/NestByValue.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3582 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/NoAlias.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9234 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/NumTraits.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    21646 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/PermutationMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    45040 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/PlainObjectBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7149 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Product.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    48917 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/ProductEvaluators.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6379 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Random.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17832 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Redux.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12729 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Ref.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5595 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Replicate.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4200 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/ReturnByValue.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7073 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Reverse.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6020 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Select.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14135 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/SelfAdjointView.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1909 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6795 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Solve.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9031 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/SolveTriangular.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4365 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/SolverBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7686 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/StableNorm.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3865 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Stride.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2683 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Swap.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14777 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Transpose.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14396 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Transpositions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    37234 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/TriangularMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3462 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/VectorBlock.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    29441 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/VectorwiseOp.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8074 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/Visitor.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:16.153179 pyoscode-1.1.2/include/Eigen/src/Core/arch/
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.282312 pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    19305 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/Complex.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17776 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    27570 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1194 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.293075 pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX512/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15827 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    50915 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.309442 pyoscode-1.1.2/include/Eigen/src/Core/arch/AltiVec/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17722 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10797 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    37102 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.340898 pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4240 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    21057 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/Half.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2387 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10744 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    35462 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5509 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.346247 pyoscode-1.1.2/include/Eigen/src/Core/arch/Default/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1746 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/Default/Settings.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.362081 pyoscode-1.1.2/include/Eigen/src/Core/arch/NEON/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17570 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/NEON/Complex.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2846 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    27880 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.383736 pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    20720 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/Complex.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    18888 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    35047 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1726 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.399205 pyoscode-1.1.2/include/Eigen/src/Core/arch/ZVector/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15259 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4418 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    32283 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.430872 pyoscode-1.1.2/include/Eigen/src/Core/functors/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6284 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    18081 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8229 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4184 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/functors/StlFunctors.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      607 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    27944 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/functors/UnaryFunctors.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.541982 pyoscode-1.1.2/include/Eigen/src/Core/products/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    81106 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    18478 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15188 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6746 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4730 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    26736 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6053 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4905 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/Parallelizer.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    19632 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10614 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9901 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4903 2021-11-24 19:50:24.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6105 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4066 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    19345 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    13238 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14216 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9895 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    13979 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6024 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5741 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularSolverVector.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.604322 pyoscode-1.1.2/include/Eigen/src/Core/util/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15722 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/BlasUtil.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    21579 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/Constants.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3564 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14150 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3970 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/MKL_support.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    36377 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/Macros.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    39712 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/Memory.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    18481 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/Meta.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)       85 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/NonMPL2.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      809 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10284 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/StaticAssert.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    34198 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Core/util/XprHelper.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.678393 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12558 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17021 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4178 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    22944 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17191 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9715 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14351 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5679 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    23586 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/RealQZ.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    20268 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/RealSchur.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3650 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    33674 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4378 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    22444 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.752482 pyoscode-1.1.2/include/Eigen/src/Geometry/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14815 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/AlignedBox.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8415 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/AngleAxis.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3639 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/EulerAngles.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    20539 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/Homogeneous.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    11961 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/Hyperplane.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8949 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/OrthoMethods.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8308 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/ParametrizedLine.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    31688 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/Quaternion.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6877 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/Rotation2D.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8063 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/RotationBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6324 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/Scaling.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    60514 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/Transform.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7773 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/Translation.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6191 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/Umeyama.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.757945 pyoscode-1.1.2/include/Eigen/src/Geometry/arch/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5387 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.773859 pyoscode-1.1.2/include/Eigen/src/Householder/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4481 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Householder/BlockHouseholder.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5345 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Householder/Householder.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    20603 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Householder/HouseholderSequence.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.815969 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6763 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7253 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9184 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15062 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15234 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    11527 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7762 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4158 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.821403 pyoscode-1.1.2/include/Eigen/src/Jacobi/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14888 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/Jacobi/Jacobi.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.848211 pyoscode-1.1.2/include/Eigen/src/LU/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3057 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/LU/Determinant.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    32803 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/LU/FullPivLU.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15068 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/LU/InverseImpl.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    21478 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/LU/PartialPivLU.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3555 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.853593 pyoscode-1.1.2/include/Eigen/src/LU/arch/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    13669 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/LU/arch/Inverse_SSE.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.859337 pyoscode-1.1.2/include/Eigen/src/MetisSupport/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4588 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/MetisSupport/MetisSupport.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.875361 pyoscode-1.1.2/include/Eigen/src/OrderingMethods/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    16396 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/OrderingMethods/Amd.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    62266 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5229 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/OrderingMethods/Ordering.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.880905 pyoscode-1.1.2/include/Eigen/src/PaStiXSupport/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    22220 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.886384 pyoscode-1.1.2/include/Eigen/src/PardisoSupport/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    20032 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.918222 pyoscode-1.1.2/include/Eigen/src/QR/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    24881 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4662 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    20805 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    25478 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14022 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/QR/HouseholderQR.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2993 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.923363 pyoscode-1.1.2/include/Eigen/src/SPQRSupport/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    11405 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.950202 pyoscode-1.1.2/include/Eigen/src/SVD/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    47664 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SVD/BDCSVD.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    32949 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SVD/JacobiSVD.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5009 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12650 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SVD/SVDBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15957 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SVD/UpperBidiagonalization.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:17.961010 pyoscode-1.1.2/include/Eigen/src/SparseCholesky/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    24010 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6898 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.117948 pyoscode-1.1.2/include/Eigen/src/SparseCore/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10532 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/AmbiVector.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8164 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/CompressedStorage.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12655 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2191 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8080 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseAssign.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    25592 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseBlock.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6485 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseColEtree.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12720 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    25840 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4711 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12487 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5808 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3080 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseDot.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1107 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    12589 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseMap.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    52349 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17923 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7329 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparsePermutation.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7049 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseProduct.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1699 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseRedux.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    15492 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseRef.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    25670 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4424 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8741 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3175 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseTranspose.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6437 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6602 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseUtil.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14831 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseVector.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8110 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseView.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9657 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseCore/TriangularSolver.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.208578 pyoscode-1.1.2/include/Eigen/src/SparseLU/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    27923 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4303 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7601 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4974 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10022 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2049 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6712 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6582 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3681 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10216 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4181 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5723 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8486 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9028 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4979 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4545 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2889 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.213996 pyoscode-1.1.2/include/Eigen/src/SparseQR/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    28084 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SparseQR/SparseQR.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.235023 pyoscode-1.1.2/include/Eigen/src/StlSupport/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5117 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/StlSupport/StdDeque.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4147 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/StlSupport/StdList.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5330 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/StlSupport/StdVector.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2809 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/StlSupport/details.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.240202 pyoscode-1.1.2/include/Eigen/src/SuperLUSupport/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    34341 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.245930 pyoscode-1.1.2/include/Eigen/src/UmfPackSupport/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17202 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.290176 pyoscode-1.1.2/include/Eigen/src/misc/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2913 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/misc/Image.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2742 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/misc/Kernel.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1748 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/misc/RealSvd2x2.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    30560 2021-11-24 19:50:25.000000 pyoscode-1.1.2/include/Eigen/src/misc/blas.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7834 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/misc/lapack.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)  1058368 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/misc/lapacke.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      474 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/misc/lapacke_mangling.h
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.327952 pyoscode-1.1.2/include/Eigen/src/plugins/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    13132 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    16929 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    37403 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/plugins/BlockMethods.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4828 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     5621 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6375 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2937 2021-11-24 19:50:26.000000 pyoscode-1.1.2/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     4367 2022-03-28 16:31:24.000000 pyoscode-1.1.2/include/interpolator.hpp
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10345 2023-03-10 20:33:47.000000 pyoscode-1.1.2/include/rksolver.hpp
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    19299 2023-06-01 21:55:57.000000 pyoscode-1.1.2/include/solver.hpp
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     3358 2022-04-08 20:27:00.000000 pyoscode-1.1.2/include/system.hpp
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    37475 2023-03-10 20:33:47.000000 pyoscode-1.1.2/include/wkbsolver.hpp
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.378174 pyoscode-1.1.2/pyoscode/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     7246 2023-03-10 20:33:47.000000 pyoscode-1.1.2/pyoscode/__init__.py
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    17616 2023-03-10 20:33:47.000000 pyoscode-1.1.2/pyoscode/_pyoscode.cpp
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1426 2023-03-10 20:33:47.000000 pyoscode-1.1.2/pyoscode/_pyoscode.hpp
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)       81 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/_python.hpp
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.648304 pyoscode-1.1.2/pyoscode/docs/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      586 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/docs/Makefile
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)       50 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/docs/requirements.txt
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.675195 pyoscode-1.1.2/pyoscode/docs/source/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     6823 2023-02-03 19:03:41.000000 pyoscode-1.1.2/pyoscode/docs/source/conf.py
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      276 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/docs/source/index.rst
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     8465 2023-06-01 21:55:57.000000 pyoscode-1.1.2/pyoscode/docs/source/introduction.rst
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10402 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/docs/source/oscode.rst
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)       98 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/docs/source/pyoscode.rst
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.998107 pyoscode-1.1.2/pyoscode/images/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    52383 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/images/airy-example.png
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    47341 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/images/burst-example.png
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      324 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/images/gamma.png
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      328 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/images/omega.png
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     1019 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/images/oscillator.gif
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      919 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/images/oscillator.png
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)  2536494 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyoscode/images/spectra.gif
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:18.638246 pyoscode-1.1.2/pyoscode.egg-info/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    10662 2023-06-01 22:07:15.000000 pyoscode-1.1.2/pyoscode.egg-info/PKG-INFO
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)    14345 2023-06-01 22:07:15.000000 pyoscode-1.1.2/pyoscode.egg-info/SOURCES.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)        1 2023-06-01 22:07:15.000000 pyoscode-1.1.2/pyoscode.egg-info/dependency_links.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      103 2023-06-01 22:07:15.000000 pyoscode-1.1.2/pyoscode.egg-info/requires.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)       19 2023-06-01 22:07:15.000000 pyoscode-1.1.2/pyoscode.egg-info/top_level.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)      107 2021-11-24 19:50:26.000000 pyoscode-1.1.2/pyproject.toml
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)       31 2022-05-03 18:43:40.000000 pyoscode-1.1.2/requirements.txt
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)       38 2023-06-01 22:07:19.058532 pyoscode-1.1.2/setup.cfg
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2173 2023-06-01 21:55:57.000000 pyoscode-1.1.2/setup.py
+drwxrwxr-x   0 fagocs    (1866) fagocs    (1866)        0 2023-06-01 22:07:19.020936 pyoscode-1.1.2/tests/
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     9585 2023-03-13 16:45:16.000000 pyoscode-1.1.2/tests/test_airy.py
+-rw-rw-r--   0 fagocs    (1866) fagocs    (1866)     2261 2021-11-24 19:50:26.000000 pyoscode-1.1.2/tests/test_arrays.py
```

### Comparing `pyoscode-1.0.2/PKG-INFO` & `pyoscode-1.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,304 +1,324 @@
 Metadata-Version: 2.1
 Name: pyoscode
-Version: 1.0.2
+Version: 1.1.2
 Summary: oscode: Oscillatory ordinary differential equation solver
 Home-page: https://github.com/fruzsinaagocs/oscode
 Author: Fruzsina Agocs
 Author-email: fa325@cam.ac.uk
 License: oscode
 Project-URL: Documentation, https://oscode.readthedocs.io
-Description: ========================================================================
-        oscode: Oscillatory ordinary differential equation solver
-        ========================================================================
-        
-        .. image:: https://codecov.io/gh/fruzsinaagocs/oscode/branch/joss-paper/graph/badge.svg
-                :target: https://codecov.io/gh/fruzsinaagocs/oscode
-                :alt: codecov status
-        .. image:: https://travis-ci.org/fruzsinaagocs/oscode.svg?branch=master
-                :target: https://travis-ci.org/fruzsinaagocs/oscode
-                :alt: Travis CI build status
-        .. image:: https://readthedocs.org/projects/oscode/badge/?version=latest
-                :target: https://oscode.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        .. image:: https://badges.gitter.im/oscode-help/community.svg
-                :target: https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-                :alt: Chat on gitter
-        .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-                :target: https://opensource.org/licenses/BSD-3-Clause
-                :alt: BSD 3-clause license
-        .. image:: https://img.shields.io/pypi/dm/pyoscode?color=indigo 
-                :target: https://pypi.org/project/pyoscode/
-                :alt: PyPI downloads
-        .. image:: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda/status.svg
-                :target: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda
-                :alt: JOSS status
-        
-        
-        |
-        |
-        
-        .. contents::
-           :local:
-        
-        |
-        
-        About
-        -----
-        
-        Oscode is a C++ tool with a Python interface that solves **osc**\illatory
-        **o**\rdinary **d**\ifferential **e**\quations efficiently. It is designed to
-        deal with equations of the form
-        
-        .. image:: 
-            https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/oscillator.png
-        
-        where |gamma| (friction term) and |omega| (frequency) can be given as arrays.
-        
-        .. |gamma| image:: https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/gamma.png
-        
-        .. |omega| image:: https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/omega.png
-        
-        Oscode makes use of an analytic approximation of x(t) embedded in a
-        stepping procedure to skip over long regions of oscillations, giving a reduction
-        in computing time. The approximation is valid when the frequency changes slowly
-        relative to the timescales of integration, it is therefore worth applying when
-        this condition holds for at least some part of the integration range. 
-        
-        For the details of the numerical method used by oscode, see Citation_.
-        
-        
-        Installation
-        ------------
-        
-        Dependencies
-        ~~~~~~~~~~~~
-        
-        Basic requirements for using the C++ interface:
-        
-        - C++11 or later
-        - `Eigen <http://eigen.tuxfamily.org/index.php?title=Main_Page>`__ (a header-only library included in this source)
-        
-        The strictly necessary Python dependencies are automatically installed when you use `pip` or the `setup.py`. They are:
-        
-        - `numpy <https://pypi.org/project/numpy/>`__
-        
-        The *optional* dependencies are: 
-        
-        - for tests
-            - `scipy <https://pypi.org/project/scipy/>`__ 
-            - `pytest <https://docs.pytest.org/en/stable/getting-started.html>`__ 
-        - for examples/plotting
-            - `matplotlib <https://pypi.org/project/matplotlib/>`__
-            - `scipy <https://pypi.org/project/scipy/>`__ 
-        - for generating offline documentation
-            - `sphinx <https://pypi.org/project/Sphinx/>`__ 
-            - `doxygen <https://www.doxygen.nl/index.html>`__
-            - `breathe <https://pypi.org/project/breathe/>`__
-            - `exhale <https://pypi.org/project/exhale/>`__
-        
-        
-        Python
-        ~~~~~~
-        
-        ``pyoscode`` can be installed via pip 
-        
-        .. code:: bash
-           
-           pip install pyoscode
-        
-        or via the setup.py
-        
-        .. code:: bash
-        
-           git clone https://github.com/fruzsinaagocs/oscode
-           cd oscode
-           python setup.py install --user
-        
-        or
-        
-        .. code:: bash
-        
-           git clone https://github.com/fruzsinaagocs/oscode
-           cd oscode
-           pip install .
-        
-        You can then import ``pyoscode`` from anywhere. Omit the ``--user`` option if
-        you wish to install globally or in a virtual environment. If you have any
-        difficulties, check out the `FAQs - Installation
-        <https://github.com/fruzsinaagocs/oscode#installation-1>`__ section below. 
-        
-        You can check that things are working by running `tests/` (also ran by Travis continuous integration):
-        
-        .. code:: bash
-        
-           pytest tests/
-        
-        C++
-        ~~~
-        
-        ``oscode`` is a header-only C++ package, it requires no installation.
-        
-        .. code:: bash
-        
-           git clone https://github.com/fruzsinaagocs/oscode
-        
-        and then include the relevant header files in your C++ code:
-        
-        .. code:: c
-        
-            #include "solver.hpp"
-            #include "system.hpp"
-        
-        
-        Quick start
-        -----------
-        
-        Try the following quick examples. They are available in the `examples
-        <https://github.com/fruzsinaagocs/oscode/tree/master/examples/>`__.
-        
-        Python
-        ~~~~~~
-        
-        :Introduction to pyoscode: |intro_binder|
-        :Cosmology examples: |cosmology_binder|
-        :Scipy 2020 lecture notebook: |scipy_binder|
-        
-        .. |intro_binder| image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/introduction_to_pyoscode.ipynb
-        
-        .. |cosmology_binder| image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/cosmology.ipynb
-        
-        .. |scipy_binder| image:: https://mybinder.org/badge_logo.svg
-         :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/pyoscode_scipy.ipynb
-        
-        
-        .. image::
-            https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/spectra.gif
-            :width: 800
-        
-        C++
-        ~~~
-        
-        :Introduction to oscode: `examples/burst.cpp`
-        :To plot results from `burst.cpp`: `examples/plot_burst.py`
-        
-        To compile and run:
-        
-        .. code:: bash
-        
-            g++ -g -Wall -std=c++11 -c -o burst.o burst.cpp
-            g++ -g -Wall -std=c++11 -o burst burst.o
-            ./burst
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is hosted at `readthedocs <https://oscode.readthedocs.io>`__.
-        
-        To build your own local copy of the documentation you can run:
-        
-        .. code:: bash
-        
-           cd pyoscode/docs
-           make html
-        
-        Citation
-        --------
-        
-        If you use ``oscode`` to solve equations for a publication, please cite:
-        
-        - `Efficient method for solving highly oscillatory ordinary differential equations with applications to physical systems <https://doi.org/10.1103/PhysRevResearch.2.013030>`__,
-        - `Dense output for highly oscillatory numerical solutions  <https://arxiv.org/abs/2007.05013>`__
-        
-        Contributing
-        ------------
-        
-        Any comments and improvements to this project are welcome. You can contribute
-        by:
-        
-        - Opening and `issue <https://www.github.com/fruzsinaagocs/oscode/issues/>`__ to report bugs and propose new features.
-        - Making a pull request.
-        
-        Further help
-        ------------
-        
-        You can get help by submitting an issue or posting a message on `Gitter <https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge>`__.
-        
-        FAQs
-        ----
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        1. Eigen import errors:
-            .. code:: bash
-        
-               pyoscode/_pyoscode.hpp:6:10: fatal error: Eigen/Dense: No such file or directory
-                #include <Eigen/Dense>
-                          ^~~~~~~~~~~~~
-        
-            Try explicitly including the location of your Eigen library via the
-            ``CPLUS_INCLUDE_PATH`` environment variable, for example:
-        
-            .. code:: bash
-        
-               CPLUS_INCLUDE_PATH=/usr/include/eigen3 python setup.py install --user
-               # or 
-               CPLUS_INCLUDE_PATH=/usr/include/eigen3 pip install pyoscode
-        
-            where  ``/usr/include/eigen3`` should be replaced with your system-specific
-            eigen location.
-        
-        Thanks
-        ------
-        
-        Many thanks to **Will Handley**, **Lukas Hergt**, **Anthony Lasenby**, and **Mike Hobson** for
-        their support and advice regarding the algorithm behind `oscode`.
-        There are many packages without which some part of `oscode` (e.g. testing and
-        examples) wouldn't run as nicely and smoothly, thank you all developers for
-        making and maintaining these open-source projects. A special thanks goes to the
-        devs of `exhale <https://pypi.org/project/exhale/>`__ for making the beautiful C++ documentation possible. 
-        
-        
-        Changelog
-        ---------
-        
-        - 1.0.2: current version
-            - Fixed getting correct numpy include directories
-        - 1.0.1:
-            - Added `pyproject.toml` to handle build dependencies (numpy)
-        - 1.0.0:
-            - Dense output
-            - Arrays for frequency and damping term need not be evenly spaced
-            - Automatic C++ documentation on readthedocs
-            - Eigen included in source for pip installability
-            - First pip release :)
-        - 0.1.2:
-            - Bug that occurred when beginning and end of integration coincided
-              corrected
-        - 0.1.1:
-            - Automatic detection of direction of integration
-        - 0.1.0:
-            - Memory leaks at python interface fixed
-            - C++ documentation added 
-        
 Keywords: PPS,cosmic inflation,cosmology,oscillatory,ODE
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Provides-Extra: docs
 Provides-Extra: examples
+Provides-Extra: docs
 Provides-Extra: testing
+License-File: LICENSE
+
+========================================================================
+oscode: Oscillatory ordinary differential equation solver
+========================================================================
+
+.. image:: https://codecov.io/gh/fruzsinaagocs/oscode/branch/joss-paper/graph/badge.svg
+        :target: https://codecov.io/gh/fruzsinaagocs/oscode
+        :alt: codecov status
+.. image:: https://github.com/fruzsinaagocs/oscode/actions/workflows/python-package.yml/badge.svg
+        :target: https://github.com/fruzsinaagocs/oscode/actions
+        :alt: GH workflow status
+.. image:: https://readthedocs.org/projects/oscode/badge/?version=latest
+        :target: https://oscode.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+.. image:: https://badges.gitter.im/oscode-help/community.svg
+        :target: https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
+        :alt: Chat on gitter
+.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+        :target: https://opensource.org/licenses/BSD-3-Clause
+        :alt: BSD 3-clause license
+.. image:: https://img.shields.io/pypi/dm/pyoscode?color=indigo 
+        :target: https://pypi.org/project/pyoscode/
+        :alt: PyPI downloads
+.. image:: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda/status.svg
+        :target: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda
+        :alt: JOSS status
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4322958.svg
+        :target: https://doi.org/10.5281/zenodo.4322958
+        :alt: Zenodo doi
+
+|
+|
+
+.. contents::
+   :local:
+
+|
+
+About
+-----
+
+Oscode is a C++ tool with a Python interface that solves **osc**\illatory
+**o**\rdinary **d**\ifferential **e**\quations efficiently. It is designed to
+deal with equations of the form
+
+.. image:: 
+    https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/oscillator.png
+
+where |gamma| (friction term) and |omega| (frequency) can be given as arrays.
+
+.. |gamma| image:: https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/gamma.png
+
+.. |omega| image:: https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/omega.png
+
+Oscode makes use of an analytic approximation of x(t) embedded in a
+stepping procedure to skip over long regions of oscillations, giving a reduction
+in computing time. The approximation is valid when the frequency changes slowly
+relative to the timescales of integration, it is therefore worth applying when
+this condition holds for at least some part of the integration range. 
+
+For the details of the numerical method used by oscode, see Citation_.
+
+
+Installation
+------------
+
+Dependencies
+~~~~~~~~~~~~
+
+Basic requirements for using the C++ interface:
+
+- C++11 or later
+- `Eigen <http://eigen.tuxfamily.org/index.php?title=Main_Page>`__ (a header-only library included in this source)
+
+The strictly necessary Python dependencies are automatically installed when you use `pip` or the `setup.py`. They are:
+
+- `numpy <https://pypi.org/project/numpy/>`__
+
+The *optional* dependencies are: 
+
+- for tests
+    - `scipy <https://pypi.org/project/scipy/>`__ 
+    - `pytest <https://docs.pytest.org/en/stable/getting-started.html>`__ 
+- for examples/plotting
+    - `matplotlib <https://pypi.org/project/matplotlib/>`__
+    - `scipy <https://pypi.org/project/scipy/>`__ 
+- for generating offline documentation
+    - `sphinx <https://pypi.org/project/Sphinx/>`__ 
+    - `doxygen <https://www.doxygen.nl/index.html>`__
+    - `breathe <https://pypi.org/project/breathe/>`__
+    - `exhale <https://pypi.org/project/exhale/>`__
+
+
+Python
+~~~~~~
+
+``pyoscode`` can be installed via pip 
+
+.. code:: bash
+   
+   pip install pyoscode
+
+or via the setup.py
+
+.. code:: bash
+
+   git clone https://github.com/fruzsinaagocs/oscode
+   cd oscode
+   python setup.py install --user
+
+or
+
+.. code:: bash
+
+   git clone https://github.com/fruzsinaagocs/oscode
+   cd oscode
+   pip install .
+
+You can then import ``pyoscode`` from anywhere. Omit the ``--user`` option if
+you wish to install globally or in a virtual environment. If you have any
+difficulties, check out the `FAQs - Installation
+<https://github.com/fruzsinaagocs/oscode#installation-1>`__ section below. 
+
+You can check that things are working by running `tests/` (also ran by Travis continuous integration):
+
+.. code:: bash
+
+   pytest tests/
+
+C++
+~~~
+
+``oscode`` is a header-only C++ package, it requires no installation.
+
+.. code:: bash
+
+   git clone https://github.com/fruzsinaagocs/oscode
+
+and then include the relevant header files in your C++ code:
+
+.. code:: c
+
+    #include "solver.hpp"
+    #include "system.hpp"
+
+
+Quick start
+-----------
+
+Try the following quick examples. They are available in the `examples
+<https://github.com/fruzsinaagocs/oscode/tree/master/examples/>`__.
+
+Python
+~~~~~~
+
+:Introduction to pyoscode: |intro_binder|
+:Cosmology examples: |cosmology_binder|
+:Scipy 2020 lecture notebook: |scipy_binder|
+
+.. |intro_binder| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/introduction_to_pyoscode.ipynb
+
+.. |cosmology_binder| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/cosmology.ipynb
+
+.. |scipy_binder| image:: https://mybinder.org/badge_logo.svg
+ :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/pyoscode_scipy.ipynb
+
+
+.. image::
+    https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/spectra.gif
+    :width: 800
+
+C++
+~~~
+
+:Introduction to oscode: `examples/burst.cpp`
+:To plot results from `burst.cpp`: `examples/plot_burst.py`
+
+To compile and run:
+
+.. code:: bash
+    
+    cd examples/
+    g++ -I../include/ -g -Wall -std=c++11 -c -o burst.o burst.cpp
+    g++ -I../include/ -g -Wall -std=c++11 -o burst burst.o
+    ./burst
+
+
+Documentation
+-------------
+
+Documentation is hosted at `readthedocs <https://oscode.readthedocs.io>`__.
+
+To build your own local copy of the documentation you can run:
+
+.. code:: bash
+
+   cd pyoscode/docs
+   make html
+
+Citation
+--------
+
+If you use ``oscode`` to solve equations for a publication, please cite:
+
+- `Efficient method for solving highly oscillatory ordinary differential equations with applications to physical systems <https://doi.org/10.1103/PhysRevResearch.2.013030>`__,
+- `Dense output for highly oscillatory numerical solutions  <https://arxiv.org/abs/2007.05013>`__
+
+Contributing
+------------
+
+Any comments and improvements to this project are welcome. You can contribute
+by:
+
+- Opening and `issue <https://www.github.com/fruzsinaagocs/oscode/issues/>`__ to report bugs and propose new features.
+- Making a pull request.
+
+Further help
+------------
+
+You can get help by submitting an issue or posting a message on `Gitter <https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge>`__.
+
+FAQs
+----
+
+Installation
+~~~~~~~~~~~~
+
+1. Eigen import errors:
+    .. code:: bash
+
+       pyoscode/_pyoscode.hpp:6:10: fatal error: Eigen/Dense: No such file or directory
+        #include <Eigen/Dense>
+                  ^~~~~~~~~~~~~
+
+    Try explicitly including the location of your Eigen library via the
+    ``CPLUS_INCLUDE_PATH`` environment variable, for example:
+
+    .. code:: bash
+
+       CPLUS_INCLUDE_PATH=/usr/include/eigen3 python setup.py install --user
+       # or 
+       CPLUS_INCLUDE_PATH=/usr/include/eigen3 pip install pyoscode
+
+    where  ``/usr/include/eigen3`` should be replaced with your system-specific
+    eigen location.
+
+Thanks
+------
+
+Many thanks to **Will Handley**, **Lukas Hergt**, **Anthony Lasenby**, and **Mike Hobson** for
+their support and advice regarding the algorithm behind `oscode`.
+There are many packages without which some part of `oscode` (e.g. testing and
+examples) wouldn't run as nicely and smoothly, thank you all developers for
+making and maintaining these open-source projects. A special thanks goes to the
+devs of `exhale <https://pypi.org/project/exhale/>`__ for making the beautiful C++ documentation possible. 
+
+
+Changelog
+---------
+
+- 1.1.2:
+    - Dense output bug fix at the C++ interface 
+- 1.1.1: 
+    - Support for mac and Windows OS at CI.
+- 1.1.0:
+    - Users can now define w, g as functions in Python (pyoscode) and call the solver via pyoscode.solve_fn(...)
+- 1.0.6:
+    - Fix issues related to dense output not being correctly generated, e.g. when timepoints at which dense output was asked for are in descending order, etc. 
+- 1.0.5:
+    - Fixes related to dense output generation
+    - Support for w, g to be given as class member functions in C++
+    - Switched to GH actions for continuous integration, and fixed code such that unit tests would run again
+    - Minor tweaks
+- 1.0.4:
+    - set minimally required numpy version: numpy>=1.20.0
+    - drop Python 2.7 support, instead support 3.8 and 3.9 in addition to 3.7
+- 1.0.3: 
+    - paper accepted to JOSS
+- 1.0.2:
+    - Fixed getting correct numpy include directories
+- 1.0.1:
+    - Added `pyproject.toml` to handle build dependencies (numpy)
+- 1.0.0:
+    - Dense output
+    - Arrays for frequency and damping term need not be evenly spaced
+    - Automatic C++ documentation on readthedocs
+    - Eigen included in source for pip installability
+    - First pip release :)
+- 0.1.2:
+    - Bug that occurred when beginning and end of integration coincided
+      corrected
+- 0.1.1:
+    - Automatic detection of direction of integration
+- 0.1.0:
+    - Memory leaks at python interface fixed
+    - C++ documentation added
```

### Comparing `pyoscode-1.0.2/README.rst` & `pyoscode-1.1.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ========================================================================
 oscode: Oscillatory ordinary differential equation solver
 ========================================================================
 
 .. image:: https://codecov.io/gh/fruzsinaagocs/oscode/branch/joss-paper/graph/badge.svg
         :target: https://codecov.io/gh/fruzsinaagocs/oscode
         :alt: codecov status
-.. image:: https://travis-ci.org/fruzsinaagocs/oscode.svg?branch=master
-        :target: https://travis-ci.org/fruzsinaagocs/oscode
-        :alt: Travis CI build status
+.. image:: https://github.com/fruzsinaagocs/oscode/actions/workflows/python-package.yml/badge.svg
+        :target: https://github.com/fruzsinaagocs/oscode/actions
+        :alt: GH workflow status
 .. image:: https://readthedocs.org/projects/oscode/badge/?version=latest
         :target: https://oscode.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 .. image:: https://badges.gitter.im/oscode-help/community.svg
         :target: https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
         :alt: Chat on gitter
 .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
@@ -19,15 +19,17 @@
         :alt: BSD 3-clause license
 .. image:: https://img.shields.io/pypi/dm/pyoscode?color=indigo 
         :target: https://pypi.org/project/pyoscode/
         :alt: PyPI downloads
 .. image:: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda/status.svg
         :target: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda
         :alt: JOSS status
-
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4322958.svg
+        :target: https://doi.org/10.5281/zenodo.4322958
+        :alt: Zenodo doi
 
 |
 |
 
 .. contents::
    :local:
 
@@ -173,17 +175,18 @@
 
 :Introduction to oscode: `examples/burst.cpp`
 :To plot results from `burst.cpp`: `examples/plot_burst.py`
 
 To compile and run:
 
 .. code:: bash
-
-    g++ -g -Wall -std=c++11 -c -o burst.o burst.cpp
-    g++ -g -Wall -std=c++11 -o burst burst.o
+    
+    cd examples/
+    g++ -I../include/ -g -Wall -std=c++11 -c -o burst.o burst.cpp
+    g++ -I../include/ -g -Wall -std=c++11 -o burst burst.o
     ./burst
 
 
 Documentation
 -------------
 
 Documentation is hosted at `readthedocs <https://oscode.readthedocs.io>`__.
@@ -252,15 +255,33 @@
 making and maintaining these open-source projects. A special thanks goes to the
 devs of `exhale <https://pypi.org/project/exhale/>`__ for making the beautiful C++ documentation possible. 
 
 
 Changelog
 ---------
 
-- 1.0.2: current version
+- 1.1.2:
+    - Dense output bug fix at the C++ interface 
+- 1.1.1: 
+    - Support for mac and Windows OS at CI.
+- 1.1.0:
+    - Users can now define w, g as functions in Python (pyoscode) and call the solver via pyoscode.solve_fn(...)
+- 1.0.6:
+    - Fix issues related to dense output not being correctly generated, e.g. when timepoints at which dense output was asked for are in descending order, etc. 
+- 1.0.5:
+    - Fixes related to dense output generation
+    - Support for w, g to be given as class member functions in C++
+    - Switched to GH actions for continuous integration, and fixed code such that unit tests would run again
+    - Minor tweaks
+- 1.0.4:
+    - set minimally required numpy version: numpy>=1.20.0
+    - drop Python 2.7 support, instead support 3.8 and 3.9 in addition to 3.7
+- 1.0.3: 
+    - paper accepted to JOSS
+- 1.0.2:
     - Fixed getting correct numpy include directories
 - 1.0.1:
     - Added `pyproject.toml` to handle build dependencies (numpy)
 - 1.0.0:
     - Dense output
     - Arrays for frequency and damping term need not be evenly spaced
     - Automatic C++ documentation on readthedocs
```

### Comparing `pyoscode-1.0.2/include/Eigen/Cholesky` & `pyoscode-1.1.2/include/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/CholmodSupport` & `pyoscode-1.1.2/include/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/Core` & `pyoscode-1.1.2/include/Eigen/Core`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/Eigenvalues` & `pyoscode-1.1.2/include/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/Geometry` & `pyoscode-1.1.2/include/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/Householder` & `pyoscode-1.1.2/include/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/IterativeLinearSolvers` & `pyoscode-1.1.2/include/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/Jacobi` & `pyoscode-1.1.2/include/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/LU` & `pyoscode-1.1.2/include/Eigen/LU`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/MetisSupport` & `pyoscode-1.1.2/include/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/OrderingMethods` & `pyoscode-1.1.2/include/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/PaStiXSupport` & `pyoscode-1.1.2/include/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/PardisoSupport` & `pyoscode-1.1.2/include/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/QR` & `pyoscode-1.1.2/include/Eigen/QR`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/QtAlignedMalloc` & `pyoscode-1.1.2/include/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/SPQRSupport` & `pyoscode-1.1.2/include/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/SVD` & `pyoscode-1.1.2/include/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/Sparse` & `pyoscode-1.1.2/include/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/SparseCholesky` & `pyoscode-1.1.2/include/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/SparseCore` & `pyoscode-1.1.2/include/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/SparseLU` & `pyoscode-1.1.2/include/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/SparseQR` & `pyoscode-1.1.2/include/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/StdDeque` & `pyoscode-1.1.2/include/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/StdList` & `pyoscode-1.1.2/include/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/StdVector` & `pyoscode-1.1.2/include/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/SuperLUSupport` & `pyoscode-1.1.2/include/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/UmfPackSupport` & `pyoscode-1.1.2/include/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Cholesky/LDLT.h` & `pyoscode-1.1.2/include/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Cholesky/LLT.h` & `pyoscode-1.1.2/include/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Cholesky/LLT_LAPACKE.h` & `pyoscode-1.1.2/include/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/CholmodSupport/CholmodSupport.h` & `pyoscode-1.1.2/include/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Array.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/ArrayBase.h` & `pyoscode-1.1.2/include/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/ArrayWrapper.h` & `pyoscode-1.1.2/include/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Assign.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/AssignEvaluator.h` & `pyoscode-1.1.2/include/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Assign_MKL.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/BandMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Block.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/BooleanRedux.h` & `pyoscode-1.1.2/include/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/CommaInitializer.h` & `pyoscode-1.1.2/include/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/ConditionEstimator.h` & `pyoscode-1.1.2/include/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/CoreEvaluators.h` & `pyoscode-1.1.2/include/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/CoreIterators.h` & `pyoscode-1.1.2/include/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/CwiseBinaryOp.h` & `pyoscode-1.1.2/include/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/CwiseNullaryOp.h` & `pyoscode-1.1.2/include/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/CwiseTernaryOp.h` & `pyoscode-1.1.2/include/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/CwiseUnaryOp.h` & `pyoscode-1.1.2/include/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/CwiseUnaryView.h` & `pyoscode-1.1.2/include/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/DenseBase.h` & `pyoscode-1.1.2/include/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/DenseCoeffsBase.h` & `pyoscode-1.1.2/include/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/DenseStorage.h` & `pyoscode-1.1.2/include/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Diagonal.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/DiagonalMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/DiagonalProduct.h` & `pyoscode-1.1.2/include/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Dot.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/EigenBase.h` & `pyoscode-1.1.2/include/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/ForceAlignedAccess.h` & `pyoscode-1.1.2/include/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Fuzzy.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/GeneralProduct.h` & `pyoscode-1.1.2/include/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/GenericPacketMath.h` & `pyoscode-1.1.2/include/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/GlobalFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/IO.h` & `pyoscode-1.1.2/include/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Inverse.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Map.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/MapBase.h` & `pyoscode-1.1.2/include/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/MathFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/MathFunctionsImpl.h` & `pyoscode-1.1.2/include/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Matrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/MatrixBase.h` & `pyoscode-1.1.2/include/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/NestByValue.h` & `pyoscode-1.1.2/include/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/NoAlias.h` & `pyoscode-1.1.2/include/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/NumTraits.h` & `pyoscode-1.1.2/include/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/PermutationMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/PlainObjectBase.h` & `pyoscode-1.1.2/include/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Product.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/ProductEvaluators.h` & `pyoscode-1.1.2/include/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Random.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Redux.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Ref.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Replicate.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/ReturnByValue.h` & `pyoscode-1.1.2/include/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Reverse.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Select.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/SelfAdjointView.h` & `pyoscode-1.1.2/include/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/SelfCwiseBinaryOp.h` & `pyoscode-1.1.2/include/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Solve.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/SolveTriangular.h` & `pyoscode-1.1.2/include/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/SolverBase.h` & `pyoscode-1.1.2/include/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/StableNorm.h` & `pyoscode-1.1.2/include/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Stride.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Swap.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Transpose.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Transpositions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/TriangularMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/VectorBlock.h` & `pyoscode-1.1.2/include/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/VectorwiseOp.h` & `pyoscode-1.1.2/include/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/Visitor.h` & `pyoscode-1.1.2/include/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/Complex.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/MathFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/PacketMath.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX/TypeCasting.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AVX512/PacketMath.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AltiVec/Complex.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/Complex.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/Half.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/PacketMath.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/Default/Settings.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/NEON/Complex.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/NEON/MathFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/NEON/PacketMath.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/Complex.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/MathFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/PacketMath.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/SSE/TypeCasting.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/ZVector/Complex.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/arch/ZVector/PacketMath.h` & `pyoscode-1.1.2/include/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/functors/AssignmentFunctors.h` & `pyoscode-1.1.2/include/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/functors/BinaryFunctors.h` & `pyoscode-1.1.2/include/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/functors/NullaryFunctors.h` & `pyoscode-1.1.2/include/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/functors/StlFunctors.h` & `pyoscode-1.1.2/include/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/functors/TernaryFunctors.h` & `pyoscode-1.1.2/include/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/functors/UnaryFunctors.h` & `pyoscode-1.1.2/include/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixVector.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/Parallelizer.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointProduct.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/SelfadjointRank2Update.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularMatrixVector.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularSolverMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/products/TriangularSolverVector.h` & `pyoscode-1.1.2/include/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/BlasUtil.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/Constants.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/DisableStupidWarnings.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/ForwardDeclarations.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/MKL_support.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/Macros.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/Memory.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/Meta.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/ReenableStupidWarnings.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/StaticAssert.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Core/util/XprHelper.h` & `pyoscode-1.1.2/include/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/ComplexSchur.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/EigenSolver.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/RealQZ.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/RealSchur.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Eigenvalues/Tridiagonalization.h` & `pyoscode-1.1.2/include/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/AlignedBox.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/AngleAxis.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/EulerAngles.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/Homogeneous.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/Hyperplane.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/OrthoMethods.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/ParametrizedLine.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/Quaternion.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/Rotation2D.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/RotationBase.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/Scaling.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/Transform.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/Translation.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/Umeyama.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Geometry/arch/Geometry_SSE.h` & `pyoscode-1.1.2/include/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Householder/BlockHouseholder.h` & `pyoscode-1.1.2/include/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Householder/Householder.h` & `pyoscode-1.1.2/include/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Householder/HouseholderSequence.h` & `pyoscode-1.1.2/include/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `pyoscode-1.1.2/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/Jacobi/Jacobi.h` & `pyoscode-1.1.2/include/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/LU/Determinant.h` & `pyoscode-1.1.2/include/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/LU/FullPivLU.h` & `pyoscode-1.1.2/include/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/LU/InverseImpl.h` & `pyoscode-1.1.2/include/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/LU/PartialPivLU.h` & `pyoscode-1.1.2/include/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `pyoscode-1.1.2/include/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/LU/arch/Inverse_SSE.h` & `pyoscode-1.1.2/include/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/MetisSupport/MetisSupport.h` & `pyoscode-1.1.2/include/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/OrderingMethods/Amd.h` & `pyoscode-1.1.2/include/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `pyoscode-1.1.2/include/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/OrderingMethods/Ordering.h` & `pyoscode-1.1.2/include/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `pyoscode-1.1.2/include/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/PardisoSupport/PardisoSupport.h` & `pyoscode-1.1.2/include/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/QR/ColPivHouseholderQR.h` & `pyoscode-1.1.2/include/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `pyoscode-1.1.2/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `pyoscode-1.1.2/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/QR/FullPivHouseholderQR.h` & `pyoscode-1.1.2/include/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/QR/HouseholderQR.h` & `pyoscode-1.1.2/include/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `pyoscode-1.1.2/include/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `pyoscode-1.1.2/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SVD/BDCSVD.h` & `pyoscode-1.1.2/include/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SVD/JacobiSVD.h` & `pyoscode-1.1.2/include/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `pyoscode-1.1.2/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SVD/SVDBase.h` & `pyoscode-1.1.2/include/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SVD/UpperBidiagonalization.h` & `pyoscode-1.1.2/include/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/AmbiVector.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/CompressedStorage.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/MappedSparseMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseAssign.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseBlock.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseColEtree.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseCompressedBase.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseDenseProduct.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseDot.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseFuzzy.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseMap.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseMatrixBase.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparsePermutation.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseProduct.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseRedux.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseRef.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseSolverBase.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseTranspose.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseTriangularView.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseUtil.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseVector.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/SparseView.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseCore/TriangularSolver.h` & `pyoscode-1.1.2/include/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLUImpl.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_Memory.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_Structs.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_Utils.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_pivotL.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_pruneL.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `pyoscode-1.1.2/include/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SparseQR/SparseQR.h` & `pyoscode-1.1.2/include/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/StlSupport/StdDeque.h` & `pyoscode-1.1.2/include/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/StlSupport/StdList.h` & `pyoscode-1.1.2/include/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/StlSupport/StdVector.h` & `pyoscode-1.1.2/include/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/StlSupport/details.h` & `pyoscode-1.1.2/include/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `pyoscode-1.1.2/include/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `pyoscode-1.1.2/include/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/misc/Image.h` & `pyoscode-1.1.2/include/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/misc/Kernel.h` & `pyoscode-1.1.2/include/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/misc/RealSvd2x2.h` & `pyoscode-1.1.2/include/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/misc/blas.h` & `pyoscode-1.1.2/include/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/misc/lapack.h` & `pyoscode-1.1.2/include/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/misc/lapacke.h` & `pyoscode-1.1.2/include/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `pyoscode-1.1.2/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `pyoscode-1.1.2/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/plugins/BlockMethods.h` & `pyoscode-1.1.2/include/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `pyoscode-1.1.2/include/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `pyoscode-1.1.2/include/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `pyoscode-1.1.2/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `pyoscode-1.1.2/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `pyoscode-1.0.2/include/interpolator.hpp` & `pyoscode-1.1.2/include/interpolator.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,14 @@
         // Does linear interpolation 
         std::complex<double> result; 
         
         if(even_ == 1){
             int i=int((x-xstart)/dx);
             std::complex<double> y0=y_[i];
             std::complex<double> y1=y_[i+1];
-            double x1 = xstart + (i+1)*dx;
-            double x0 = xstart + i*dx; 
             result = (y0+(y1-y0)*(x-xstart-dx*i)/dx);
         }
         else{
 
             x_upper_it = std::upper_bound(x_lower_bound, x_upper_bound, x);
             x_lower_it = x_upper_it-1; 
             x_lower = *x_lower_it;
```

### Comparing `pyoscode-1.0.2/include/rksolver.hpp` & `pyoscode-1.1.2/include/rksolver.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  *
  * [1] Agocs, F. J., et al. “Efficient Method for Solving Highly Oscillatory Ordinary Differential Equations with Applications to Physical Systems.” Physical Review Research, vol. 2, no. 1, 2020, doi:10.1103/physrevresearch.2.013030. 
  */
 class RKSolver
 {
     private: 
     // Frequency and friction term
-    //std::function<std::complex<double>(double)> w;
+    std::function<std::complex<double>(double)> w;
     std::function<std::complex<double>(double)> g;
     
 
     // Butcher tablaus
     Eigen::Matrix<double,5,5> butcher_a5;
     Eigen::Matrix<double,3,3> butcher_a4;
     Eigen::Matrix<double,6,1> butcher_b5, butcher_c5, dense_b5;
@@ -28,15 +28,15 @@
    
     public:
 
     /** Defines the ODE */
     de_system *de_sys_;
 
     /** Callable that gives the frequency term in the ODE at a given time */
-    std::function<std::complex<double>(double)> w;
+    //std::function<std::complex<double>(double)> w;
     
     // constructors
     RKSolver();
     RKSolver(de_system &de_sys);
     // grid of ws, gs
     /** 6 values of the frequency term per step, evaluated at the nodes of 6th
      * order Gauss-Lobatto quadrature
@@ -61,14 +61,16 @@
     Eigen::Matrix<std::complex<double>,1,2> f(double t, const Eigen::Matrix<std::complex<double>,1,2> &y);  
     // For dense output
     Eigen::Matrix<std::complex<double>,6,2> k5;
     Eigen::Matrix<std::complex<double>,1,2> dense_point(std::complex<double> x, std::complex<double> dx, const Eigen::Matrix<std::complex<double>,6,2> &k5);
     Eigen::Matrix<std::complex<double>,7,2> k_dense;
     Eigen::Matrix<double,7,4> P_dense;
     void dense_step(double t0, double h0, std::complex<double> y0, std::complex<double> dy0, const std::list<double> &dots, std::list<std::complex<double>> &doxs, std::list<std::complex<double>> &dodxs);
+    // Experimental continuous representation of solution
+    Eigen::Matrix<std::complex<double>,7,1> x_vdm;
 
 };
 
 /** Default constructor. */
 RKSolver::RKSolver(){
 };
 
@@ -78,14 +80,18 @@
  * @param de_sys[in] the system of first-order equations defining the
  * second-order ODE to solve. 
  */
 RKSolver::RKSolver(de_system &de_sys){
 
    
     de_sys_ = &de_sys;
+    if(de_sys_->is_interpolated == 0){
+        w = de_sys.w;
+        g = de_sys.g;
+    }
     // Set Butcher tableaus
     RKSolver::butcher_a5 << 0.1174723380352676535740,0,0,0,0,
                  -0.1862479800651504276304,0.5436322218248278794734,0,0,0,
                  -0.6064303885508280518989,1,0.2490461467911506000559,0,0,
                  2.899356540015731406420,-4.368525611566240669139,2.133806714786316899991,0.2178900187289247091542,0,
                  18.67996349995727204273,-28.85057783973131956546,10.72053408420926869789,1.414741756508049078612,-0.9646615009432702537787;
 	RKSolver::butcher_a4 << 0.172673164646011428100,0,0,
@@ -114,22 +120,29 @@
  *
  * @param t[in] time \f$ t \f$
  * @param y[in] vector of unknowns \f$ y = [x, \dot{x}] \f$
  * @returns a vector of the derivative of \f$ y \f$
  */
 Eigen::Matrix<std::complex<double>,1,2> RKSolver::f(double t, const Eigen::Matrix<std::complex<double>,1,2> &y){
     
-    if(de_sys_->islogw_)
-        wi = de_sys_->Winterp.expit(t);
-    else
-        wi = de_sys_->Winterp(t);
-    if(de_sys_->islogg_)
-        gi = de_sys_->Ginterp.expit(t);
-    else
-        gi = de_sys_->Ginterp(t);
+//    std::cout << "Are we interpolating? " << de_sys_->is_interpolated << std::endl;
+    if(de_sys_->is_interpolated == 1){ 
+        if(de_sys_->islogw_)
+            wi = de_sys_->Winterp.expit(t);
+        else
+            wi = de_sys_->Winterp(t);
+        if(de_sys_->islogg_)
+            gi = de_sys_->Ginterp.expit(t);
+        else
+            gi = de_sys_->Ginterp(t);
+    }
+    else{
+        wi = w(t);
+        gi = g(t);
+    }
     Eigen::Matrix<std::complex<double>,1,2> result;
     result << y[1], -wi*wi*y[0]-2.0*gi*y[1];
     return result;
 };
 
 /** Gives dense output at a single point during the step "for free", i.e. at no
  * extra evaluations of \f$ \omega(t), \gamma(t) \f$. This solution is roughly
@@ -190,15 +203,17 @@
     Eigen::Matrix<std::complex<double>,1,2> y0, y, y4, y5, delta, k5_i, k4_i;
     y4 = Eigen::Matrix<std::complex<double>,1,2>::Zero();
     y0 << x0, dx0;
     y5 = y4;
     // TODO: resizing of ws5, gs5, insertion
     Eigen::Matrix<std::complex<double>,4,2> k4;
     Eigen::Matrix<std::complex<double>,2,2> result;
+//    std::cout << "Set up RK step" << std::endl;
     k5.row(0) = h*f(t0, y0);
+//    std::cout << "Asked for f" << std::endl;
     ws(0) = wi;
     gs(0) = gi;
     for(int s=1; s<=5; s++){
         y = y0;
         for(int i=0; i<=(s-1); i++)
             y += butcher_a5(s-1,i)*k5.row(i);
         k5_i = h*f(t0 + butcher_c5(s)*h, y);
@@ -224,26 +239,38 @@
         y4 += butcher_b4(j)*k4.row(j);
     delta = y5 - y4;
     y5 += y0;
     result << y5, delta;
     // Add in missing w, g at t+h/2
     ws5(4) = ws5(3);
     ws5(3) = ws5(2);
-    if(de_sys_->islogw_)
-        ws5(2) = de_sys_->Winterp.expit(t0+h/2);
-    else
-        ws5(2) = de_sys_->Winterp(t0+h/2);
     gs5(4) = gs5(3);
     gs5(3) = gs5(2);
-    if(de_sys_->islogg_)
-        gs5(2) = de_sys_->Ginterp.expit(t0+h/2);
-    else
-        gs5(2) = de_sys_->Ginterp(t0+h/2);
+    if(de_sys_->is_interpolated == 1){
+        if(de_sys_->islogw_)
+            ws5(2) = de_sys_->Winterp.expit(t0+h/2);
+        else
+            ws5(2) = de_sys_->Winterp(t0+h/2);
+        if(de_sys_->islogg_)
+            gs5(2) = de_sys_->Ginterp.expit(t0+h/2);
+        else
+            gs5(2) = de_sys_->Ginterp(t0+h/2);
+    }
+    else{
+        ws5(2) = w(t0+h/2);
+        gs5(2) = g(t0+h/2);
+    }
 
 
     // Fill up k_dense matrix for dense output
     for(int i=0; i<=5; i++)
         k_dense.row(i) = k5.row(i);
     k_dense.row(6) = h*f(t0+h,y5);
+
+    // Experimental continuous output
+    Eigen::Matrix<std::complex<double>,1,4> Q_dense = (k_dense.transpose()*P_dense).row(0);
+    x_vdm.tail(6) << Q_dense(0), Q_dense(1), Q_dense(2), Q_dense(3), 0.0, 0.0;
+    x_vdm(0) = x0;
+
     return result;
 };
```

### Comparing `pyoscode-1.0.2/include/solver.hpp` & `pyoscode-1.1.2/include/solver.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     WKBSolver2 wkbsolver2;
     WKBSolver3 wkbsolver3;
     /** A \a de_system object to carry information about the ODE. */
     de_system *de_sys_;
     /** These define the event at which integration finishes (currently: when tf
      * is reached. */
     double fend, fnext;
+    /** a boolean encoding the direction of integration: 1/True for forward. */
+    bool sign;
 
     public:
     Solution(de_system &de_sys, std::complex<double> x0, std::complex<double>
     dx0, double t_i, double t_f, int o=3, double r_tol=1e-4, double a_tol=0.0,
     double h_0=1, const char* full_output="");
 
     template<typename X = double> Solution(de_system &de_sys,
@@ -44,31 +46,33 @@
     void solve();
     
     /** Object to call RK steps */
     RKSolver rksolver;
     
     /** Successful, total attempted, and successful WKB steps the solver took,
      * respectively  */
-    int ssteps,totsteps,wkbsteps;
+    int ssteps, totsteps, wkbsteps;
     /** Lists to contain the solution and its derivative evaluated at internal
      * points taken by the solver (i.e. not dense output) after a run */
     std::list<std::complex<double>> sol, dsol;
     /** List to contain the timepoints at which the solution and derivative are
      * internally evaluated by the solver */
     std::list<double> times;
     /** List to contain the "type" of each step (RK/WKB) taken internally by the
      * solver after a run */
     std::list<bool> wkbs;
-    /** Lists to contain the timepoints at which dense output was evaluated */
-    std::list<double> dotimes, dotimes_rk;
+    /** Lists to contain the timepoints at which dense output was evaluated. This list will always be sorted in ascending order (with possible duplicates), regardless of the order the timepoints were specified upon input. */
+    std::list<double> dotimes;
     /** Lists to contain the dense output of the solution and its derivative */
-    std::list<std::complex<double>> dosol, dodsol, dosol_rk, dodsol_rk;
+    std::list<std::complex<double>> dosol, dodsol;
     /** Iterator to iterate over the dense output timepoints, for when these
      * need to be written out to file */
     std::list<double>::iterator dotit;
+    // Experimental: list to contain continuous representation of the solution
+    std::list<Eigen::Matrix<std::complex<double>,7,1>> sol_vdm;
 
 };
 
 /** Constructor for when dense output was not requested. Sets up solution of the
  * ODE.
  *
  * @param[in] de_sys de_system object carrying information about the ODE being
@@ -101,31 +105,39 @@
     atol = a_tol;
     h0 = h_0;
     fo = full_output;
     rksolver = RKSolver(*de_sys_);
 
     // Determine direction of integration, fend>0 and integration ends when
     // it crosses zero
-    if((t>=tf) and h0<0){
+    if((t>=tf) && h0<0){
         // backwards
         fend = t-tf;
         fnext = fend;
-        de_sys_->Winterp.sign_ = 0;
-        de_sys_->Ginterp.sign_ = 0;
+        if(de_sys_->is_interpolated == 1){
+            de_sys_->Winterp.sign_ = 0;
+            de_sys_->Ginterp.sign_ = 0;
+        }
+        else
+            sign = 0;
 
     }
-    else if((t<=tf) and h0>0){
+    else if((t<=tf) && h0>0){
         // forward
         fend = tf-t;
         fnext = fend;
-        de_sys_->Winterp.sign_ = 1;
-        de_sys_->Ginterp.sign_ = 1;
+        if(de_sys_->is_interpolated == 1){
+            de_sys_->Winterp.sign_ = 1;
+            de_sys_->Ginterp.sign_ = 1;
+        }
+        else
+            sign = 1;
     }
     else{
-        throw "Direction of integration in conflict with direction of initial step, terminating. Please check your values for ti, tf, and h. ";
+        throw std::logic_error("Direction of integration in conflict with direction of initial step, terminating. Please check your values for ti, tf, and h.");
         return;
     }
 
     // No dense output desired if this constructor was called, so only output
     // answer at t_i and t_f
     dotimes.push_back(t_i);
     dotimes.push_back(t_f);
@@ -152,15 +164,15 @@
  *
  * @param[in] de_sys de_system object carrying information about the ODE being
  * solved
  * @param[in] x0, dx0 initial conditions for the ODE, \f$ x(t) \f$, \f$ \frac{dx}{dt} \f$ evaluated at 
  * the start of the integration range
  * @param[in] t_i start of integration range
  * @param[in] t_f end of integration range
- * @param[in] do_times timepoints at which dense output is to be produced
+ * @param[in] do_times timepoints at which dense output is to be produced. Doesn't need to be sorted, and duplicated are allowed.
  * @param[in] o order of WKB approximation to be used
  * @param[in] r_tol (local) relative tolerance
  * @param[in] a_tol (local) absolute tolerance 
  * @param[in] h_0 initial stepsize to use
  * @param[in] full_output file name to write results to
  *  
  */ 
@@ -180,64 +192,74 @@
     atol = a_tol;
     h0 = h_0;
     fo = full_output;
     rksolver = RKSolver(*de_sys_);
 
     // Determine direction of integration, fend>0 and integration ends when
     // it crosses zero
-    if((t>=tf) and h0<0){
+    if((t>=tf) && h0<0){
         // backwards
         fend = t-tf;
         fnext = fend;
-        de_sys_->Winterp.sign_ = 0;
-        de_sys_->Ginterp.sign_ = 0;
+        if(de_sys_->is_interpolated == 1){
+            de_sys_->Winterp.sign_ = 0;
+            de_sys_->Ginterp.sign_ = 0;
+        }
+        else
+            sign = 0;
     }
-    else if((t<=tf) and h0>0){
+    else if((t<=tf) && h0>0){
         // forward
         fend = tf-t;
         fnext = fend;
-        de_sys_->Winterp.sign_ = 1;
-        de_sys_->Ginterp.sign_ = 1;
+        if(de_sys_->is_interpolated == 1){
+            de_sys_->Winterp.sign_ = 1;
+            de_sys_->Ginterp.sign_ = 1;
+        }
+        else
+            sign = 1;
     }
     else{
-        throw "Direction of integration in conflict with direction of initial step, terminating. Please check your values for ti, tf, and h. ";
+        throw std::logic_error("Direction of integration in conflict with direction of initial step, terminating. Please check your values for ti, tf, and h.");
         return;
     }
 
-    // Dense output checks: 
+    // Dense output preprocessing: sort and reverse if necessary
     int dosize = do_times.size();
     dotimes.resize(dosize);
     dosol.resize(dosize);
     dodsol.resize(dosize);
-    int docount = 0;
+
+    // Copy dense output points to list
     auto doit = do_times.begin();
-    if(de_sys_->Winterp.sign_ == 1){
-                for(auto it=dotimes.begin(); it!=dotimes.end(); it++){
-            *it = *doit;
-            docount++; doit++;
-        }
+    for(auto it=dotimes.begin(); it!=dotimes.end(); it++){
+        *it = *doit;
+        doit++;
     }
-    else{
-         for(auto it=dotimes.rbegin(); it!=dotimes.rend(); ++it){
-            *it = *doit;
-            docount++; ++doit;
-        }
+    // Sort to ensure ascending order
+    dotimes.sort();
+
+    // Reverse if necessary
+    if((de_sys_->is_interpolated == 1 && de_sys_->Winterp.sign_ == 0) || (de_sys_->is_interpolated == 0 && sign == 0)){
+        dotimes.reverse();
     }
+
     dotit = dotimes.begin();
     switch(order){
         case 1: wkbsolver1 = WKBSolver1(*de_sys_, order);
                 wkbsolver = &wkbsolver1;
                 break;
         case 2: wkbsolver2 = WKBSolver2(*de_sys_, order);
                 wkbsolver = &wkbsolver2;
                 break;
         case 3: wkbsolver3 = WKBSolver3(*de_sys_, order);
                 wkbsolver = &wkbsolver3;
                 break;
     };
+
 };
 
 /** \brief Function to solve the ODE \f$ \ddot{x} + 2\gamma(t)\dot{x} +
  * \omega^2(t)x = 0 \f$ for \f$ x(t), \frac{dx}{dt} \f$.
  *
  * While solving the ODE, this function will populate the \a Solution object
  * with the following results:
@@ -274,21 +296,23 @@
     // Dense output
     std::list<double> inner_dotimes;
     std::list<std::complex<double>> inner_dosols, inner_dodsols;
     auto it_dosol = dosol.begin();
     auto it_dodsol = dodsol.begin();
     Eigen::Matrix<std::complex<double>,1,2> y_dense_rk;
     std::complex<double> x_dense_rk, dx_dense_rk;
+    // Experimental continuous solution, vandermonde representation
+    Eigen::Matrix<std::complex<double>,7,1> xvdm;
 
     while(fend > 0){
         // Check if we are reaching the end of integration
         if(fnext < 0){
             h = tf - t;
             tnext = tf;
-        };
+        }
 
         // Keep updating stepsize until step is accepted
         while(true){
             // RK step
             rkstep = rksolver.step(x, dx, t, h);
             rkx << rkstep(0,0), rkstep(0,1);
             rkerr << rkstep(1,0), rkstep(1,1);
@@ -345,36 +369,40 @@
                 wkbdelta = std::max(1e-10, errmeasure_wkb.tail(2).maxCoeff());
                 hnext = h*std::pow(1.0/wkbdelta,1.0/nwkb2);
             }
             else{
                 xnext = rkx(0);
                 dxnext = rkx(1);
                 hnext = hrk;
-            };
+            }
             totsteps += 1;
             // Checking for too many steps and low acceptance ratio:
             if(totsteps % 5000 == 0){
                 std::cerr << "Warning: the solver took " << totsteps << " steps, and may take a while to converge." << std::endl; 
                 if(ssteps/totsteps < 0.05){
                     std::cerr << "Warning: the step acceptance ratio is below 5%, the solver may take a while to converge." << std::endl;
                 }
             }
 
             // check if chosen step was successful
             if(std::abs(hnext)>=std::abs(h)){
+//                std::cout << "All dense output points: " << std::endl;
                 if(dotit!=dotimes.end()){
-                    while((*dotit-t>=0 && tnext-*dotit>=0) or (*dotit-t<=0 && tnext-*dotit<=0)){
+//                    std::cout << *dotit << std::endl;
+                    while((*dotit-t>=0 && tnext-*dotit>=0) || (*dotit-t<=0 && tnext-*dotit<=0)){
                         inner_dotimes.push_back(*dotit);
                         dotit++;
                     }
                     if(inner_dotimes.size() > 0){
                         inner_dosols.resize(inner_dotimes.size());
                         inner_dodsols.resize(inner_dotimes.size());
                         if(wkb){
                             // Dense output after successful WKB step
+//                            std::cout << "Attempting " << inner_dosols.size() << " dense output points after successful WKB step from " << t << " to " << t+h << std::endl;
+
                             wkbsolver->dense_step(t,inner_dotimes,inner_dosols,inner_dodsols);
                         }
                         else{
                             // Dense output after successful RK step
                             for(auto it=inner_dotimes.begin(); it!=inner_dotimes.end(); it++)
                                 rksolver.dense_step(t,h,x,dx,inner_dotimes,inner_dosols,inner_dodsols);
                         }
@@ -394,38 +422,43 @@
                 inner_dosols.resize(0);
                 inner_dodsols.resize(0);
                
                 // record type of step
                 if(wkb){
                     wkbsteps +=1;
                     wkbs.push_back(true);
+                    xvdm = wkbsolver->x_vdm;
                 }
                 else{
                     wkbs.push_back(false);
+                    xvdm = rksolver.x_vdm; 
                 }
                 sol.push_back(xnext);
                 dsol.push_back(dxnext);
+                sol_vdm.push_back(xvdm);
                 times.push_back(tnext);
                 tnext += hnext;
                 x = xnext;
                 dx = dxnext;
                 t += h;
                 h = hnext;
                 if(h>0){
                     fend=tf-t;
                     fnext=tf-tnext;
                 }
                 else{
                     fend=t-tf;
                     fnext=tnext-tf;
-                };
+                }
                 ssteps +=1;
                 // Update interpolation bounds
-                de_sys_->Winterp.update_interp_bounds();
-                de_sys_->Ginterp.update_interp_bounds();
+                if(de_sys_->is_interpolated == 1){
+                    de_sys_->Winterp.update_interp_bounds();
+                    de_sys_->Ginterp.update_interp_bounds();
+                }
 
                 break;
             }
             else{
                 if(wkb){
                     if(maxindex_wkb<=1){
                         if(nwkb1 > 1)
@@ -441,28 +474,38 @@
                 h = hnext;
                 tnext = t + hnext;
                 if(h>0){
                     fnext=tf-tnext;
                 }
                 else{
                     fnext=tnext-tf;
-                };
-            };
-        };
-    };
+                }
+            }
+        }
+    }
 
     // If integrating backwards, reverse dense output (because it will have been
     // reversed at the start)
-    if(de_sys_->Winterp.sign_ == 0){
-        dosol.reverse();
-        dodsol.reverse();
+    if(de_sys_->is_interpolated == 1){
+        if(de_sys_->Winterp.sign_ == 0){
+            dotimes.reverse();
+            dosol.reverse();
+            dodsol.reverse();
+        }
+    }
+    else{
+        if(sign == 0){
+            dotimes.reverse();
+            dosol.reverse();
+            dodsol.reverse();
+        }
     }
 
     // Write output to file if prompted
-    if(not (*fo==0)){
+    if(!(*fo==0)){
         std::string output(fo);
         std::ofstream f;
         f.open(output);
         f << "# Summary:\n# total steps taken: " + std::to_string(totsteps) +
         "\n# of which successful: " + std::to_string(ssteps) + "\n# of which"+
         +" wkb: " + std::to_string(wkbsteps) + "\n# time, sol, dsol, wkb? (type)\n";
         auto it_t = times.begin();
@@ -488,9 +531,9 @@
             ++it_dosol;
             ++it_dodsol;
             ++it_dotimes;
         }
 
         f.close();
     }
-    
+   
 };
```

### Comparing `pyoscode-1.0.2/include/system.hpp` & `pyoscode-1.1.2/include/system.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -7,35 +7,38 @@
     private:
         int even_;
 
     public:
         template<typename X, typename Y, typename Z, typename X_it>de_system(X
         &ts, Y &ws, Z &gs, X_it x_it, int size, bool isglogw=false, bool
         islogg=false, int even=0, int check_grid=0);
-        de_system(std::complex<double> (*w)(double), std::complex<double> (*g)(double));
+        de_system(std::complex<double> (*)(double, void*), std::complex<double> (*)(double, void*), void*);
+        de_system(std::complex<double> (*)(double), std::complex<double> (*)(double));
         de_system();
         std::function<std::complex<double>(double)> w;
         std::function<std::complex<double>(double)> g;
         LinearInterpolator<> Winterp;
         LinearInterpolator<> Ginterp; 
         bool islogg_, islogw_;
         bool grid_fine_enough = 1;
+        bool is_interpolated;
 };
 
 /** Default contructor */
 de_system::de_system(){
 }
 
 /** Constructor for the case of the user having defined the frequency and
  * damping terms as sequences
  */
 template<typename X, typename Y, typename Z, typename X_it>
 de_system::de_system(X &ts, Y &ws, Z &gs, X_it x_it, int size, bool islogw, bool
 islogg, int even, int check_grid){
     
+    is_interpolated = 1; 
     even_ = even;
     islogg_ = islogg;
     islogw_ = islogw;
 
     /** Set up interpolation on the supplied frequency and damping arrays */
     LinearInterpolator<X,Y,X_it> winterp(ts,ws,even_);
     LinearInterpolator<X,Z,X_it> ginterp(ts,gs,even_);
@@ -80,13 +83,25 @@
      
       
 }
 
 /** Constructor for the case when the frequency and damping terms have been
  * defined as functions
  */
-de_system::de_system(std::complex<double> (*W)(double), std::complex<double> (*G)(double)){
+de_system::de_system(std::complex<double> (*W)(double, void*),
+std::complex<double> (*G)(double, void*), void *p){
+    
+    is_interpolated = 0;
+    w = [W, p](double x){ return W(x, p); };
+    g = [G, p](double x){ return G(x, p); };
+};
 
+/** Constructor for the case when the frequency and damping terms have been
+ * defined as functions (and there are no additional parameters that the function might need)
+ */
+de_system::de_system(std::complex<double> (*W)(double), std::complex<double> (*G)(double)){
+    
+    is_interpolated = 0;
     w = W;
     g = G;
 };
```

### Comparing `pyoscode-1.0.2/include/wkbsolver.hpp` & `pyoscode-1.1.2/include/wkbsolver.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -96,14 +96,16 @@
     int order_;
     // error estimate on step
     std::complex<double> err_fp, err_fm, err_dfp, err_dfm;
     // dense output
     std::list<std::complex<double>> doxs, dodxs, dows;
     Eigen::Matrix<std::complex<double>,1,4> dense_s_, dense_ds_, dense_ds_i;
     std::complex<double> dense_ap_, dense_am_, dense_bp_, dense_bm_;
+    // experimental dense output + quadrature
+    Eigen::Matrix<double,6,6> integ_vandermonde, interp_vandermonde;
 
     public:
     // constructor
     WKBSolver();
     WKBSolver(de_system &de_sys, int order);
     Eigen::Matrix<std::complex<double>,3,2> step(std::complex<double> x0,
     std::complex<double> dx0, double t0, double h0, const
@@ -115,14 +117,16 @@
     void dense_step(double t0, const std::list<double> &dots, std::list<std::complex<double>> &doxs, std::list<std::complex<double>> &dodxs);
     Eigen::Matrix<double,6,1> dense_weights_6(double t);
     Eigen::Matrix<double,6,1> dense_weights_derivs_6(double t);
     std::complex<double> dense_integrate(const Eigen::Matrix<double,6,1>
     &denseweights6, const Eigen::Matrix<std::complex<double>,6,1> &integrand6);
     std::complex<double> dense_interpolate(const Eigen::Matrix<double,6,1>
     &denseweights6, const Eigen::Matrix<std::complex<double>,6,1> &integrand6);
+    // Experimental continuous representation of solution
+    Eigen::Matrix<std::complex<double>,7,1> x_vdm;
 
 
 };
 
 WKBSolver::WKBSolver(){
 };
 
@@ -186,14 +190,34 @@
         -1736.74461287884, 1322.01528240287, -879.397812956524, 335.999999851893;
     d1w2_5_w << -2.48198050935042, 0.560400997591235e-8,
         3.49148624058567, -1.52752523062733, 0.518019493788063;
     d1w3_5_w << 0.750000000213852, -2.67316915534181,
         0.360673032443906e-10, 2.67316915534181, -0.750000000213853;
     d1w4_5_w << -0.518019493788065, 1.52752523062733,
         -3.49148624058568, -0.560400043118500e-8, 2.48198050935041;
+    // Set polynomial Gauss--Lobatto coefficients for dense output + quadrature
+    double a = std::sqrt(147+42*std::sqrt(7.));
+    double b = std::sqrt(147-42*std::sqrt(7.));
+
+    interp_vandermonde << 0.06250000000, -0.1946486424, 0.6321486424, 0.6321486424, -0.1946486424, 0.06250000000,
+              -0.06250000000, 0.2544242701, -2.216265054, 2.216265054, -0.2544242701, 0.06250000000,
+               -0.8750000000, 2.587172940, -1.712172940, -1.712172940, 2.587172940, -0.8750000000,
+                0.8750000000, -3.381680853, 6.002748088, -6.002748088, 3.381680853, -0.8750000000,
+                 1.312500000, -2.392524298, 1.080024298, 1.080024298, -2.392524298, 1.312500000,
+                  -1.312500000, 3.127256583, -3.786483034, 3.786483034, -3.127256583, 1.312500000;
+
+   
+    integ_vandermonde << 0.06250000000, -0.1946486424, 0.6321486424, 0.6321486424, -0.1946486424, 0.06250000000,
+              -0.03125000000, 0.1272121350, -1.108132527, 1.108132527, -0.1272121350, 0.03125000000,
+               -0.2916666667, 0.8623909801, -0.5707243134, -0.5707243134, 0.8623909801, -0.2916666667,
+                0.2187500000, -0.8454202132, 1.500687022, -1.500687022, 0.8454202132, -0.2187500000,
+                 0.2625000000, -0.4785048596, 0.2160048596, 0.2160048596, -0.4785048596, 0.2625000000,
+                  -0.2187500000, 0.5212094304, -0.6310805056, 0.6310805056, -0.5212094304, 0.2187500000;
+ 
+
 };
 
 /** Computes a WKB step of a given order and returns the solution and its local
  * error estimate. 
  *
  *
  * @param x0[in] value of the solution \f$x(t)\f$ at the start of the step
@@ -220,14 +244,28 @@
  */
 Eigen::Matrix<std::complex<double>,3,2> WKBSolver::step(std::complex<double> x0,
 std::complex<double> dx0, double t0, double h0, const
 Eigen::Matrix<std::complex<double>,6,1> &ws, const
 Eigen::Matrix<std::complex<double>,6,1> &gs, const
 Eigen::Matrix<std::complex<double>,5,1> &ws5, const
 Eigen::Matrix<std::complex<double>,5,1> &gs5){
+
+
+    // Vandermonde dense output
+    Eigen::Matrix<std::complex<double>,6,1> s0_vdm_vec,s1_vdm_vec,s2_vdm_vec,s3_vdm_vec;
+    std::complex<double> s0_vdm,s1_vdm,s2_vdm,s3_vdm;
+    Eigen::Matrix<std::complex<double>,7,1> s_vdm_vec;
+    Eigen::Matrix<double,6,1> dows6, dodws6; // weights for dense integration/interpolation
+    Eigen::Matrix<std::complex<double>,6,1> integrand6, s3_interp, s2_interp, s1_interp;
+    Eigen::Matrix<std::complex<double>,6,1> ds1_interp, ds2_interp, ds3_interp; 
+    double t_trans;
+    std::complex<double> s0,s1,s2,s3,dense_fp,dense_fm,dense_x;
+    std::complex<double> ds0,ds1,ds2,ds3,dense_dfpf,dense_dfmf,dense_dx;
+
+
     
     Eigen::Matrix<std::complex<double>,3,2> result;
     result << 0.0, 0.0, 0.0, 0.0, 0.0, 0.0;
     // Set grid of ws, gs:
     ws_ = ws;
     gs_ = gs;
     ws5_ = ws5;
@@ -264,14 +302,49 @@
     // Error estimate on this
         err_fp = s_error.cwiseAbs().sum()*fp_;
         err_fm = std::conj(err_fp);
         err_dfp = dfpf_/fp_*err_fp; 
         err_dfm = std::conj(err_dfp);
         result(2,0) = ap_*err_fp + am_*err_fm;
         result(2,1) = bp_*err_dfp + bm_*err_dfm;
+    
+    // Experimental continuous representation
+        // Compute some derivatives only necessary for dense output
+        d1g2(); d1g3(); d1g4(); d1g5(); d2w2(); d2w3(); d2w4(); d2w5();
+        dgs_ << d1g1_, d1g2_, d1g3_, d1g4_, d1g5_, d1g6_;
+        d2ws_ << d2w1_, d2w2_, d2w3_, d2w4_, d2w5_, d2w6_;      
+        
+        integrand6 = 4.0*gs_.cwiseProduct(gs_).cwiseQuotient(ws_) +
+        4.0*dws_.cwiseProduct(gs_).cwiseQuotient(ws_.cwiseProduct(ws_)) +
+        dws_.cwiseProduct(dws_).cwiseQuotient(ws_.cwiseProduct(ws_.cwiseProduct(ws_)));
+        for(int i=0; i<=5; i++)
+            s1_interp(i) = -1./2*std::log(ws_(i));
+        s2_interp = -1/4.0*(dws_.cwiseQuotient(ws_.cwiseProduct(ws_)) + 2.0*gs_.cwiseQuotient(ws_));
+        s3_interp =
+        1/4.0*(gs_.cwiseProduct(gs_).cwiseQuotient((ws_.cwiseProduct(ws_)))) +
+        1/4.0*(dgs_.cwiseQuotient(ws_.cwiseProduct(ws_))) -
+        3/16.0*(dws_.cwiseProduct(dws_).cwiseQuotient(ws_.cwiseProduct(ws_).cwiseProduct(ws_.cwiseProduct(ws_))))
+        + 1/8.0*(d2ws_.cwiseQuotient(ws_.cwiseProduct(ws_).cwiseProduct(ws_)));
+       
+        // S0
+        s0_vdm_vec = h/2.0*std::complex<double>(0,1)*integ_vandermonde*ws_;
+        // S1
+        s1_vdm_vec = -h/2.0*integ_vandermonde*gs_;
+        s1_vdm_vec.head(5) += (interp_vandermonde*s1_interp).tail(5);
+        // S2
+        s2_vdm_vec = -h/2.0*1/8.0*integ_vandermonde*integrand6;
+        s2_vdm_vec.head(5) += (interp_vandermonde*s2_interp).tail(5);
+        // S3
+        s3_vdm_vec = Eigen::Matrix<std::complex<double>,6,1>::Zero(); 
+        s3_vdm_vec.head(5) += (interp_vandermonde*s3_interp).tail(5);
+        
+        x_vdm.tail(6) = s0_vdm_vec + s1_vdm_vec + std::complex<double>(0,1)*s2_vdm_vec + s3_vdm_vec; 
+        x_vdm(0) = ap_;
+
+        
     // Lower order step for correction
         // A, B
         dsi_(order_) = 0.0; dds_(order_) = 0.0;
         dfpi(); dfmi();
         ddfp(); ddfm();
         ap(); am(); bp(); bm();
         // Calculate step
@@ -304,14 +377,21 @@
     dodxs.resize(docount);
     Eigen::Matrix<double,6,1> dows6, dodws6; // weights for dense integration/interpolation
     Eigen::Matrix<std::complex<double>,6,1> integrand6, s3_interp, s2_interp, s1_interp;
     Eigen::Matrix<std::complex<double>,6,1> ds1_interp, ds2_interp, ds3_interp; 
     double t_trans;
     std::complex<double> s0,s1,s2,s3,dense_fp,dense_fm,dense_x;
     std::complex<double> ds0,ds1,ds2,ds3,dense_dfpf,dense_dfmf,dense_dx;
+    // Vandermonde dense output
+    Eigen::Matrix<std::complex<double>,6,1> s0_vdm_vec,s1_vdm_vec,s2_vdm_vec,s3_vdm_vec;
+    Eigen::Matrix<double,6,1> t_trans_vec,t_trans_vec_interp;
+    std::complex<double> s0_vdm,s1_vdm,s2_vdm,s3_vdm;
+    Eigen::Matrix<std::complex<double>,7,1> s_vdm_vec;
+    double tt1,tt2,tt3,tt4,tt5,tt6;
+
    
     // Compute some derivatives only necessary for dense output
     d1g2(); d1g3(); d1g4(); d1g5(); d2w2(); d2w3(); d2w4(); d2w5();
     d2g2(); d2g3(); d2g4(); d2g5(); d3w2(); d3w3(); d3w4(); d3w5();
     dgs_ << d1g1_, d1g2_, d1g3_, d1g4_, d1g5_, d1g6_;
     d2ws_ << d2w1_, d2w2_, d2w3_, d2w4_, d2w5_, d2w6_;      
     d2gs_ << d2g1_, d2g2_, d2g3_, d2g4_, d2g5_, d2g6_;
@@ -350,14 +430,55 @@
             dense_s_ << s0, s1, std::complex<double>(0,1)*s2, s3;
             dense_fp = std::exp(dense_s_.sum());
             dense_fm = std::conj(dense_fp);
             dense_x = dense_ap_*dense_fp + dense_am_*dense_fm;
             *doxit = dense_x;
             doxit++;
 
+            // Same, but with Vandermonde matrix:
+            tt1 = t_trans; 
+            tt2 = tt1*t_trans;
+            tt3 = tt2*t_trans;
+            tt4 = tt3*t_trans;
+            tt5 = tt4*t_trans;
+            tt6 = tt5*t_trans;
+            t_trans_vec << tt1+1, tt2-1, tt3+1, tt4-1, tt5+1, tt6-1; 
+            t_trans_vec_interp << 0, tt1+1, tt2-1, tt3+1, tt4-1, tt5+1;
+            // S0
+            s0_vdm_vec = h/2.0*std::complex<double>(0,1)*integ_vandermonde*ws_;
+            s0_vdm = t_trans_vec.dot(s0_vdm_vec); 
+            // S1
+            s1_vdm = -h/2.0*t_trans_vec.dot(integ_vandermonde*gs_) + t_trans_vec_interp.dot(interp_vandermonde*s1_interp);
+            s1_vdm_vec = -h/2.0*integ_vandermonde*gs_;
+            s1_vdm_vec.head(5) += (interp_vandermonde*s1_interp).tail(5);
+            s1_vdm = t_trans_vec.dot(s1_vdm_vec);
+            // S2
+            s2_vdm_vec = -h/2.0*1/8.0*integ_vandermonde*integrand6;
+            s2_vdm_vec.head(5) += (interp_vandermonde*s2_interp).tail(5);
+            s2_vdm = t_trans_vec.dot(s2_vdm_vec);
+            // S3
+            s3_vdm_vec = Eigen::Matrix<std::complex<double>,6,1>::Zero(); 
+            s3_vdm_vec.head(5) += (interp_vandermonde*s3_interp).tail(5);
+            s3_vdm = t_trans_vec.dot(s3_vdm_vec) ;
+            //x_vdm = dense_ap_*(s0_vdm_vec + s1_vdm_vec + s2_vdm_vec + s3_vdm_vec); 
+
+            //std::cout << std::setprecision(15) << "dense S0 with Vandermonde matrix: " << s0_vdm << std::endl;
+            //std::cout << "dense S0 with classical theory: " << s0 << std::endl;
+            //std::cout << std::setprecision(15) << "dense S1 with Vandermonde matrix: " << s1_vdm << std::endl;
+            //std::cout << "dense S1 with classical theory: " << s1 << std::endl;
+            //std::cout << std::setprecision(15) << "dense S2 with Vandermonde matrix: " << s2_vdm << std::endl;
+            //std::cout << "dense S1 with classical theory: " << s2 << std::endl;
+            //std::cout << std::setprecision(15) << "dense S3 with Vandermonde matrix: " << s3_vdm << std::endl;
+            //std::cout << "dense S3 with classical theory: " << s3 << std::endl;
+
+            //std::cout << "Representation of S0: " << s0_vdm_vec << std::endl;
+            //std::cout << "Representation of S1: " << s1_vdm_vec << std::endl;
+            //std::cout << "Ap: " << dense_ap_ << ", Am: " << dense_am_ << std::endl;
+
+
             // Dense output dx
             ds0 = std::complex<double>(0,1)*dense_interpolate(dodws6,ws_);
             ds1 = dense_interpolate(dodws6,gs_);
             ds1_interp = -1./2*dws_.cwiseQuotient(ws_);
             ds1 = dense_interpolate(dodws6,ds1_interp) - ds1;
             ds2_interp = -1./2*gs_.cwiseProduct(gs_.cwiseQuotient(ws_)) - 1./2*dgs_.cwiseQuotient(ws_) + 3./8*(dws_.cwiseProduct(dws_)).cwiseQuotient((ws_.cwiseProduct(ws_)).cwiseProduct(ws_)) - 1./4*d2ws_.cwiseQuotient(ws_.cwiseProduct(ws_));
             ds2 = dense_interpolate(dodws6,ds2_interp);
```

### Comparing `pyoscode-1.0.2/pyoscode/_pyoscode.hpp` & `pyoscode-1.1.2/pyoscode/_pyoscode.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -8,25 +8,34 @@
 #include <fstream>
 #include <complex>
 #include <iostream>
 #include <cmath>
 
 /* Docstrings */
 static char module_docstring[] = 
-"pyoscode: this module provides an interface for oscode, for solving oscillatory ordinary differential equations with the RKWKB method.";
+"pyoscode: this module provides an interface for oscode, for solving\
+oscillatory ordinary differential equations with the RKWKB method.";
 
-static char solve_docstring[] =
-"Runs the solver";
+static char solve_docstring[] = "Runs the solver with w, g provided as arrays",
+            solve_fn_docstring[] = "Runs the solver with w, g provided as\
+            functions";
 
 /* Available functions */
+/* Solve with w, g provided as arrays */
 static PyObject *_pyoscode_solve(PyObject *self, PyObject *args, PyObject *kwargs);
+/* Solve with w, g provided as functions */
+static PyObject *_pyoscode_solve_fn(PyObject *self, PyObject *args, PyObject *kwargs);
+/* Callback functions */
+static std::complex<double> w(double t);
+static std::complex<double> g(double t);
 
 /* Module interface */
 static PyMethodDef module_methods[] = {
     {"solve", (PyCFunction) _pyoscode_solve, METH_VARARGS | METH_KEYWORDS, solve_docstring},
+    {"solve_fn", (PyCFunction) _pyoscode_solve_fn, METH_VARARGS | METH_KEYWORDS, solve_fn_docstring},
     {NULL, NULL, 0, NULL}
 };
  
 #ifdef PYTHON3
 static struct PyModuleDef _pyoscodemodule = {
     PyModuleDef_HEAD_INIT,
     "_pyoscode",
```

### Comparing `pyoscode-1.0.2/pyoscode.egg-info/PKG-INFO` & `pyoscode-1.1.2/pyoscode.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,304 +1,324 @@
 Metadata-Version: 2.1
 Name: pyoscode
-Version: 1.0.2
+Version: 1.1.2
 Summary: oscode: Oscillatory ordinary differential equation solver
 Home-page: https://github.com/fruzsinaagocs/oscode
 Author: Fruzsina Agocs
 Author-email: fa325@cam.ac.uk
 License: oscode
 Project-URL: Documentation, https://oscode.readthedocs.io
-Description: ========================================================================
-        oscode: Oscillatory ordinary differential equation solver
-        ========================================================================
-        
-        .. image:: https://codecov.io/gh/fruzsinaagocs/oscode/branch/joss-paper/graph/badge.svg
-                :target: https://codecov.io/gh/fruzsinaagocs/oscode
-                :alt: codecov status
-        .. image:: https://travis-ci.org/fruzsinaagocs/oscode.svg?branch=master
-                :target: https://travis-ci.org/fruzsinaagocs/oscode
-                :alt: Travis CI build status
-        .. image:: https://readthedocs.org/projects/oscode/badge/?version=latest
-                :target: https://oscode.readthedocs.io/en/latest/?badge=latest
-                :alt: Documentation Status
-        .. image:: https://badges.gitter.im/oscode-help/community.svg
-                :target: https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
-                :alt: Chat on gitter
-        .. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-                :target: https://opensource.org/licenses/BSD-3-Clause
-                :alt: BSD 3-clause license
-        .. image:: https://img.shields.io/pypi/dm/pyoscode?color=indigo 
-                :target: https://pypi.org/project/pyoscode/
-                :alt: PyPI downloads
-        .. image:: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda/status.svg
-                :target: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda
-                :alt: JOSS status
-        
-        
-        |
-        |
-        
-        .. contents::
-           :local:
-        
-        |
-        
-        About
-        -----
-        
-        Oscode is a C++ tool with a Python interface that solves **osc**\illatory
-        **o**\rdinary **d**\ifferential **e**\quations efficiently. It is designed to
-        deal with equations of the form
-        
-        .. image:: 
-            https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/oscillator.png
-        
-        where |gamma| (friction term) and |omega| (frequency) can be given as arrays.
-        
-        .. |gamma| image:: https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/gamma.png
-        
-        .. |omega| image:: https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/omega.png
-        
-        Oscode makes use of an analytic approximation of x(t) embedded in a
-        stepping procedure to skip over long regions of oscillations, giving a reduction
-        in computing time. The approximation is valid when the frequency changes slowly
-        relative to the timescales of integration, it is therefore worth applying when
-        this condition holds for at least some part of the integration range. 
-        
-        For the details of the numerical method used by oscode, see Citation_.
-        
-        
-        Installation
-        ------------
-        
-        Dependencies
-        ~~~~~~~~~~~~
-        
-        Basic requirements for using the C++ interface:
-        
-        - C++11 or later
-        - `Eigen <http://eigen.tuxfamily.org/index.php?title=Main_Page>`__ (a header-only library included in this source)
-        
-        The strictly necessary Python dependencies are automatically installed when you use `pip` or the `setup.py`. They are:
-        
-        - `numpy <https://pypi.org/project/numpy/>`__
-        
-        The *optional* dependencies are: 
-        
-        - for tests
-            - `scipy <https://pypi.org/project/scipy/>`__ 
-            - `pytest <https://docs.pytest.org/en/stable/getting-started.html>`__ 
-        - for examples/plotting
-            - `matplotlib <https://pypi.org/project/matplotlib/>`__
-            - `scipy <https://pypi.org/project/scipy/>`__ 
-        - for generating offline documentation
-            - `sphinx <https://pypi.org/project/Sphinx/>`__ 
-            - `doxygen <https://www.doxygen.nl/index.html>`__
-            - `breathe <https://pypi.org/project/breathe/>`__
-            - `exhale <https://pypi.org/project/exhale/>`__
-        
-        
-        Python
-        ~~~~~~
-        
-        ``pyoscode`` can be installed via pip 
-        
-        .. code:: bash
-           
-           pip install pyoscode
-        
-        or via the setup.py
-        
-        .. code:: bash
-        
-           git clone https://github.com/fruzsinaagocs/oscode
-           cd oscode
-           python setup.py install --user
-        
-        or
-        
-        .. code:: bash
-        
-           git clone https://github.com/fruzsinaagocs/oscode
-           cd oscode
-           pip install .
-        
-        You can then import ``pyoscode`` from anywhere. Omit the ``--user`` option if
-        you wish to install globally or in a virtual environment. If you have any
-        difficulties, check out the `FAQs - Installation
-        <https://github.com/fruzsinaagocs/oscode#installation-1>`__ section below. 
-        
-        You can check that things are working by running `tests/` (also ran by Travis continuous integration):
-        
-        .. code:: bash
-        
-           pytest tests/
-        
-        C++
-        ~~~
-        
-        ``oscode`` is a header-only C++ package, it requires no installation.
-        
-        .. code:: bash
-        
-           git clone https://github.com/fruzsinaagocs/oscode
-        
-        and then include the relevant header files in your C++ code:
-        
-        .. code:: c
-        
-            #include "solver.hpp"
-            #include "system.hpp"
-        
-        
-        Quick start
-        -----------
-        
-        Try the following quick examples. They are available in the `examples
-        <https://github.com/fruzsinaagocs/oscode/tree/master/examples/>`__.
-        
-        Python
-        ~~~~~~
-        
-        :Introduction to pyoscode: |intro_binder|
-        :Cosmology examples: |cosmology_binder|
-        :Scipy 2020 lecture notebook: |scipy_binder|
-        
-        .. |intro_binder| image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/introduction_to_pyoscode.ipynb
-        
-        .. |cosmology_binder| image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/cosmology.ipynb
-        
-        .. |scipy_binder| image:: https://mybinder.org/badge_logo.svg
-         :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/pyoscode_scipy.ipynb
-        
-        
-        .. image::
-            https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/spectra.gif
-            :width: 800
-        
-        C++
-        ~~~
-        
-        :Introduction to oscode: `examples/burst.cpp`
-        :To plot results from `burst.cpp`: `examples/plot_burst.py`
-        
-        To compile and run:
-        
-        .. code:: bash
-        
-            g++ -g -Wall -std=c++11 -c -o burst.o burst.cpp
-            g++ -g -Wall -std=c++11 -o burst burst.o
-            ./burst
-        
-        
-        Documentation
-        -------------
-        
-        Documentation is hosted at `readthedocs <https://oscode.readthedocs.io>`__.
-        
-        To build your own local copy of the documentation you can run:
-        
-        .. code:: bash
-        
-           cd pyoscode/docs
-           make html
-        
-        Citation
-        --------
-        
-        If you use ``oscode`` to solve equations for a publication, please cite:
-        
-        - `Efficient method for solving highly oscillatory ordinary differential equations with applications to physical systems <https://doi.org/10.1103/PhysRevResearch.2.013030>`__,
-        - `Dense output for highly oscillatory numerical solutions  <https://arxiv.org/abs/2007.05013>`__
-        
-        Contributing
-        ------------
-        
-        Any comments and improvements to this project are welcome. You can contribute
-        by:
-        
-        - Opening and `issue <https://www.github.com/fruzsinaagocs/oscode/issues/>`__ to report bugs and propose new features.
-        - Making a pull request.
-        
-        Further help
-        ------------
-        
-        You can get help by submitting an issue or posting a message on `Gitter <https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge>`__.
-        
-        FAQs
-        ----
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        1. Eigen import errors:
-            .. code:: bash
-        
-               pyoscode/_pyoscode.hpp:6:10: fatal error: Eigen/Dense: No such file or directory
-                #include <Eigen/Dense>
-                          ^~~~~~~~~~~~~
-        
-            Try explicitly including the location of your Eigen library via the
-            ``CPLUS_INCLUDE_PATH`` environment variable, for example:
-        
-            .. code:: bash
-        
-               CPLUS_INCLUDE_PATH=/usr/include/eigen3 python setup.py install --user
-               # or 
-               CPLUS_INCLUDE_PATH=/usr/include/eigen3 pip install pyoscode
-        
-            where  ``/usr/include/eigen3`` should be replaced with your system-specific
-            eigen location.
-        
-        Thanks
-        ------
-        
-        Many thanks to **Will Handley**, **Lukas Hergt**, **Anthony Lasenby**, and **Mike Hobson** for
-        their support and advice regarding the algorithm behind `oscode`.
-        There are many packages without which some part of `oscode` (e.g. testing and
-        examples) wouldn't run as nicely and smoothly, thank you all developers for
-        making and maintaining these open-source projects. A special thanks goes to the
-        devs of `exhale <https://pypi.org/project/exhale/>`__ for making the beautiful C++ documentation possible. 
-        
-        
-        Changelog
-        ---------
-        
-        - 1.0.2: current version
-            - Fixed getting correct numpy include directories
-        - 1.0.1:
-            - Added `pyproject.toml` to handle build dependencies (numpy)
-        - 1.0.0:
-            - Dense output
-            - Arrays for frequency and damping term need not be evenly spaced
-            - Automatic C++ documentation on readthedocs
-            - Eigen included in source for pip installability
-            - First pip release :)
-        - 0.1.2:
-            - Bug that occurred when beginning and end of integration coincided
-              corrected
-        - 0.1.1:
-            - Automatic detection of direction of integration
-        - 0.1.0:
-            - Memory leaks at python interface fixed
-            - C++ documentation added 
-        
 Keywords: PPS,cosmic inflation,cosmology,oscillatory,ODE
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Provides-Extra: docs
 Provides-Extra: examples
+Provides-Extra: docs
 Provides-Extra: testing
+License-File: LICENSE
+
+========================================================================
+oscode: Oscillatory ordinary differential equation solver
+========================================================================
+
+.. image:: https://codecov.io/gh/fruzsinaagocs/oscode/branch/joss-paper/graph/badge.svg
+        :target: https://codecov.io/gh/fruzsinaagocs/oscode
+        :alt: codecov status
+.. image:: https://github.com/fruzsinaagocs/oscode/actions/workflows/python-package.yml/badge.svg
+        :target: https://github.com/fruzsinaagocs/oscode/actions
+        :alt: GH workflow status
+.. image:: https://readthedocs.org/projects/oscode/badge/?version=latest
+        :target: https://oscode.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+.. image:: https://badges.gitter.im/oscode-help/community.svg
+        :target: https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
+        :alt: Chat on gitter
+.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+        :target: https://opensource.org/licenses/BSD-3-Clause
+        :alt: BSD 3-clause license
+.. image:: https://img.shields.io/pypi/dm/pyoscode?color=indigo 
+        :target: https://pypi.org/project/pyoscode/
+        :alt: PyPI downloads
+.. image:: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda/status.svg
+        :target: https://joss.theoj.org/papers/d4c9396ef9b2b595e2f3881a4f8a7cda
+        :alt: JOSS status
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4322958.svg
+        :target: https://doi.org/10.5281/zenodo.4322958
+        :alt: Zenodo doi
+
+|
+|
+
+.. contents::
+   :local:
+
+|
+
+About
+-----
+
+Oscode is a C++ tool with a Python interface that solves **osc**\illatory
+**o**\rdinary **d**\ifferential **e**\quations efficiently. It is designed to
+deal with equations of the form
+
+.. image:: 
+    https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/oscillator.png
+
+where |gamma| (friction term) and |omega| (frequency) can be given as arrays.
+
+.. |gamma| image:: https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/gamma.png
+
+.. |omega| image:: https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/omega.png
+
+Oscode makes use of an analytic approximation of x(t) embedded in a
+stepping procedure to skip over long regions of oscillations, giving a reduction
+in computing time. The approximation is valid when the frequency changes slowly
+relative to the timescales of integration, it is therefore worth applying when
+this condition holds for at least some part of the integration range. 
+
+For the details of the numerical method used by oscode, see Citation_.
+
+
+Installation
+------------
+
+Dependencies
+~~~~~~~~~~~~
+
+Basic requirements for using the C++ interface:
+
+- C++11 or later
+- `Eigen <http://eigen.tuxfamily.org/index.php?title=Main_Page>`__ (a header-only library included in this source)
+
+The strictly necessary Python dependencies are automatically installed when you use `pip` or the `setup.py`. They are:
+
+- `numpy <https://pypi.org/project/numpy/>`__
+
+The *optional* dependencies are: 
+
+- for tests
+    - `scipy <https://pypi.org/project/scipy/>`__ 
+    - `pytest <https://docs.pytest.org/en/stable/getting-started.html>`__ 
+- for examples/plotting
+    - `matplotlib <https://pypi.org/project/matplotlib/>`__
+    - `scipy <https://pypi.org/project/scipy/>`__ 
+- for generating offline documentation
+    - `sphinx <https://pypi.org/project/Sphinx/>`__ 
+    - `doxygen <https://www.doxygen.nl/index.html>`__
+    - `breathe <https://pypi.org/project/breathe/>`__
+    - `exhale <https://pypi.org/project/exhale/>`__
+
+
+Python
+~~~~~~
+
+``pyoscode`` can be installed via pip 
+
+.. code:: bash
+   
+   pip install pyoscode
+
+or via the setup.py
+
+.. code:: bash
+
+   git clone https://github.com/fruzsinaagocs/oscode
+   cd oscode
+   python setup.py install --user
+
+or
+
+.. code:: bash
+
+   git clone https://github.com/fruzsinaagocs/oscode
+   cd oscode
+   pip install .
+
+You can then import ``pyoscode`` from anywhere. Omit the ``--user`` option if
+you wish to install globally or in a virtual environment. If you have any
+difficulties, check out the `FAQs - Installation
+<https://github.com/fruzsinaagocs/oscode#installation-1>`__ section below. 
+
+You can check that things are working by running `tests/` (also ran by Travis continuous integration):
+
+.. code:: bash
+
+   pytest tests/
+
+C++
+~~~
+
+``oscode`` is a header-only C++ package, it requires no installation.
+
+.. code:: bash
+
+   git clone https://github.com/fruzsinaagocs/oscode
+
+and then include the relevant header files in your C++ code:
+
+.. code:: c
+
+    #include "solver.hpp"
+    #include "system.hpp"
+
+
+Quick start
+-----------
+
+Try the following quick examples. They are available in the `examples
+<https://github.com/fruzsinaagocs/oscode/tree/master/examples/>`__.
+
+Python
+~~~~~~
+
+:Introduction to pyoscode: |intro_binder|
+:Cosmology examples: |cosmology_binder|
+:Scipy 2020 lecture notebook: |scipy_binder|
+
+.. |intro_binder| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/introduction_to_pyoscode.ipynb
+
+.. |cosmology_binder| image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/cosmology.ipynb
+
+.. |scipy_binder| image:: https://mybinder.org/badge_logo.svg
+ :target: https://mybinder.org/v2/gh/fruzsinaagocs/oscode/master?filepath=examples/pyoscode_scipy.ipynb
+
+
+.. image::
+    https://github.com/fruzsinaagocs/oscode/raw/master/pyoscode/images/spectra.gif
+    :width: 800
+
+C++
+~~~
+
+:Introduction to oscode: `examples/burst.cpp`
+:To plot results from `burst.cpp`: `examples/plot_burst.py`
+
+To compile and run:
+
+.. code:: bash
+    
+    cd examples/
+    g++ -I../include/ -g -Wall -std=c++11 -c -o burst.o burst.cpp
+    g++ -I../include/ -g -Wall -std=c++11 -o burst burst.o
+    ./burst
+
+
+Documentation
+-------------
+
+Documentation is hosted at `readthedocs <https://oscode.readthedocs.io>`__.
+
+To build your own local copy of the documentation you can run:
+
+.. code:: bash
+
+   cd pyoscode/docs
+   make html
+
+Citation
+--------
+
+If you use ``oscode`` to solve equations for a publication, please cite:
+
+- `Efficient method for solving highly oscillatory ordinary differential equations with applications to physical systems <https://doi.org/10.1103/PhysRevResearch.2.013030>`__,
+- `Dense output for highly oscillatory numerical solutions  <https://arxiv.org/abs/2007.05013>`__
+
+Contributing
+------------
+
+Any comments and improvements to this project are welcome. You can contribute
+by:
+
+- Opening and `issue <https://www.github.com/fruzsinaagocs/oscode/issues/>`__ to report bugs and propose new features.
+- Making a pull request.
+
+Further help
+------------
+
+You can get help by submitting an issue or posting a message on `Gitter <https://gitter.im/oscode-help/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge>`__.
+
+FAQs
+----
+
+Installation
+~~~~~~~~~~~~
+
+1. Eigen import errors:
+    .. code:: bash
+
+       pyoscode/_pyoscode.hpp:6:10: fatal error: Eigen/Dense: No such file or directory
+        #include <Eigen/Dense>
+                  ^~~~~~~~~~~~~
+
+    Try explicitly including the location of your Eigen library via the
+    ``CPLUS_INCLUDE_PATH`` environment variable, for example:
+
+    .. code:: bash
+
+       CPLUS_INCLUDE_PATH=/usr/include/eigen3 python setup.py install --user
+       # or 
+       CPLUS_INCLUDE_PATH=/usr/include/eigen3 pip install pyoscode
+
+    where  ``/usr/include/eigen3`` should be replaced with your system-specific
+    eigen location.
+
+Thanks
+------
+
+Many thanks to **Will Handley**, **Lukas Hergt**, **Anthony Lasenby**, and **Mike Hobson** for
+their support and advice regarding the algorithm behind `oscode`.
+There are many packages without which some part of `oscode` (e.g. testing and
+examples) wouldn't run as nicely and smoothly, thank you all developers for
+making and maintaining these open-source projects. A special thanks goes to the
+devs of `exhale <https://pypi.org/project/exhale/>`__ for making the beautiful C++ documentation possible. 
+
+
+Changelog
+---------
+
+- 1.1.2:
+    - Dense output bug fix at the C++ interface 
+- 1.1.1: 
+    - Support for mac and Windows OS at CI.
+- 1.1.0:
+    - Users can now define w, g as functions in Python (pyoscode) and call the solver via pyoscode.solve_fn(...)
+- 1.0.6:
+    - Fix issues related to dense output not being correctly generated, e.g. when timepoints at which dense output was asked for are in descending order, etc. 
+- 1.0.5:
+    - Fixes related to dense output generation
+    - Support for w, g to be given as class member functions in C++
+    - Switched to GH actions for continuous integration, and fixed code such that unit tests would run again
+    - Minor tweaks
+- 1.0.4:
+    - set minimally required numpy version: numpy>=1.20.0
+    - drop Python 2.7 support, instead support 3.8 and 3.9 in addition to 3.7
+- 1.0.3: 
+    - paper accepted to JOSS
+- 1.0.2:
+    - Fixed getting correct numpy include directories
+- 1.0.1:
+    - Added `pyproject.toml` to handle build dependencies (numpy)
+- 1.0.0:
+    - Dense output
+    - Arrays for frequency and damping term need not be evenly spaced
+    - Automatic C++ documentation on readthedocs
+    - Eigen included in source for pip installability
+    - First pip release :)
+- 0.1.2:
+    - Bug that occurred when beginning and end of integration coincided
+      corrected
+- 0.1.1:
+    - Automatic detection of direction of integration
+- 0.1.0:
+    - Memory leaks at python interface fixed
+    - C++ documentation added
```

### Comparing `pyoscode-1.0.2/pyoscode.egg-info/SOURCES.txt` & `pyoscode-1.1.2/pyoscode.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,36 @@
-MANIFEST.in
+.gitignore
+.readthedocs.yml
+Dockerfile
+LICENSE
 README.rst
 pyproject.toml
+requirements.txt
 setup.py
+.github/pull_request_template.md
+.github/workflows/python-package.yml
+JOSS-paper/paper.bib
+JOSS-paper/paper.md
+examples/airy.py
+examples/burst.cpp
+examples/cosmology.ipynb
+examples/introduction_to_pyoscode.ipynb
+examples/plot_burst.py
+examples/pyoscode_scipy.ipynb
+examples/test-rk.py
+examples/images/airy.png
+examples/images/bingo-singlek-k1e-5-ref.txt
+examples/images/bingo-singlek-k1e-5.txt
+examples/images/cambridge.png
+examples/images/caplogo.svg
+examples/images/cmb.png
+examples/images/kavli.jpg
+examples/images/rkwkb-single-k1e-5.txt
+examples/images/singlek-kd-bd-2a.txt
+examples/images/singlek-kd-bg-2a-ref.txt
 include/interpolator.hpp
 include/rksolver.hpp
 include/solver.hpp
 include/system.hpp
 include/wkbsolver.hpp
 include/Eigen/Cholesky
 include/Eigen/CholmodSupport
@@ -311,8 +336,24 @@
 pyoscode/_pyoscode.cpp
 pyoscode/_pyoscode.hpp
 pyoscode/_python.hpp
 pyoscode.egg-info/PKG-INFO
 pyoscode.egg-info/SOURCES.txt
 pyoscode.egg-info/dependency_links.txt
 pyoscode.egg-info/requires.txt
-pyoscode.egg-info/top_level.txt
+pyoscode.egg-info/top_level.txt
+pyoscode/docs/Makefile
+pyoscode/docs/requirements.txt
+pyoscode/docs/source/conf.py
+pyoscode/docs/source/index.rst
+pyoscode/docs/source/introduction.rst
+pyoscode/docs/source/oscode.rst
+pyoscode/docs/source/pyoscode.rst
+pyoscode/images/airy-example.png
+pyoscode/images/burst-example.png
+pyoscode/images/gamma.png
+pyoscode/images/omega.png
+pyoscode/images/oscillator.gif
+pyoscode/images/oscillator.png
+pyoscode/images/spectra.gif
+tests/test_airy.py
+tests/test_arrays.py
```

### Comparing `pyoscode-1.0.2/setup.py` & `pyoscode-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     include_dirs=['include','pyoscode',np.get_include()],
     depends=["pyoscode/_python.hpp", "pyoscode/_pyoscode.hpp"],
     extra_compile_args=['-std=c++11','-Wall']
     )
 
 setup(
     name="pyoscode",
-    version="1.0.2",
+    version="1.1.2",
     description=readme(short=True),
     long_description=readme(),
     url="https://github.com/fruzsinaagocs/oscode",
     project_urls={"Documentation":"https://oscode.readthedocs.io"},
     author="Fruzsina Agocs",
     author_email="fa325@cam.ac.uk",
     packages=find_packages(),
@@ -39,15 +39,14 @@
     headers=["pyoscode/_python.hpp", "pyoscode/_pyoscode.hpp"],
     include_dirs=[np.get_include()],
     keywords="PPS, cosmic inflation, cosmology, oscillatory, ODE",
     classifiers=[
                 'Intended Audience :: Developers',
                 'Intended Audience :: Science/Research',
                 'Natural Language :: English',
-                'Programming Language :: Python :: 2.7',
                 'Programming Language :: Python :: 3.4',
                 'Programming Language :: Python :: 3.5',
                 'Programming Language :: Python :: 3.6',
                 'Programming Language :: Python :: 3.7',
                 'Topic :: Scientific/Engineering',
                 'Topic :: Scientific/Engineering :: Astronomy',
                 'Topic :: Scientific/Engineering :: Physics',
```

