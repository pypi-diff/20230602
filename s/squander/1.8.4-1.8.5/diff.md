# Comparing `tmp/squander-1.8.4.tar.gz` & `tmp/squander-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squander-1.8.4.tar", last modified: Sat May 27 16:26:58 2023, max compression
+gzip compressed data, was "squander-1.8.5.tar", last modified: Fri Jun  2 12:16:50 2023, max compression
```

## Comparing `squander-1.8.4.tar` & `squander-1.8.5.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15412 2023-05-27 16:25:37.000000 squander-1.8.4/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    35149 2023-05-27 16:24:34.000000 squander-1.8.4/LICENSE
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      121 2023-05-27 16:24:34.000000 squander-1.8.4/MANIFEST.in
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16207 2023-05-27 16:26:58.646819 squander-1.8.4/PKG-INFO
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15619 2023-05-27 16:24:34.000000 squander-1.8.4/README.md
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.630819 squander-1.8.4/cmake/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4306 2023-05-27 16:24:34.000000 squander-1.8.4/cmake/check_AVX.cmake
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.630819 squander-1.8.4/common/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6776 2023-05-27 16:24:34.000000 squander-1.8.4/common/Adam.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8316 2023-05-27 16:24:34.000000 squander-1.8.4/common/common.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-27 16:24:34.000000 squander-1.8.4/common/common_DFE.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5524 2023-05-27 16:24:34.000000 squander-1.8.4/common/config_element.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14292 2023-05-27 16:24:34.000000 squander-1.8.4/common/dot.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.634819 squander-1.8.4/common/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3441 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/Adam.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      166 2023-05-27 16:26:35.000000 squander-1.8.4/common/include/Config.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      216 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/Config.h.in
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2109 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/QGDTypes.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5357 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/common.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3026 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/common_DFE.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3423 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/config_element.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7798 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/dot.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9130 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/lbfgs.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2443 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/logging.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3812 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/matrix.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13831 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/matrix_base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3752 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/matrix_real.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1393 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/mpi_base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1468 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/numpy_interface.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9234 2023-05-27 16:24:34.000000 squander-1.8.4/common/include/tolmin.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   156010 2023-05-27 16:24:34.000000 squander-1.8.4/common/lbfgs.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2515 2023-05-27 16:24:34.000000 squander-1.8.4/common/logging.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5065 2023-05-27 16:24:34.000000 squander-1.8.4/common/matrix.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4497 2023-05-27 16:24:34.000000 squander-1.8.4/common/matrix_real.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1095 2023-05-27 16:24:34.000000 squander-1.8.4/common/mpi_base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4808 2023-05-27 16:24:34.000000 squander-1.8.4/common/numpy_interface.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    58339 2023-05-27 16:24:34.000000 squander-1.8.4/common/tolmin.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.634819 squander-1.8.4/decomposition/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    57710 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    37081 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   117800 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition_Base.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16713 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    70942 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition_adaptive.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    12741 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/N_Qubit_Decomposition_custom.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23508 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/Sub_Matrix_Decomposition.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8536 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.634819 squander-1.8.4/decomposition/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16528 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7166 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15866 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition_Base.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5077 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8301 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition_adaptive.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3393 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/N_Qubit_Decomposition_custom.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6924 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/Sub_Matrix_Decomposition.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3723 2023-05-27 16:24:34.000000 squander-1.8.4/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/gates/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5728 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Adaptive.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4900 2023-05-27 16:24:34.000000 squander-1.8.4/gates/CH.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4937 2023-05-27 16:24:34.000000 squander-1.8.4/gates/CNOT.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5839 2023-05-27 16:24:34.000000 squander-1.8.4/gates/CRY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4841 2023-05-27 16:24:34.000000 squander-1.8.4/gates/CZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7781 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Composite.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11507 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Gate.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   120998 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Gates_block.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8547 2023-05-27 16:24:34.000000 squander-1.8.4/gates/ON.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6819 2023-05-27 16:24:34.000000 squander-1.8.4/gates/RX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6815 2023-05-27 16:24:34.000000 squander-1.8.4/gates/RY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7110 2023-05-27 16:24:34.000000 squander-1.8.4/gates/RZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8697 2023-05-27 16:24:34.000000 squander-1.8.4/gates/SX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9587 2023-05-27 16:24:34.000000 squander-1.8.4/gates/SYC.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15837 2023-05-27 16:24:34.000000 squander-1.8.4/gates/U3.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8769 2023-05-27 16:24:34.000000 squander-1.8.4/gates/UN.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7950 2023-05-27 16:24:34.000000 squander-1.8.4/gates/X.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5671 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Y.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5672 2023-05-27 16:24:34.000000 squander-1.8.4/gates/Z.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/gates/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3421 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Adaptive.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2454 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/CH.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2530 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/CNOT.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3139 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/CRY.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2453 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/CZ.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3594 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Composite.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5097 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Gate.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15824 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Gates_block.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/ON.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2838 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/RX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3114 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/RY.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2834 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/RZ.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2809 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/SX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2454 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/SYC.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6043 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/U3.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/UN.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2800 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/X.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2798 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Y.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2798 2023-05-27 16:24:34.000000 squander-1.8.4/gates/include/Z.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/gates/kernels/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23630 2023-05-27 16:24:34.000000 squander-1.8.4/gates/kernels/apply_kernel_to_input_AVX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    32382 2023-05-27 16:24:34.000000 squander-1.8.4/gates/kernels/apply_kernel_to_state_vector_input.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/gates/kernels/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1786 2023-05-27 16:24:34.000000 squander-1.8.4/gates/kernels/include/apply_kernel_to_input_AVX.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2099 2023-05-27 16:24:34.000000 squander-1.8.4/gates/kernels/include/apply_kernel_to_state_vector_input.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/nn/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    18465 2023-05-27 16:24:34.000000 squander-1.8.4/nn/NN.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/nn/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5212 2023-05-27 16:24:34.000000 squander-1.8.4/nn/include/NN.h
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/optimization_engines/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9698 2023-05-27 16:24:34.000000 squander-1.8.4/optimization_engines/RL_experience.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/optimization_engines/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3549 2023-05-27 16:24:34.000000 squander-1.8.4/optimization_engines/include/RL_experience.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      123 2023-05-27 16:24:34.000000 squander-1.8.4/pyproject.toml
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.638819 squander-1.8.4/qgd_python/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/__init__.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.642819 squander-1.8.4/qgd_python/decomposition/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4472 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7661 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    36701 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    25000 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    82737 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14278 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    40978 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3367 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.642819 squander-1.8.4/qgd_python/decomposition/test/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11142 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_Compression.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_Global_Phase.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7037 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_IBM.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1777 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_Project_Name.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5616 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_QX2.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4399 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_State_Preparation.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1656 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_Unitary.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4672 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_decomposition.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7190 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_fmo.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7018 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_heavy_hex.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6583 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_optmization_problem_combined.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4905 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/decomposition/test/test_parametric_circuit.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.642819 squander-1.8.4/qgd_python/gates/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13911 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8355 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_CH.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8292 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_CNOT.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8165 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_CZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    28668 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_Gates_Block.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8661 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_RX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8660 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_RY.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8659 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_RZ.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7903 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_SX.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7941 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_SYC.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9186 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_U3.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7621 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_X.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8499 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_Y.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8499 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/qgd_Z.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/qgd_python/gates/test/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3364 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_CH.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3409 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_CNOT.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3444 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_CZ.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3466 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_RX.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3348 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_RY.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3919 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_RZ.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3278 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_SX.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3676 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_U3.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3182 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_X.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3179 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_Y.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3232 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_Z.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6878 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/gates/test/test_gates.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/qgd_python/nn/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1332 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/nn/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/nn/__init__.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2387 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/nn/qgd_nn.py
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9606 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/nn/qgd_nn_Wrapper.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1573 2023-05-27 16:24:34.000000 squander-1.8.4/qgd_python/utils.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/random_unitary/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6628 2023-05-27 16:24:34.000000 squander-1.8.4/random_unitary/Random_Orthogonal.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11039 2023-05-27 16:24:34.000000 squander-1.8.4/random_unitary/Random_Unitary.cpp
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/random_unitary/include/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-27 16:24:34.000000 squander-1.8.4/random_unitary/include/Random_Orthogonal.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4476 2023-05-27 16:24:34.000000 squander-1.8.4/random_unitary/include/Random_Unitary.h
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       38 2023-05-27 16:26:58.646819 squander-1.8.4/setup.cfg
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1898 2023-05-27 16:24:49.000000 squander-1.8.4/setup.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/squander/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1442 2023-05-27 16:24:34.000000 squander-1.8.4/squander/__init__.py
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/squander.egg-info/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16207 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/PKG-INFO
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5157 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/SOURCES.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        1 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/dependency_links.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       50 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/requires.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       20 2023-05-27 16:26:58.000000 squander-1.8.4/squander.egg-info/top_level.txt
-drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:26:58.646819 squander-1.8.4/test_standalone/
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1996 2023-05-27 16:24:34.000000 squander-1.8.4/test_standalone/CMakeLists.txt
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6325 2023-05-27 16:24:34.000000 squander-1.8.4/test_standalone/custom_gate_structure_test.cpp
--rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4837 2023-05-27 16:24:34.000000 squander-1.8.4/test_standalone/decomposition_test.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.981646 squander-1.8.5/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15412 2023-06-02 12:15:48.000000 squander-1.8.5/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    35149 2023-05-27 16:24:34.000000 squander-1.8.5/LICENSE
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      121 2023-05-27 16:24:34.000000 squander-1.8.5/MANIFEST.in
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16207 2023-06-02 12:16:50.981646 squander-1.8.5/PKG-INFO
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15619 2023-05-27 16:24:34.000000 squander-1.8.5/README.md
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.893648 squander-1.8.5/cmake/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4306 2023-05-27 16:24:34.000000 squander-1.8.5/cmake/check_AVX.cmake
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.897647 squander-1.8.5/common/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6776 2023-05-27 16:24:34.000000 squander-1.8.5/common/Adam.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8316 2023-05-27 16:24:34.000000 squander-1.8.5/common/common.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5293 2023-05-27 16:24:34.000000 squander-1.8.5/common/common_DFE.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5524 2023-05-27 16:24:34.000000 squander-1.8.5/common/config_element.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14292 2023-05-27 16:24:34.000000 squander-1.8.5/common/dot.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.901647 squander-1.8.5/common/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3441 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/Adam.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      166 2023-05-27 16:26:35.000000 squander-1.8.5/common/include/Config.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      216 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/Config.h.in
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2109 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/QGDTypes.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5357 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/common.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3026 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/common_DFE.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3423 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/config_element.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7798 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/dot.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9130 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/lbfgs.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2443 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/logging.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3812 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/matrix.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13831 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/matrix_base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3752 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/matrix_real.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1393 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/mpi_base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1468 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/numpy_interface.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9234 2023-05-27 16:24:34.000000 squander-1.8.5/common/include/tolmin.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   156010 2023-05-27 16:24:34.000000 squander-1.8.5/common/lbfgs.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2515 2023-05-27 16:24:34.000000 squander-1.8.5/common/logging.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5065 2023-05-27 16:24:34.000000 squander-1.8.5/common/matrix.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4497 2023-05-27 16:24:34.000000 squander-1.8.5/common/matrix_real.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1095 2023-05-27 16:24:34.000000 squander-1.8.5/common/mpi_base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4808 2023-05-27 16:24:34.000000 squander-1.8.5/common/numpy_interface.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    58339 2023-05-27 16:24:34.000000 squander-1.8.5/common/tolmin.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.921647 squander-1.8.5/decomposition/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    57710 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    37081 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/N_Qubit_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   117961 2023-06-02 12:11:11.000000 squander-1.8.5/decomposition/N_Qubit_Decomposition_Base.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16713 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/N_Qubit_Decomposition_Cost_Function.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    70942 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/N_Qubit_Decomposition_adaptive.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    12741 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/N_Qubit_Decomposition_custom.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23508 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/Sub_Matrix_Decomposition.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8536 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.925647 squander-1.8.5/decomposition/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16528 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/include/Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7166 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/include/N_Qubit_Decomposition.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15866 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/include/N_Qubit_Decomposition_Base.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5077 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/include/N_Qubit_Decomposition_Cost_Function.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8301 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/include/N_Qubit_Decomposition_adaptive.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3393 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/include/N_Qubit_Decomposition_custom.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6924 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/include/Sub_Matrix_Decomposition.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3723 2023-05-27 16:24:34.000000 squander-1.8.5/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.945647 squander-1.8.5/gates/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5728 2023-05-27 16:24:34.000000 squander-1.8.5/gates/Adaptive.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4900 2023-05-27 16:24:34.000000 squander-1.8.5/gates/CH.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4937 2023-05-27 16:24:34.000000 squander-1.8.5/gates/CNOT.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5839 2023-05-27 16:24:34.000000 squander-1.8.5/gates/CRY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4841 2023-05-27 16:24:34.000000 squander-1.8.5/gates/CZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7781 2023-05-27 16:24:34.000000 squander-1.8.5/gates/Composite.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11507 2023-05-27 16:24:34.000000 squander-1.8.5/gates/Gate.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)   120998 2023-05-27 16:24:34.000000 squander-1.8.5/gates/Gates_block.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8547 2023-05-27 16:24:34.000000 squander-1.8.5/gates/ON.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6819 2023-05-27 16:24:34.000000 squander-1.8.5/gates/RX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6815 2023-05-27 16:24:34.000000 squander-1.8.5/gates/RY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7110 2023-05-27 16:24:34.000000 squander-1.8.5/gates/RZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8697 2023-05-27 16:24:34.000000 squander-1.8.5/gates/SX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9587 2023-05-27 16:24:34.000000 squander-1.8.5/gates/SYC.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15837 2023-05-27 16:24:34.000000 squander-1.8.5/gates/U3.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8769 2023-05-27 16:24:34.000000 squander-1.8.5/gates/UN.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7950 2023-05-27 16:24:34.000000 squander-1.8.5/gates/X.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5671 2023-05-27 16:24:34.000000 squander-1.8.5/gates/Y.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5672 2023-05-27 16:24:34.000000 squander-1.8.5/gates/Z.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.949647 squander-1.8.5/gates/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3421 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/Adaptive.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2454 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/CH.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2530 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/CNOT.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3139 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/CRY.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2453 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/CZ.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3594 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/Composite.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5097 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/Gate.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    15824 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/Gates_block.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/ON.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2838 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/RX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3114 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/RY.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2834 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/RZ.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2809 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/SX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2454 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/SYC.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6043 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/U3.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3412 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/UN.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2800 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/X.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2798 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/Y.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2798 2023-05-27 16:24:34.000000 squander-1.8.5/gates/include/Z.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.949647 squander-1.8.5/gates/kernels/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    23630 2023-05-27 16:24:34.000000 squander-1.8.5/gates/kernels/apply_kernel_to_input_AVX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    32382 2023-05-27 16:24:34.000000 squander-1.8.5/gates/kernels/apply_kernel_to_state_vector_input.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.949647 squander-1.8.5/gates/kernels/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1786 2023-05-27 16:24:34.000000 squander-1.8.5/gates/kernels/include/apply_kernel_to_input_AVX.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2099 2023-05-27 16:24:34.000000 squander-1.8.5/gates/kernels/include/apply_kernel_to_state_vector_input.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.949647 squander-1.8.5/nn/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    18465 2023-05-27 16:24:34.000000 squander-1.8.5/nn/NN.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.949647 squander-1.8.5/nn/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5212 2023-05-27 16:24:34.000000 squander-1.8.5/nn/include/NN.h
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.949647 squander-1.8.5/optimization_engines/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9699 2023-06-02 12:11:11.000000 squander-1.8.5/optimization_engines/RL_experience.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.949647 squander-1.8.5/optimization_engines/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3567 2023-06-02 12:11:11.000000 squander-1.8.5/optimization_engines/include/RL_experience.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)      123 2023-05-27 16:24:34.000000 squander-1.8.5/pyproject.toml
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.949647 squander-1.8.5/qgd_python/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/__init__.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.965647 squander-1.8.5/qgd_python/decomposition/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4472 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7661 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    36701 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    25000 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    82737 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    14278 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    40978 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3367 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.969647 squander-1.8.5/qgd_python/decomposition/test/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11142 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_Compression.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_Global_Phase.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7037 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_IBM.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1777 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_Project_Name.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5616 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_QX2.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4399 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_State_Preparation.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1656 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_Unitary.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4672 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_decomposition.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7190 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_fmo.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7018 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_heavy_hex.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6583 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_optmization_problem_combined.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4905 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/decomposition/test/test_parametric_circuit.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.973646 squander-1.8.5/qgd_python/gates/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    13911 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8355 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_CH.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8292 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_CNOT.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8165 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_CZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    28668 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_Gates_Block.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8661 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_RX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8660 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_RY.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8659 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_RZ.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7903 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_SX.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7941 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_SYC.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9186 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_U3.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     7621 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_X.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8499 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_Y.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     8499 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/qgd_Z.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.973646 squander-1.8.5/qgd_python/gates/test/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        0 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3364 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_CH.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3409 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_CNOT.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3444 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_CZ.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3466 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_RX.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3348 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_RY.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3919 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_RZ.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3278 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_SX.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3676 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_U3.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3182 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_X.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3179 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_Y.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     3232 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_Z.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6878 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/gates/test/test_gates.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.977646 squander-1.8.5/qgd_python/nn/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1332 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/nn/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       27 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/nn/__init__.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     2387 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/nn/qgd_nn.py
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     9606 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/nn/qgd_nn_Wrapper.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1573 2023-05-27 16:24:34.000000 squander-1.8.5/qgd_python/utils.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.977646 squander-1.8.5/random_unitary/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6628 2023-05-27 16:24:34.000000 squander-1.8.5/random_unitary/Random_Orthogonal.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    11039 2023-05-27 16:24:34.000000 squander-1.8.5/random_unitary/Random_Unitary.cpp
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.977646 squander-1.8.5/random_unitary/include/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1927 2023-05-27 16:24:34.000000 squander-1.8.5/random_unitary/include/Random_Orthogonal.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4476 2023-05-27 16:24:34.000000 squander-1.8.5/random_unitary/include/Random_Unitary.h
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       38 2023-06-02 12:16:50.981646 squander-1.8.5/setup.cfg
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1898 2023-06-02 12:15:26.000000 squander-1.8.5/setup.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.977646 squander-1.8.5/squander/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1442 2023-05-27 16:24:34.000000 squander-1.8.5/squander/__init__.py
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.977646 squander-1.8.5/squander.egg-info/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)    16207 2023-06-02 12:16:50.000000 squander-1.8.5/squander.egg-info/PKG-INFO
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     5157 2023-06-02 12:16:50.000000 squander-1.8.5/squander.egg-info/SOURCES.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)        1 2023-06-02 12:16:50.000000 squander-1.8.5/squander.egg-info/dependency_links.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       50 2023-06-02 12:16:50.000000 squander-1.8.5/squander.egg-info/requires.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)       20 2023-06-02 12:16:50.000000 squander-1.8.5/squander.egg-info/top_level.txt
+drwxrwxr-x   0 rakytap   (1000) rakytap   (1000)        0 2023-06-02 12:16:50.977646 squander-1.8.5/test_standalone/
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     1996 2023-05-27 16:24:34.000000 squander-1.8.5/test_standalone/CMakeLists.txt
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     6325 2023-05-27 16:24:34.000000 squander-1.8.5/test_standalone/custom_gate_structure_test.cpp
+-rw-rw-r--   0 rakytap   (1000) rakytap   (1000)     4837 2023-05-27 16:24:34.000000 squander-1.8.5/test_standalone/decomposition_test.cpp
```

### Comparing `squander-1.8.4/CMakeLists.txt` & `squander-1.8.5/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cmake_minimum_required(VERSION 3.10.2)
 
 # CMAKE to create the shared library of the quantum gate decomposition project
 
 # set the project name and version
-project(CQGD VERSION 1.8.4)
+project(CQGD VERSION 1.8.5)
 
 # reuse compilation time linking for use runtime linking 
 SET(CMAKE_INSTALL_RPATH_USE_LINK_PATH TRUE)
 
 # specify the C++ standard
 set(CMAKE_CXX_STANDARD 11)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
```

### Comparing `squander-1.8.4/LICENSE` & `squander-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/PKG-INFO` & `squander-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.4
+Version: 1.8.5
 Summary: Package to decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.4 Summary: Package to
+Metadata-Version: 2.1 Name: squander Version: 1.8.5 Summary: Package to
 decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta Maintainer-email: peter.rakyta@ttk.elte.hu License:
 GNU General Public License v3.0 Keywords: test,cmake,extension Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: C Classifier: Programming Language :: C++
 Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
```

### Comparing `squander-1.8.4/README.md` & `squander-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/cmake/check_AVX.cmake` & `squander-1.8.5/cmake/check_AVX.cmake`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/Adam.cpp` & `squander-1.8.5/common/Adam.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/common.cpp` & `squander-1.8.5/common/common.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/common_DFE.cpp` & `squander-1.8.5/common/common_DFE.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/config_element.cpp` & `squander-1.8.5/common/config_element.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/dot.cpp` & `squander-1.8.5/common/dot.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/Adam.h` & `squander-1.8.5/common/include/Adam.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/QGDTypes.h` & `squander-1.8.5/common/include/QGDTypes.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/common.h` & `squander-1.8.5/common/include/common.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/common_DFE.h` & `squander-1.8.5/common/include/common_DFE.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/config_element.h` & `squander-1.8.5/common/include/config_element.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/dot.h` & `squander-1.8.5/common/include/dot.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/lbfgs.h` & `squander-1.8.5/common/include/lbfgs.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/logging.h` & `squander-1.8.5/common/include/logging.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/matrix.h` & `squander-1.8.5/common/include/matrix.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/matrix_base.h` & `squander-1.8.5/common/include/matrix_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/matrix_real.h` & `squander-1.8.5/common/include/matrix_real.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/mpi_base.h` & `squander-1.8.5/common/include/mpi_base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/numpy_interface.h` & `squander-1.8.5/common/include/numpy_interface.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/include/tolmin.h` & `squander-1.8.5/common/include/tolmin.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/lbfgs.cpp` & `squander-1.8.5/common/lbfgs.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/logging.cpp` & `squander-1.8.5/common/logging.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/matrix.cpp` & `squander-1.8.5/common/matrix.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/matrix_real.cpp` & `squander-1.8.5/common/matrix_real.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/mpi_base.cpp` & `squander-1.8.5/common/mpi_base.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/numpy_interface.cpp` & `squander-1.8.5/common/numpy_interface.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/common/tolmin.cpp` & `squander-1.8.5/common/tolmin.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/Decomposition_Base.cpp` & `squander-1.8.5/decomposition/Decomposition_Base.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/N_Qubit_Decomposition.cpp` & `squander-1.8.5/decomposition/N_Qubit_Decomposition.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/N_Qubit_Decomposition_Base.cpp` & `squander-1.8.5/decomposition/N_Qubit_Decomposition_Base.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1305,18 +1305,14 @@
 
                 
             
                
             // CPU time                                                     
             CPU_time += (tbb::tick_count::now() - t0_CPU).seconds();
             
-          
-            // determine the current minimum  at the shifted parameters  
-            //current_minimum_agents = optimization_problem_batched( solution_guess_mtx_agents ); 
-
   
             // CPU time                                        
             t0_CPU = tbb::tick_count::now();        
 
 
             // generate random numbers to manage the behavior of the agents
             Matrix_real random_numbers(   agent_num, 2 );
@@ -1362,14 +1358,23 @@
                 for( int agent_idx=0; agent_idx<agent_num; agent_idx++ ) {
                     agent_probs[agent_idx] = agent_probs[agent_idx]/prob_sum;
                 }
 
 
             }
 */
+
+            // ocassionaly recalculate teh current cost functions of the agents
+            if ( iter_idx % agent_lifetime_loc == 0 )
+            {
+                // recalculate the current cost functions
+                current_minimum_agents = optimization_problem_batched( solution_guess_mtx_agents ); 
+            }
+
+
             
             // govern the behavior of the agents
             for ( int agent_idx=0; agent_idx<agent_num; agent_idx++ ) {
                 double& current_minimum_agent = current_minimum_agents[ agent_idx ];
                    
            
                 
@@ -1380,14 +1385,16 @@
                
                 
                 Matrix_real& solution_guess_mtx_agent = solution_guess_mtx_agents[ agent_idx ];                             
 
                 // look for the best agent periodicaly
                 if ( iter_idx % agent_lifetime_loc == 0 )
                 {
+
+                    
                             
                     if ( current_minimum_agent <= current_minimum ) {
 
                         most_successfull_agent = agent_idx;
                     
                         // export the parameters of the curremt, most successful agent
                         memcpy(optimized_parameters_mtx.get_data(), solution_guess_mtx_agent.get_data(), num_of_parameters*sizeof(double) );
```

### Comparing `squander-1.8.4/decomposition/N_Qubit_Decomposition_Cost_Function.cpp` & `squander-1.8.5/decomposition/N_Qubit_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/N_Qubit_Decomposition_adaptive.cpp` & `squander-1.8.5/decomposition/N_Qubit_Decomposition_adaptive.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/N_Qubit_Decomposition_custom.cpp` & `squander-1.8.5/decomposition/N_Qubit_Decomposition_custom.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/Sub_Matrix_Decomposition.cpp` & `squander-1.8.5/decomposition/Sub_Matrix_Decomposition.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp` & `squander-1.8.5/decomposition/Sub_Matrix_Decomposition_Cost_Function.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/include/Decomposition_Base.h` & `squander-1.8.5/decomposition/include/Decomposition_Base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/include/N_Qubit_Decomposition.h` & `squander-1.8.5/decomposition/include/N_Qubit_Decomposition.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/include/N_Qubit_Decomposition_Base.h` & `squander-1.8.5/decomposition/include/N_Qubit_Decomposition_Base.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/include/N_Qubit_Decomposition_Cost_Function.h` & `squander-1.8.5/decomposition/include/N_Qubit_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/include/N_Qubit_Decomposition_adaptive.h` & `squander-1.8.5/decomposition/include/N_Qubit_Decomposition_adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/include/N_Qubit_Decomposition_custom.h` & `squander-1.8.5/decomposition/include/N_Qubit_Decomposition_custom.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/include/Sub_Matrix_Decomposition.h` & `squander-1.8.5/decomposition/include/Sub_Matrix_Decomposition.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h` & `squander-1.8.5/decomposition/include/Sub_Matrix_Decomposition_Cost_Function.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/Adaptive.cpp` & `squander-1.8.5/gates/Adaptive.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/CH.cpp` & `squander-1.8.5/gates/CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/CNOT.cpp` & `squander-1.8.5/gates/CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/CRY.cpp` & `squander-1.8.5/gates/CRY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/CZ.cpp` & `squander-1.8.5/gates/CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/Composite.cpp` & `squander-1.8.5/gates/Composite.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/Gate.cpp` & `squander-1.8.5/gates/Gate.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/Gates_block.cpp` & `squander-1.8.5/gates/Gates_block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/ON.cpp` & `squander-1.8.5/gates/ON.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/RX.cpp` & `squander-1.8.5/gates/RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/RY.cpp` & `squander-1.8.5/gates/RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/RZ.cpp` & `squander-1.8.5/gates/RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/SX.cpp` & `squander-1.8.5/gates/SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/SYC.cpp` & `squander-1.8.5/gates/SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/U3.cpp` & `squander-1.8.5/gates/U3.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/UN.cpp` & `squander-1.8.5/gates/UN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/X.cpp` & `squander-1.8.5/gates/X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/Y.cpp` & `squander-1.8.5/gates/Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/Z.cpp` & `squander-1.8.5/gates/Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/Adaptive.h` & `squander-1.8.5/gates/include/Adaptive.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/CH.h` & `squander-1.8.5/gates/include/CH.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/CNOT.h` & `squander-1.8.5/gates/include/CNOT.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/CRY.h` & `squander-1.8.5/gates/include/CRY.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/CZ.h` & `squander-1.8.5/gates/include/CZ.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/Composite.h` & `squander-1.8.5/gates/include/Composite.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/Gate.h` & `squander-1.8.5/gates/include/Gate.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/Gates_block.h` & `squander-1.8.5/gates/include/Gates_block.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/ON.h` & `squander-1.8.5/gates/include/ON.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/RX.h` & `squander-1.8.5/gates/include/RX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/RY.h` & `squander-1.8.5/gates/include/RY.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/RZ.h` & `squander-1.8.5/gates/include/RZ.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/SX.h` & `squander-1.8.5/gates/include/SX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/SYC.h` & `squander-1.8.5/gates/include/SYC.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/U3.h` & `squander-1.8.5/gates/include/U3.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/UN.h` & `squander-1.8.5/gates/include/UN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/X.h` & `squander-1.8.5/gates/include/X.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/Y.h` & `squander-1.8.5/gates/include/Y.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/include/Z.h` & `squander-1.8.5/gates/include/Z.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/kernels/apply_kernel_to_input_AVX.cpp` & `squander-1.8.5/gates/kernels/apply_kernel_to_input_AVX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/kernels/apply_kernel_to_state_vector_input.cpp` & `squander-1.8.5/gates/kernels/apply_kernel_to_state_vector_input.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/kernels/include/apply_kernel_to_input_AVX.h` & `squander-1.8.5/gates/kernels/include/apply_kernel_to_input_AVX.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/gates/kernels/include/apply_kernel_to_state_vector_input.h` & `squander-1.8.5/gates/kernels/include/apply_kernel_to_state_vector_input.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/nn/NN.cpp` & `squander-1.8.5/nn/NN.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/nn/include/NN.h` & `squander-1.8.5/nn/include/NN.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/optimization_engines/RL_experience.cpp` & `squander-1.8.5/optimization_engines/RL_experience.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 /*! \file RL_experience.cpp
     \brief A class for RL_experience 
 */
 
 #include "RL_experience.h"
 #include "tbb/tbb.h"
 
+
 #include <cfloat>	
 
 /** Nullary constructor of the class
 @return An instance of the class
 */
 RL_experience::RL_experience() {
```

### Comparing `squander-1.8.4/optimization_engines/include/RL_experience.h` & `squander-1.8.5/optimization_engines/include/RL_experience.h`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 #include "matrix_real.h"
 #include "matrix_base.h"
 #include "Gates_block.h"
 #include <map>
 #include <cstdlib>
 #include <time.h>
 #include <ctime>
+#include <random>
 
 
 /**
 @brief A class for RL_experience optimization according to https://towardsdatascience.com/how-to-implement-an-adam-optimizer-from-scratch-76e7b217f1cc
 */
 class RL_experience  {
```

### Comparing `squander-1.8.4/qgd_python/decomposition/CMakeLists.txt` & `squander-1.8.5/qgd_python/decomposition/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py` & `squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp` & `squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py` & `squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp` & `squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_adaptive_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py` & `squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp` & `squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_Decomposition_custom_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py` & `squander-1.8.5/qgd_python/decomposition/qgd_N_Qubit_State_Preparation_adaptive.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_Compression.py` & `squander-1.8.5/qgd_python/decomposition/test/test_Compression.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_Global_Phase.py` & `squander-1.8.5/qgd_python/decomposition/test/test_Global_Phase.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_IBM.py` & `squander-1.8.5/qgd_python/decomposition/test/test_IBM.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_Project_Name.py` & `squander-1.8.5/qgd_python/decomposition/test/test_Project_Name.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_QX2.py` & `squander-1.8.5/qgd_python/decomposition/test/test_QX2.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_State_Preparation.py` & `squander-1.8.5/qgd_python/decomposition/test/test_State_Preparation.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_Unitary.py` & `squander-1.8.5/qgd_python/decomposition/test/test_Unitary.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_decomposition.py` & `squander-1.8.5/qgd_python/decomposition/test/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_fmo.py` & `squander-1.8.5/qgd_python/decomposition/test/test_fmo.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_heavy_hex.py` & `squander-1.8.5/qgd_python/decomposition/test/test_heavy_hex.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_optmization_problem_combined.py` & `squander-1.8.5/qgd_python/decomposition/test/test_optmization_problem_combined.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/decomposition/test/test_parametric_circuit.py` & `squander-1.8.5/qgd_python/decomposition/test/test_parametric_circuit.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/CMakeLists.txt` & `squander-1.8.5/qgd_python/gates/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_CH.cpp` & `squander-1.8.5/qgd_python/gates/qgd_CH.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_CNOT.cpp` & `squander-1.8.5/qgd_python/gates/qgd_CNOT.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_CZ.cpp` & `squander-1.8.5/qgd_python/gates/qgd_CZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_Gates_Block.cpp` & `squander-1.8.5/qgd_python/gates/qgd_Gates_Block.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_RX.cpp` & `squander-1.8.5/qgd_python/gates/qgd_RX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_RY.cpp` & `squander-1.8.5/qgd_python/gates/qgd_RY.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_RZ.cpp` & `squander-1.8.5/qgd_python/gates/qgd_RZ.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_SX.cpp` & `squander-1.8.5/qgd_python/gates/qgd_SX.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_SYC.cpp` & `squander-1.8.5/qgd_python/gates/qgd_SYC.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_U3.cpp` & `squander-1.8.5/qgd_python/gates/qgd_U3.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_X.cpp` & `squander-1.8.5/qgd_python/gates/qgd_X.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_Y.cpp` & `squander-1.8.5/qgd_python/gates/qgd_Y.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/qgd_Z.cpp` & `squander-1.8.5/qgd_python/gates/qgd_Z.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_CH.py` & `squander-1.8.5/qgd_python/gates/test/test_CH.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_CNOT.py` & `squander-1.8.5/qgd_python/gates/test/test_CNOT.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_CZ.py` & `squander-1.8.5/qgd_python/gates/test/test_CZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_RX.py` & `squander-1.8.5/qgd_python/gates/test/test_RX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_RY.py` & `squander-1.8.5/qgd_python/gates/test/test_RY.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_RZ.py` & `squander-1.8.5/qgd_python/gates/test/test_RZ.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_SX.py` & `squander-1.8.5/qgd_python/gates/test/test_SX.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_U3.py` & `squander-1.8.5/qgd_python/gates/test/test_U3.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_X.py` & `squander-1.8.5/qgd_python/gates/test/test_X.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_Y.py` & `squander-1.8.5/qgd_python/gates/test/test_Y.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_Z.py` & `squander-1.8.5/qgd_python/gates/test/test_Z.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/gates/test/test_gates.py` & `squander-1.8.5/qgd_python/gates/test/test_gates.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/nn/CMakeLists.txt` & `squander-1.8.5/qgd_python/nn/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/nn/qgd_nn.py` & `squander-1.8.5/qgd_python/nn/qgd_nn.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/nn/qgd_nn_Wrapper.cpp` & `squander-1.8.5/qgd_python/nn/qgd_nn_Wrapper.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/qgd_python/utils.py` & `squander-1.8.5/qgd_python/utils.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/random_unitary/Random_Orthogonal.cpp` & `squander-1.8.5/random_unitary/Random_Orthogonal.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/random_unitary/Random_Unitary.cpp` & `squander-1.8.5/random_unitary/Random_Unitary.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/random_unitary/include/Random_Orthogonal.h` & `squander-1.8.5/random_unitary/include/Random_Orthogonal.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/random_unitary/include/Random_Unitary.h` & `squander-1.8.5/random_unitary/include/Random_Unitary.h`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/setup.py` & `squander-1.8.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 setup(
     name="squander",
     packages=find_packages(
         exclude=(
             "test_standalone", "test_standalone.*",
         )
     ),
-    version='1.8.4',
+    version='1.8.5',
     url="https://github.com/rakytap/sequential-quantum-gate-decomposer", 
     maintainer="Peter Rakyta",
     maintainer_email="peter.rakyta@ttk.elte.hu",
     include_package_data=True,
     install_requires=[
         "setuptools>=40.8.0",
         "wheel",
```

### Comparing `squander-1.8.4/squander/__init__.py` & `squander-1.8.5/squander/__init__.py`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/squander.egg-info/PKG-INFO` & `squander-1.8.5/squander.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squander
-Version: 1.8.4
+Version: 1.8.5
 Summary: Package to decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta
 Maintainer-email: peter.rakyta@ttk.elte.hu
 License: GNU General Public License v3.0
 Keywords: test,cmake,extension
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: squander Version: 1.8.4 Summary: Package to
+Metadata-Version: 2.1 Name: squander Version: 1.8.5 Summary: Package to
 decompose unitaries into a quantum circuit and for quantum state preparation.
 Home-page: https://github.com/rakytap/sequential-quantum-gate-decomposer
 Maintainer: Peter Rakyta Maintainer-email: peter.rakyta@ttk.elte.hu License:
 GNU General Public License v3.0 Keywords: test,cmake,extension Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: Programming Language :: C Classifier: Programming Language :: C++
 Description-Content-Type: text/markdown License-File: LICENSE [![DOI](https://
```

### Comparing `squander-1.8.4/squander.egg-info/SOURCES.txt` & `squander-1.8.5/squander.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/test_standalone/CMakeLists.txt` & `squander-1.8.5/test_standalone/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/test_standalone/custom_gate_structure_test.cpp` & `squander-1.8.5/test_standalone/custom_gate_structure_test.cpp`

 * *Files identical despite different names*

### Comparing `squander-1.8.4/test_standalone/decomposition_test.cpp` & `squander-1.8.5/test_standalone/decomposition_test.cpp`

 * *Files identical despite different names*

