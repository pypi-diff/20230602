# Comparing `tmp/struphy-1.9.9.tar.gz` & `tmp/struphy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struphy-1.9.9.tar", last modified: Tue May  2 10:33:35 2023, max compression
+gzip compressed data, was "struphy-2.0.0.tar", last modified: Fri Jun  2 10:34:40 2023, max compression
```

## Comparing `struphy-1.9.9.tar` & `struphy-2.0.0.tar`

### file list

```diff
@@ -1,356 +1,362 @@
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.643776 struphy-1.9.9/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1428 2023-05-02 08:34:02.000000 struphy-1.9.9/LICENSE
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6305 2023-05-02 10:33:35.643776 struphy-1.9.9/PKG-INFO
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     3854 2022-10-10 09:53:17.000000 struphy-1.9.9/README.md
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2095 2023-05-02 08:34:02.000000 struphy-1.9.9/pyproject.toml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)      124 2023-05-02 10:33:35.643776 struphy-1.9.9/setup.cfg
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.599776 struphy-1.9.9/src/
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.604776 struphy-1.9.9/src/struphy/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.606776 struphy-1.9.9/src/struphy/b_splines/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1621 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/b_splines/Bspline.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/b_splines/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4670 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/b_splines/bspline_evaluation_1d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    14007 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/b_splines/bspline_evaluation_2d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    27508 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/b_splines/bspline_evaluation_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    20754 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/b_splines/bsplines.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    20660 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/b_splines/bsplines_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6303 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/b_splines/bsplines_kernels_particles.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6384 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/compile_struphy.mk
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.607776 struphy-1.9.9/src/struphy/console/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/console/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2096 2023-04-28 20:42:52.000000 struphy-1.9.9/src/struphy/console/compile.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)      740 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/console/example.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    15509 2023-05-02 08:34:02.000000 struphy-1.9.9/src/struphy/console/main.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1155 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/console/pproc.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5419 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/console/profile.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7004 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/console/run.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3973 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/console/test.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)      929 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/console/units.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.608776 struphy-1.9.9/src/struphy/diagnostics/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/diagnostics/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    13821 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/diagnostics/continuous_spectra.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    20203 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/diagnostics/diagn_tools.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.608776 struphy-1.9.9/src/struphy/diagnostics/paraview/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/diagnostics/paraview/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    13277 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/diagnostics/paraview/mesh_creator.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3004 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/diagnostics/paraview/vtk_writer.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.608776 struphy-1.9.9/src/struphy/dispersion_relations/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/dispersion_relations/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    28395 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/dispersion_relations/analytic.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3838 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/dispersion_relations/base.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.610776 struphy-1.9.9/src/struphy/eigenvalue_solvers/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5540 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/derivatives.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5212 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/kernels_2d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7722 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/kernels_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    23321 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/kernels_projectors_global.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    34110 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/kernels_projectors_global_mhd.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.611776 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    32233 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/MHD_eigenvalues_cylinder_1D.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.612776 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    15856 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/control_variate.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8521 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kernels_control_variate.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.613776 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7080 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_control_variate.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    20929 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_kernels_control_variate.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    11250 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_control_variate.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1618 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_cv_kernel_2.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    21155 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_kernels_control_variate.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     9994 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_control_variate.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8890 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_cvker.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    32983 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_kernels_control_variate.py
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     9189 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/emw_operators.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3606 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/inner_products_1d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    11738 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/inner_products_2d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    12358 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/inner_products_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3432 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/l2_error_1d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    17672 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/l2_error_2d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    17438 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/l2_error_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    16554 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/mass_matrices_3d_pre.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.613776 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    18026 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_arrays.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    14698 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bb_kernel.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    25326 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bv_kernel.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    46819 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_massless_linear_operators.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    27140 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_vv_kernel.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   139137 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   146225 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF_for_tests.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.614776 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.614776 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    10395 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    22026 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local_mhd.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   144069 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/mhd_operators_3d_local.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    72812 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/projectors_local.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.615776 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    94136 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_L2_projector_kernel.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    26256 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_L2.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    33024 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_local.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   129589 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_local_projector_kernel.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8106 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/mass_matrices_1d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    19797 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/mass_matrices_2d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    21575 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/mass_matrices_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     9492 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/mhd_axisymmetric_main.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2212 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/mhd_axisymmetric_pproc.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    45855 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/mhd_operators.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    70280 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/mhd_operators_core.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    86755 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/projectors_global.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    93476 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/eigenvalue_solvers/spline_space.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.616776 struphy-1.9.9/src/struphy/examples/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7572 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/TAE_tokamak.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2354 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/_draw_parallel.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5860 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/_mhd_eigenvalues_cylinder.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6072 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/_mhd_eigenvalues_slab.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8292 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/_sendrecv.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6798 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/gc_orbits_tokamak.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4795 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/linearmhd.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4035 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/linearmhdvlasov_cc.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4035 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/linearmhdvlasov_pc.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3315 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/maxwell.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6766 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/examples/orbits_tokamak.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.616776 struphy-1.9.9/src/struphy/fields_background/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/fields_background/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.616776 struphy-1.9.9/src/struphy/fields_background/electric_equil/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/fields_background/electric_equil/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)      654 2023-04-28 17:43:50.000000 struphy-1.9.9/src/struphy/fields_background/electric_equil/analytical.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1681 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/electric_equil/base.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.617776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    21082 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/base.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.617776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/eqdsk/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/eqdsk/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.622776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/eqdsk/data/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)  8579339 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/eqdsk/data/AUGNLED_g031213.00830.high
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/eqdsk/data/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     9280 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/eqdsk/readeqdsk.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    73612 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/equils.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.623776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.601776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.623776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    65028 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7253 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.623776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    89724 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7276 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.623776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   161316 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7249 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.623776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/output/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/output/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.624776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/output/vtk/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/output/vtk/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.624776 struphy-1.9.9/src/struphy/fields_background/mhd_equil/vmec/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/fields_background/mhd_equil/vmec/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.625776 struphy-1.9.9/src/struphy/geometry/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    68560 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/base.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    26666 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/domains.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3359 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/kernels.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.625776 struphy-1.9.9/src/struphy/geometry/map_coef/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/map_coef/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    20659 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/map_eval.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    33123 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/mappings_fast.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    16513 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/transform.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8862 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/geometry/utilities.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.625776 struphy-1.9.9/src/struphy/initial/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/initial/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3897 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/initial/analytic.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7822 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/initial/base.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7895 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/initial/eigenfunctions.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4104 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/initial/initialize.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4294 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/initial/perturbations.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.625776 struphy-1.9.9/src/struphy/io/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.626776 struphy-1.9.9/src/struphy/io/batch/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/batch/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1073 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/batch/batch_cobra.sh
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1302 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/batch/p_016.sh
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1531 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/batch/p_032.sh
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1531 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/batch/p_064.sh
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1534 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/batch/p_128.sh
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1534 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/batch/p_256.sh
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1535 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/batch/p_512.sh
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.626776 struphy-1.9.9/src/struphy/io/inp/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.627776 struphy-1.9.9/src/struphy/io/inp/examples/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4478 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_TAE_tokamak.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4990 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5470 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5256 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2981 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_linearmhd.yml
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     8160 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_linvlasovmaxwell.yml
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     5150 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     5589 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_linvlasovmaxwell_weibel.yml
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     2049 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_maxwell.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4849 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/examples/params_orbits_tokamak.yml
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)    20609 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/parameters.yml
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.629776 struphy-1.9.9/src/struphy/io/inp/tests/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5665 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_cc_linmhd_5d.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7764 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_hybrid_fA.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5423 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5639 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5703 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5206 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3065 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_linearmhd.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3342 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_linearmhd_gvec.yml
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     5585 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_linvlasovmaxwell.yml
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     2239 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_maxwell_1.yml
--rwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)     2315 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/params_maxwell_2.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1956 2023-04-28 17:43:51.000000 struphy-1.9.9/src/struphy/io/inp/tests/strscl.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1902 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/inp/tests/wkscl_1.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1902 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/inp/tests/wkscl_2.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1902 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/inp/tests/wkscl_3.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1902 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/inp/tests/wkscl_4.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1903 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/inp/tests/wkscl_5.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1905 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/inp/tests/wkscl_6.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1905 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/inp/tests/wkscl_7.yml
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1905 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/inp/tests/wkscl_8.yml
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.630776 struphy-1.9.9/src/struphy/io/out/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/io/out/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.630776 struphy-1.9.9/src/struphy/kinetic_background/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/kinetic_background/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    22918 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/kinetic_background/analytical.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1238 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/kinetic_background/background_eval.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1656 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/kinetic_background/f0_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     9831 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/kinetic_background/moments_kernels.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.631776 struphy-1.9.9/src/struphy/linear_algebra/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/linear_algebra/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5790 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/linear_algebra/core.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    21910 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/linear_algebra/iterative_solvers.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    12463 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/linear_algebra/linalg_kron.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5299 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/linear_algebra/schur_solver.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8558 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/linear_algebra/stencil_dot_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    14375 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/linear_algebra/stencil_transpose_kernels.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.631776 struphy-1.9.9/src/struphy/models/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/models/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    37220 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/models/base.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8605 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/models/main.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    79448 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/models/models.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4976 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/models/output_handling.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    13064 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/models/utilities.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.633776 struphy-1.9.9/src/struphy/pic/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   125402 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/accum_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    20171 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/filler_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   247165 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/mat_vec_filler.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    33757 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/particles.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    18057 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/particles_to_grid.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    10146 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/pusher.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   178736 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/pusher_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    21154 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/pusher_utilities.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8535 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/sampling.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    14923 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/sobol_seq.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5608 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/utilities.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    74143 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/pic/utilities_kernels.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.634776 struphy-1.9.9/src/struphy/polar/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/polar/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    16532 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/polar/basic.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    52335 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/polar/extraction_operators.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    32352 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/polar/linear_operators.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.634776 struphy-1.9.9/src/struphy/post_processing/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/post_processing/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6362 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/post_processing/cprofile_analyser.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    17794 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/post_processing/post_processing_tools.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5708 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/post_processing/pproc_struphy.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5301 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/post_processing/profile_struphy.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.635776 struphy-1.9.9/src/struphy/propagators/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/propagators/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3393 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/propagators/base.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    53409 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/propagators/propagators_coupling.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    46663 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/propagators/propagators_fields.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    40903 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/propagators/propagators_markers.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3826 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/propagators/solvers.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)  1335528 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac-0.1-py3-none-any.whl
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.636776 struphy-1.9.9/src/struphy/psydac_api/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1839 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/banded_to_stencil_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    19977 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/basis_projection_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    43032 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/basis_projection_ops.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    22625 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/fields.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    22918 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/linear_operators.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    43888 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/mass.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    15604 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/mass_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    15886 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/preconditioner.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    19799 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/projectors.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    35047 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/psydac_derham.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5396 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/quadrature_evaluation_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    14732 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/utilities.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     5381 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/psydac_api/utilities_kernels.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.636776 struphy-1.9.9/src/struphy/tests/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/__init__.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.638776 struphy-1.9.9/src/struphy/tests/tests_mpi/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    29086 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_accumulation.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    24190 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_basis_operators.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2942 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_draw_parallel.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    16166 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_eval_spline_mpi.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6548 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_iterative_solvers.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    37762 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_mass_matrices.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    16313 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_mat_vec_filler.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.639776 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    19425 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    51404 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    22396 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    14116 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    11123 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    64611 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    17908 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_2d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    38069 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    14178 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_2d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    33254 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    13453 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_polar.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    14324 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_psydac_basics.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8477 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_psydac_derham.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    31560 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_pushers.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    11285 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    11191 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6583 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_mpi/xx_test_send_ghost_regions.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.643776 struphy-1.9.9/src/struphy/tests/tests_serial/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     7092 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_bsplines_kernels.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    38312 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_domain.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6770 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_gvec_equil.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    45727 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     4901 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_legacy_polar_splines.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6283 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_numerical_MHD_equil.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    28774 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_projectors_global.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2556 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_prop_solvers.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    20678 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_psydac_basis_operators.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6177 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_psydac_linear_operators.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2345 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_psydac_mapping.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2924 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/test_spline_space_1d.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    23198 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_psydac_lin_ops.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    23652 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_GVEC.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1566 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_codes.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     1702 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_cprofiler.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    19344 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_divB.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    10695 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_filler_kernel.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    12684 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_mappings.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    16292 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_mat_vec_filler.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     2435 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_mhd_equil.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    15899 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_paraview.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)   277942 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_polar_splines_3D.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     3530 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_preconditioner.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    32930 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_psydac_lin_ops_loop.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    15913 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_spline_evaluation.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     8515 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_spline_interpolation.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    10294 2023-04-28 17:43:52.000000 struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_template_gvec.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1000)        0 2023-05-02 10:33:35.605776 struphy-1.9.9/src/struphy.egg-info/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)     6305 2023-05-02 10:33:35.000000 struphy-1.9.9/src/struphy.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)    15232 2023-05-02 10:33:35.000000 struphy-1.9.9/src/struphy.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        1 2023-05-02 10:33:35.000000 struphy-1.9.9/src/struphy.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)       57 2023-05-02 10:33:35.000000 struphy-1.9.9/src/struphy.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)      195 2023-05-02 10:33:35.000000 struphy-1.9.9/src/struphy.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1000)        8 2023-05-02 10:33:35.000000 struphy-1.9.9/src/struphy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.615116 struphy-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-05-24 14:21:27.000000 struphy-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7601 2023-06-02 10:34:40.615116 struphy-2.0.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5143 2023-05-25 12:17:28.000000 struphy-2.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2128 2023-06-02 07:48:31.000000 struphy-2.0.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-06-02 10:34:40.615116 struphy-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.431117 struphy-2.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.439117 struphy-2.0.0/src/struphy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.451117 struphy-2.0.0/src/struphy/b_splines/
+-rw-rw-rw-   0 root         (0) root         (0)     1621 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/Bspline.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4670 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    14007 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    27508 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    20754 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bsplines.py
+-rw-rw-rw-   0 root         (0) root         (0)    20660 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bsplines_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)     6303 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/b_splines/bsplines_kernels_particles.py
+-rw-rw-rw-   0 root         (0) root         (0)     6384 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/compile_struphy.mk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.455117 struphy-2.0.0/src/struphy/console/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/console/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/console/compile.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/console/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    18252 2023-05-30 13:00:48.000000 struphy-2.0.0/src/struphy/console/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/console/pproc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5507 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/console/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     6986 2023-06-01 11:22:35.000000 struphy-2.0.0/src/struphy/console/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/console/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/console/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.455117 struphy-2.0.0/src/struphy/diagnostics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/diagnostics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13919 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/diagnostics/continuous_spectra.py
+-rw-rw-rw-   0 root         (0) root         (0)    19187 2023-05-30 06:30:19.000000 struphy-2.0.0/src/struphy/diagnostics/diagn_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.455117 struphy-2.0.0/src/struphy/diagnostics/paraview/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/diagnostics/paraview/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13277 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/diagnostics/paraview/mesh_creator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/diagnostics/paraview/vtk_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.455117 struphy-2.0.0/src/struphy/dispersion_relations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/dispersion_relations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32608 2023-05-26 07:35:05.000000 struphy-2.0.0/src/struphy/dispersion_relations/analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)     3838 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/dispersion_relations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.459117 struphy-2.0.0/src/struphy/eigenvalue_solvers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5540 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/derivatives.py
+-rw-rw-rw-   0 root         (0) root         (0)     5212 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)     7722 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    23321 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_projectors_global.py
+-rw-rw-rw-   0 root         (0) root         (0)    34110 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_projectors_global_mhd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.459117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/
+-rw-rw-rw-   0 root         (0) root         (0)    32233 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/MHD_eigenvalues_cylinder_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.463117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15856 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8521 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kernels_control_variate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.463117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7080 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)    20929 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_kernels_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)    11250 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_cv_kernel_2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21155 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_kernels_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)     9994 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_control_variate.py
+-rw-rw-rw-   0 root         (0) root         (0)     8890 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_cvker.py
+-rw-rw-rw-   0 root         (0) root         (0)    32983 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_kernels_control_variate.py
+-rwxrwxrwx   0 root         (0) root         (0)     9189 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/emw_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3606 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    11738 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)     3432 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    17672 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    17438 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    16554 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mass_matrices_3d_pre.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.463117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18026 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_arrays.py
+-rw-rw-rw-   0 root         (0) root         (0)    14698 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bb_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)    25326 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bv_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)    46819 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_massless_linear_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    27140 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_vv_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)   139137 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF.py
+-rw-rw-rw-   0 root         (0) root         (0)   146225 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF_for_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.463117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.467117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10395 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local.py
+-rw-rw-rw-   0 root         (0) root         (0)    22026 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local_mhd.py
+-rw-rw-rw-   0 root         (0) root         (0)   144069 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/mhd_operators_3d_local.py
+-rw-rw-rw-   0 root         (0) root         (0)    72812 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/projectors_local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.467117 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    94136 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_L2_projector_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)    26256 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_L2.py
+-rw-rw-rw-   0 root         (0) root         (0)    33024 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_local.py
+-rw-rw-rw-   0 root         (0) root         (0)   129589 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_local_projector_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)     8106 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    19797 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    21575 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)     9590 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_axisymmetric_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_axisymmetric_pproc.py
+-rw-rw-rw-   0 root         (0) root         (0)    45855 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    70280 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_operators_core.py
+-rw-rw-rw-   0 root         (0) root         (0)    86755 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/projectors_global.py
+-rw-rw-rw-   0 root         (0) root         (0)    93476 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/eigenvalue_solvers/spline_space.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     7775 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/TAE_tokamak.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/_draw_parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)     5860 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/_mhd_eigenvalues_cylinder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6072 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/_mhd_eigenvalues_slab.py
+-rw-rw-rw-   0 root         (0) root         (0)     8292 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/examples/_sendrecv.py
+-rw-rw-rw-   0 root         (0) root         (0)     6905 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/gc_orbits_tokamak.py
+-rw-rw-rw-   0 root         (0) root         (0)     6715 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/examples/linearextendedmhd.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/linearmhd.py
+-rw-rw-rw-   0 root         (0) root         (0)     3953 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/linearmhdvlasov_cc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3953 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/linearmhdvlasov_pc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/maxwell.py
+-rw-rw-rw-   0 root         (0) root         (0)     6873 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/examples/orbits_tokamak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/fields_background/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/fields_background/electric_equil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/electric_equil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/electric_equil/analytical.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/electric_equil/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20147 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.471117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.519117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/data/
+-rw-rw-rw-   0 root         (0) root         (0)  8579339 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/data/AUGNLED_g031213.00830.high
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9280 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/readeqdsk.py
+-rw-rw-rw-   0 root         (0) root         (0)    56499 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/equils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.523117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.435117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.523117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    65028 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7253 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.527117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)    89724 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.531117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/
+-rw-rw-rw-   0 root         (0) root         (0)   161316 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.535117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/output/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/output/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.535117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/output/vtk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/output/vtk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.535117 struphy-2.0.0/src/struphy/fields_background/mhd_equil/vmec/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/fields_background/mhd_equil/vmec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.539117 struphy-2.0.0/src/struphy/geometry/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    68581 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    25913 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/geometry/domains.py
+-rw-rw-rw-   0 root         (0) root         (0)     3359 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.539117 struphy-2.0.0/src/struphy/geometry/map_coef/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/map_coef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26068 2023-05-25 08:07:41.000000 struphy-2.0.0/src/struphy/geometry/map_eval.py
+-rw-rw-rw-   0 root         (0) root         (0)    33123 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/mappings_fast.py
+-rw-rw-rw-   0 root         (0) root         (0)    16513 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8862 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/geometry/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.539117 struphy-2.0.0/src/struphy/initial/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3897 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)     7822 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8005 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/initial/eigenfunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4104 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/initialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     4294 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/initial/perturbations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.539117 struphy-2.0.0/src/struphy/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.547117 struphy-2.0.0/src/struphy/io/batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/batch_cobra.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_016.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_032.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_064.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_128.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_256.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/batch/p_512.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.547117 struphy-2.0.0/src/struphy/io/inp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.559117 struphy-2.0.0/src/struphy/io/inp/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_TAE_tokamak.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4989 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5470 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2023-05-26 07:35:05.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_linearextendedmhd.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_linearmhd.yml
+-rwxrwxrwx   0 root         (0) root         (0)     4791 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml
+-rwxrwxrwx   0 root         (0) root         (0)     6403 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_linvlasovmaxwell_weibel.yml
+-rwxrwxrwx   0 root         (0) root         (0)     2049 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_maxwell.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4849 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/io/inp/examples/params_orbits_tokamak.yml
+-rwxrwxrwx   0 root         (0) root         (0)    22014 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/io/inp/parameters.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.583116 struphy-2.0.0/src/struphy/io/inp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6000 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_cc_linmhd_5d.yml
+-rwxrwxrwx   0 root         (0) root         (0)     5493 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_deltafvlasovmaxwell.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7714 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybrid_fA.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5423 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5596 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5356 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5206 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_linearmhd.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_linearmhd_gvec.yml
+-rwxrwxrwx   0 root         (0) root         (0)     5592 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_linvlasovmaxwell.yml
+-rwxrwxrwx   0 root         (0) root         (0)     2240 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_maxwell_1.yml
+-rwxrwxrwx   0 root         (0) root         (0)     2316 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/params_maxwell_2.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/strscl.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_1.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_2.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_3.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_4.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1903 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_5.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_6.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_7.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/inp/tests/wkscl_8.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.583116 struphy-2.0.0/src/struphy/io/out/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/io/out/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.583116 struphy-2.0.0/src/struphy/kinetic_background/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22958 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/analytical.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/background_eval.py
+-rw-rw-rw-   0 root         (0) root         (0)     1722 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/f0_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    10095 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/kinetic_background/moments_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.587116 struphy-2.0.0/src/struphy/linear_algebra/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5790 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/linear_algebra/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    21910 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/iterative_solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)    12463 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/linalg_kron.py
+-rw-rw-rw-   0 root         (0) root         (0)     5299 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/schur_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)     8558 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/stencil_dot_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    14375 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/linear_algebra/stencil_transpose_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.591117 struphy-2.0.0/src/struphy/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    35985 2023-05-25 07:43:56.000000 struphy-2.0.0/src/struphy/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    17825 2023-05-26 07:35:05.000000 struphy-2.0.0/src/struphy/models/fluid.py
+-rw-rw-rw-   0 root         (0) root         (0)    41877 2023-05-25 12:17:28.000000 struphy-2.0.0/src/struphy/models/hybrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    27537 2023-05-25 12:17:28.000000 struphy-2.0.0/src/struphy/models/kinetic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9164 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/models/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2023-05-25 07:43:56.000000 struphy-2.0.0/src/struphy/models/output_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)    11468 2023-05-25 12:17:28.000000 struphy-2.0.0/src/struphy/models/toy.py
+-rw-rw-rw-   0 root         (0) root         (0)    13506 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/models/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.595116 struphy-2.0.0/src/struphy/pic/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   132313 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/pic/accum_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    20171 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/filler_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)   247659 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/mat_vec_filler.py
+-rw-rw-rw-   0 root         (0) root         (0)    33953 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/pic/particles.py
+-rw-rw-rw-   0 root         (0) root         (0)    18057 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/particles_to_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    10146 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/pic/pusher.py
+-rw-rw-rw-   0 root         (0) root         (0)   184071 2023-05-31 15:13:34.000000 struphy-2.0.0/src/struphy/pic/pusher_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    21310 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/pusher_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8535 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/sampling.py
+-rw-rw-rw-   0 root         (0) root         (0)    14923 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/sobol_seq.py
+-rw-rw-rw-   0 root         (0) root         (0)     5608 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/pic/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    74158 2023-05-31 15:13:35.000000 struphy-2.0.0/src/struphy/pic/utilities_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.599116 struphy-2.0.0/src/struphy/polar/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/polar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16532 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/polar/basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    52606 2023-05-26 09:43:56.000000 struphy-2.0.0/src/struphy/polar/extraction_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    32352 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/polar/linear_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.599116 struphy-2.0.0/src/struphy/post_processing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/post_processing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6362 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/post_processing/cprofile_analyser.py
+-rw-rw-rw-   0 root         (0) root         (0)    18854 2023-05-25 12:17:28.000000 struphy-2.0.0/src/struphy/post_processing/post_processing_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2023-05-25 07:43:56.000000 struphy-2.0.0/src/struphy/post_processing/pproc_struphy.py
+-rw-rw-rw-   0 root         (0) root         (0)     5300 2023-05-25 07:43:56.000000 struphy-2.0.0/src/struphy/post_processing/profile_struphy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.599116 struphy-2.0.0/src/struphy/propagators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/propagators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3393 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/propagators/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    60910 2023-05-31 15:13:35.000000 struphy-2.0.0/src/struphy/propagators/propagators_coupling.py
+-rw-rw-rw-   0 root         (0) root         (0)    64079 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/propagators/propagators_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    43013 2023-05-31 15:13:35.000000 struphy-2.0.0/src/struphy/propagators/propagators_markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/propagators/solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)  1335528 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac-0.1-py3-none-any.whl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.603116 struphy-2.0.0/src/struphy/psydac_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/banded_to_stencil_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    19977 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/basis_projection_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    43532 2023-05-31 15:13:35.000000 struphy-2.0.0/src/struphy/psydac_api/basis_projection_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)    22585 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    22918 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/linear_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    46576 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/mass.py
+-rw-rw-rw-   0 root         (0) root         (0)    15604 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/mass_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    15886 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/preconditioner.py
+-rw-rw-rw-   0 root         (0) root         (0)    19799 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/projectors.py
+-rw-rw-rw-   0 root         (0) root         (0)    35047 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/psydac_derham.py
+-rw-rw-rw-   0 root         (0) root         (0)     5396 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/quadrature_evaluation_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    14732 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)     5381 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/psydac_api/utilities_kernels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.603116 struphy-2.0.0/src/struphy/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.607116 struphy-2.0.0/src/struphy/tests/tests_mpi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29086 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_accumulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    24190 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_basis_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2942 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_draw_parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)    16166 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_eval_spline_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6548 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_iterative_solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)    37762 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_mass_matrices.py
+-rw-rw-rw-   0 root         (0) root         (0)    16313 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_mat_vec_filler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.611116 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19425 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py
+-rw-rw-rw-   0 root         (0) root         (0)    51404 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    22396 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    14116 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py
+-rw-rw-rw-   0 root         (0) root         (0)    11123 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py
+-rw-rw-rw-   0 root         (0) root         (0)    64611 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py
+-rw-rw-rw-   0 root         (0) root         (0)    17908 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    38069 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    14178 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    33254 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py
+-rw-rw-rw-   0 root         (0) root         (0)    13453 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_polar.py
+-rw-rw-rw-   0 root         (0) root         (0)    14324 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_psydac_basics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8477 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_psydac_derham.py
+-rw-rw-rw-   0 root         (0) root         (0)    31560 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_pushers.py
+-rw-rw-rw-   0 root         (0) root         (0)    11285 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    11191 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)     6583 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_mpi/xx_test_send_ghost_regions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.615116 struphy-2.0.0/src/struphy/tests/tests_serial/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7092 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_bsplines_kernels.py
+-rw-rw-rw-   0 root         (0) root         (0)    38312 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_gvec_equil.py
+-rw-rw-rw-   0 root         (0) root         (0)    45727 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_legacy_polar_splines.py
+-rw-rw-rw-   0 root         (0) root         (0)    33620 2023-05-26 09:13:16.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_mhd_equils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6283 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_numerical_MHD_equil.py
+-rw-rw-rw-   0 root         (0) root         (0)    28774 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_projectors_global.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_prop_solvers.py
+-rw-rw-rw-   0 root         (0) root         (0)    20678 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_basis_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6177 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_linear_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)     2924 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/test_spline_space_1d.py
+-rw-rw-rw-   0 root         (0) root         (0)    23198 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_psydac_lin_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)    23652 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_GVEC.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_cprofiler.py
+-rw-rw-rw-   0 root         (0) root         (0)    19344 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_divB.py
+-rw-rw-rw-   0 root         (0) root         (0)    10695 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_filler_kernel.py
+-rw-rw-rw-   0 root         (0) root         (0)    12684 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mappings.py
+-rw-rw-rw-   0 root         (0) root         (0)    16292 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mat_vec_filler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mhd_equil.py
+-rw-rw-rw-   0 root         (0) root         (0)    15899 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_paraview.py
+-rw-rw-rw-   0 root         (0) root         (0)   277942 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_polar_splines_3D.py
+-rw-rw-rw-   0 root         (0) root         (0)     3530 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_preconditioner.py
+-rw-rw-rw-   0 root         (0) root         (0)    32930 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_psydac_lin_ops_loop.py
+-rw-rw-rw-   0 root         (0) root         (0)    15913 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_spline_evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8515 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_spline_interpolation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10294 2023-05-24 14:21:27.000000 struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_template_gvec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:34:40.447117 struphy-2.0.0/src/struphy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7601 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15465 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      195 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 10:34:40.000000 struphy-2.0.0/src/struphy.egg-info/top_level.txt
```

### Comparing `struphy-1.9.9/LICENSE` & `struphy-2.0.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT 
 NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. 
 IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
 SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-In addition, we ask you to cite the following reference inscientific publications which contain
+In addition, we ask you to cite the following reference in scientific publications which contain
 results obtained with this software and developments:
 
 F. Holderied, S. Possanner, X. Wang, 
 "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell",
 J. Comp. Phys. 433 (2021) 110143
```

### Comparing `struphy-1.9.9/PKG-INFO` & `struphy-2.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struphy
-Version: 1.9.9
+Version: 2.0.0
 Summary: Multi-model plasma physics package
 Author: Max Planck Institute for Plasma Physics
 Author-email: stefan.possanner@ipp.mpg.de, florian.holderied@ipp.mpg.de
 License: Copyright 2019 (c) Struphy dev team | Max Planck Institute for Plasma Physics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and 
         associated documentation files (the "Software"), to deal in the Software without restriction, 
@@ -17,69 +17,89 @@
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT 
         NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. 
         IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
         WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
         SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
-        In addition, we ask you to cite the following reference inscientific publications which contain
+        In addition, we ask you to cite the following reference in scientific publications which contain
         results obtained with this software and developments:
         
         F. Holderied, S. Possanner, X. Wang, 
         "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell",
         J. Comp. Phys. 433 (2021) 110143
         
 Project-URL: homepage, https://struphy.pages.mpcdf.de/struphy/
 Project-URL: documentation, https://struphy.pages.mpcdf.de/struphy/
 Project-URL: repository, https://gitlab.mpcdf.mpg.de/struphy/struphy
 Project-URL: changelog, https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/CHANGELOG.md
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/struphy/struphy/-/issues
 Keywords: plasma physics, fusion, numerical modeling, partial differential equations, energetic particles
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # STRUPHY - STRUcture-Preserving HYbrid codes
 
 A Python package for energetic particles in plasma.
 
 The package is developed since 2019 at [Max Planck Institute for Plasma Physics](https://www.ipp.mpg.de/) 
 in the division [NMPP (Numerical Methods for Plasma Physics)](https://www.ipp.mpg.de/ippcms/de/for/bereiche/numerik).
 
 ## What you can do with struphy
 
-* Solve a variety of [plasma physics PDEs](https://struphy.pages.mpcdf.de/struphy/sections/models.html) with fluid and/or kinetic components on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
-* [Post process](https://struphy.pages.mpcdf.de/struphy/sections/userguide.html#post-processing) data and generate `.vtk` files for 3d views
-* Add your own [model equations](https://struphy.pages.mpcdf.de/struphy/sections/developers.html#model-equations) or [physics feature](https://struphy.pages.mpcdf.de/struphy/sections/developers.html#how-to-add) 
+* Investigate plasma physics problems with multiple [models equations](https://struphy.pages.mpcdf.de/struphy/sections/models.html) containing fluid and/or kinetic components 
+* Simulate each model on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
+* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
+* Use [diagnostic tools](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html) to visualize results
+* Compare simulations to analytic [dispersion relations](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html#module-struphy.dispersion_relations.analytic)
+* Solve the [MHD eigenvalue problem](https://struphy.pages.mpcdf.de/struphy/index.html) in axisymmetric toroidal geometries
+* [Improve Struphy](https://struphy.pages.mpcdf.de/struphy/sections/developers.html) by adding
+    * model equations
+    * domains (geometry)
+    * MHD equilibria
+    * kinetic backgrounds
+    * diagnostic tools
+    * dispersion relations
+    * other physics features (e.g. collision operators etc.)
 
 ## Algorithmic features
 
 * Particle-in-cell method for kinetic species
 * Discrete differential forms based on high-order B-spline finite elements ([Psydac library](https://github.com/pyccel/psydac)) for fields/fluids
 * Exact conservation laws
 * Polar splines to treat a polar singularity 
 * Kernels are pre-compiled with [Pyccel](https://github.com/pyccel/pyccel) to achieve near-Fortran performance
 * MPI/OpenMP hybrid parallelization  
 
 ## Installation
 
-* See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+
+## Tutorials
+
+* [Turorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Learn about Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
+
+* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Learn about the data generated by Struphy simulations, data post processing and simple plotting 
+of field/fluid and kinetic variables.
+
+* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Learn about plotting field/fluid variables in toroidal geometry.
 
 ## Key references
 
 * F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", [J. Comp. Phys. 433 (2021) 110143](https://www.sciencedirect.com/science/article/pii/S0021999121000358?via%3Dihub)
 
 * F. Holderied, S. Possanner, "Magneto-hydrodynamic eigenvalue solver for axis-symmetric equilibria based on smooth polar splines", [J. Comp. Phys. 464 (2022) 111329](https://www.sciencedirect.com/science/article/pii/S0021999122003916?via%3Dihub)
 
 * F. Holderied, "STRUPHY: a structure-preserving hybrid MHD-kinetic code for the interaction of energetic particles with Alfvén waves in magnetized plasmas", [PhD thesis (2022)](https://mediatum.ub.tum.de/?id=1656539)
 
 ## License
 
-Copyright 2022 (c) struphy dev team | CONTRIBUTING.md | Max Planck Institute for Plasma Physics
+Copyright 2019 (c) Struphy dev team | Max Planck Institute for Plasma Physics
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `struphy-1.9.9/README.md` & `struphy-2.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,42 +3,62 @@
 A Python package for energetic particles in plasma.
 
 The package is developed since 2019 at [Max Planck Institute for Plasma Physics](https://www.ipp.mpg.de/) 
 in the division [NMPP (Numerical Methods for Plasma Physics)](https://www.ipp.mpg.de/ippcms/de/for/bereiche/numerik).
 
 ## What you can do with struphy
 
-* Solve a variety of [plasma physics PDEs](https://struphy.pages.mpcdf.de/struphy/sections/models.html) with fluid and/or kinetic components on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
-* [Post process](https://struphy.pages.mpcdf.de/struphy/sections/userguide.html#post-processing) data and generate `.vtk` files for 3d views
-* Add your own [model equations](https://struphy.pages.mpcdf.de/struphy/sections/developers.html#model-equations) or [physics feature](https://struphy.pages.mpcdf.de/struphy/sections/developers.html#how-to-add) 
+* Investigate plasma physics problems with multiple [models equations](https://struphy.pages.mpcdf.de/struphy/sections/models.html) containing fluid and/or kinetic components 
+* Simulate each model on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
+* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
+* Use [diagnostic tools](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html) to visualize results
+* Compare simulations to analytic [dispersion relations](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html#module-struphy.dispersion_relations.analytic)
+* Solve the [MHD eigenvalue problem](https://struphy.pages.mpcdf.de/struphy/index.html) in axisymmetric toroidal geometries
+* [Improve Struphy](https://struphy.pages.mpcdf.de/struphy/sections/developers.html) by adding
+    * model equations
+    * domains (geometry)
+    * MHD equilibria
+    * kinetic backgrounds
+    * diagnostic tools
+    * dispersion relations
+    * other physics features (e.g. collision operators etc.)
 
 ## Algorithmic features
 
 * Particle-in-cell method for kinetic species
 * Discrete differential forms based on high-order B-spline finite elements ([Psydac library](https://github.com/pyccel/psydac)) for fields/fluids
 * Exact conservation laws
 * Polar splines to treat a polar singularity 
 * Kernels are pre-compiled with [Pyccel](https://github.com/pyccel/pyccel) to achieve near-Fortran performance
 * MPI/OpenMP hybrid parallelization  
 
 ## Installation
 
-* See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+
+## Tutorials
+
+* [Turorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Learn about Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
+
+* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Learn about the data generated by Struphy simulations, data post processing and simple plotting 
+of field/fluid and kinetic variables.
+
+* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Learn about plotting field/fluid variables in toroidal geometry.
 
 ## Key references
 
 * F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", [J. Comp. Phys. 433 (2021) 110143](https://www.sciencedirect.com/science/article/pii/S0021999121000358?via%3Dihub)
 
 * F. Holderied, S. Possanner, "Magneto-hydrodynamic eigenvalue solver for axis-symmetric equilibria based on smooth polar splines", [J. Comp. Phys. 464 (2022) 111329](https://www.sciencedirect.com/science/article/pii/S0021999122003916?via%3Dihub)
 
 * F. Holderied, "STRUPHY: a structure-preserving hybrid MHD-kinetic code for the interaction of energetic particles with Alfvén waves in magnetized plasmas", [PhD thesis (2022)](https://mediatum.ub.tum.de/?id=1656539)
 
 ## License
 
-Copyright 2022 (c) struphy dev team | CONTRIBUTING.md | Max Planck Institute for Plasma Physics
+Copyright 2019 (c) Struphy dev team | Max Planck Institute for Plasma Physics
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `struphy-1.9.9/pyproject.toml` & `struphy-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "struphy"
-version = "1.9.9"
+version = "2.0.0"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.7, <3.11"
 license = {file = "LICENSE"}
 authors = [
   { name = "Max Planck Institute for Plasma Physics"},
   { email = "stefan.possanner@ipp.mpg.de"},
   { email = "florian.holderied@ipp.mpg.de"}
 ]
 description = "Multi-model plasma physics package"
@@ -69,8 +69,9 @@
 'struphy.io.inp' = ['parameters.yml',
                     'tests/*.yml',
                     'examples/*.yml',
                     ]
                     
 struphy = ['compile_struphy.mk',
            'psydac-0.1-py3-none-any.whl',
+           'io_path.txt',
            ]
```

### Comparing `struphy-1.9.9/src/struphy/b_splines/Bspline.py` & `struphy-2.0.0/src/struphy/b_splines/Bspline.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/b_splines/bspline_evaluation_1d.py` & `struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/b_splines/bspline_evaluation_2d.py` & `struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/b_splines/bspline_evaluation_3d.py` & `struphy-2.0.0/src/struphy/b_splines/bspline_evaluation_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/b_splines/bsplines.py` & `struphy-2.0.0/src/struphy/b_splines/bsplines.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/b_splines/bsplines_kernels.py` & `struphy-2.0.0/src/struphy/b_splines/bsplines_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/b_splines/bsplines_kernels_particles.py` & `struphy-2.0.0/src/struphy/b_splines/bsplines_kernels_particles.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/compile_struphy.mk` & `struphy-2.0.0/src/struphy/compile_struphy.mk`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/console/compile.py` & `struphy-2.0.0/src/struphy/console/compile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 def struphy_compile(no_openmp=False, delete=False, verbose=False):
     """
     Compile Struphy kernels.
-    
+
     Parameters
     ----------
     no_openmp : bool, optional
         Whether to compile kernels with (no_openmp=False) or without (no_openmp=True).
-        
+
     delete : bool, optional
         If True, deletes generated Fortran and .so files.
-        
+
     verbose : bool, optional
         Call pyccel in verbose mode.
     """
-    
+
     import subprocess
     import struphy
     import os
 
     libpath = struphy.__path__[0]
-        
+
     if delete:
-        
+
         # (change dir not to be in source path)
         print('\nDeleting .f90 and .so files ...')
-        subprocess.run(['make', 
-                        'clean', 
+        subprocess.run(['make',
+                        'clean',
                         '-f',
                         'compile_struphy.mk',
                         ], check=True, cwd=libpath)
         print('Done.')
-        
+
     else:
-        
+
         # struphy and psydac (change dir not to be in source path)
         flag_omp_pic = '--openmp'
         flag_omp_mhd = ''
         if no_openmp:
             flag_omp_pic = ''
-            
+
         flag_verb = ''
         if verbose:
             flag_verb = '--verbose'
-            
+
         try:
             import psydac.api
         except:
             print('\nInstalling Psydac ...')
-            subprocess.run(['pip', 
-                            'install', 
-                            os.path.join(libpath, 'psydac-0.1-py3-none-any.whl'),
+            subprocess.run(['pip',
+                            'install',
+                            os.path.join(
+                                libpath, 'psydac-0.1-py3-none-any.whl'),
                             ], check=True)
-            print('Done.') 
-            
+            print('Done.')
+
         # gvec_to_python (change dir not to be in source path)
-        subprocess.run(['compile-gvec-tp'], check=True, cwd=libpath) 
-            
+        subprocess.run(['compile-gvec-tp'], check=True, cwd=libpath)
+
         print('\nCompiling Struphy and Psydac kernels ...')
-        subprocess.run(['make', 
-                        '-f', 
+        subprocess.run(['make',
+                        '-f',
                         'compile_struphy.mk',
                         'flags=' + flag_verb,
                         'flags_openmp_pic=' + flag_omp_pic,
                         'flags_openmp_mhd=' + flag_omp_mhd,
                         ], check=True, cwd=libpath)
-        print('Done.')  
+        print('Done.')
```

### Comparing `struphy-1.9.9/src/struphy/console/example.py` & `struphy-2.0.0/src/struphy/console/example.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 def struphy_example(case, diagnostics, mpi=1):
     """
     Run a Struphy example.
-    
+
     Parameters
     ----------
     case : str
         Name of the example case to run.
-        
+
     diagnostics : bool
         Wether to do diagnostics and plot only, if example has already been run before, and the output folder still exists.
-        
+
     mpi : int
         Number of MPI processes used to run the example.
     """
-    
+
     import subprocess
     import struphy
 
     libpath = struphy.__path__[0]
-    
+
     command = ['python3',
                'examples/' + case + '.py',
                '--mpi',
                str(mpi)]
-    
+
     if diagnostics:
         command += ['--diagnostics']
-    
-    subprocess.run(command, check=True, cwd=libpath)
+
+    subprocess.run(command, check=True, cwd=libpath)
```

### Comparing `struphy-1.9.9/src/struphy/console/pproc.py` & `struphy-2.0.0/src/struphy/console/pproc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 def struphy_pproc(dirr, dir_abs=None, step=1, celldivide=1):
     """
     Post process data from finished Struphy runs.
-    
+
     Parameters
     ----------
     dirr : str
         Path of simulation output folder relative to <struphy_path>/io/out.
-        
+
     dir_abs : str
         Absolute path to the simulation output folder.
-        
+
     step : int, optional
         Whether to do post-processing at every time step (step=1, default), every second time step (step=2), etc.
-        
+
     celldivide : int, optional
         Number of grid point in each cell used to create vtk files (default=1).
     """
     import subprocess
     import os
     import struphy
 
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+
     # create absolute path
     if dir_abs is None:
-        dir_abs = os.path.join(libpath, 'io/out', dirr)
-    
+        dir_abs = os.path.join(io_path, 'io/out', dirr)
+
     # loop over output folders and call post-processing .py file
     subprocess.run(['python3',
                     'post_processing/pproc_struphy.py',
                     dir_abs,
                     '-s',
                     str(step),
                     '--celldivide',
-                    str(celldivide)], 
-                    cwd=libpath)
+                    str(celldivide)],
+                    cwd=libpath, 
+                    check=True)
```

### Comparing `struphy-1.9.9/src/struphy/console/profile.py` & `struphy-2.0.0/src/struphy/console/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,22 @@
     import numpy as np
     from matplotlib import pyplot as plt
     from struphy.post_processing.cprofile_analyser import get_cprofile_data, replace_keys
     import struphy
 
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+
     # absolute paths
     abs_paths = []
     for d in dirs:
-        abs_paths += [os.path.join(libpath, 'io/out/', d)]
-        
+        abs_paths += [os.path.join(io_path, 'io/out/', d)]
+
     # define the function filter
     list_of_funcs = ['assemble_',
                      'propagator',
                      'accumulate',
                      '_fill',
                      'pusher',
                      'update_ghost_regions',
@@ -56,28 +59,28 @@
 
         with open(os.path.join(path, 'profile_dict.sav'), 'rb') as f:
             dicts_pre += [pickle.load(f)]
 
         with open(os.path.join(path, 'meta.txt'), 'r') as f:
             lines = f.readlines()
 
-        nproc += [int(lines[-1].split()[-1])]
+        nproc += [int(lines[4].split()[-1])]
 
         with open(os.path.join(path, 'parameters.yml'), 'r') as f:
             params = yaml.load(f, Loader=yaml.FullLoader)
 
         Nel += [params['grid']['Nel']]
 
     # Nicer key names for output:
     dicts = []
     for d in dicts_pre:
 
         tmp = {}
         for key, val in d.items():
-            #tmp[key] = float(val['cumtime'])
+            # tmp[key] = float(val['cumtime'])
             tmp[key] = val
 
         if replace:
             tmp2 = replace_keys(tmp)
         else:
             tmp2 = tmp
 
@@ -114,15 +117,15 @@
 
             for dict, sim_name, n, dim in zip(dicts, sim_names, nproc, Nel):
 
                 string = f'{sim_name}'.ljust(
                     20) + f'{n}'.ljust(7) + f'{position:2d}'.ljust(5) + str(key.ljust(70))
                 for value in dict[key].values():
                     string += str(value).ljust(15)
-                    #string += '\t\t'
+                    # string += '\t\t'
                 print(string)
 
                 d_saved[key]['mpi_size'] += [n]
                 d_saved[key]['Nel'] += [dim]
                 d_saved[key]['time'] += [dict[key]['cumtime']]
             print('')
 
@@ -153,11 +156,11 @@
             else:
                 plt.plot(val['mpi_size'], val['time'], label=key)
                 plt.xlabel('mpi_size')
                 plt.ylabel('time [s]')
                 plt.title('Weak scaling for cells/mpi_size=' +
                           str(np.prod(val['Nel'][0])/val['mpi_size'][0]) + '=const.')
                 plt.legend(loc='upper left')
-                #plt.loglog(val['mpi_size'], val['time'][0]*np.ones_like(val['time']), 'k--', alpha=0.3)
+                # plt.loglog(val['mpi_size'], val['time'][0]*np.ones_like(val['time']), 'k--', alpha=0.3)
                 plt.xscale('log')
 
     plt.show()
```

### Comparing `struphy-1.9.9/src/struphy/console/run.py` & `struphy-2.0.0/src/struphy/console/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,152 +1,158 @@
-def struphy_run(model='Maxwell', 
-                input='parameters.yml', 
-                input_abs=None, 
+def struphy_run(model='Maxwell',
+                input='parameters.yml',
+                input_abs=None,
                 output='sim_1',
                 output_abs=None,
                 batch=None,
                 batch_abs=None,
                 runtime=300,
                 save_step=1,
                 restart=False,
                 mpi=1,
                 debug=False):
     """
     Run a Struphy model: prepare arguments, output folder and execute main().
-    
+
     Parameters
     ----------
     model : str
         The name of the Struphy model.
-        
+
     input : str
         The .yml input paramter file relative to <struphy_path>/io/inp.
-        
+
     input_abs : str
         The absolute path to the .yml input parameter file.
-        
+
     output : str
         Name of the output folder in <struphy_path>/io/out.
-        
+
     output_abs : str
         Absolute path to the output folder.
-        
+
     batch : str
         Name of the batch script for runs on a cluster.
-        
+
     batch_abs : str
         Absolute path to the batch scripts for runs on a cluster.
-        
+
     runtime : int
         Maximum runtime of the simulation in minutes. Will complete the time step and exit after this time is reached.
-        
+
     save_step : int
         How often to save data in hdf5 file, i.e. every "save_step" time step.
-        
+
     restart : bool
         Wether to restart an existing simulation.
-        
+
     mpi : int
         Number of MPI processes for runs with "mpirun".
-        
+
     debug : bool
         Wether to run in Cobra debug mode.
     """
-    
+
     import subprocess
     import shutil
     import os
     import glob
     import struphy
 
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+
     # create absolute i/o paths
     if input_abs is None:
-        input_abs = os.path.join(libpath, 'io/inp/', input)
-        
+        input_abs = os.path.join(io_path, 'io/inp/', input)
+
     if output_abs is None:
-        output_abs = os.path.join(libpath, 'io/out/', output)
-        
+        output_abs = os.path.join(io_path, 'io/out/', output)
+
     if batch_abs is None:
         if batch is not None:
-            batch_abs = os.path.join(libpath, 'io/batch/', batch)
-     
-    # take existing parameter file for restart   
+            batch_abs = os.path.join(io_path, 'io/batch/', batch)
+
+    # take existing parameter file for restart
     if restart:
         input_abs = os.path.join(output_abs, 'parameters.yml')
-    
+
     # run in normal or debug mode
     if batch_abs is None:
 
         if debug:
             print('\nLaunching main() in Cobra debug mode ...')
-            command = ['srun', # use mpi
+            command = ['srun',  # use mpi
                        '-n',
                        str(mpi),
-                       '-p', # interactive commands
+                       '-p',  # interactive commands
                        'interactive',
                        '--time',
                        '119',
                        '--mem',
                        '2000',
-                       'python3', # use python3 
-                       '-m', 
-                       'cProfile', # start the profiler
-                       '-o', 
-                       os.path.join(output_abs, 'profile_tmp'), # location of profiling data
+                       'python3',  # use python3
+                       '-m',
+                       'cProfile',  # start the profiler
+                       '-o',
+                       # location of profiling data
+                       os.path.join(output_abs, 'profile_tmp'),
                        '-s',
-                       'time', # sort profile data according to runtime
-                       'models/main.py', # run main.main()
-                       model, # from here on, command line arguments for main()
+                       'time',  # sort profile data according to runtime
+                       'models/main.py',  # run main.main()
+                       model,  # from here on, command line arguments for main()
                        '-i',
                        input_abs,
                        '-o',
                        output_abs,
                        '--runtime',
                        str(runtime),
                        '-s',
                        str(save_step)]
 
         else:
             print('\nLaunching main() in normal mode ...')
-            command = ['mpirun', # always use mpi
+            command = ['mpirun',  # always use mpi
                        '-n',
                        str(mpi),
-                       'python3', # use python3 
-                       '-m', 
-                       'cProfile', # start the profiler
-                       '-o', 
-                       os.path.join(output_abs, 'profile_tmp'), # location of profiling data
+                       'python3',  # use python3
+                       '-m',
+                       'cProfile',  # start the profiler
+                       '-o',
+                       # location of profiling data
+                       os.path.join(output_abs, 'profile_tmp'),
                        '-s',
-                       'time', # sort profile data according to runtime
-                       'models/main.py', # run main.main()
-                       model, # from here on, command line arguments for main()
+                       'time',  # sort profile data according to runtime
+                       'models/main.py',  # run main.main()
+                       model,  # from here on, command line arguments for main()
                        '-i',
                        input_abs,
                        '-o',
                        output_abs,
                        '--runtime',
                        str(runtime),
                        '-s',
                        str(save_step)]
-            
+
         # add restart flag
         if restart:
             command += ['-r']
-            
+
         # run command as subprocess
         subprocess.run(command, check=True, cwd=libpath)
-    
+
     # run in batch mode
     else:
 
         # create output folder if it does not exit
         if not os.path.exists(output_abs):
             os.mkdir(output_abs)
+            os.mkdir(os.path.join(output_abs, 'data/'))
 
         # remove sim.out file
         file = os.path.join(output_abs, 'sim.out')
         if os.path.exists(file):
             os.remove(file)
             print('Removed file ' + file)
 
@@ -167,41 +173,42 @@
         if os.path.exists(file):
             os.remove(file)
             print('Removed file ' + file)
 
         # copy batch script to output folder
         batch_abs_new = os.path.join(output_abs, 'batch_script.sh')
         shutil.copy2(batch_abs, batch_abs_new)
-        
+
         # delete srun command from batch script
         with open(batch_abs_new, 'r') as f:
             lines = f.readlines()
             if 'srun' in lines[-1]:
                 lines = lines[:-2]
-            
+
         # add new srun command
         with open(batch_abs_new, 'w') as f:
             for line in lines:
                 f.write(line)
             f.write('# Run command added by Struphy')
-            
-            command_string  = '\nsrun python3 -m cProfile -o ' + os.path.join(output_abs, 'profile_tmp') + ' -s time '
+
+            command_string = '\nsrun python3 -m cProfile -o ' + \
+                os.path.join(output_abs, 'profile_tmp') + ' -s time '
             command_string += libpath + '/models/main.py '
             command_string += model + ' '
             command_string += '-i ' + input_abs + ' '
             command_string += '-o ' + output_abs + ' '
             command_string += '--runtime ' + str(runtime) + ' '
             command_string += '-s ' + str(save_step) + ' '
-            
+
             if restart:
                 command_string += '-r '
-                
+
             command_string += '> ' + os.path.join(output_abs, 'struphy.out')
-            
+
             f.write(command_string)
-        
+
         # submit batch script in output folder
         print('\nLaunching main() in batch mode ...')
-        subprocess.run(['sbatch', 
+        subprocess.run(['sbatch',
                         'batch_script.sh',
-                        ], 
-                        check=True, cwd=output_abs)
+                        ],
+                       check=True, cwd=output_abs)
```

### Comparing `struphy-1.9.9/src/struphy/console/test.py` & `struphy-2.0.0/src/struphy/console/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,105 +1,118 @@
 def struphy_test(serial=True, mpi=0, codes=False):
     """
     Run Struphy unit and/or code tests.
-    
+
     Parameters
     ----------
     serial : bool
         Whether to run serial units tests.
-        
+
     mpi : int
         If >0, parallel units tests are run with mpi number of processes.
-        
+
     codes : bool
         Whether to run code tests.
     """
-    
+
     import os
     import subprocess
     import struphy
 
     libpath = struphy.__path__[0]
-    
+
     if serial:
         subprocess.run(['pytest',
-                        'tests/tests_serial'], 
-                        check=True, cwd=libpath)
-        
+                        'tests/tests_serial'],
+                       check=True, cwd=libpath)
+
     if mpi > 0:
         subprocess.run(['mpirun',
                         '-n',
                         str(mpi),
                         'pytest',
                         '--with-mpi',
                         'tests/tests_mpi'],
-                        check=True, cwd=libpath)
-        
+                       check=True, cwd=libpath)
+
     if codes:
-        
+
         # test Maxwell
         subprocess.run(['struphy', 'run', 'Maxwell',
                         '-i', 'tests/params_maxwell_1.yml',
                         '-o', 'sim_test_1'], check=True)
         subprocess.run(['struphy', 'run', 'Maxwell',
                         '-i', 'tests/params_maxwell_2.yml',
                         '-o', 'sim_test_2'], check=True)
         subprocess.run(['struphy', 'run', 'Maxwell',
                         '-i', 'tests/params_maxwell_2.yml',
                         '-o', 'sim_test_3',
                         '--mpi', '2'], check=True)
-        
+
         subprocess.run(['struphy', 'pproc',
                         '-d', 'sim_test_1'], check=True)
-        subprocess.run(['struphy', 'pproc', 
+        subprocess.run(['struphy', 'pproc',
                         '-d', 'sim_test_2'], check=True)
-        subprocess.run(['struphy', 'pproc', 
+        subprocess.run(['struphy', 'pproc',
                         '-d', 'sim_test_3'], check=True)
-        
+
         # test LinearMHD
         subprocess.run(['struphy', 'run', 'LinearMHD',
                         '-i', 'tests/params_linearmhd.yml',
                         '-o', 'sim_test_4'], check=True)
         subprocess.run(['struphy', 'run', 'LinearMHD',
                         '-i', 'tests/params_linearmhd.yml',
                         '-o', 'sim_test_5',
                         '--mpi', '2'], check=True)
-        
-        subprocess.run(['struphy', 'pproc', 
-                        '-d', 'sim_test_4', 
+
+        subprocess.run(['struphy', 'pproc',
+                        '-d', 'sim_test_4',
                         '-s', '2',
                         '--celldivide', '3'], check=True)
-        subprocess.run(['struphy', 'pproc', 
+        subprocess.run(['struphy', 'pproc',
                         '-d', 'sim_test_5',
                         '-s', '3',
                         '--celldivide', '2'], check=True)
-        
+
         # test LinearMHDVlasovCC
         subprocess.run(['struphy', 'run', 'LinearMHDVlasovCC',
                         '-i', 'tests/params_hybridmhdvlasovcc.yml',
                         '-o', 'sim_test_6',
                         '--mpi', '2'], check=True)
         subprocess.run(['struphy', 'run', 'LinearMHDVlasovCC',
                         '-i', 'tests/params_hybridmhdvlasovcc_control.yml',
                         '-o', 'sim_test_7',
                         '--mpi', '2'], check=True)
-        
-        subprocess.run(['struphy', 'pproc', 
+
+        subprocess.run(['struphy', 'pproc',
                         '-d', 'sim_test_6'], check=True)
         subprocess.run(['struphy', 'pproc',
                         '-d', 'sim_test_7'], check=True)
-       
+        
+        # (test restart flag -r)
+        subprocess.run(['struphy', 'run', 'LinearMHDVlasovCC',
+                        '-o', 'sim_test_7',
+                        '--mpi', '2', '-r'], check=True)
+
         # test LinearMHDVlasovPC
         subprocess.run(['struphy', 'run', 'LinearMHDVlasovPC',
                         '-i', 'tests/params_hybridmhdvlasovpc.yml',
                         '-o', 'sim_test_8',
                         '--mpi', '2'], check=True)
-        
+
         # test LinearVlasovMaxwell
         subprocess.run(['struphy', 'run', 'LinearVlasovMaxwell',
                         '-i', 'tests/params_linvlasovmaxwell.yml',
                         '-o', 'sim_test_9',
                         '--mpi', '2'], check=True)
-        
-        subprocess.run(['struphy', 'pproc', 
+
+        subprocess.run(['struphy', 'pproc',
                         '-d', 'sim_test_9'], check=True)
-        
+
+        # test DeltaFVlasovMaxwell
+        subprocess.run(['struphy', 'run', 'DeltaFVlasovMaxwell',
+                        '-i', 'tests/params_deltafvlasovmaxwell.yml',
+                        '-o', 'sim_test_10',
+                        '--mpi', '2'], check=True)
+
+        subprocess.run(['struphy', 'pproc',
+                        '-d', 'sim_test_10'], check=True)
```

### Comparing `struphy-1.9.9/src/struphy/diagnostics/continuous_spectra.py` & `struphy-2.0.0/src/struphy/diagnostics/continuous_spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,17 +206,20 @@
                         default=3)
 
     args = parser.parse_args()
     
     import struphy
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     # create absolute input folder path
     if args.input_abs is None:
-        input_path = os.path.join(libpath, 'io/out', args.input)
+        input_path = os.path.join(io_path, 'io/out', args.input)
     else:
         input_path = args.input_abs
         
     # absolute path of .npy spectrum and toroidal mode number
     spec_path = os.path.join(input_path, args.name)
     n_tor = int(os.path.split(spec_path)[-1][-6:-4])
```

### Comparing `struphy-1.9.9/src/struphy/diagnostics/diagn_tools.py` & `struphy-2.0.0/src/struphy/diagnostics/diagn_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,68 +37,73 @@
                         help='(for plot_distr) at which time to plot the distribution function')
     parser.add_argument('-e1', nargs=1, type=float, default=[None],
                         help='(for plot_distr) at which position in eta1 direction to plot')
     parser.add_argument('-e2', nargs=1, type=float, default=[None],
                         help='(for plot_distr) at which position in eta2 direction to plot')
     parser.add_argument('-e3', nargs=1, type=float, default=[None],
                         help='(for plot_distr) at which position in eta3 direction to plot')
-    parser.add_argument('-vx', nargs=1, type=float, default=[None],
+    parser.add_argument('-v1', nargs=1, type=float, default=[None],
                         help='(for plot_distr) at which point in v1 direction to plot')
-    parser.add_argument('-vy', nargs=1, type=float, default=[None],
+    parser.add_argument('-v2', nargs=1, type=float, default=[None],
                         help='(for plot_distr) at which point in v2 direction to plot')
-    parser.add_argument('-vz', nargs=1, type=float, default=[None],
+    parser.add_argument('-v3', nargs=1, type=float, default=[None],
                         help='(for plot_distr) at which point in v3 direction to plot')
 
     args = parser.parse_args()
     actions = args.actions
     foldername = args.f[0]
     time = args.t[0]
     do_log = args.log
     scalars_plot = args.scalars[0]
-    path = os.path.join(os.path.dirname(struphy.__file__),
-                        'io/out', foldername)
+    
+    libpath = struphy.__path__[0]
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+        
+    path = os.path.join(io_path, 'io/out', foldername)
 
     grid_slices = {'e': {'e1': args.e1[0], 'e2': args.e2[0], 'e3': args.e3[0]},
-                   'v': {'vx': args.vx[0], 'vy': args.vy[0], 'vz': args.vz[0]}}
+                   'v': {'v1': args.v1[0], 'v2': args.v2[0], 'v3': args.v3[0]}}
 
     # code name
     with open(path + '/meta.txt', 'r') as f:
         lines = f.readlines()
 
-    code = lines[-2].split()[-1]
+    code = lines[3].split()[-1]
 
     # Get fields
-    file = h5py.File(path + '/data_proc0.hdf5', 'r')
+    file = h5py.File(os.path.join(path, 'data/', 'data_proc0.hdf5'), 'r')
     field_names = list(file['feec'].keys())
     saved_scalars = file['scalar']
+    saved_time = file['time']['value'][:]
 
     # read in parameters
     with open(path + '/parameters.yml') as file:
         params = yaml.load(file, Loader=yaml.FullLoader)
 
     if 'fourier_1d' in actions:
-        assert os.path.exists(os.path.join(path, 'eval_fields')), \
+        assert os.path.exists(os.path.join(path, 'post_processing', 'fields_data')), \
             'For Fourier analysis needs fields in the model.'
 
         point_data_log = []
         # load data dicts for e_field
         for k in range(len(field_names)):
-            with open(path + '/eval_fields/' + field_names[k] + '_log.bin', 'rb') as handle:
+            with open(os.path.join(path, 'post_processing', 'fields_data', field_names[k], '_log.bin'), 'rb') as handle:
                 point_data_log += [pickle.load(handle)]
 
         point_data_phys = []
         for k in range(len(field_names)):
-            with open(path + '/eval_fields/' + field_names[k] + '_phy.bin', 'rb') as handle:
+            with open(os.path.join(path, 'post_processing', 'fields_data', field_names[k], '_phy.bin'), 'rb') as handle:
                 point_data_phys += [pickle.load(handle)]
 
         # load grids
-        with open(path + '/eval_fields/grids_log.bin', 'rb') as handle:
+        with open(os.path.join(path, 'post_processing', 'fields_data', field_names[k], '_log.bin'), 'rb') as handle:
             grids = pickle.load(handle)
 
-        with open(path + '/eval_fields/grids_phy.bin', 'rb') as handle:
+        with open(os.path.join(path, 'post_processing', 'fields_data', field_names[k], '_phy.bin'), 'rb') as handle:
             grids_mapped = pickle.load(handle)
 
         if code == 'LinearMHD':
             equil_type = params['mhd_equilibrium']['name']
 
             if equil_type == 'HomogenSlab':
                 B0x = params['mhd_equilibrium']['HomogenSlab']['B0x']
@@ -138,24 +143,25 @@
                        save_plot=True, save_name=os.path.join(path, code + '_' + field_names[1]))
 
         else:
             raise NotImplementedError(
                 f'1D Fourier analysis is not yet implemented for the model {code}')
 
     if 'plot_scalars' in actions:
-        plot_scalars(saved_scalars,
+        plot_scalars(saved_time,
+                     saved_scalars,
                      scalars_plot=scalars_plot,
                      do_log=do_log,
                      save_plot=True,
                      savename=os.path.join(path, code))
 
     if 'plot_distr' in actions:
         for species in params['kinetic'].keys():
-            time_idx = np.argmin(np.abs(time - saved_scalars['time'][:]))
-            plot_distr_fun(path=os.path.join(path, 'kinetic_data', species),
+            time_idx = np.argmin(np.abs(time - saved_time))
+            plot_distr_fun(path=os.path.join(path, 'post_processing', 'kinetic_data', species),
                            time_idx=time_idx,
                            grid_slices=grid_slices,
                            save_plot=True, savepath=path)
 
     file.close()
 
 
@@ -322,15 +328,15 @@
         else:
             plt.show()
 
     else:
         return kvec, omega, dispersion
 
 
-def plot_scalars(scalar_quantities, scalars_plot=[], do_log=False, save_plot=False, savename=None, file_format='png'):
+def plot_scalars(time, scalar_quantities, scalars_plot=[], do_log=False, save_plot=False, savename=None, file_format='png'):
     """
     Plot the scalar quantities and the relative error in the total energy for a simulation.
 
     Parameters
     ----------
     scalar_quantities : dict
         HDF5 dictionary dataset containing the scalar quantities that were saved during the simulation
@@ -346,15 +352,14 @@
 
     savename : str
         Name under which the plot of the result should be saved.
 
     file_format : str
         Type of file which the plot of the result should be saved.
     """
-    time = scalar_quantities['time'][:]
 
     if 'en_tot' in scalar_quantities.keys():
         en_tot = scalar_quantities['en_tot'][:]
 
         plt.figure('en_tot')
         if do_log:
             plt.semilogy(time, en_tot)
@@ -425,117 +430,78 @@
         Path under which the plot of the result should be saved.
 
     file_format : str
         Type of file which the plot of the result should be saved.
     """
 
     species = str(path.split('/')[-1])
+    path = os.path.join(path, 'distribution_function')
 
     # make empty dictionaries
     f = {'e': None, 'v': None}
     delta_f = {'e': None, 'v': None}
-    ints_to_names = {'e': {}, 'v': {}}
-    names_to_ints = {'e': {}, 'v': {}}
-    grids = {'e': {}, 'v': {}}
+    grids = {'e': [], 'v': []}
 
     # Loop over files and load distribution function data
-    for filename in os.listdir(os.path.join(path, 'f')):
-        filepath = os.path.join(path, 'f', filename)
+    for filename in os.listdir(path):
+        filepath = os.path.join(path, filename)
 
-        # load full distribution functions
+        # load full distribution functions and compute inds_to_names and names_to_inds
         if filename[:3] == 'f_e':
-            k = 1
-            while True:
-                try:
-                    ints_to_names['e'][str(k)] = \
-                        filename.split('_')[k].split('.')[0]
-                    names_to_ints['e'][filename.split('_')[k].split('.')[0]] = \
-                        str(k)
-                except:
-                    break
-                else:
-                    k += 1
             f['e'] = np.load(filepath)
+            for comp in filename.split('_')[1:]:
+                comp = comp.split('.')[0]
+                grids['e'] += [np.load(os.path.join(path, 'grid_' + comp + '.npy'))]
         elif filename[:3] == 'f_v':
-            k = 1
-            while True:
-                try:
-                    ints_to_names['v'][str(k)] = \
-                        filename.split('_')[k].split('.')[0]
-                    names_to_ints['v'][filename.split('_')[k].split('.')[0]] = \
-                        str(k)
-                except:
-                    break
-                else:
-                    k += 1
             f['v'] = np.load(filepath)
+            for comp in filename.split('_')[1:]:
+                comp = comp.split('.')[0]
+                grids['v'] += [np.load(os.path.join(path, 'grid_' + comp + '.npy'))]
 
         # load delta f
         elif filename[:9] == 'delta_f_e':
             delta_f['e'] = np.load(filepath)
         elif filename[:9] == 'delta_f_v':
             delta_f['v'] = np.load(filepath)
 
-    # loop over files and load grid data
-    for filename in os.listdir(os.path.join(path, 'f')):
-        filepath = os.path.join(path, 'f', filename)
-        # load position grids
-        if filename[:6] == 'grid_e':
-            suffix = filename.split('_')[-1].split('.')[0]
-            grids['e'][suffix] = np.load(filepath)
-
-        # load velocity grids
-        elif filename[:6] == 'grid_v':
-            suffix = filename.split('_')[-1].split('.')[0]
-            grids['v'][suffix] = np.load(filepath)
-
     for typ in ['e', 'v']:
-        # plot in all available directions
-        for plot_dir, plot_grid in grids[typ].items():
-            slicing = [slice(None)] * len(grids[typ])
-
-            # find indices where values are in all directions
-            for direction, grid in grids[typ].items():
-                if direction != plot_dir:
-                    if grid_slices[typ][ints_to_names[typ][direction]] is None:
-                        idx = len(grid) // 2
-                    else:
-                        idx = np.argmin(np.abs(grid - grid_slices[typ][ints_to_names[typ][direction]]))
-                    slicing[int(direction) - 1] = idx
-
-            # create slicing tuple
-            f_slicing = tuple([time_idx] + slicing)
+        for k in range(f[typ].ndim - 1):
 
+            f_slicing = [0] * f[typ].ndim
+            f_slicing[k + 1] = slice(None)
             # plot delta_f
             if delta_f[typ] is not None:
                 plt.figure('delta_f')
-                plt.plot(plot_grid, delta_f[typ][f_slicing].squeeze())
-                plt.xlabel(ints_to_names[typ][plot_dir])
+                plt.plot(grids[typ][k], delta_f[typ][tuple(f_slicing)].squeeze())
+                plt.xlabel(typ + str(k + 1))
                 plt.ylabel(r'$\delta f$')
+                print(f'Created plot for delta_f in {typ + str(k + 1)}')
 
                 if save_plot:
                     assert savepath is not None, 'When wanting to save the plot a path has to be given!'
                     savename = os.path.join(savepath, species + '_delta_f_'
-                                            + ints_to_names[typ][plot_dir] + '.' + file_format)
+                                            + typ + str(k + 1) + '.' + file_format)
                     plt.savefig(savename)
                 else:
                     plt.show()
                 plt.close()
 
-            # plot full distribution function
-            plt.figure('f')
-            plt.plot(plot_grid, f[typ][f_slicing].squeeze())
-            plt.xlabel(ints_to_names[typ][plot_dir])
-            plt.ylabel(r'$f$')
-
-            if save_plot:
-                assert savepath is not None, 'When wanting to save the plot a path has to be given!'
-                savename = os.path.join(savepath, species + '_f_'
-                                        + ints_to_names[typ][plot_dir] + '.' + file_format)
-                plt.savefig(savename)
-            else:
-                plt.show()
-            plt.close()
+            # plot full f
+            if f[typ] is not None:
+                plt.figure('f')
+                plt.plot(grids[typ][k], f[typ][tuple(f_slicing)].squeeze())
+                plt.xlabel(typ + str(k + 1))
+                plt.ylabel(r'$f$')
+                print(f'Created plot for f in {typ + str(k + 1)}')
+
+                if save_plot:
+                    assert savepath is not None, 'When wanting to save the plot a path has to be given!'
+                    savename = os.path.join(savepath, species + '_f_'
+                                            + typ + str(k + 1) + '.' + file_format)
+                    plt.savefig(savename)
+                else:
+                    plt.show()
+                plt.close()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `struphy-1.9.9/src/struphy/diagnostics/paraview/mesh_creator.py` & `struphy-2.0.0/src/struphy/diagnostics/paraview/mesh_creator.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/diagnostics/paraview/vtk_writer.py` & `struphy-2.0.0/src/struphy/diagnostics/paraview/vtk_writer.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/dispersion_relations/analytic.py` & `struphy-2.0.0/src/struphy/dispersion_relations/analytic.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,132 @@
         omegas = {}
         for name, tmp in zip(self.branches, tmps):
             omegas[name] = tmp
 
         return omegas
 
 
+class ExtendedMhd1D(DispersionRelations1D):
+    r"""
+    Dispersion relation for linear Extended MHD equations for homogeneous background :math:`(n_0,p_0,\mathbf B_0)` and wave propagation along z-axis in Struphy units (see ``LinearMHD`` in :ref:`models`):
+
+    .. math::
+
+        \textnormal{shear Alfvén}:\quad &\omega^2 = c_\textnormal{A}^2 k^2\frac{B_{0z}^2}{|\mathbf B_0|^2}\,,
+
+        \textnormal{fast (+) and slow (-) magnetosonic}:\quad &\omega^2 =\frac{1}{2}(c_\textnormal{S}^2+c_\textnormal{A}^2)k^2(1\pm\sqrt{1-\delta}\,)\,,\quad\delta=\frac{4B_{0z}^2c_\textnormal{S}^2c_\textnormal{A}^2}{(c_\textnormal{S}^2+c_\textnormal{A}^2)^2|\mathbf B_0|^2}\,,
+
+    where :math:`c_\textnormal{A}^2=|\mathbf B_0|^2/n_0` is the Alfvén velocity and :math:`c_\textnormal{S}^2=\gamma\,p_0/n_0` is the speed of sound.
+    """
+
+    def __init__(self, **params):
+        super().__init__('fast magnetosonic', 'slow magnetosonic','compression Alfvén','shear Alfvén', **params)
+
+    def __call__(self, k):
+        """
+        The evaluation of all branches of the 1d dispersion relation.
+
+        Parameters
+        ----------
+        k : array_like
+            Evaluation wave numbers.
+
+        Returns
+        -------
+        omegas : dict
+            A dictionary with key=branch_name and value=omega(k) (complex ndarray).
+        """
+
+        # One complex array for each branch
+        tmps = []
+        for n in range(self.nbranches):
+            tmps += [np.zeros_like(k, dtype=complex)]
+
+        ########### Model specific part ##############################
+
+        #Quantities related with backgorund magnetic field
+        B0x = self.params['B0x']
+        B0y = self.params['B0y']
+        B0z = self.params['B0z']
+        B0n = np.sqrt(B0x**2.0 + B0y**2.0 + B0z**2.0)
+        
+        #Cos(theta)
+        cos = B0z/B0n
+        
+        #Background number density
+        n0 = self.params['n0']
+        
+        #Background pressures
+        pi0 = self.params['p0']
+        pe0 = self.params['p0']
+        gamma = self.params['gamma']
+        
+        #Basic units of magnetic field and time
+        Bu = self.params['Bu']
+        tu = self.params['tu']
+        
+        # compute coupling parameter kappa
+        ee = 1.602176634e-19  # elementary charge (C)
+        mH = 1.67262192369e-27  # proton mass (kg)
+        Ab = self.params['A']
+        Zb = self.params['Z']
+        
+        omega_ch = (Zb*ee*Bu)/(Ab*mH)
+        kappa = omega_ch*tu/(2.0 * np.pi)
+
+        if abs(kappa - 1) < 1e-6:
+            kappa = 1.
+        
+        # Alfvén velocity 
+        cA = B0n/np.sqrt(n0)
+        
+        #We will need some auxiliary arrays to compute the las three waves
+        bs = np.zeros_like(k, dtype=complex)
+        bs[:] = - k**2.0 *(cA**2.0)*(cos**2.0*(1.0+ k**2.0 * kappa**2.0/n0) + 1.0 + (gamma/B0n**2.0)*(pi0+pe0) )
+
+        cs = np.zeros_like(k, dtype=complex)
+        cs[:] = k**4.0 * cos**2.0 * cA**4.0 * (1.0 + (pi0+pe0)*(gamma/B0n**2.0)*(2.0 + k**2.0 * kappa**2.0 / n0) )
+
+        ds = np.zeros_like(k, dtype=complex)
+        ds[:] = -k**6.0 * (B0n**4.0 / n0**3.0) * gamma * (pi0 + pe0) * cos**4.0
+
+        D0s = np.zeros_like(k, dtype=complex)
+        D0s[:] = bs**2.0 - 3.0*cs
+
+        D1s = np.zeros_like(k, dtype=complex)
+        D1s[:] = 2.0* bs**3.0 - 9.0*bs*cs + 27.0*ds
+
+        Ccs = np.zeros_like(k, dtype=complex)
+        Ccs[:] = ( (D1s + (D1s**2.0 - 4.0*D0s**3.0 )**(1.0/2.0) )/2.0 )**(1.0/3.0)
+
+        #Finally we need a special complex number
+        SHI = (-1.0 + (-3.0)**(1.0/2.0))*0.5
+        
+        # fast magnetosonic branch
+        tmps[0][:] = (B0n*kappa*cos/n0)*k**2.0 
+        
+        # slow magnetosonic
+        tmps[1][:] = ( (-1.0/3.0)*(bs + Ccs + D0s/Ccs) )**(1.0/2.0) 
+        
+        # compression Alfvén branch
+        tmps[2][:] = ( (-1.0/3.0)*(bs + SHI*Ccs + D0s/(SHI*Ccs) ) )**(1.0/2.0) 
+        
+        # shear Alfvén branch
+        tmps[3][:] = ( (-1.0/3.0)*(bs + SHI*SHI*Ccs + D0s/(SHI*SHI*Ccs) ) )**(1.0/2.0)
+
+        ##############################################################
+
+        # fill output dictionary
+        omegas = {}
+        for name, tmp in zip(self.branches, tmps):
+            omegas[name] = tmp
+
+        return omegas
+
+
 class ColdPlasma1D(DispersionRelations1D):
     r'''Dispersion relation for cold plasma model :math:`(\alpha,\mathbf B_0)`
     and wave propagation along z-axis :math:`(\mathbf k = k \mathbf e_z)` in Struphy units
     (see ``ColdPlasma`` in :ref:`models`):
     
     .. math::
     
@@ -195,15 +313,15 @@
 
         # fill output dictionary
         dict_disp = {}
         for name, tmp in zip(self.branches, tmps):
             dict_disp[name] = tmp
 
         return dict_disp
-
+    
 
 class CurrentCoupling6DParallel(DispersionRelations1D):
     r"""
     Dispersion relation for linearized hybrid MHD-Vlasov model (current coupling scheme) in Struphy units for homogeneous background :math:`(n_0=1,p_0,\mathbf B_0=B_0\mathbf e_z)`, wave propagation along z-axis and EP distribution function
 
     .. math::
```

### Comparing `struphy-1.9.9/src/struphy/dispersion_relations/base.py` & `struphy-2.0.0/src/struphy/dispersion_relations/base.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/derivatives.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/derivatives.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/kernels_2d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/kernels_3d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/kernels_projectors_global.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_projectors_global.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/kernels_projectors_global_mhd.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/kernels_projectors_global_mhd.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/MHD_eigenvalues_cylinder_1D.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/MHD_eigenvalues_cylinder_1D.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/control_variate.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kernels_control_variate.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kernels_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_control_variate.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_kernels_control_variate.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fB_massless_kernels_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_control_variate.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_cv_kernel_2.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_cv_kernel_2.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_kernels_control_variate.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/fnB_massless_kernels_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_control_variate.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_cvker.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_cvker.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_kernels_control_variate.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/control_variates/kinetic_extended/massless_kernels_control_variate.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/emw_operators.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/emw_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/inner_products_1d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/inner_products_2d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/inner_products_3d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/inner_products_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/l2_error_1d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/l2_error_2d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/l2_error_3d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/l2_error_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/mass_matrices_3d_pre.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mass_matrices_3d_pre.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_arrays.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_arrays.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bb_kernel.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bb_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bv_kernel.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_bv_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_massless_linear_operators.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_massless_linear_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_vv_kernel.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/massless_operators/fB_vv_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF_for_tests.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/mhd_operators_MF_for_tests.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local_mhd.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/kernels_projectors_local_mhd.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/mhd_operators_3d_local.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/mhd_operators_3d_local.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/projectors_local.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/pro_local/projectors_local.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_L2_projector_kernel.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_L2_projector_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_L2.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_L2.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_local.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_function_projectors_local.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_local_projector_kernel.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/legacy/projectors_local/shape_pro_local/shape_local_projector_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/mass_matrices_1d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/mass_matrices_2d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/mass_matrices_3d.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/mass_matrices_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/mhd_axisymmetric_main.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_axisymmetric_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,22 +199,25 @@
                         help='output directory, absolute path')    
 
     args = parser.parse_args()
     
     import struphy
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     # create absolute i/o paths
     if args.input_abs is None:
-        input_abs = os.path.join(libpath, 'io/inp', args.input)
+        input_abs = os.path.join(io_path, 'io/inp', args.input)
     else:
         input_abs = args.input_abs
         
     if args.output_abs is None:
-        output_abs = os.path.join(libpath, 'io/out', args.output)
+        output_abs = os.path.join(io_path, 'io/out', args.output)
     else:
         output_abs = args.output_abs
         
     # create output folder (if it does not already exist)
     if not os.path.exists(output_abs):
         os.mkdir(output_abs)
         print('\nCreated folder ' + output_abs)
```

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/mhd_axisymmetric_pproc.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_axisymmetric_pproc.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,17 +32,20 @@
                         help='upper range of squared eigenfrequency')
 
     args = parser.parse_args()
     
     import struphy
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     # create absolute input folder path
     if args.input_abs is None:
-        input_path = os.path.join(libpath, 'io/out', args.input)
+        input_path = os.path.join(io_path, 'io/out', args.input)
     else:
         input_path = args.input_abs
         
     # load spectrum and restrict to range
     if args.n < 0:
         n_tor_str = str(args.n)
     else:
```

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/mhd_operators.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/mhd_operators_core.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/mhd_operators_core.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/projectors_global.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/projectors_global.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/eigenvalue_solvers/spline_space.py` & `struphy-2.0.0/src/struphy/eigenvalue_solvers/spline_space.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/examples/TAE_tokamak.py` & `struphy-2.0.0/src/struphy/examples/TAE_tokamak.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     """
     
     import os
     import subprocess
     import struphy
 
     libpath = struphy.__path__[0]
+    
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
 
     # name of simulation output folder
     out_name = 'sim_example_TAE_tokamak'
     
     # run MHD eigenvalue solver
     subprocess.run(['python3',
                     'eigenvalue_solvers/mhd_axisymmetric_main.py',
@@ -39,15 +42,15 @@
                     check=True, cwd=libpath)
     
     # run the model
     subprocess.run(['struphy', 
                     'run', 
                     'LinearMHD',
                     '--input-abs',
-                    os.path.join(libpath, 'io/out', out_name, 'parameters.yml'),
+                    os.path.join(io_path, 'io/out', out_name, 'parameters.yml'),
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
@@ -75,16 +78,19 @@
     from struphy.dispersion_relations.analytic import MhdContinousSpectraCylinder
     from struphy.eigenvalue_solvers.spline_space import Spline_space_1d, Tensor_spline_space
     
     import struphy
 
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     out_name = 'sim_example_TAE_tokamak'
-    out_path = os.path.join(libpath, 'io/out', out_name)
+    out_path = os.path.join(io_path, 'io/out', out_name)
 
     # load simulation parameters
     with open(os.path.join(out_path, 'parameters.yml')) as file:
         params = yaml.load(file, Loader=yaml.FullLoader)
 
     # load grid data
     Nel = params['grid']['Nel']
@@ -97,15 +103,15 @@
     # create domain and MHD equilibrium
     domain, mhd_equil = setup_domain_mhd(params)
     
     # get MHD equilibrium parameters
     mhd_params = params['mhd_equilibrium'][params['mhd_equilibrium']['type']]
 
     # field names, grid info and energies
-    file = h5py.File(os.path.join(out_path, 'data_proc0.hdf5'), 'r')
+    file = h5py.File(os.path.join(out_path, 'data/', 'data_proc0.hdf5'), 'r')
 
     names = list(file['feec'].keys())
 
     t  = file['time/value'][:]
     eU = file['scalar']['en_U'][:]
     eB = file['scalar']['en_B'][:]
 
@@ -115,15 +121,15 @@
     with open(os.path.join(out_path, 'post_processing/fields_data/grids_log.bin'), 'rb') as handle:
         grids_log = pickle.load(handle)
 
     with open(os.path.join(out_path, 'post_processing/fields_data/grids_phy.bin'), 'rb') as handle:
         grids_phy = pickle.load(handle)
 
     # load data dicts for logical u_field
-    with open(os.path.join(out_path, 'post_processing/fields_data', names[3] + '_log.bin'), 'rb') as handle:
+    with open(os.path.join(out_path, 'post_processing/fields_data/mhd/u2_log.bin'), 'rb') as handle:
         u_field_log = pickle.load(handle)
 
     # perform continuous spectra diagnostics
     spec_path = os.path.join(out_path, 'spec_n_-1.npy')
     n_tor = int(spec_path[-6:-4])
 
     fem_1d_1 = Spline_space_1d(Nel[0], p[0], spl_kind[0], nq_el[0], bc[0])
@@ -148,25 +154,25 @@
 
     f_size = 16
     plt.rcParams.update({'font.size': f_size})
 
     # plot safety factor
     plt.subplot(2, 2, 1)
     r = np.linspace(0., 1., 101)
-    plt.plot(r, mhd_equil.q(r))
+    plt.plot(r, mhd_equil.q_r(r))
     plt.xlabel('r [m]')
     plt.ylabel('safety factor')
 
     # plot shear Alfvén continuous spectra for m = [2, 3, 4]
 
     # analytical continuous spectra
     spec_calc = MhdContinousSpectraCylinder(R0=mhd_params['R0'],
                                             Bz=lambda r: mhd_params['B0'] - 0*r,
-                                            q=mhd_equil.q, rho=mhd_equil.nr,
-                                            p=mhd_equil.pr, gamma=5/3)
+                                            q=mhd_equil.q_r, rho=mhd_equil.n_r,
+                                            p=mhd_equil.p_r, gamma=5/3)
 
     plt.subplot(2, 2, 2)
     for m in range(2, 4 + 1):
         plt.plot(0.1 + 0.9*A[m][0], A[m][1]/omegaA **2,
                  '+', label='m = ' + str(m))
         plt.plot(domain(grids_log[0], 0., 0.)[0] - mhd_params['R0'],
                  spec_calc(domain(grids_log[0], 0., 0.)[0] \
```

### Comparing `struphy-1.9.9/src/struphy/examples/_draw_parallel.py` & `struphy-2.0.0/src/struphy/examples/_draw_parallel.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/examples/_mhd_eigenvalues_cylinder.py` & `struphy-2.0.0/src/struphy/examples/_mhd_eigenvalues_cylinder.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/examples/_mhd_eigenvalues_slab.py` & `struphy-2.0.0/src/struphy/examples/_mhd_eigenvalues_slab.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/examples/_sendrecv.py` & `struphy-2.0.0/src/struphy/examples/_sendrecv.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/examples/gc_orbits_tokamak.py` & `struphy-2.0.0/src/struphy/examples/gc_orbits_tokamak.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,28 +44,31 @@
     
     from struphy.models.utilities import setup_domain_mhd
     from struphy.fields_background.mhd_equil.equils import EQDSKequilibrium
     
     import struphy
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     # output path
     out_name = 'sim_example_gc_orbits_tokamak'
-    out_path = os.path.join(libpath, 'io/out', out_name)
+    out_path = os.path.join(io_path, 'io/out', out_name)
     
     # load simulation parameters
     with open(os.path.join(out_path, 'parameters.yml')) as file:
         params = yaml.load(file, Loader=yaml.FullLoader)
 
     # create domain and MHD equilibrium
     domain, mhd_equil = setup_domain_mhd(params)
     domain_name = domain.__class__.__name__
     
     # load grid_info (domain decomposition)
-    file = h5py.File(os.path.join(out_path, 'data_proc0.hdf5'), 'r')
+    file = h5py.File(os.path.join(out_path, 'data/', 'data_proc0.hdf5'), 'r')
     grid_info = file['scalar'].attrs['grid_info']
     file.close()
     
     # load time grid info
     tgrid = np.load(os.path.join(out_path, 'post_processing/t_grid.npy'))
     Nt = len(tgrid) - 1
```

### Comparing `struphy-1.9.9/src/struphy/examples/linearmhd.py` & `struphy-2.0.0/src/struphy/examples/linearmhd.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,19 @@
     
     from struphy.diagnostics.diagn_tools import fourier_1d
     
     import struphy
 
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     out_name = 'sim_example_linearmhd'
-    out_path = os.path.join(libpath, 'io/out', out_name)
+    out_path = os.path.join(io_path, 'io/out', out_name)
     
     # read in parameters for analytical dispersion relation
     with open(os.path.join(out_path, 'parameters.yml')) as file:
         params = yaml.load(file, Loader=yaml.FullLoader)
 
     # parameters for dispersion relation
     B0x = params['mhd_equilibrium']['HomogenSlab']['B0x']
@@ -70,51 +73,47 @@
     # code name
     with open(os.path.join(out_path, 'parameters.yml')) as f:
         lines = f.readlines()
 
     code = lines[-2].split()[-1]
 
     # field names
-    file = h5py.File(os.path.join(out_path, 'data_proc0.hdf5'), 'r')
+    file = h5py.File(os.path.join(out_path, 'data/', 'data_proc0.hdf5'), 'r')
     names = list(file['feec'].keys())
     file.close()
 
     # load grids
     with open(os.path.join(out_path, 'post_processing/fields_data/grids_log.bin'), 'rb') as handle:
         grids_log = pickle.load(handle)
 
     with open(os.path.join(out_path, 'post_processing/fields_data/grids_phy.bin'), 'rb') as handle:
         grids_phy = pickle.load(handle)
 
+    print(names)
+
     # load data dicts for u_field
-    with open(os.path.join(out_path, 'post_processing/fields_data', names[3] + '_log.bin'), 'rb') as handle:
+    with open(os.path.join(out_path, 'post_processing/fields_data/mhd/uv_log.bin'), 'rb') as handle:
         point_data_log = pickle.load(handle)
 
-    with open(os.path.join(out_path, 'post_processing/fields_data', names[3] + '_phy.bin'), 'rb') as handle:
-        point_data_phy = pickle.load(handle)
-
     # fft in (t, z) of first component of u_field on physical grid
     fourier_1d(point_data_log,
                names[3],
                code,
                grids_log,
                grids_mapped=grids_phy, 
                component=0,
                slice_at=[0, 0, None],
                do_plot=True, 
                disp_name='Mhd1D', 
                disp_params=disp_params)
 
     # load data dicts for pressure
-    with open(os.path.join(out_path, 'post_processing/fields_data', names[2] + '_log.bin'), 'rb') as handle:
+    with open(os.path.join(out_path, 'post_processing/fields_data/mhd/p3_log.bin'), 'rb') as handle:
         point_data_log = pickle.load(handle)
 
-    with open(os.path.join(out_path, 'post_processing/fields_data', names[2] + '_phy.bin'), 'rb') as handle:
-        point_data_phy = pickle.load(handle)
-
     # fft in (t, z) of pressure on physical grid
     fourier_1d(point_data_log,
                names[2], 
                code, 
                grids_log,
                grids_mapped=grids_phy,
                component=0,
```

### Comparing `struphy-1.9.9/src/struphy/examples/linearmhdvlasov_cc.py` & `struphy-2.0.0/src/struphy/examples/linearmhdvlasov_pc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 def run(n_procs):
     """
-    Run an example for the model "LinearMHDVlasovCC", including post-processing.
+    Run an example for the model "LinearMHDVlasovPC", including post-processing.
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
     import subprocess
     
     # name of simulation output folder
-    out_name = 'sim_example_linearmhdvlasovcc'
+    out_name = 'sim_example_linearmhdvlasovpc'
     
     # run the model
     subprocess.run(['struphy', 
                     'run', 
-                    'LinearMHDVlasovCC',
+                    'LinearMHDVlasovPC',
                     '-i',
-                    'examples/params_hybridmhdvlasovcc.yml',
+                    'examples/params_hybridmhdvlasovpc.yml',
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
@@ -41,19 +41,22 @@
     import numpy as np
     import matplotlib.pyplot as plt
     
     import struphy
 
     libpath = struphy.__path__[0]
     
-    out_name = 'sim_example_linearmhdvlasovcc'
-    out_path = os.path.join(libpath, 'io/out', out_name)
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
+    out_name = 'sim_example_linearmhdvlasovpc'
+    out_path = os.path.join(io_path, 'io/out', out_name)
 
     # load data
-    file = h5py.File(os.path.join(out_path, 'data_proc0.hdf5'), 'r')
+    file = h5py.File(os.path.join(out_path, 'data/', 'data_proc0.hdf5'), 'r')
 
     t  = file['time/value'][:]
     eu = file['scalar/en_U'][:]
     eb = file['scalar/en_B'][:]
     ef = file['scalar/en_f'][:]
 
     field_names = list(file['feec'].keys())
@@ -62,21 +65,17 @@
 
     # load grid
     with open(os.path.join(out_path, 'post_processing/fields_data/grids_phy.bin'), 'rb') as handle:
         grids_phy = pickle.load(handle)
 
     Lz = grids_phy[2][0, 0, -1]
 
-    # load data dict for u_field
-    with open(os.path.join(out_path, 'post_processing/fields_data/' + field_names[3] + '_phy.bin'), 'rb') as handle:
-        point_data_phys = pickle.load(handle)
-
     # load distriution function
-    f  = np.load(os.path.join(out_path, 'post_processing/kinetic_data/energetic_ions/distribution_function/f_vz.npy'))
-    vz = np.load(os.path.join(out_path, 'post_processing/kinetic_data/energetic_ions/distribution_function/grid_vz_1.npy'))
+    f  = np.load(os.path.join(out_path, 'post_processing/kinetic_data/energetic_ions/distribution_function/v3/f_binned.npy'))
+    vz = np.load(os.path.join(out_path, 'post_processing/kinetic_data/energetic_ions/distribution_function/v3/grid_v3.npy'))
 
     fig = plt.figure()
     fig.set_figheight(3.5)
     fig.set_figwidth(12)
 
     plt.subplot(1, 2, 1)
 
@@ -94,15 +93,15 @@
     plt.text(15, 2.5e-2, 'analytical growth')
     plt.arrow(51, 2.8e-2, 7., 0., head_width=.01, head_length=.5000)
     plt.text(15, 2e-3, 'linear phase')
     plt.text(80, 1e-4, 'nonlinear phase')
 
     plt.subplot(1, 2, 2)
     plt.plot(vz, f[0], label='$t=0$')
-    plt.plot(vz, f[100], label='$t=60$')
+    plt.plot(vz, f[300], label='$t=60$')
     plt.xlabel('$v_z$')
     plt.ylabel('$f_{v_z}$')
     plt.title('EP distribution function')
     plt.text(3.5, 0.03, 'resonance velocity')
     plt.arrow(3.3, 0.03, -0.5, 0., head_width=.002, head_length=.15)
     plt.legend(loc='upper left')
 
@@ -114,15 +113,15 @@
     
 
 if __name__ == '__main__':
     
     import argparse
     
     # get number of MPI processes
-    parser = argparse.ArgumentParser(description='Run an example for the model "LinearMHDVlasovCC".')
+    parser = argparse.ArgumentParser(description='Run an example for the model "LinearMHDVlasovPC".')
     
     parser.add_argument('--mpi',
                         type=int,
                         metavar='N',
                         help='number of MPI processes used to run the model (default=1)',
                         default=1)
```

### Comparing `struphy-1.9.9/src/struphy/examples/linearmhdvlasov_pc.py` & `struphy-2.0.0/src/struphy/examples/linearmhdvlasov_cc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 def run(n_procs):
     """
-    Run an example for the model "LinearMHDVlasovPC", including post-processing.
+    Run an example for the model "LinearMHDVlasovCC", including post-processing.
     
     Parameters
     ----------
     n_procs : int
         Number of MPI processes to run the model.
     """
     
     import subprocess
     
     # name of simulation output folder
-    out_name = 'sim_example_linearmhdvlasovpc'
+    out_name = 'sim_example_linearmhdvlasovcc'
     
     # run the model
     subprocess.run(['struphy', 
                     'run', 
-                    'LinearMHDVlasovPC',
+                    'LinearMHDVlasovCC',
                     '-i',
-                    'examples/params_hybridmhdvlasovpc.yml',
+                    'examples/params_hybridmhdvlasovcc.yml',
                     '-o',
                     out_name,
                     '--mpi',
                     str(n_procs)], check=True)
     
     # perform post-processing
     subprocess.run(['struphy',
@@ -41,19 +41,22 @@
     import numpy as np
     import matplotlib.pyplot as plt
     
     import struphy
 
     libpath = struphy.__path__[0]
     
-    out_name = 'sim_example_linearmhdvlasovpc'
-    out_path = os.path.join(libpath, 'io/out', out_name)
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
+    out_name = 'sim_example_linearmhdvlasovcc'
+    out_path = os.path.join(io_path, 'io/out', out_name)
 
     # load data
-    file = h5py.File(os.path.join(out_path, 'data_proc0.hdf5'), 'r')
+    file = h5py.File(os.path.join(out_path, 'data/', 'data_proc0.hdf5'), 'r')
 
     t  = file['time/value'][:]
     eu = file['scalar/en_U'][:]
     eb = file['scalar/en_B'][:]
     ef = file['scalar/en_f'][:]
 
     field_names = list(file['feec'].keys())
@@ -62,21 +65,17 @@
 
     # load grid
     with open(os.path.join(out_path, 'post_processing/fields_data/grids_phy.bin'), 'rb') as handle:
         grids_phy = pickle.load(handle)
 
     Lz = grids_phy[2][0, 0, -1]
 
-    # load data dict for u_field
-    with open(os.path.join(out_path, 'post_processing/fields_data/' + field_names[3] + '_phy.bin'), 'rb') as handle:
-        point_data_phys = pickle.load(handle)
-
     # load distriution function
-    f  = np.load(os.path.join(out_path, 'post_processing/kinetic_data/energetic_ions/distribution_function/f_vz.npy'))
-    vz = np.load(os.path.join(out_path, 'post_processing/kinetic_data/energetic_ions/distribution_function/grid_vz_1.npy'))
+    f  = np.load(os.path.join(out_path, 'post_processing/kinetic_data/energetic_ions/distribution_function/v3/f_binned.npy'))
+    vz = np.load(os.path.join(out_path, 'post_processing/kinetic_data/energetic_ions/distribution_function/v3/grid_v3.npy'))
 
     fig = plt.figure()
     fig.set_figheight(3.5)
     fig.set_figwidth(12)
 
     plt.subplot(1, 2, 1)
 
@@ -94,15 +93,15 @@
     plt.text(15, 2.5e-2, 'analytical growth')
     plt.arrow(51, 2.8e-2, 7., 0., head_width=.01, head_length=.5000)
     plt.text(15, 2e-3, 'linear phase')
     plt.text(80, 1e-4, 'nonlinear phase')
 
     plt.subplot(1, 2, 2)
     plt.plot(vz, f[0], label='$t=0$')
-    plt.plot(vz, f[300], label='$t=60$')
+    plt.plot(vz, f[100], label='$t=60$')
     plt.xlabel('$v_z$')
     plt.ylabel('$f_{v_z}$')
     plt.title('EP distribution function')
     plt.text(3.5, 0.03, 'resonance velocity')
     plt.arrow(3.3, 0.03, -0.5, 0., head_width=.002, head_length=.15)
     plt.legend(loc='upper left')
 
@@ -114,15 +113,15 @@
     
 
 if __name__ == '__main__':
     
     import argparse
     
     # get number of MPI processes
-    parser = argparse.ArgumentParser(description='Run an example for the model "LinearMHDVlasovPC".')
+    parser = argparse.ArgumentParser(description='Run an example for the model "LinearMHDVlasovCC".')
     
     parser.add_argument('--mpi',
                         type=int,
                         metavar='N',
                         help='number of MPI processes used to run the model (default=1)',
                         default=1)
```

### Comparing `struphy-1.9.9/src/struphy/examples/maxwell.py` & `struphy-2.0.0/src/struphy/examples/maxwell.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,36 +40,36 @@
     
     from struphy.diagnostics.diagn_tools import fourier_1d
     
     import struphy
 
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     # output path
     out_name = 'sim_example_maxwell'
-    out_path = os.path.join(libpath, 'io/out', out_name) 
+    out_path = os.path.join(io_path, 'io/out', out_name) 
     
     # code name
     with open(os.path.join(out_path, 'meta.txt'), 'r') as f:
         lines = f.readlines()
 
-    code = lines[-2].split()[-1]
+    code = lines[3].split()[-1]
 
     # field names
-    file = h5py.File(os.path.join(out_path, 'data_proc0.hdf5'), 'r')
+    file = h5py.File(os.path.join(out_path,'data/', 'data_proc0.hdf5'), 'r')
     names = list(file['feec'].keys())
     file.close()
 
     # load data dicts for e_field
-    with open(os.path.join(out_path, 'post_processing/fields_data', names[1] + '_log.bin'), 'rb') as handle:
+    with open(os.path.join(out_path, 'post_processing/fields_data/em_fields/e1_log.bin'), 'rb') as handle:
         point_data_log = pickle.load(handle)
 
-    with open(os.path.join(out_path, 'post_processing/fields_data', names[1] + '_phy.bin'), 'rb') as handle:
-        point_data_phy = pickle.load(handle)
-
     # load grids
     with open(os.path.join(out_path, 'post_processing/fields_data/grids_log.bin'), 'rb') as handle:
         grids_log = pickle.load(handle)
 
     with open(os.path.join(out_path, 'post_processing/fields_data/grids_phy.bin'), 'rb') as handle:
         grids_phy = pickle.load(handle)
```

### Comparing `struphy-1.9.9/src/struphy/examples/orbits_tokamak.py` & `struphy-2.0.0/src/struphy/examples/orbits_tokamak.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,28 +44,31 @@
     
     from struphy.models.utilities import setup_domain_mhd
     from struphy.fields_background.mhd_equil.equils import EQDSKequilibrium
     
     import struphy
     libpath = struphy.__path__[0]
     
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
+    
     # output path
     out_name = 'sim_example_orbits_tokamak'
-    out_path = os.path.join(libpath, 'io/out', out_name)
+    out_path = os.path.join(io_path, 'io/out', out_name)
     
     # load simulation parameters
     with open(os.path.join(out_path, 'parameters.yml')) as file:
         params = yaml.load(file, Loader=yaml.FullLoader)
 
     # create domain and MHD equilibrium
     domain, mhd_equil = setup_domain_mhd(params)
     domain_name = domain.__class__.__name__
     
     # load grid_info (domain decomposition)
-    file = h5py.File(os.path.join(out_path, 'data_proc0.hdf5'), 'r')
+    file = h5py.File(os.path.join(out_path, 'data/', 'data_proc0.hdf5'), 'r')
     grid_info = file['scalar'].attrs['grid_info']
     file.close()
 
     # load time grid info
     tgrid = np.load(os.path.join(out_path, 'post_processing/t_grid.npy'))
     Nt = len(tgrid) - 1
```

### Comparing `struphy-1.9.9/src/struphy/fields_background/electric_equil/analytical.py` & `struphy-2.0.0/src/struphy/fields_background/electric_equil/analytical.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/electric_equil/base.py` & `struphy-2.0.0/src/struphy/fields_background/electric_equil/base.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/base.py` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         return self.domain.pull(self.unit_b_cart(*etas, squeeze_out=False)[0], *etas, kind='1_form', squeeze_out=squeeze_out)
 
     def unit_b2(self, *etas, squeeze_out=True):
         """ Unit vector components of equilibrium magnetic field (2-form) on logical cube [0, 1]^3.
         """
         return self.domain.pull(self.unit_b_cart(*etas, squeeze_out=False)[0], *etas, kind='2_form', squeeze_out=squeeze_out)
     
-    def unit_bv(self, *etas, squeeze_out=False):
+    def unit_bv(self, *etas, squeeze_out=True):
         """ Unit vector components of  equilibrium magnetic field (contra-variant) on logical cube [0, 1]^3.
         """
         return self.domain.pull(self.unit_b_cart(*etas, squeeze_out=False)[0], *etas, kind='vector', squeeze_out=squeeze_out)
     
     def unit_b_cart(self, *etas, squeeze_out=True):
         """ Unit vector Cartesian components of equilibrium magnetic field evaluated on logical cube [0, 1]^3. Returns also (x,y,z).
         """
@@ -84,30 +84,32 @@
         """
         j_out = self.domain.push(self.j2(*etas, squeeze_out=False), *etas, kind='2_form', a_kwargs={'squeeze_out' : False}, squeeze_out=squeeze_out)
         return j_out, self.domain(*etas)
 
     def p0(self, *etas, squeeze_out=True):
         """ 0-form equilibrium pressure on logical cube [0, 1]^3.
         """
-        return self.domain.pull([self.p_xyz], *etas, kind='0_form', squeeze_out=squeeze_out)
+        xyz = self.domain(*etas, squeeze_out=False)
+        return self.domain.pull(self.p_xyz(xyz[0], xyz[1], xyz[2]), *etas, kind='0_form', squeeze_out=squeeze_out)
 
     def p3(self, *etas, squeeze_out=True):
         """ 3-form equilibrium pressure on logical cube [0, 1]^3.
         """
-        return self.domain.transform([self.p0], *etas, kind='0_to_3', a_kwargs={'squeeze_out' : False}, squeeze_out=squeeze_out)
+        return self.domain.transform(self.p0(*etas, squeeze_out=False), *etas, kind='0_to_3', a_kwargs={'squeeze_out' : False}, squeeze_out=squeeze_out)
 
     def n0(self, *etas, squeeze_out=True):
         """ 0-form equilibrium number density on logical cube [0, 1]^3.
         """
-        return self.domain.pull([self.n_xyz], *etas, kind='0_form', squeeze_out=squeeze_out)
+        xyz = self.domain(*etas, squeeze_out=False)
+        return self.domain.pull(self.n_xyz(xyz[0], xyz[1], xyz[2]), *etas, kind='0_form', squeeze_out=squeeze_out)
 
     def n3(self, *etas, squeeze_out=True):
         """ 3-form equilibrium number density on logical cube [0, 1]^3.
         """
-        return self.domain.transform([self.n0], *etas, kind='0_to_3', a_kwargs={'squeeze_out' : False}, squeeze_out=squeeze_out)
+        return self.domain.transform(self.n0(*etas, squeeze_out=False), *etas, kind='0_to_3', a_kwargs={'squeeze_out' : False}, squeeze_out=squeeze_out)
 
     ###################
     # Single components
     ###################
 
     def b1_1(self, *etas, squeeze_out=True):
         return self.b1(*etas, squeeze_out=squeeze_out)[0]
@@ -481,76 +483,44 @@
         """
         pass
     
     def b_xyz(self, x, y, z):
         """ Cartesian B-field components calculated as BR = -(dpsi/dZ)/R, BPhi = g_tor/R, BZ = (dpsi/dR)/R.
         """
         
-        from struphy.geometry.base import Domain
-        
-        # check for point-wise evaluation and broadcast input to 3d numpy arrays.
-        is_float = all(isinstance(v, (int, float)) for v in [x, y, z])
-        
-        # x, y, z, is_sparse_meshgrid = Domain.prepare_eval_pts(x, y, z)
-        
         R, Phi, Z = self.inverse_map(x, y, z)
         
         # at phi = 0°
         BR = -self.psi(R, Z, dZ=1)/R
         BP = self.g_tor(R, Z)/R
         BZ =  self.psi(R, Z, dR=1)/R
         
         # push-forward to Cartesian components
         Bx = BR*np.cos(Phi) - BP*np.sin(Phi)
         By = BR*np.sin(Phi) + BP*np.cos(Phi)
         Bz = 1*BZ
-        
-        # remove all "dimensions" for point-wise evaluation
-        if is_float:
-            assert Bx.ndim == 3
-            assert By.ndim == 3
-            assert Bz.ndim == 3
-            Bx = Bx.item()
-            By = By.item()
-            Bz = Bz.item()
 
         return Bx, By, Bz
 
     def j_xyz(self, x, y, z):
         """ Cartesian current density components calculated as curl(B).
         """
         
-        from struphy.geometry.base import Domain
-        
-        # check for point-wise evaluation and broadcast input to 3d numpy arrays.
-        is_float = all(isinstance(v, (int, float)) for v in [x, y, z])
-        
-        # x, y, z, is_sparse_meshgrid = Domain.prepare_eval_pts(x, y, z)
-        
         R, Phi, Z = self.inverse_map(x, y, z)
         
         # at phi = 0° (j = curl(B))
         jR = -self.g_tor(R, Z, dZ=1)/R
         jP = -self.psi(R, Z, dZ=2)/R + self.psi(R, Z, dR=1)/R**2 - self.psi(R, Z, dR=2)/R
         jZ =  self.g_tor(R, Z, dR=1)/R
         
         # push-forward to Cartesian components
         jx = jR*np.cos(Phi) - jP*np.sin(Phi)
         jy = jR*np.sin(Phi) + jP*np.cos(Phi)
         jz = 1*jZ
 
-        # remove all "dimensions" for point-wise evaluation
-        if is_float:
-            assert jx.ndim == 3
-            assert jy.ndim == 3
-            assert jz.ndim == 3
-            jx = jx.item()
-            jy = jy.item()
-            jz = jz.item()
-
         return jx, jy, jz
     
     @staticmethod
     def inverse_map(x, y, z):
         """ Inverse cylindrical mapping.
         """
```

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/eqdsk/data/AUGNLED_g031213.00830.high` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/data/AUGNLED_g031213.00830.high`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/eqdsk/readeqdsk.py` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/eqdsk/readeqdsk.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E1D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/newBC_E4D6_M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini` & `struphy-2.0.0/src/struphy/fields_background/mhd_equil/gvec/ellipstell_v2/oldBC_E40D5M6N6/parameter.ini`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/geometry/base.py` & `struphy-2.0.0/src/struphy/geometry/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1338,15 +1338,15 @@
 
         # plot control points in case of IGA mappings
         if not logical and self.kind_map < 10 and show_control_pts:
             if self.__class__.__name__ == 'GVECunit':
                 Yc = self.cz[:, :, 0].flatten()
             else:
                 Yc = self.cy[:, :, 0].flatten()
-            ax.scatter(self.cx[:, :, 0].flatten(), Yc, s=3, color='b')
+            ax.scatter(self.cx[:, :, 0].flatten(), Yc, s=1, color='b')
              
         # plot given markers
         if markers is not None:
             
             assert not (logical and marker_coords != 'logical')
             
             if 'Torus' in self.__class__.__name__ or self.__class__.__name__ == 'GVECunit' or self.__class__.__name__ == 'Tokamak':
@@ -1392,15 +1392,15 @@
             ylab = 'z'
         else:
             ylab = 'y'
         ax.set_xlabel('x')
         ax.set_ylabel(ylab)
 
         if save_dir is not None:
-            plt.savefig(save_dir)
+            plt.savefig(save_dir, bbox_inches='tight')
         else:
             plt.show()
 
 
 class Spline(Domain):
     r'''
     .. math::
```

### Comparing `struphy-1.9.9/src/struphy/geometry/domains.py` & `struphy-2.0.0/src/struphy/geometry/domains.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from struphy.geometry.base import Domain, Spline, PoloidalSplineStraight, PoloidalSplineTorus
 from struphy.geometry.utilities import field_line_tracing
 import numpy as np
 
 
 class Tokamak(PoloidalSplineTorus):
-    '''Mappings for Tokamak MHD equilibria constructed via field line tracing of a poloidal flux function.'''
+    '''Mappings for Tokamak MHD equilibria constructed via field line tracing of a poloidal flux function.
+    
+    .. image:: ../pics/mappings/tokamak.png'''
     
     def __init__(self, **params):
         
         from struphy.fields_background.mhd_equil.base import AxisymmMHDequilibrium
         from struphy.fields_background.mhd_equil.equils import EQDSKequilibrium
         
         # set default
@@ -74,44 +76,19 @@
         # init base class
         super().__init__(**params_map)
         
         self._params_map['equilibrium'] = equilibrium
         self._params_map['psi_power'] = psi_power
         self._params_map['psi_shifts'] = psi_shifts
         self._params_map['xi_param'] = xi_param
+        self._params_map['r0'] = r0
         self._params_map['Nel_pre'] = Nel_pre
         self._params_map['p_pre'] = p_pre
 
 
-class EQDSKTorus(PoloidalSplineTorus):
-    '''Mappings constructed via field line tracing from EQDSK data.
-    
-    .. image:: ../pics/mappings/eqdsk_raw.png
-
-    |
-
-    .. image:: ../pics/mappings/eqdsk.png'''
-
-    def __init__(self, **params):
-
-        from struphy.fields_background.mhd_equil.equils import EQDSKequilibriumWithDomain
-
-        eqdsk = EQDSKequilibriumWithDomain(**params)
-
-        new_params = {}
-        new_params['cx'] = eqdsk.domain.cx[:, :, 0].squeeze()
-        new_params['cy'] = eqdsk.domain.cy[:, :, 0].squeeze()
-        new_params['Nel'] = eqdsk.domain.params_map['Nel']
-        new_params['p'] = eqdsk.domain.params_map['p']
-        new_params['spl_kind'] = eqdsk.domain.params_map['spl_kind']
-        new_params['tor_period'] = eqdsk.domain.params_map['tor_period']
-
-        super().__init__(**new_params)
-
-
 class GVECunit(Spline):
     '''The mapping "f_unit" from `gvec_to_python <https://gitlab.mpcdf.mpg.de/spossann/gvec_to_python>`_, 
     computed by the GVEC MHD equilibirum code.
     
     .. image:: ../pics/mappings/gvec.png'''
 
     def __init__(self, **params):
```

### Comparing `struphy-1.9.9/src/struphy/geometry/kernels.py` & `struphy-2.0.0/src/struphy/geometry/kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/geometry/mappings_fast.py` & `struphy-2.0.0/src/struphy/geometry/mappings_fast.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/geometry/transform.py` & `struphy-2.0.0/src/struphy/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/geometry/utilities.py` & `struphy-2.0.0/src/struphy/geometry/utilities.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/initial/analytic.py` & `struphy-2.0.0/src/struphy/initial/analytic.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/initial/base.py` & `struphy-2.0.0/src/struphy/initial/base.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/initial/eigenfunctions.py` & `struphy-2.0.0/src/struphy/initial/eigenfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,26 +30,29 @@
     """
     
     def __init__(self, derham, **params):
         
         import struphy
         libpath = struphy.__path__[0]
         
+        with open(os.path.join(libpath, 'io_path.txt')) as f:
+            io_path = f.readlines()[0]
+        
         params_default = {'spec': 'sim_1/spec_n_-1.npy',
                           'spec_abs': None,
                           'eig_freq_upper': 0.02, 
                           'eig_freq_lower': 0.03,
                           'kind': 'r',
                           'scaling': 1.}
         
         params = set_defaults(params, params_default)
         
         # absolute path of spectrum
         if params['spec_abs'] is None:
-            spec_path = os.path.join(libpath, 'io/out', params['spec'])
+            spec_path = os.path.join(io_path, 'io/out', params['spec'])
         else:
             spec_path = params['spec_abs']
         
         # load eigenvector for velocity field
         omega2, U2_eig = np.split(np.load(spec_path), [1], axis=0)
         omega2 = omega2.flatten()
```

### Comparing `struphy-1.9.9/src/struphy/initial/initialize.py` & `struphy-2.0.0/src/struphy/initial/initialize.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/initial/perturbations.py` & `struphy-2.0.0/src/struphy/initial/perturbations.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/batch/batch_cobra.sh` & `struphy-2.0.0/src/struphy/io/batch/batch_cobra.sh`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/batch/p_016.sh` & `struphy-2.0.0/src/struphy/io/batch/p_016.sh`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/batch/p_032.sh` & `struphy-2.0.0/src/struphy/io/batch/p_032.sh`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/batch/p_064.sh` & `struphy-2.0.0/src/struphy/io/batch/p_064.sh`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/batch/p_128.sh` & `struphy-2.0.0/src/struphy/io/batch/p_128.sh`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/batch/p_256.sh` & `struphy-2.0.0/src/struphy/io/batch/p_256.sh`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/batch/p_512.sh` & `struphy-2.0.0/src/struphy/io/batch/p_512.sh`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_TAE_tokamak.yml` & `struphy-2.0.0/src/struphy/io/inp/examples/params_TAE_tokamak.yml`

 * *Files 10% similar despite different names*

```diff
@@ -25,26 +25,29 @@
         a2       : 1.0 # minor radius
         R0       : 5.0 # major radius
         tor_period : 2 # toroidal periodicity built into the mapping: phi = 2*pi * eta3 / tor_period
             
 mhd_equilibrium : 
     type : AdhocTorus # (possible choices seen below)
     AdhocTorus :
-        a      : 1. # minor radius
-        R0     : 5. # major radius
-        B0     : 5. # on-axis toroidal magnetic field
-        q0     : 1.15 # safety factor at r=0
-        q1     : 1.60 # safety factor at r=a
-        n1     : 0. # shape factor for number density profile 
-        n2     : 0. # shape factor for number density profile 
-        na     : 1. # number density at r=a
-        p_kind : 1 # kind of pressure profile (0 : cylindrical limit, 1 : ad hoc)
-        p1     : 0. # shape factor for ad hoc pressure profile
-        p2     : 0. # shape factor for ad hoc pressure profile
-        beta   : .2 # plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)   
+        a       : 1. # minor radius
+        R0      : 5. # major radius
+        B0      : 5. # on-axis toroidal magnetic field
+        q_kind  : 0 # which profile (0 : parabolic, 1 : other, see documentation)
+        q0      : 1.15 # safety factor at r=0
+        q1      : 1.60 # safety factor at r=a
+        n1      : 0. # shape factor for number density profile 
+        n2      : 0. # shape factor for number density profile 
+        na      : 1. # number density at r=a
+        p_kind  : 1 # kind of pressure profile (0 : cylindrical limit, 1 : ad hoc)
+        p1      : 0. # shape factor for ad hoc pressure profile
+        p2      : 0. # shape factor for ad hoc pressure profile
+        beta    : .2 # plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)
+        psi_k   : 3 # spline degree to be used for interpolation of poloidal flux function (only needed if q_kind = 1)
+        psi_nel : 50 # number of cells to be used for interpolation of poloidal flux function (only needed if q_kind = 1)
         
 em_fields : 
     init :
         type : InitialMHDAxisymHdivEigFun # initial conditions (possible types seen below)
         InitialMHDAxisymHdivEigFun :
             spec : 'sim_example_TAE_tokamak/spec_0.1_0.2_n_-1.npy' # relative path (to <install_path>/io/out/) of the .npy spectrum
             spec_abs : null # absolute path of .npy spectrum (is used instead of "spec", if "spec_abs" is not null)
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml` & `struphy-2.0.0/src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     dt         : 0.2  # time step
     Tend       : 100. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Tokamak # mapping F (possible types seen below)
     Tokamak :
-        Nel        : [32, 72] # number of poloidal grid cells, >p
+        Nel        : [28, 72] # number of poloidal grid cells, >p
         p          : [3, 3] # poloidal spline degrees, >1
         psi_power  : 0.6 # parametrization of radial flux coordinate eta1=psi_norm^psi_power, where psi_norm is normalized flux
         psi_shifts : [0., 1.] # start and end shifts of polidal flux in % --> cuts away regions at the axis and edge
         xi_param   : equal_angle # parametrization of angular coordinate (equal_angle, equal_arc_length or sfl (straight field line))
         r0         : 0.3 # initial guess for radial distance from axis used in Newton root-finding method for flux surfaces
         Nel_pre    : [64, 256] # number of poloidal grid cells of pre-mapping needed for equal_arc_length and sfl
         p_pre      : [3, 3] # poloidal spline degrees of pre-mapping needed for equal_arc_length and sfl
@@ -62,15 +62,15 @@
                 seed    : 1608 # seed for random number generator
                 moments : [0., 0., 1., 1.] # moments of Gaussian s3, see background/moms_spec
                 initial : [[.501, 0.001, 0.001,  1.935 , -1.72], # counter-passing particle
                            [.501, 0.001, 0.001, -1.935 , -1.72], # co-passing particle
                            [.501, 0.001, 0.001,  0.4515, -1.72], # counter-trapped particle
                            [.501, 0.001, 0.001, -0.6665, -1.72]] # co-trapped particle
 
-        init : 
+        init :
             type : Maxwellian5DUniform
             Maxwellian5DUniform:
                 n : 0.05
         save_data :
             n_markers : 4 # number of markers to be save during simulation
         push_algos :
             integrator : implicit # explicit or implicit
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml` & `struphy-2.0.0/src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml`

 * *Files 1% similar despite different names*

```diff
@@ -84,19 +84,19 @@
                 type    : pseudo_random # particle loading mechanism
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
-                uz : 2.5
+                u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
             f :
-                slices : [vz] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
+                slices : [v3] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
                 n_bins : [[32]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
                 ranges : [[[-0.5, 5.5]]] # bin range in each direction
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
 
 solvers :
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml` & `struphy-2.0.0/src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml`

 * *Files 1% similar despite different names*

```diff
@@ -84,19 +84,19 @@
                 type    : pseudo_random # particle loading mechanism
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
-                uz : 2.5
+                u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
             f :
-                slices : [vz] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
+                slices : [v3] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
                 n_bins : [[32]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
                 ranges : [[[-0.5, 5.5]]] # bin range in each direction
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
         use_perp_model : True # for pressure coupling
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_linearmhd.yml` & `struphy-2.0.0/src/struphy/io/inp/examples/params_linearmhd.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_linvlasovmaxwell.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_linvlasovmaxwell.yml`

 * *Files 26% similar despite different names*

```diff
@@ -4,26 +4,22 @@
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [2, 2, 2] # quadrature points per grid cell
     nq_pr    : [2, 2, 2] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
-model_units :
-    B   : 1. # magnetic field unit in T
-    L   : 1. # length scale unit in m
-    nb  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
-    nuh : 5. # ratio of hot/bulk number density units in %
-    Ab  : 1 # mass number of bulk ion species
-    Ah  : 1 # mass number of energetic ion species
-    Zh  : 1 # charge number of energetic ion species
+units :
+    x : 1. # length scale unit in m
+    B : 1. # magnetic field unit in T
+    n : 1. # number density unit of fluid species in 1 x 10^20 m^(-3)
 
 time :
-    dt         : 0.01 # time step
-    Tend       : 5. # simulation time interval is [0, Tend]
+    dt         : 0.05 # time step
+    Tend       : 0.5 # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
         l1       : 0. # start of interval in eta1
         r1       : 2. # end of interval in eta1, r1>l1
@@ -31,132 +27,102 @@
         r2       : 2. # end of interval in eta2, r2>l2
         l3       : 0. # start of interval in eta3
         r3       : 20. # end of interval in eta3, r3>l3
 
 mhd_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
-        B0x  : 0.5 # magnetic field in x
+        B0x  : 0. # magnetic field in x
         B0y  : 0. # magnetic field in y
-        B0z  : 1.4 # magnetic field in z
+        B0z  : 1. # magnetic field in z
         beta : 0. # plasma beta = 2*p*mu_0/B^2
         n0   : 1. # number density
 
 electric_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         phi0  : 1. # constant electric potential
 
 em_fields :
     init :
-        type : ModesSin # initial conditions (possible types seen below)
+        type : noise # initial conditions (possible types seen below)
         noise :
             comps :
                 e_field : [True, False, False]  # components to be initialized (for scalar fields: no list)
-                b_field : [False, False, False] # components to be initialized (for scalar fields: no list)
+                b_field : [False, True, True] # components to be initialized (for scalar fields: no list)
             variation_in : e3 # noise variation (logical space): e1, e2, e3 (1d), e1e2, e1e3, e2e3 (2d), e1e2e3 (3d)
             amp : 0.1   # noise amplitude
-        ModesSin : 
-            coords : 'logical' # in which coordinates (logical or physical)
-            comps :
-                e_field : [True, False, False]  # components to be initialized (for scalar fields: no list)
-                b_field : [False, False, False] # components to be initialized (for scalar fields: no list)
-            ls : [0] # Integer mode numbers in x or eta_1 (depending on coords)
-            ms : [0] # Integer mode numbers in y or eta_2 (depending on coords)
-            ns : [1] # Integer mode numbers in z or eta_3 (depending on coords)
-            amp : [2.1] # amplitudes of each mode
-        ModesCos :
-            coords : 'logical' # in which coordinates (logical or physical)
-            comps :
-                e_field : [True, False, False]  # components to be initialized (for scalar fields: no list)
-                b_field : [False, False, False] # components to be initialized (for scalar fields: no list)
-            ls : [0] # Integer mode numbers in x or eta_1 (depending on coords)
-            ms : [0] # Integer mode numbers in y or eta_2 (depending on coords)
-            ns : [1] # Integer mode numbers in z or eta_3 (depending on coords)
-            amp : [0.001] # amplitudes of each mode
-        TorusModesSin :
-            coords : 'logical' # in which coordinates (logical or physical)
-            comps :
-                e_field : [True, False, False]  # components to be initialized (for scalar fields: no list)
-                b_field : [False, False, False] # components to be initialized (for scalar fields: no list)
-            ms : [1] # poloidal mode numbers
-            ns : [0] # toroidal mode numbers
-            amp : [0.001] # amplitudes of each mode
-            pfuns : ['sin'] # profile function in eta1-direction ('sin' or 'exp')
-            pfun_params : [null] # Provides [r_0, sigma] parameters for each "exp" profile fucntion, and null for "sin"
-        InitialMHDSlab :
-            a  : 1. # minor radius (Lx=a, Ly=2*pi*a)
-            R0 : 3. # major radius (Lz=2*pi*R0)
-            m  : 0  # poloidal (y) mode number
-            n  : 1  # toroidal (z) mode number
-            U  : 0.1 # amplitude of Ux/Uy
-            A  : 0. # amplitude of Uz
-        InitialMHDAxisymHdivEigFun :
-            spec : '/path_to_spec/spec.npy' # relative path (to <install_path/struphy>) of the .npy spectrum
-            eig_freq_upper : 0.15 # upper search limit of squared eigenfrequency to identify eigenfunction
-            eig_freq_lower : 0.14 # lower search limit of squared eigenfrequency to identify eigenfunction
-            kind : r # real (r) or imaginary (i) part of eigenfunction
-            scaling : 1. # scaling factor to scale the amplitude of the eigenfunction
 
 kinetic :
     electrons :
+        phys_params:
+            A : 0.0005446170214876324  # electron mass number in units of proton mass
+            Z : -1 # signed charge number in units of elementary charge
         markers :
             type    : delta_f # full_f, control_variate, or delta_f
-            Np      : 50000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
-            eps     : 0.5 # MPI send/receive buffer (0.1 <= eps <= 1.0)
+            ppc     : 10  # number of markers per 3d grid cell
+            Np      : 3 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
+            eps     : .5 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # remove, reflect or periodic
             loading :
                 type          : pseudo_random # particle loading mechanism
                 seed          : 1234 # seed for random number generator
                 dir_particles : path_to_particles # directory of particles if loaded externally
-                moments       : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                moments       : [0., 0., 0., 0.1, 0.1, 0.1] # moments of Gaussian s3, see background/moms_spec
         init :
             type : Maxwellian6DPerturbed
             Maxwellian6DPerturbed :
                 n :
-                    n0 : 0.
+                    n0 : 0.2
                     perturbation :
-                        l : [0.07957747154594767] # 0.5 / (2 * pi)
+                        l : [1]
                         m : [0]
                         n : [0]
                         amps_sin : [0.]
-                        amps_cos : [1.5]
-                ux :
-                    ux0 : 0.
-                uy :
-                    uy0 : 0.
-                uz :
-                    uz0 : 0.
-                vthx :
-                    vthx0 : 1.
-                vthy :
-                    vthy0 : 1.
-                vthy :
-                    vthz0 : 1.
+                        amps_cos : [0.05]
+                u1 :
+                    u01 : 0.1
+                u2 :
+                    u02 : 0.1
+                u3 :
+                    u03 : 0.1
+                vth1 :
+                    vth01 : 0.1
+                vth2 :
+                    vth02 : 0.1
+                vth3 :
+                    vth03 : 0.1
         background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
-                n  : 1.
-                ux : 0.
-                uy : 0.
-                uz : 0.
-                vthx : 1.
-                vthy : 1.
-                vthz : 1.
+                n  : 0.2
+                u1 : 0.1
+                u2 : 0.1
+                u3 : 0.1
+                vth1 : 0.1
+                vth2 : 0.1
+                vth3 : 0.1
         save_data :
-            n_markers : 10 # number of markers to be saved during simulation
+            n_markers : 3 # number of markers to be save during simulation
             f :
-                slices : [e3, vx_vy_vz] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
-                n_bins : [[64], [64, 64, 64]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
-                ranges : [[[0., 1.]], [[-5., 5.], [-5., 5.], [-5., 5.]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
+                slices : [v3] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
+                n_bins : [[32]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
+                ranges : [[[-10., 10.]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
 
 solvers :
+    solver_poisson :
+        type : PConjugateGradient
+        pc : null # MassMatrixPreconditioner # null or name of preconditioner class
+        tol : 1.e-10
+        maxiter : 3000
+        info : False
+        verbose : False
     solver_ew :
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-10
         maxiter : 3000
         info : False
         verbose : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_deltafvlasovmaxwell.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 grid :
-    Nel      : [2, 2, 64] # number of grid cells, >p
-    p        : [1, 1, 3]  # spline degree
+    Nel      : [64, 2, 2] # number of grid cells, >p
+    p        : [3, 1, 1]  # spline degree
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [2, 2, 2] # quadrature points per grid cell
     nq_pr    : [2, 2, 2] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
-model_units :
-    x   : 1. # length scale unit in m
+units :
+    x   : 0.0017045090240267625 # c * m_e / e
     B   : 1. # magnetic field unit in T
-    nb  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
-    nuh : 5. # ratio of hot/bulk number density units in %
-    Ab  : 1 # mass number of bulk ion species (1 : Hydrogen, 2 : Deuterium, 3 : Tritium, etc.)
-    Ah  : 1 # mass number of energetic ion species (1 : Hydrogen, 2 : Deuterium, 3 : Tritium, etc.)
-    Zh  : 1 # charge number of energetic ion species (1 : Hydrogen, 2 : Helium, etc.)
+    n   : 0.09719853837468743 # eps_0 / m_e / 1e20 # bulk number density unit in 1 x 10^20 m^(-3)
 
 time :
     dt         : 0.01 # time step
-    Tend       : 30. # simulation time interval is [0, Tend]
+    Tend       : 0.1 # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
         l1       : 0. # start of interval in eta1
-        r1       : 2. # end of interval in eta1, r1>l1
+        r1       : 1. # end of interval in eta1, r1>l1
         l2       : 0. # start of interval in eta2
-        r2       : 2. # end of interval in eta2, r2>l2
+        r2       : 1. # end of interval in eta2, r2>l2
         l3       : 0. # start of interval in eta3
-        r3       : 20. # end of interval in eta3, r3>l3
+        r3       : 1. # end of interval in eta3, r3>l3
 
 mhd_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         B0x  : 0.5 # magnetic field in x
         B0y  : 0. # magnetic field in y
         B0z  : 1.4 # magnetic field in z
@@ -44,73 +40,85 @@
 electric_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         phi0  : 1. # constant electric potential
 
 em_fields :
     init :
-        type : null # initial conditions (possible types seen below)
+        type : ModesSin
+        ModesSin : 
+            coords : 'logical' # in which coordinates (logical or physical)
+            comps :
+                e_field : [False, False, False]  # components to be initialized
+                b_field : [False, False, True] # components to be initialized
+            ls : [1] # Integer mode numbers in x or eta_1 (depending on coords)
+            ms : [0] # Integer mode numbers in y or eta_2 (depending on coords)
+            ns : [0] # Integer mode numbers in z or eta_3 (depending on coords)
+            amp : [0.01] # amplitudes of each mode
 
 kinetic :
     electrons :
+        phys_params:
+            A : 0.0005446170214876324  # electron mass number in units of proton mass
+            Z : -1 # signed charge number in units of elementary charge
         markers :
             type    : delta_f # full_f, control_variate, or delta_f
-            Np      : 5000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
-            eps     : 0.5 # MPI send/receive buffer (0.1 <= eps <= 1.0)
+            Np      : 10000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
+            eps     : 0.25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
             bc_type : [periodic, periodic, periodic] # remove, reflect or periodic
             loading :
                 type          : pseudo_random # particle loading mechanism
                 seed          : 1234 # seed for random number generator
                 dir_particles : path_to_particles # directory of particles if loaded externally
-                moments       : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                moments       : [0., 0., 0., 0.1, 0.1, 0.1] # moments of Gaussian s3, see background/moms_spec
         init :
             type : Maxwellian6DPerturbed
             Maxwellian6DPerturbed :
                 n :
                     n0 : 0.
-                    perturbation :
-                        # l : [0.07957747154594767] # 0.5 / (2 * pi)
-                        l : [5]
-                        m : [0]
-                        n : [0]
-                        amps_sin : [0.]
-                        amps_cos : [0.5]
-                ux :
-                    ux0 : 0.
-                uy :
-                    uy0 : 0.
-                uz :
-                    uz0 : 0.
-                vthx :
-                    vthx0 : 2.
-                vthy :
-                    vthy0 : 2.
-                vthy :
-                    vthz0 : 2.
+                u1 :
+                    u01 : 0.
+                u2 :
+                    u02 : 0.
+                u3 :
+                    u03 : 0.
+                vth1 :
+                    vth01 : 0.5
+                vth2 :
+                    vth02 : 0.5
+                vth3 :
+                    vth03 : 0.5
         background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 1.
-                ux : 0.
-                uy : 0.
-                uz : 0.
-                vthx : 2.
-                vthy : 2.
-                vthz : 2.
+                u1 : 0.
+                u2 : 0.
+                u3 : 0.
+                vth1 : 0.5
+                vth2 : 0.5
+                vth3 : 0.5
         save_data :
             n_markers : 10 # number of markers to be saved during simulation
             f :
-                slices : [e3, vx_vy] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
+                slices : [e3, v1_v2] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
                 n_bins : [[64], [64, 64]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
                 ranges : [[[0., 1.]], [[-5., 5.], [-5., 5.]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
 
 solvers :
+    solver_poisson :
+        type : PConjugateGradient
+        pc : null # MassMatrixPreconditioner # null or name of preconditioner class
+        tol : 1.e-10
+        maxiter : 3000
+        info : False
+        verbose : False
     solver_ew :
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-10
         maxiter : 3000
         info : False
         verbose : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_linvlasovmaxwell_weibel.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,125 +1,124 @@
 grid :
-    Nel      : [2, 2, 64] # number of grid cells, >p
-    p        : [1, 1, 3]  # spline degree
+    Nel      : [3, 3, 10] # number of grid cells, >p
+    p        : [2, 2, 3]  # spline degree
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
-    nq_el    : [2, 2, 2] # quadrature points per grid cell
-    nq_pr    : [2, 2, 2] # quadrature points per histopolation cell (for commuting projectors)
+    nq_el    : [6, 6, 6] # quadrature points per grid cell
+    nq_pr    : [6, 6, 6] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
-model_units :
-    x   : 1. # length scale unit in m
-    B   : 1. # magnetic field unit in T
-    nb  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
-    nuh : 5. # ratio of hot/bulk number density units in %
-    Ab  : 1 # mass number of bulk ion species (1 : Hydrogen, 2 : Deuterium, 3 : Tritium, etc.)
-    Ah  : 1 # mass number of energetic ion species (1 : Hydrogen, 2 : Deuterium, 3 : Tritium, etc.)
-    Zh  : 1 # charge number of energetic ion species (1 : Hydrogen, 2 : Helium, etc.)
-
-time :
-    dt         : 0.01 # time step
-    Tend       : 5. # simulation time interval is [0, Tend]
+units :
+    x  : 1. # length scale unit in m
+    B  : 1. # magnetic field unit in T
+    n  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
+
+time : 
+    dt         : 0.1  # time step
+    Tend       : .5 # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
-        l1       : 0. # start of interval in eta1
-        r1       : 2. # end of interval in eta1, r1>l1
-        l2       : 0. # start of interval in eta2
-        r2       : 2. # end of interval in eta2, r2>l2
-        l3       : 0. # start of interval in eta3
-        r3       : 20. # end of interval in eta3, r3>l3
+        l1 : 0. # start of interval in eta1
+        r1 : 1. # end of interval in eta1, r1>l1
+        l2 : 0. # start of interval in eta2
+        r2 : 1. # end of interval in eta2, r2>l2
+        l3 : 0. # start of interval in eta3
+        r3 : 10. # end of interval in eta3, r3>l3 
 
 mhd_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
-        B0x  : 0.5 # magnetic field in x
+        B0x  : 0. # magnetic field in x
         B0y  : 0. # magnetic field in y
-        B0z  : 1.4 # magnetic field in z
+        B0z  : 1. # magnetic field in z
         beta : 0. # plasma beta = 2*p*mu_0/B^2
         n0   : 1. # number density
 
-electric_equilibrium :
-    type : HomogenSlab # (possible choices seen below)
-    HomogenSlab :
-        phi0  : 1. # constant electric potential
-
 em_fields :
     init :
-        type : ModesCos # initial conditions (possible types seen below)
-        ModesCos :
-            coords : 'logical' # in which coordinates (logical or physical)
-            comps :
-                e_field : [False, False, False]  # components to be initialized (for scalar fields: no list)
-                b_field : [False, True, False] # components to be initialized (for scalar fields: no list)
-            ls : [1.25] # Mode numbers in x or eta_1 (depending on coords)
-            ms : [0] # Mode numbers in y or eta_2 (depending on coords)
-            ns : [0] # Mode numbers in z or eta_3 (depending on coords)
-            amp : [-0.1] # amplitudes of each mode
+        type : null # initial conditions (possible types seen below)
+
+fluid :
+    mhd :
+        phys_params:
+            A : 1 # mass number in units of proton mass
+            Z : 1 # signed charge number in units of elementary charge
+        mhd_u_space : H1vec # Hdiv | H1vec
+        init :
+            type : null # type of initialization
+            ModesCos :
+                coords : 'physical' # in which coordinates (logical or physical)
+                comps :
+                    n3 : False                # components to be initialized (for scalar fields: no list)
+                    uv : [False, True, False] # components to be initialized (for scalar fields: no list)
+                    p3 : False                # components to be initialized (for scalar fields: no list)
+                ls : [0] # Integer mode numbers in x or eta_1 (depending on coords)
+                ms : [0] # Integer mode numbers in y or eta_2 (depending on coords)
+                ns : [-1] # Integer mode numbers in z or eta_3 (depending on coords)
+                amp : [0.0001] # amplitudes of each mode
+                Lx : 1.
+                Ly : 1.
+                Lz : 10.
+            InitialMHDSlab :
+                a  : 1.
+                R0 : 1.
+                m  : 0
+                n  : -1
+                U  : 0.001
+                A  : 0.
 
 kinetic :
-    electrons :
+    energetic_ions :
+        phys_params:
+            A : 1 # mass number in units of proton mass
+            Z : 1 # signed charge number in units of elementary charge
         markers :
-            type    : delta_f # full_f, control_variate, or delta_f
-            Np      : 5000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
-            eps     : 0.5 # MPI send/receive buffer (0.1 <= eps <= 1.0)
-            bc_type : [periodic, periodic, periodic] # remove, reflect or periodic
+            type    : full_f # full_f, control_variate, or delta_f
+            ppc     : 800 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
+            eps     : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
+            bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
             loading :
-                type          : pseudo_random # particle loading mechanism
-                seed          : 1234 # seed for random number generator
-                dir_particles : path_to_particles # directory of particles if loaded externally
-                moments       : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                type    : pseudo_random # particle loading mechanism
+                seed    : 1234 # seed for random number generator
+                moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
         init :
-            type : Maxwellian6DPerturbed
-            Maxwellian6DPerturbed :
-                n :
-                    n0 : 0.
-                ux :
-                    ux0 : 0.
-                uy :
-                    uy0 : 0.
-                uz :
-                    uz0 : 0.
-                vthx :
-                    vthx0 : 1.
-                vthy :
-                    vthy0 : 1.
-                vthy :
-                    vthz0 : 1.
-        background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
-                n  : 1.
-                ux : 0.
-                uy : 0.
-                uz : 0.
-                vthx : 0.028284271247461898 # 2 * 0.02 / sqrt(2)
-                vthy : 0.09797958971132711 # 2 * 0.02 * sqrt(6)
-                vthz : 0.028284271247461898 # 2 * 0.02 / sqrt(2)
+                n  : 0.05
+                u3 : 2.5
         save_data :
-            n_markers : 10 # number of markers to be saved during simulation
+            n_markers : 10 # number of markers to be save during simulation
             f :
-                slices : [e3, vx_vy] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
-                n_bins : [[64], [64, 64]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
-                ranges : [[[0., 1.]], [[-1., 1.], [-1., 1.]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
+                slices : [v3] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
+                n_bins : [[32]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
+                ranges : [[[-0.5, 5.5]]] # bin range in each direction
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
+        use_perp_model : True # for pressure coupling
 
 solvers :
-    solver_ew :
+    solver_1 :
         type : PConjugateGradient
-        pc : MassMatrixPreconditioner # null or name of preconditioner class
-        tol : 1.e-10
+        pc : MassMatrixPreconditioner # null or fft
+        tol : 1.e-14
         maxiter : 3000
         info : False
         verbose : False
-    solver_eb :
+    solver_2 :
         type : PConjugateGradient
-        pc : MassMatrixPreconditioner # null or name of preconditioner class
-        tol : 1.e-10
+        pc : MassMatrixPreconditioner # null or fft
+        tol : 1.e-14
+        maxiter : 3000
+        info : False
+        verbose : False
+    solver_3 :
+        type : PBiConjugateGradientStab
+        pc : MassMatrixPreconditioner # null or fft
+        tol : 1.e-14
         maxiter : 3000
         info : False
         verbose : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_maxwell.yml` & `struphy-2.0.0/src/struphy/io/inp/examples/params_maxwell.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/examples/params_orbits_tokamak.yml` & `struphy-2.0.0/src/struphy/io/inp/examples/params_orbits_tokamak.yml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     dt         : 0.2  # time step
     Tend       : 3000. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Tokamak # mapping F (possible types seen below)
     Tokamak :
-        Nel        : [32, 72] # number of poloidal grid cells, >p
+        Nel        : [28, 72] # number of poloidal grid cells, >p
         p          : [3, 3] # poloidal spline degrees, >1
         psi_power  : 0.6 # parametrization of radial flux coordinate eta1=psi_norm^psi_power, where psi_norm is normalized flux
         psi_shifts : [0., 1.] # start and end shifts of polidal flux in % --> cuts away regions at the axis and edge
         xi_param   : equal_angle # parametrization of angular coordinate (equal_angle, equal_arc_length or sfl (straight field line))
         r0         : 0.3 # initial guess for radial distance from axis used in Newton root-finding method for flux surfaces
         Nel_pre    : [64, 256] # number of poloidal grid cells of pre-mapping needed for equal_arc_length and sfl
         p_pre      : [3, 3] # poloidal spline degrees of pre-mapping needed for equal_arc_length and sfl
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/parameters.yml` & `struphy-2.0.0/src/struphy/io/inp/parameters.yml`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 time :
     dt         : 0.05 # time step
     Tend       : 0.5 # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)  
-    Tokamak :
-        Nel        : [8, 32] # number of poloidal grid cells, >p
-        p          : [3, 3] # poloidal spline degrees, >1
+    Tokamak : # the mapping is defined from the mhd equilibrium below
+        Nel        : [8, 32] # number of poloidal grid cells for spline mapping, >p
+        p          : [3, 3] # poloidal spline degrees for spline mapping, >1
         psi_power  : 0.7 # parametrization of radial flux coordinate eta1=psi_norm^psi_power, where psi_norm is normalized flux
         psi_shifts : [2., 2.] # start and end shifts of polidal flux in % --> cuts away regions at the axis and edge
         xi_param   : equal_angle # parametrization of angular coordinate (equal_angle, equal_arc_length or sfl (straight field line))
         r0         : 0.3 # initial guess for radial distance from axis used in Newton root-finding method for flux surfaces
         Nel_pre    : [64, 256] # number of poloidal grid cells of pre-mapping needed for equal_arc_length and sfl
         p_pre      : [3, 3] # poloidal spline degrees of pre-mapping needed for equal_arc_length and sfl
         tor_period : 1 # toroidal periodicity built into the mapping: phi = 2*pi * eta3 / tor_period
@@ -134,26 +134,44 @@
         q0   : 1.05 # safety factor at r=0
         q1   : 1.80 # safety factor at r=a
         n1   : 0. # shape factor for number density profile 
         n2   : 0. # shape factor for number density profile 
         na   : 1. # number density at r=a
         beta : .01 # plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)
     AdhocTorus :
-        a      : 1. # minor radius
-        R0     : 3. # major radius
-        B0     : 1. # on-axis toroidal magnetic field
-        q0     : 1.05 # safety factor at r=0
-        q1     : 1.80 # safety factor at r=a
-        n1     : 0. # shape factor for number density profile 
-        n2     : 0. # shape factor for number density profile 
-        na     : 1. # number density at r=a
-        p_kind : .5 # kind of pressure profile (0 : cylindrical limit, 1 : ad hoc)
-        p1     : .1 # shape factor for ad hoc pressure profile
-        p2     : .1 # shape factor for ad hoc pressure profile
-        beta   : .01 # plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)
+        a       : 1. # minor radius
+        R0      : 3. # major radius
+        B0      : 1. # on-axis toroidal magnetic field
+        q_kind  : 0 # which profile (0 : parabolic, 1 : other, see documentation)
+        q0      : 1.05 # safety factor at r=0
+        q1      : 1.80 # safety factor at r=a
+        n1      : 0. # 1st shape factor for number density profile 
+        n2      : 0. # 2nd shape factor for number density profile 
+        na      : 1. # number density at r=a
+        p_kind  : 1 # kind of pressure profile (0 : cylindrical limit, 1 : ad hoc)
+        p1      : .1 # 1st shape factor for ad hoc pressure profile
+        p2      : .1 # 2nd shape factor for ad hoc pressure profile
+        beta    : .01 # plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)
+        psi_k   : 3 # spline degree to be used for interpolation of poloidal flux function (only needed if q_kind = 1)
+        psi_nel : 50 # number of cells to be used for interpolation of poloidal flux function (only needed if q_kind = 1)
+    AdhocTorusQPsi :
+        a       : 0.361925 # minor radius
+        R0      : 1. # major radius
+        B0      : 1. # on-axis toroidal magnetic field
+        q0      : 0.6 # safety factor at r=0
+        q1      : 2.5 # safety factor at r=a
+        q0p     : 0.78 # derivative of safety factor at r=0 (w.r.t. to poloidal flux function)
+        q1p     : 5.00 # derivative of safety factor at r=a (w.r.t. to poloidal flux function)
+        n1      : 0. # shape factor for number density profile 
+        n2      : 0. # shape factor for number density profile 
+        na      : 1. # number density at r=a
+        beta    : 4. # plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)
+        p1      : 0.25 # shape factor of pressure profile
+        psi_k   : 3 # spline degree to be used for interpolation of poloidal flux function
+        psi_nel : 50 # number of cells to be used for interpolation of poloidal flux function
     EQDSKequilibrium :
         rel_path        : True # whether eqdsk file path relative to "<struphy_path>/fields_background/mhd_equil/gvec", or the absolute path
         file            : 'AUGNLED_g031213.00830.high' # path to eqdsk file
         data_type       : 0 # 0: there is no space between data, 1: there is space between data
         p_for_psi       : [3, 3] # spline degrees used in interpolation of poloidal flux function grid data
         psi_resolution  : [25., 6.25] # resolution used in interpolation of poloidal flux function grid data in %, i.e. [100., 100.] uses all grid points
         p_for_flux      : 3 # spline degree used in interpolation of 1d functions f=f(psi) (e.g. toroidal field function)
@@ -311,49 +329,49 @@
                     n0 : 1.
                     perturbation :
                         l : [0]
                         m : [0]
                         n : [0]
                         amps_sin : [0.]
                         amps_cos : [0.]
-                ux :
-                    ux0 : 0.
-                uy :
-                    uy0 : 0.
-                uz :
-                    uz0 : 0.
-                vthx :
-                    vthx0 : 1.
-                vthy :
-                    vthy0 : 1.
-                vthy :
-                    vthz0 : 1.
+                u1 :
+                    u10 : 0.
+                u2 :
+                    u20 : 0.
+                u3 :
+                    u30 : 0.
+                vth1 :
+                    vth10 : 1.
+                vth2 :
+                    vth20 : 1.
+                vth3 :
+                    vth30 : 1.
         background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 1.
-                ux : 0.
-                uy : 0.
-                uz : 0.
-                vthx : 1.
-                vthy : 1.
-                vthz : 1.
+                u1 : 0.
+                u2 : 0.
+                u3 : 0.
+                vth1 : 1.
+                vth2 : 1.
+                vth3 : 1.
         save_data :
             n_markers : 3 # number of markers to be saved during simulation
             f :
-                slices : [vz] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
+                slices : [v3] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
                 n_bins : [[32]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
                 ranges : [[[-3., 3.]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
         use_perp_model : True # for pressure coupling 
 
 solvers :
-    solver_1 : 
+    solver_1 :
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
         info : False
         verbose : False
     solver_2 :
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_cc_linmhd_5d.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_cc_linmhd_5d.yml`

 * *Files 5% similar despite different names*

```diff
@@ -29,26 +29,29 @@
         a2 : 1. # minor radius
         R0 : 4. # major radius
         tor_period: 1 # toroidal periodicity built into the mapping: phi = 2*pi * eta3 / tor_period
             
 mhd_equilibrium : 
     type : AdhocTorus # (possible choices seen below)
     AdhocTorus :
-        a      : 1. # minor radius (radius of cylinder)
-        R0     : 4. # major radius (Lz = 2*pi*R0)
-        B0     : 3. # on-axis toroidal magnetic field
-        q0     : 1.71 # safety factor at r=0
-        q1     : 1.87 # safety factor at r=a
-        n1     : 0. # shape factor for number density profile 
-        n2     : 0. # shape factor for number density profile 
-        na     : 1. # number density at r=a
-        p_kind : 1 # kind of pressure profile (0 : cylindrical limit, 1 : ad hoc)
-        p1     : .1 # shape factor for ad hoc pressure profile
-        p2     : .1 # shape factor for ad hoc pressure profile
-        beta   : .01 # plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)
+        a       : 1. # minor radius (radius of cylinder)
+        R0      : 4. # major radius (Lz = 2*pi*R0)
+        B0      : 3. # on-axis toroidal magnetic field
+        q_kind  : 0 # which profile (0 : parabolic, 1 : other, see documentation)
+        q0      : 1.71 # safety factor at r=0
+        q1      : 1.87 # safety factor at r=a
+        n1      : 0. # shape factor for number density profile 
+        n2      : 0. # shape factor for number density profile 
+        na      : 1. # number density at r=a
+        p_kind  : 1 # kind of pressure profile (0 : cylindrical limit, 1 : ad hoc)
+        p1      : .1 # shape factor for ad hoc pressure profile
+        p2      : .1 # shape factor for ad hoc pressure profile
+        beta    : .01 # plasma beta in % for flat safety factor (ratio of kinetic pressure to magnetic pressure)
+        psi_k   : 3 # spline degree to be used for interpolation of poloidal flux function (only needed if q_kind = 1)
+        psi_nel : 50 # number of cells to be used for interpolation of poloidal flux function (only needed if q_kind = 1)
 
 em_fields : 
     init :
         type : null # type of initialization
       
 fluid : 
     mhd :
@@ -81,15 +84,15 @@
         init : 
             type : Maxwellian6DUniform
         background :
             type : Maxwellian6DUniform
         save_data :
             n_markers : 4 # number of markers to be save during simulation
             f :
-                slices : [vz]
+                slices : [v3]
                 n_bins : [[32]]
                 ranges : [[[-3., 3.]]]
         push_algos :
             integrator : implicit # explicit or implicit
             method : discrete_gradients # possible choices: discrete_gradients, forward_euler, heun2, rk2, heun3, rk4
             maxiter : 10
             tol : 1.e-15
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_hybrid_fA.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_hybrid_fA.yml`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
     p        : [2, 2, 2]  # spline degree, 
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [5, 4, 4] # quadrature points per grid cell
     nq_pr    : [4, 4, 4] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
-      
+
 units :
     x  : 1. # length scale unit in m
     B  : 1. # magnetic field unit in T
     n  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
 
 time : 
     dt         : 0.01 # time step
     Tend       : 0.05 # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
-      
+
 geometry : 
     type : Cuboid # mapping F (possible types seen below)  
     Cuboid : 
         l1 : 0. # start of interval in eta1
         r1 : 1. # end of interval in eta1, r1>l1
         l2 : 0. # start of interval in eta2
         r2 : 1. # end of interval in eta2, r2>l2
@@ -79,15 +79,14 @@
             A  : 0. # amplitude of Uz
         InitialMHDAxisymHdivEigFun :
             spec : '/path_to_spec/spec.npy' # relative path (to <install_path/struphy>) of the .npy spectrum
             eig_freq_upper : 0.15 # upper search limit of squared eigenfrequency to identify eigenfunction
             eig_freq_lower : 0.14 # lower search limit of squared eigenfrequency to identify eigenfunction
             kind : r # real (r) or imaginary (i) part of eigenfunction
             scaling : 1. # scaling factor to scale the amplitude of the eigenfunction
-      
 
 kinetic :
     electrons :
         temperature : 1.0
     ions :
         ionsshape :
             degree : [2, 2, 2]
@@ -105,48 +104,47 @@
                 seed          : 1234 # seed for random number generator
                 dir_particles : path_to_particles # directory of particles if loaded externally
                 moments   : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 1.
-                ux : 0.
-                uy : 0.
-                uz : 0.
-                vthx : 1.
-                vthy : 1.
-                vthz : 1.
+                u1 : 0.
+                u2 : 0.
+                u3 : 0.
+                vth1 : 1.
+                vth2 : 1.
+                vth3 : 1.
         background :
               type        : 0 # 0: Maxwellian in 6d
               moms_spec   : [0, 0, 0, 0, 0, 0, 0] # Specifier for the moments n0, u0x, u0y, u0z, vth0x, etc. 0 means constant
               moms_params : [1., 0., 0., 2.5, 1., 1., 1.] # parameters needed to specify the moments
         perturbations : # always in logical position space
             type : null # null or possible types seen below
-            moms : [n, uz] # which velocity moment to perturb: n, ux, uy, uz, vthx, vthy, vthz
+            moms : [n, u3] # which velocity moment to perturb: n, u1, u2, u3, vth1, vth2, vth3
             Modes_sin : 
                 k1 : [6.283186] # wave vectors in eta_1 
                 k2 : [0.] # wave vectors in eta_2 
                 k3 : [0.] # wave vectors in eta_3 
                 amp : [0.001] # amplitudes
             Modes_cos : 
                 k1 : [6.283186] # wave vectors in eta_1 
                 k2 : [0.] # wave vectors in eta_2
                 k3 : [0.] # wave vectors in eta_3
                 amp : [0.001] # amplitudes
         save_data :
             n_markers : 3 # number of markers to be save during simulation
             f :
-                slices : [vz]
+                slices : [v3]
                 n_bins : [[32]]
                 ranges : [[[-3., 3.]]]
         push_algos :
             pxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
         pc : full # for pressure coupling: full or perp
-            
 
 solvers :
     solver_1 : 
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or fft
         tol : 1.e-12
         maxiter : 3000
@@ -162,9 +160,7 @@
     solver_3 :
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or fft
         tol : 1.e-12
         maxiter : 3000
         info : False
         verbose : False
-
-
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,19 @@
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
         init :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
-                uz : 2.5
+                u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
             f :
-                slices : [vz] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
+                slices : [v3] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
                 n_bins : [[32]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
                 ranges : [[[-0.5, 5.5]]] # bin range in each direction
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
 
 solvers :
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,30 +8,30 @@
     nq_pr    : [6, 6, 6] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
 units :
     x  : 1. # length scale unit in m
     B  : 1. # magnetic field unit in T
     n  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
-       
+
 time : 
     dt         : 0.2  # time step
     Tend       : 1. # simulation time interval is [0, Tend]
     split_algo : Strang # LieTrotter | Strang
-      
+
 geometry : 
     type : Cuboid # mapping F (possible types seen below)  
     Cuboid : 
         l1 : 0. # start of interval in eta1
         r1 : 1. # end of interval in eta1, r1>l1
         l2 : 0. # start of interval in eta2
         r2 : 1. # end of interval in eta2, r2>l2
         l3 : 0. # start of interval in eta3
         r3 : 10. # end of interval in eta3, r3>l3 
-            
+
 mhd_equilibrium : 
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         B0x  : 0. # magnetic field in x
         B0y  : 0. # magnetic field in y
         B0z  : 1. # magnetic field in z
         beta : 0. # plasma beta = 2*p*mu_0/B^2
@@ -65,15 +65,15 @@
             InitialMHDSlab : 
                 a  : 1.
                 R0 : 1.
                 m  : 0
                 n  : -1
                 U  : 0.001
                 A  : 0.    
-            
+
 kinetic :
     energetic_ions :
         phys_params:
             A : 1 # mass number in units of proton mass
             Z : 1 # signed charge number in units of elementary charge
         markers :
             type    : control_variate # full_f, control_variate, or delta_f
@@ -84,30 +84,30 @@
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
         init : 
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
-                uz : 2.5
+                u3 : 2.5
         background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
                 n  : 0.05
-                uz : 2.5
+                u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
             f :
-                slices : [vz] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
+                slices : [v3] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
                 n_bins : [[32]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
                 ranges : [[[-0.5, 5.5]]] # bin range in each direction
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
-      
+
 solvers :
     solver_1 : 
         type : PBiConjugateGradientStab
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-14
         maxiter : 3000
         info : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,18 @@
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [6, 6, 6] # quadrature points per grid cell
     nq_pr    : [6, 6, 6] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
           
-model_units :
+units :
     x   : 1. # length scale unit in m
     B   : 1. # magnetic field unit in T
-    nb  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
-    nuh : 5. # ratio of hot/bulk number density units in %
-    Ab  : 1 # mass number of bulk ion species (1 : Hydrogen, 2 : Deuterium, 3 : Tritium, etc.)
-    Ah  : 1 # mass number of energetic ion species (1 : Hydrogen, 2 : Deuterium, 3 : Tritium, etc.)
-    Zh  : 1 # charge number of energetic ion species (1 : Hydrogen, 2 : Helium, etc.)
+    n  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
 
 time : 
     dt         : 0.1  # time step
     Tend       : 1. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
       
 geometry : 
@@ -82,15 +78,15 @@
             loading :
                 type    : pseudo_random # particle loading mechanism 
                 seed    : 1234 # seed for random number generator
                 moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
         init : 
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
-                uz : 2.5
+                u3 : 2.5
         save_data :
             n_markers : 10 # number of markers to be save during simulation
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
       
 solvers :
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml` & `struphy-2.0.0/src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,119 @@
 grid :
-    Nel      : [3, 3, 10] # number of grid cells, >p
-    p        : [2, 2, 3]  # spline degree
+    Nel      : [2, 2, 64] # number of grid cells, >p
+    p        : [1, 1, 3]  # spline degree
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
-    nq_el    : [6, 6, 6] # quadrature points per grid cell
-    nq_pr    : [6, 6, 6] # quadrature points per histopolation cell (for commuting projectors)
+    nq_el    : [2, 2, 2] # quadrature points per grid cell
+    nq_pr    : [2, 2, 2] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
 
 units :
-    x  : 1. # length scale unit in m
-    B  : 1. # magnetic field unit in T
-    n  : 0.0005185219355 # bulk number density unit in 1 x 10^20 m^(-3)
-
-time : 
-    dt         : 0.1  # time step
-    Tend       : .5 # simulation time interval is [0, Tend]
+    x   : 1. # length scale unit in m
+    B   : 1. # magnetic field unit in T
+    n   : 1. # bulk number density unit in 1 x 10^20 m^(-3)
+
+time :
+    dt         : 0.01 # time step
+    Tend       : 30. # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
 
 geometry :
     type : Cuboid # mapping F (possible types seen below)
     Cuboid :
-        l1 : 0. # start of interval in eta1
-        r1 : 1. # end of interval in eta1, r1>l1
-        l2 : 0. # start of interval in eta2
-        r2 : 1. # end of interval in eta2, r2>l2
-        l3 : 0. # start of interval in eta3
-        r3 : 10. # end of interval in eta3, r3>l3 
+        l1       : 0. # start of interval in eta1
+        r1       : 2. # end of interval in eta1, r1>l1
+        l2       : 0. # start of interval in eta2
+        r2       : 2. # end of interval in eta2, r2>l2
+        l3       : 0. # start of interval in eta3
+        r3       : 20. # end of interval in eta3, r3>l3
 
 mhd_equilibrium :
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
-        B0x  : 0. # magnetic field in x
+        B0x  : 0.5 # magnetic field in x
         B0y  : 0. # magnetic field in y
-        B0z  : 1. # magnetic field in z
+        B0z  : 1.4 # magnetic field in z
         beta : 0. # plasma beta = 2*p*mu_0/B^2
         n0   : 1. # number density
 
+electric_equilibrium :
+    type : HomogenSlab # (possible choices seen below)
+    HomogenSlab :
+        phi0  : 1. # constant electric potential
+
 em_fields :
     init :
         type : null # initial conditions (possible types seen below)
 
-fluid :
-    mhd :
-        phys_params:
-            A : 1 # mass number in units of proton mass
-            Z : 1 # signed charge number in units of elementary charge
-        mhd_u_space : H1vec # Hdiv | H1vec
-        init :
-            type : null # type of initialization
-            ModesCos :
-                coords : 'physical' # in which coordinates (logical or physical)
-                comps :
-                    n3 : False                # components to be initialized (for scalar fields: no list)
-                    uv : [False, True, False] # components to be initialized (for scalar fields: no list)
-                    p3 : False                # components to be initialized (for scalar fields: no list)
-                ls : [0] # Integer mode numbers in x or eta_1 (depending on coords)
-                ms : [0] # Integer mode numbers in y or eta_2 (depending on coords)
-                ns : [-1] # Integer mode numbers in z or eta_3 (depending on coords)
-                amp : [0.0001] # amplitudes of each mode
-                Lx : 1.
-                Ly : 1.
-                Lz : 10.
-            InitialMHDSlab :
-                a  : 1.
-                R0 : 1.
-                m  : 0
-                n  : -1
-                U  : 0.001
-                A  : 0.
-
 kinetic :
-    energetic_ions :
-        phys_params:
-            A : 1 # mass number in units of proton mass
-            Z : 1 # signed charge number in units of elementary charge
+    electrons :
         markers :
-            type    : full_f # full_f, control_variate, or delta_f
-            ppc     : 800 # alternative if ppc = null (total number of markers, must be larger or equal than # MPI processes)
-            eps     : .25 # MPI send/receive buffer (0.1 <= eps <= 1.0)
-            bc_type : [periodic, periodic, periodic] # marker boundary conditions: remove, reflect or periodic
+            type    : delta_f # full_f, control_variate, or delta_f
+            Np      : 5000 # alternative if ppc not given (total number of markers, Np must be >= # MPI processes)
+            eps     : 0.5 # MPI send/receive buffer (0.1 <= eps <= 1.0)
+            bc_type : [periodic, periodic, periodic] # remove, reflect or periodic
             loading :
-                type    : pseudo_random # particle loading mechanism
-                seed    : 1234 # seed for random number generator
-                moments : [0., 0., 2.5, 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
+                type          : pseudo_random # particle loading mechanism
+                seed          : 1234 # seed for random number generator
+                dir_particles : path_to_particles # directory of particles if loaded externally
+                moments       : [0., 0., 0., 1., 1., 1.] # moments of Gaussian s3, see background/moms_spec
         init :
+            type : Maxwellian6DPerturbed
+            Maxwellian6DPerturbed :
+                n :
+                    n0 : 0.
+                    perturbation :
+                        # l : [0.07957747154594767] # 0.5 / (2 * pi)
+                        l : [5]
+                        m : [0]
+                        n : [0]
+                        amps_sin : [0.]
+                        amps_cos : [0.5]
+                u1 :
+                    u01 : 0.
+                u2 :
+                    u02 : 0.
+                u3 :
+                    u03 : 0.
+                vth1 :
+                    vth01 : 2.
+                vth2 :
+                    vth02 : 2.
+                vth3 :
+                    vth03 : 2.
+        background :
             type : Maxwellian6DUniform
             Maxwellian6DUniform :
-                n  : 0.05
-                uz : 2.5
+                n  : 1.
+                u1 : 0.
+                u2 : 0.
+                u3 : 0.
+                vth1 : 2.
+                vth2 : 2.
+                vth3 : 2.
         save_data :
-            n_markers : 10 # number of markers to be save during simulation
+            n_markers : 10 # number of markers to be saved during simulation
             f :
-                slices : [vz] # in which directions to bin (e.g. [e1_e2, vx_vy_vz])
-                n_bins : [[32]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
-                ranges : [[[-0.5, 5.5]]] # bin range in each direction
+                slices : [e3, v1_v2] # in which directions to bin (e.g. [e1_e2, v1_v2_v3])
+                n_bins : [[64], [64, 64]] # number of bins in each direction (e.g. [[16, 20], [16, 18, 22]])
+                ranges : [[[0., 1.]], [[-5., 5.], [-5., 5.]]] # bin range in each direction (e.g. [[[0., 1.], [0., 1.]], [[-3., 3.], [-4., 4.], [-5., 5.]]])
         push_algos :
             vxb : analytic # possible choices: analytic, implicit
             eta : rk4 # possible choices: forward_euler, heun2, rk2, heun3, rk4
-        use_perp_model : True # for pressure coupling
 
 solvers :
-    solver_1 :
+    solver_ew :
         type : PConjugateGradient
-        pc : MassMatrixPreconditioner # null or fft
-        tol : 1.e-14
+        pc : MassMatrixPreconditioner # null or name of preconditioner class
+        tol : 1.e-10
         maxiter : 3000
         info : False
         verbose : False
-    solver_2 :
+    solver_eb :
         type : PConjugateGradient
-        pc : MassMatrixPreconditioner # null or fft
-        tol : 1.e-14
-        maxiter : 3000
-        info : False
-        verbose : False
-    solver_3 :
-        type : PBiConjugateGradientStab
-        pc : MassMatrixPreconditioner # null or fft
-        tol : 1.e-14
+        pc : MassMatrixPreconditioner # null or name of preconditioner class
+        tol : 1.e-10
         maxiter : 3000
         info : False
         verbose : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_linearmhd.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_linearmhd.yml`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,35 @@
     p        : [2, 2, 3]  # spline degree, 
     spl_kind : [True, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [6, 6, 6] # quadrature points per grid cell
     nq_pr    : [4, 4, 4] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
-          
+
 units :
     x : 1. # length scale unit in m
     B : 1. # magnetic field unit in T
     n : 1. # number density unit of fluid species in 1 x 10^20 m^(-3)
 
 time : 
     dt         : 0.15 # time step
     Tend       : 1.5 # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
-      
+
 geometry : 
     type : Cuboid # mapping F (possible types seen below)  
     Cuboid : 
         l1 : 0. # start of interval in eta1
         r1 : 1. # end of interval in eta1, r1>l1
         l2 : 0. # start of interval in eta2
         r2 : 1. # end of interval in eta2, r2>l2
         l3 : 0. # start of interval in eta3
         r3 : 60. # end of interval in eta3, r3>l3
-            
+
 mhd_equilibrium : 
     type : HomogenSlab # (possible choices seen below)
     HomogenSlab :
         B0x  : 0. # magnetic field in x
         B0y  : 1. # magnetic field in y
         B0z  : 1. # magnetic field in z
         beta : 100. # plasma beta = 2*p*mu_0/B^2
@@ -52,15 +52,15 @@
             noise :
                 comps : 
                     n3 : False              # components to be initialized (for scalar fields: no list)
                     uv : [True, True, True] # components to be initialized (for scalar fields: no list)
                     p3 : False              # components to be initialized (for scalar fields: no list)
                 variation_in : e3 # noise variation (logical space): e1, e2, e3 (1d), e1e2, e1e3, e2e3 (2d), e1e2e3 (3d)
                 amp : 0.1 # noise amplitude
-      
+
 solvers :
     solver_1 : 
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
         info : False
@@ -68,8 +68,7 @@
     solver_2 :
         type : PBiConjugateGradientStab
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
         info : False
         verbose : False
-
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_linearmhd_gvec.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_linearmhd_gvec.yml`

 * *Files 9% similar despite different names*

```diff
@@ -3,66 +3,71 @@
     p        : [2, 2, 3]  # spline degree, 
     spl_kind : [False, True, True] # spline type: True=periodic, False=clamped
     bc       : [[null, null], [null, null], [null, null]] # boundary conditions for N-splines (homogeneous Dirichlet='d')
     dims_mask : [True, True, True] # True if the dimension is to be used in the mpi domain decomposition (=default for each dimension).
     nq_el    : [6, 6, 6] # quadrature points per grid cell
     nq_pr    : [4, 4, 4] # quadrature points per histopolation cell (for commuting projectors)
     polar_ck : -1 # C^k smoothness at polar singularity at eta_1=0 (default: -1 --> standard tensor product, 1 : polar splines)
-          
-time : 
+
+units :
+    x : 1. # length scale unit in m
+    B : 1. # magnetic field unit in T
+    n : 1. # number density unit of fluid species in 1 x 10^20 m^(-3)
+
+time :
     dt         : 0.15 # time step
     Tend       : 1.5 # simulation time interval is [0, Tend]
     split_algo : LieTrotter # LieTrotter | Strang
-      
-geometry : 
+
+geometry :
     type : Cuboid # mapping F (possible types seen below)  
-    Cuboid : 
+    Cuboid :
         l1 : 0. # start of interval in eta1
         r1 : 1. # end of interval in eta1, r1>l1
         l2 : 0. # start of interval in eta2
         r2 : 1. # end of interval in eta2, r2>l2
         l3 : 0. # start of interval in eta3
         r3 : 60. # end of interval in eta3, r3>l3
-            
-mhd_equilibrium : 
+
+mhd_equilibrium :
     type : GVECequilibrium # (possible choices seen below)
     use_equil_domain : True # use the mapping given by the equilibrium (flux aligned) or not
-    GVECequilibrium : 
+    GVECequilibrium :
         rel_path  : True # whether to state dat_file (json_file) relative to "<struphy_path>/fields_background/mhd_equil/gvec", or give the absolute path
         dat_file  : '/ellipstell_v2/newBC_E1D6_M6N6/GVEC_ELLIPSTELL_V2_State_0000_00200000.dat' # path to gvec .dat output file 
         json_file : Null # give directly the parsed json file, if it exists (then dat_file is not used)
         use_pest  : False # Whether to use straight-field line coordinates (PEST)
         Nel       : [16, 16, 8] # Number of cells in each direction used for interpolation of the mapping.
         p         : [3, 3, 3] # Spline degree in each direction used for interpolation of the mapping.
 
-em_fields : 
+em_fields :
     init :
         type : null # initialization
 
 fluid :
     mhd :
         mhd_u_space : H1vec # Hdiv | H1vec
         init :
             type : noise # initial conditions (possible types seen below)
             noise :
-                comps : 
+                comps :
                     n3 : False              # components to be initialized (for scalar fields: no list)
                     uv : [True, True, True] # components to be initialized (for scalar fields: no list)
                     p3 : False              # components to be initialized (for scalar fields: no list)
                 variation_in : e3 # noise variation (logical space): e1, e2, e3 (1d), e1e2, e1e3, e2e3 (2d), e1e2e3 (3d)
                 amp : 0.1   # noise amplitude
-      
+
 solvers :
-    solver_1 : 
+    solver_1 :
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
         info : False
         verbose : False
     solver_2 :
         type : PBiConjugateGradientStab
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
         info : False
-        verbose : False       
+        verbose : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_maxwell_1.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_maxwell_1.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 solvers :
     solver_1 : 
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
         info : False
-        verbose : False
+        verbose : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/params_maxwell_2.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/params_maxwell_2.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,8 @@
 solvers :
     solver_1 : 
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
         info : False
-        verbose : False
+        verbose : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/strscl.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/strscl.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 solvers :
     solver_1 :
         type : PConjugateGradient
         pc : MassMatrixPreconditioner # null or name of preconditioner class
         tol : 1.e-8
         maxiter : 3000
         info : False
-        verbose : False
+        verbose : False
```

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/wkscl_1.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_1.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/wkscl_2.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_2.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/wkscl_3.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_3.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/wkscl_4.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_4.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/wkscl_5.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_5.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/wkscl_6.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_6.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/wkscl_7.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_7.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/io/inp/tests/wkscl_8.yml` & `struphy-2.0.0/src/struphy/io/inp/tests/wkscl_8.yml`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/kinetic_background/analytical.py` & `struphy-2.0.0/src/struphy/kinetic_background/analytical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from abc import ABCMeta, abstractmethod
 import numpy as np
 
 from struphy.fields_background.mhd_equil.equils import set_defaults
-from struphy.geometry.base import Domain
 
 
 class Maxwellian(metaclass=ABCMeta):
     r"""
     Base class for a Maxwellian distribution function defined on :math:`[0, 1]^3 \times \mathbb R^n, n \geq 1,` 
     with logical position coordinates :math:`\boldsymbol{\eta} \in [0, 1]^3`:
 
@@ -76,15 +75,15 @@
 
     def gaussian(self, v, u=0., vth=1.):
         """1D Gaussian, to which array-valued mean- and thermal velocities can be passed.
 
         Parameters
         ----------
         v : float | array-like
-            Velocits coordinate(s).
+            Velocity coordinate(s).
 
         u : float | array-like
             Mean velocity evaluated at position array.
 
         vth : float | array-like
             Thermal velocity evaluated at position array, same shape as u.
 
@@ -96,20 +95,20 @@
         if isinstance(v, np.ndarray) and isinstance(u, np.ndarray):
             assert v.shape == u.shape
 
         return 1./(np.sqrt(np.pi) * vth) * np.exp(-(v - u)**2/vth**2)
 
     def __call__(self, *args):
         """
-        Evaluates the Maxwellian distribution function M(etas, v1,..., vn).
+        Evaluates the Maxwellian distribution function M(etas, v1, ..., vn).
 
         Parameters
         ----------
         *args : array_like
-            Position-velocity arguments in the order etas, v1,..., vn.
+            Position-velocity arguments in the order etas, v1, ..., vn.
 
         Returns
         -------
         f : np.ndarray
             The evaluated Maxwellian.
         """
 
@@ -125,32 +124,35 @@
 
 class Maxwellian6DUniform(Maxwellian):
     r"""
     6d Maxwellian distribution function defined on [0, 1]^3 x R^3, with logical position and Cartesian velocity coordinates, with uniform velocity moments.
 
     .. math::
 
-        f(\boldsymbol{\eta}, \mathbf v) = n\,\frac{1}{\pi^{3/2}\,v_{\mathrm{th},x}\,v_{\mathrm{th},y}\,v_{\mathrm{th},z}}\,\exp\left[-\frac{(v_x-u_x)^2}{v_{\mathrm{th},x}^2}-\frac{(v_y-u_y)^2}{v_{\mathrm{th},y}^2}-\frac{(v_z-u_z)^2}{v_{\mathrm{th},z}^2}\right].
+        f(\boldsymbol{\eta}, \mathbf v) = n \, \frac{1}{\pi^{3/2} \, v_{\mathrm{th},1} \, v_{\mathrm{th},2} \, v_{\mathrm{th},3}} \,
+            \exp\left[- \frac{(v_1 - u_1)^2}{v_{\mathrm{th},1}^2}
+                      - \frac{(v_2 - u_2)^2}{v_{\mathrm{th},2}^2}
+                      - \frac{(v_3 - u_3)^2}{v_{\mathrm{th},3}^2}\right].
 
     Parameters
     ----------
     **params
-        Keyword arguments (n= , ux=, etc.) defining the moments of the 6d Maxwellian.
+        Keyword arguments (n= , u1=, etc.) defining the moments of the 6d Maxwellian.
     """
 
     def __init__(self, **params):
 
         # default parameters
         params_default = {'n': 1.,
-                          'ux': 0.,
-                          'uy': 0.,
-                          'uz': 0.,
-                          'vthx': 1.,
-                          'vthy': 1.,
-                          'vthz': 1.}
+                          'u1': 0.,
+                          'u2': 0.,
+                          'u3': 0.,
+                          'vth1': 1.,
+                          'vth2': 1.,
+                          'vth3': 1.}
 
         self._params = set_defaults(params, params_default)
 
     @property
     def params(self):
         """ Parameters dictionary defining the moments of the Maxwellian.
         """
@@ -187,17 +189,17 @@
         Returns
         -------
         A numpy.array with the thermal velocity evaluated at evaluation points (one dimension more than etas).
         The additional dimension is in the first index.
         """
         res_list = []
 
-        res_list += [self.params['vthx'] - 0*eta1]
-        res_list += [self.params['vthy'] - 0*eta1]
-        res_list += [self.params['vthz'] - 0*eta1]
+        res_list += [self.params['vth1'] - 0*eta1]
+        res_list += [self.params['vth2'] - 0*eta1]
+        res_list += [self.params['vth3'] - 0*eta1]
 
         return np.array(res_list)
 
     def u(self, eta1, eta2, eta3):
         """ Mean velocities (Cartesian components evaluated at x = F(eta)).
 
         Parameters
@@ -208,17 +210,17 @@
         Returns
         -------
         A numpy.array with the mean velocity evaluated at evaluation points (one dimension more than etas).
         The additional dimension is in the first index.
         """
         res_list = []
 
-        res_list += [self.params['ux'] - 0*eta1]
-        res_list += [self.params['uy'] - 0*eta1]
-        res_list += [self.params['uz'] - 0*eta1]
+        res_list += [self.params['u1'] - 0*eta1]
+        res_list += [self.params['u2'] - 0*eta1]
+        res_list += [self.params['u3'] - 0*eta1]
 
         return np.array(res_list)
 
 
 class Maxwellian6DPerturbed(Maxwellian):
     r"""
     6d Maxwellian distribution function defined on [0, 1]^3 x R^3, with logical position and Cartesian velocity coordinates, with sin/cos perturbed velocity moments.
@@ -235,17 +237,17 @@
     ----------
     **params
         Keyword arguments defining the moments of the 6d Maxwellian. For each moment, a dictionary of the form {'n0' : float, 'perturbation' : {'l' : list, 'm' : list, 'n' : list, 'amps_sin' : list, 'amps_cos' : list}} must be passed.
     """
 
     def __init__(self, **params):
 
-        moment_keys = ['n', 'ux', 'uy', 'uz', 'vthx', 'vthy', 'vthz']
+        moment_keys = ['n', 'u1', 'u2', 'u3', 'vth1', 'vth2', 'vth3']
 
-        backgr_keys = ['n0', 'ux0', 'uy0', 'uz0', 'vthx0', 'vthy0', 'vthz0']
+        backgr_keys = ['n0', 'u01', 'u02', 'u0_3', 'vth01', 'vth02', 'vth03']
 
         # set default background, mode numbers and amplitudes if no perturbation of a moment in given
         for moment_key, backgr_key in zip(moment_keys, backgr_keys):
 
             # add moment key if not there
             if moment_key not in params.keys():
                 params[moment_key] = {}
@@ -380,48 +382,48 @@
         -------
         A numpy.array with the mean velocity evaluated at evaluation points (one dimension more than etas).
         The additional dimension is in the first index.
         """
 
         res_list = []
 
-        ls = self.params['ux']['perturbation']['l']
-        ms = self.params['ux']['perturbation']['m']
-        ns = self.params['ux']['perturbation']['n']
+        ls = self.params['u1']['perturbation']['l']
+        ms = self.params['u1']['perturbation']['m']
+        ns = self.params['u1']['perturbation']['n']
 
-        amps_sin = self.params['ux']['perturbation']['amps_sin']
-        amps_cos = self.params['ux']['perturbation']['amps_cos']
+        amps_sin = self.params['u1']['perturbation']['amps_sin']
+        amps_cos = self.params['u1']['perturbation']['amps_cos']
 
-        res = self.params['ux']['ux0']
+        res = self.params['u1']['u01']
         res += self.modes_sin(eta1, eta2, eta3, ls, ms, ns, amps_sin)
         res += self.modes_cos(eta1, eta2, eta3, ls, ms, ns, amps_cos)
 
         res_list += [res]
 
-        ls = self.params['uy']['perturbation']['l']
-        ms = self.params['uy']['perturbation']['m']
-        ns = self.params['uy']['perturbation']['n']
+        ls = self.params['u2']['perturbation']['l']
+        ms = self.params['u2']['perturbation']['m']
+        ns = self.params['u2']['perturbation']['n']
 
-        amps_sin = self.params['uy']['perturbation']['amps_sin']
-        amps_cos = self.params['uy']['perturbation']['amps_cos']
+        amps_sin = self.params['u2']['perturbation']['amps_sin']
+        amps_cos = self.params['u2']['perturbation']['amps_cos']
 
-        res = self.params['uy']['uy0']
+        res = self.params['u2']['u02']
         res += self.modes_sin(eta1, eta2, eta3, ls, ms, ns, amps_sin)
         res += self.modes_cos(eta1, eta2, eta3, ls, ms, ns, amps_cos)
 
         res_list += [res]
 
-        ls = self.params['uz']['perturbation']['l']
-        ms = self.params['uz']['perturbation']['m']
-        ns = self.params['uz']['perturbation']['n']
+        ls = self.params['u3']['perturbation']['l']
+        ms = self.params['u3']['perturbation']['m']
+        ns = self.params['u3']['perturbation']['n']
 
-        amps_sin = self.params['uz']['perturbation']['amps_sin']
-        amps_cos = self.params['uz']['perturbation']['amps_cos']
+        amps_sin = self.params['u3']['perturbation']['amps_sin']
+        amps_cos = self.params['u3']['perturbation']['amps_cos']
 
-        res = self.params['uz']['uz0']
+        res = self.params['u3']['u0_3']
         res += self.modes_sin(eta1, eta2, eta3, ls, ms, ns, amps_sin)
         res += self.modes_cos(eta1, eta2, eta3, ls, ms, ns, amps_cos)
 
         res_list += [res]
 
         return np.array(res_list)
 
@@ -437,48 +439,48 @@
         -------
         A numpy.array with the thermal velocity evaluated at evaluation points (one dimension more than etas).
         The additional dimension is in the first index.
         """
 
         res_list = []
 
-        ls = self.params['vthx']['perturbation']['l']
-        ms = self.params['vthx']['perturbation']['m']
-        ns = self.params['vthx']['perturbation']['n']
+        ls = self.params['vth1']['perturbation']['l']
+        ms = self.params['vth1']['perturbation']['m']
+        ns = self.params['vth1']['perturbation']['n']
 
-        amps_sin = self.params['vthx']['perturbation']['amps_sin']
-        amps_cos = self.params['vthx']['perturbation']['amps_cos']
+        amps_sin = self.params['vth1']['perturbation']['amps_sin']
+        amps_cos = self.params['vth1']['perturbation']['amps_cos']
 
-        res = self.params['vthx']['vthx0']
+        res = self.params['vth1']['vth01']
         res += self.modes_sin(eta1, eta2, eta3, ls, ms, ns, amps_sin)
         res += self.modes_cos(eta1, eta2, eta3, ls, ms, ns, amps_cos)
 
         res_list += [res]
 
-        ls = self.params['vthy']['perturbation']['l']
-        ms = self.params['vthy']['perturbation']['m']
-        ns = self.params['vthy']['perturbation']['n']
+        ls = self.params['vth2']['perturbation']['l']
+        ms = self.params['vth2']['perturbation']['m']
+        ns = self.params['vth2']['perturbation']['n']
 
-        amps_sin = self.params['vthy']['perturbation']['amps_sin']
-        amps_cos = self.params['vthy']['perturbation']['amps_cos']
+        amps_sin = self.params['vth2']['perturbation']['amps_sin']
+        amps_cos = self.params['vth2']['perturbation']['amps_cos']
 
-        res = self.params['vthy']['vthy0']
+        res = self.params['vth2']['vth02']
         res += self.modes_sin(eta1, eta2, eta3, ls, ms, ns, amps_sin)
         res += self.modes_cos(eta1, eta2, eta3, ls, ms, ns, amps_cos)
 
         res_list += [res]
 
-        ls = self.params['vthz']['perturbation']['l']
-        ms = self.params['vthz']['perturbation']['m']
-        ns = self.params['vthz']['perturbation']['n']
+        ls = self.params['vth3']['perturbation']['l']
+        ms = self.params['vth3']['perturbation']['m']
+        ns = self.params['vth3']['perturbation']['n']
 
-        amps_sin = self.params['vthz']['perturbation']['amps_sin']
-        amps_cos = self.params['vthz']['perturbation']['amps_cos']
+        amps_sin = self.params['vth3']['perturbation']['amps_sin']
+        amps_cos = self.params['vth3']['perturbation']['amps_cos']
 
-        res = self.params['vthz']['vthz0']
+        res = self.params['vth3']['vth03']
         res += self.modes_sin(eta1, eta2, eta3, ls, ms, ns, amps_sin)
         res += self.modes_cos(eta1, eta2, eta3, ls, ms, ns, amps_cos)
 
         res_list += [res]
 
         return np.array(res_list)
 
@@ -564,17 +566,17 @@
         -------
         A numpy.array with the thermal velocity evaluated at evaluation points (one dimension more than etas).
         The additional dimension is in the first index.
         """
 
         res_list = []
 
-        res_list += [self.params['vthx'] - 0*eta1]
-        res_list += [self.params['vthy'] - 0*eta1]
-        res_list += [self.params['vthz'] - 0*eta1]
+        res_list += [self.params['vth1'] - 0*eta1]
+        res_list += [self.params['vth2'] - 0*eta1]
+        res_list += [self.params['vth3'] - 0*eta1]
 
         return np.array(res_list)
 
     def u(self, eta1, eta2, eta3):
         """ Mean velocities (Cartesian components evaluated at x = F(eta)).
 
         Parameters
```

### Comparing `struphy-1.9.9/src/struphy/kinetic_background/background_eval.py` & `struphy-2.0.0/src/struphy/kinetic_background/background_eval.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,16 @@
         v : array[float]
             Velocity at which to evaluate f0.
 
         f0_spec : int
             Specifier for kinetic background, 0 -> maxwellian_6d. See Notes.
 
         moms_spec : array[int]
-            Specifier for the seven moments n0, u0x, u0y, u0z, vth0x, vth0y, vth0z (in this order).
-            Is 0 for constant moment, for more see :meth:`struphy.kinetic_background.moments_kernels.moments`.
+            Specifier for the seven moments n0, u01, u02, u03, vth01, vth02, vth03 (in this order).
+            Is 0 for constant moment, for more see :math:`struphy.kinetic_background.moments_kernels.moments`.
 
         params : array[float]
             Parameters needed to specify the moments; the order is specified in :ref:`struphy.kinetic_background.moments_kernels` for the respective functions available.
 
     Notes
     -----
         See :ref:`struphy.kinetic_background.f0_kernels` for available backgrounds.
```

### Comparing `struphy-1.9.9/src/struphy/kinetic_background/f0_kernels.py` & `struphy-2.0.0/src/struphy/kinetic_background/f0_kernels.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,39 +5,42 @@
 
 def maxwellian_6d(x: 'float[:]', v: 'float[:]', moms_spec: 'int[:]', params: 'float[:]') -> float:
     r"""
     Point-wise evaluation of Maxwellian:
 
     .. math::
 
-        f_0(\mathbf x, \mathbf v) = \frac{n_0(\mathbf x)}{(\pi)^{3/2}\, \hat v_{0,x}(\mathbf x) \hat v_{0,y}(\mathbf x) \hat v_{0,z}(\mathbf x)}\,\exp{\left[ - \frac{(v_x - u_{0,x}(\mathbf x))^2}{\hat v_{0,x}^2(\mathbf x)} \frac{(v_y - u_{0,y}(\mathbf x))^2}{\hat v_{0,y}^2(\mathbf x)} \frac{(v_z - u_{0,z}(\mathbf x))^2}{\hat v_{0,z}^2(\mathbf x)} \right]}
+        f_0(\mathbf x, \mathbf v) = \frac{n_0(\mathbf x)}{(\pi)^{3/2}\, \hat v_{0,1}(\mathbf x) \hat v_{0,2}(\mathbf x) \hat v_{0,3}(\mathbf x)} \,
+        \exp{\left[ - \frac{(v_1 - u_{0,1}(\mathbf x))^2}{\hat v_{0,1}^2(\mathbf x)}
+                      \frac{(v_2 - u_{0,2}(\mathbf x))^2}{\hat v_{0,2}^2(\mathbf x)}
+                      \frac{(v_3 - u_{0,3}(\mathbf x))^2}{\hat v_{0,3}^2(\mathbf x)} \right]}
 
     Parameters
     ----------
         x : array[float]
             Position at which to evaluate the Maxwellian.
 
         v : array[float]
             Velocity at which to evaluate the Maxwellian.
 
         moms_spec : array[int]
-            Specifier for the seven moments n0, u0x, u0y, u0z, vth0x, vth0y, vth0z (in this order).
+            Specifier for the seven moments n0, u01, u02, u03, vth01, vth02, vth03 (in this order).
             Is 0 for constant moment, for more see :meth:`kinetic_moments`.
 
         params : array[float]
             Parameters needed to specify the moments; the order is specified in :ref:`kinetic_moments` for the respective functions available.
 
     Notes
     -----
         See :meth:`kinetic_moments` for available moment functions.
 
         parameters.yml specifier: 0
     """
 
-    n0, u0x, u0y, u0z, vth0x, vth0y, vth0z = moments_kernels.moments(
+    n0, u01, u02, u03, vth01, vth02, vth03 = moments_kernels.moments(
         x, moms_spec, params)
 
-    Gx = exp(-(v[0] - u0x)**2 / (vth0x**2)) / (sqrt(pi)*vth0x)
-    Gy = exp(-(v[1] - u0y)**2 / (vth0y**2)) / (sqrt(pi)*vth0y)
-    Gz = exp(-(v[2] - u0z)**2 / (vth0z**2)) / (sqrt(pi)*vth0z)
+    g1 = exp(-(v[0] - u01)**2 / (vth01**2)) / (sqrt(pi) * vth01)
+    g2 = exp(-(v[1] - u02)**2 / (vth02**2)) / (sqrt(pi) * vth02)
+    g3 = exp(-(v[2] - u03)**2 / (vth03**2)) / (sqrt(pi) * vth03)
 
-    return n0*Gx*Gy*Gz
+    return n0 * g1 * g2 * g3
```

### Comparing `struphy-1.9.9/src/struphy/kinetic_background/moments_kernels.py` & `struphy-2.0.0/src/struphy/kinetic_background/moments_kernels.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,31 +3,34 @@
 from numpy import sin, cos
 
 
 def _docstring():
     '''MODULE DOCSTRING for :ref:`kinetic_moments`.
 
     The module contains pyccelized functions that can be used to specify moments of background distribution functions f0.
-    
-    The main method is :meth:`kinetic_moments.moments` at the end of the file, which calls the functions defined before.
-    
+
+    The main method is :math:`kinetic_moments.moments` at the end of the file, which calls the functions defined before.
+
     New functions must be added at the top of the file, right after the docstring. 
     In the "Note" of the new function you must state a **moment specifier**; this is an integer that identifies the function in 
-    the if-clause of :meth:`kinetic_moments.moments`.'''
+    the if-clause of :math:`kinetic_moments.moments`.'''
 
     print('This is just the docstring function.')
 
 
 @pure
-def modes_sin_cos(x: 'float', y: 'float', z: 'float', n_modes: 'int', kxs: 'float[:]', kys: 'float[:]', kzs: 'float[:]', amps_sin: 'float[:]', amps_cos: 'float[:]') -> float:
+def modes_sin_cos(x: 'float', y: 'float', z: 'float',
+                  n_modes: 'int',
+                  kxs: 'float[:]', kys: 'float[:]', kzs: 'float[:]',
+                  amps_sin: 'float[:]', amps_cos: 'float[:]') -> float:
     r'''
     Point-wise evaluation of  
-    
+
     .. math::
-    
+
         u(x, y, z) = \sum_{i=0}^N \left[ A_i\sin(k_{x,i}\,x + k_{y,i}\,y + k_{z,i}\,z) + B_i\cos(k_{x,i}\,x + k_{y,i}\,y + k_{z,i}\,z) \right]\,.
 
     Parameters
     ----------
         x,y,z : float
             Evaluation point.
 
@@ -52,20 +55,21 @@
     Notes
     -----
         Specifier: 1
     '''
 
     value = 0.
     for k in range(n_modes):
-        value += amps_sin[k]*sin( kxs[k]*x + kys[k]*y + kzs[k]*z ) + amps_cos[k]*cos( kxs[k]*x + kys[k]*y + kzs[k]*z )
+        value += amps_sin[k]*sin(kxs[k]*x + kys[k]*y + kzs[k]*z) + \
+            amps_cos[k]*cos(kxs[k]*x + kys[k]*y + kzs[k]*z)
 
     return value
 
 
-def moments(eta : 'float[:]', moms_spec : 'int[:]', params: 'float[:]'):
+def moments(eta: 'float[:]', moms_spec: 'int[:]', params: 'float[:]'):
     r"""
     Point-wise evaluation at logical (eta1, eta2, eta3) of the moments density, mean velocity and thermal velocity:
 
     .. math::
 
         n_0(\mathbf x) &= \int f_0(\mathbf x, \mathbf v)\,\textnormal d \mathbf v
 
@@ -73,219 +77,231 @@
 
         v_{\textnormal{th},0,i}(\mathbf x) &= \sqrt{\frac{1}{n_0(\mathbf x)} \int \mathbf |v_i - u_{0,i}|^2\, f_0(\mathbf x, \mathbf v)\,\textnormal d \mathbf v }
 
     Parameters
     ----------
         eta : array[float]
             Position at which to evaluate the moments.
-        
+
         moms_spec : array[int]
-            Specifier for the seven moments n0, u0x, u0y, u0z, vth0x, vth0y, vth0z (in this order).
+            Specifier for the seven moments n0, u01, u02, u03, vth01, vth02, vth03 (in this order).
             Is 0 for constant moment, for more see Notes.
 
         params : array[float]
             Parameters needed to specify the moments; the order is specified in :ref:`kinetic_moments` in the function's docstrings.
 
     Returns
     -------
         The function values at (eta1, eta2, eta3).
 
     Notes
     -----
         See :ref:`kinetic_moments` for available moment functions.
     """
 
-    ind = 0 # helps you count through params
+    ind = 0  # helps you count through params
 
     # density
-    if moms_spec[0] == 0: # constant value
+    if moms_spec[0] == 0:  # constant value
         n0 = params[ind]
         ind += 1
-    elif moms_spec[0] == 1: # modes_sin_cos
+    elif moms_spec[0] == 1:  # modes_sin_cos
         n_modes = int(params[ind])
         ind += 1
-        kxs = params[ind : ind + n_modes]
+        kxs = params[ind: ind + n_modes]
         ind += n_modes
-        kys = params[ind : ind + n_modes]
+        kys = params[ind: ind + n_modes]
         ind += n_modes
-        kzs = params[ind : ind + n_modes]
+        kzs = params[ind: ind + n_modes]
         ind += n_modes
-        amps_sin = params[ind : ind + n_modes]
+        amps_sin = params[ind: ind + n_modes]
         ind += n_modes
-        amps_cos = params[ind : ind + n_modes]
+        amps_cos = params[ind: ind + n_modes]
         ind += n_modes
-        n0 = modes_sin_cos(eta[0], eta[1], eta[2], n_modes, kxs, kys, kzs, amps_sin, amps_cos)
+        n0 = modes_sin_cos(eta[0], eta[1], eta[2], n_modes,
+                           kxs, kys, kzs, amps_sin, amps_cos)
     else:
         print('Invalid moms_spec[0]', moms_spec[0])
 
     # x-momentum
-    if moms_spec[1] == 0: # constant value
-        u0x = params[ind]
+    if moms_spec[1] == 0:  # constant value
+        u01 = params[ind]
         ind += 1
-    elif moms_spec[1] == 1: # modes_sin_cos
+    elif moms_spec[1] == 1:  # modes_sin_cos
         n_modes = int(params[ind])
         ind += 1
-        kxs = params[ind : ind + n_modes]
+        kxs = params[ind: ind + n_modes]
         ind += n_modes
-        kys = params[ind : ind + n_modes]
+        kys = params[ind: ind + n_modes]
         ind += n_modes
-        kzs = params[ind : ind + n_modes]
+        kzs = params[ind: ind + n_modes]
         ind += n_modes
-        amps_sin = params[ind : ind + n_modes]
+        amps_sin = params[ind: ind + n_modes]
         ind += n_modes
-        amps_cos = params[ind : ind + n_modes]
+        amps_cos = params[ind: ind + n_modes]
         ind += n_modes
-        u0x = modes_sin_cos(eta[0], eta[1], eta[2], n_modes, kxs, kys, kzs, amps_sin, amps_cos)
+        u01 = modes_sin_cos(eta[0], eta[1], eta[2],
+                            n_modes, kxs, kys, kzs, amps_sin, amps_cos)
     else:
         print('Invalid moms_spec[1]', moms_spec[1])
 
     # y-momentum
-    if moms_spec[2] == 0: # constant value
-        u0y = params[ind]
+    if moms_spec[2] == 0:  # constant value
+        u02 = params[ind]
         ind += 1
-    elif moms_spec[2] == 1: # modes_sin_cos
+    elif moms_spec[2] == 1:  # modes_sin_cos
         n_modes = int(params[ind])
         ind += 1
-        kxs = params[ind : ind + n_modes]
+        kxs = params[ind: ind + n_modes]
         ind += n_modes
-        kys = params[ind : ind + n_modes]
+        kys = params[ind: ind + n_modes]
         ind += n_modes
-        kzs = params[ind : ind + n_modes]
+        kzs = params[ind: ind + n_modes]
         ind += n_modes
-        amps_sin = params[ind : ind + n_modes]
+        amps_sin = params[ind: ind + n_modes]
         ind += n_modes
-        amps_cos = params[ind : ind + n_modes]
+        amps_cos = params[ind: ind + n_modes]
         ind += n_modes
-        u0y = modes_sin_cos(eta[0], eta[1], eta[2], n_modes, kxs, kys, kzs, amps_sin, amps_cos)
+        u02 = modes_sin_cos(eta[0], eta[1], eta[2],
+                            n_modes, kxs, kys, kzs, amps_sin, amps_cos)
     else:
         print('Invalid moms_spec[2]', moms_spec[2])
 
     # z-momentum
-    if moms_spec[3] == 0: # constant value
-        u0z = params[ind]
+    if moms_spec[3] == 0:  # constant value
+        u03 = params[ind]
         ind += 1
-    elif moms_spec[3] == 1: # modes_sin_cos
+    elif moms_spec[3] == 1:  # modes_sin_cos
         n_modes = int(params[ind])
         ind += 1
-        kxs = params[ind : ind + n_modes]
+        kxs = params[ind: ind + n_modes]
         ind += n_modes
-        kys = params[ind : ind + n_modes]
+        kys = params[ind: ind + n_modes]
         ind += n_modes
-        kzs = params[ind : ind + n_modes]
+        kzs = params[ind: ind + n_modes]
         ind += n_modes
-        amps_sin = params[ind : ind + n_modes]
+        amps_sin = params[ind: ind + n_modes]
         ind += n_modes
-        amps_cos = params[ind : ind + n_modes]
+        amps_cos = params[ind: ind + n_modes]
         ind += n_modes
-        u0z = modes_sin_cos(eta[0], eta[1], eta[2], n_modes, kxs, kys, kzs, amps_sin, amps_cos)
+        u03 = modes_sin_cos(eta[0], eta[1], eta[2],
+                            n_modes, kxs, kys, kzs, amps_sin, amps_cos)
     else:
         print('Invalid moms_spec[3]', moms_spec[3])
 
     # x-thermal velocity
-    if moms_spec[4] == 0: # constant value
-        vth0x = params[ind]
+    if moms_spec[4] == 0:  # constant value
+        vth01 = params[ind]
         ind += 1
-    elif moms_spec[4] == 1: # modes_sin_cos
+    elif moms_spec[4] == 1:  # modes_sin_cos
         n_modes = int(params[ind])
         ind += 1
-        kxs = params[ind : ind + n_modes]
+        kxs = params[ind: ind + n_modes]
         ind += n_modes
-        kys = params[ind : ind + n_modes]
+        kys = params[ind: ind + n_modes]
         ind += n_modes
-        kzs = params[ind : ind + n_modes]
+        kzs = params[ind: ind + n_modes]
         ind += n_modes
-        amps_sin = params[ind : ind + n_modes]
+        amps_sin = params[ind: ind + n_modes]
         ind += n_modes
-        amps_cos = params[ind : ind + n_modes]
+        amps_cos = params[ind: ind + n_modes]
         ind += n_modes
-        vth0x = modes_sin_cos(eta[0], eta[1], eta[2], n_modes, kxs, kys, kzs, amps_sin, amps_cos)
+        vth01 = modes_sin_cos(eta[0], eta[1], eta[2],
+                              n_modes, kxs, kys, kzs, amps_sin, amps_cos)
     else:
         print('Invalid moms_spec[4]', moms_spec[4])
 
     # y-thermal velocity
-    if moms_spec[5] == 0: # constant value
-        vth0y = params[ind]
+    if moms_spec[5] == 0:  # constant value
+        vth02 = params[ind]
         ind += 1
-    elif moms_spec[5] == 1: # modes_sin_cos
+    elif moms_spec[5] == 1:  # modes_sin_cos
         n_modes = int(params[ind])
         ind += 1
-        kxs = params[ind : ind + n_modes]
+        kxs = params[ind: ind + n_modes]
         ind += n_modes
-        kys = params[ind : ind + n_modes]
+        kys = params[ind: ind + n_modes]
         ind += n_modes
-        kzs = params[ind : ind + n_modes]
+        kzs = params[ind: ind + n_modes]
         ind += n_modes
-        amps_sin = params[ind : ind + n_modes]
+        amps_sin = params[ind: ind + n_modes]
         ind += n_modes
-        amps_cos = params[ind : ind + n_modes]
+        amps_cos = params[ind: ind + n_modes]
         ind += n_modes
-        vth0y = modes_sin_cos(eta[0], eta[1], eta[2], n_modes, kxs, kys, kzs, amps_sin, amps_cos)
+        vth02 = modes_sin_cos(eta[0], eta[1], eta[2],
+                              n_modes, kxs, kys, kzs, amps_sin, amps_cos)
     else:
         print('Invalid moms_spec[5]', moms_spec[5])
 
     # z-thermal velocity
-    if moms_spec[6] == 0: # constant value
-        vth0z = params[ind]
+    if moms_spec[6] == 0:  # constant value
+        vth03 = params[ind]
         ind += 1
-    elif moms_spec[6] == 1: # modes_sin_cos
+    elif moms_spec[6] == 1:  # modes_sin_cos
         n_modes = int(params[ind])
         ind += 1
-        kxs = params[ind : ind + n_modes]
+        kxs = params[ind: ind + n_modes]
         ind += n_modes
-        kys = params[ind : ind + n_modes]
+        kys = params[ind: ind + n_modes]
         ind += n_modes
-        kzs = params[ind : ind + n_modes]
+        kzs = params[ind: ind + n_modes]
         ind += n_modes
-        amps_sin = params[ind : ind + n_modes]
+        amps_sin = params[ind: ind + n_modes]
         ind += n_modes
-        amps_cos = params[ind : ind + n_modes]
+        amps_cos = params[ind: ind + n_modes]
         ind += n_modes
-        vth0z = modes_sin_cos(eta[0], eta[1], eta[2], n_modes, kxs, kys, kzs, amps_sin, amps_cos)
+        vth03 = modes_sin_cos(eta[0], eta[1], eta[2],
+                              n_modes, kxs, kys, kzs, amps_sin, amps_cos)
     else:
         print('Invalid moms_spec[6]', moms_spec[6])
 
-    return n0, u0x, u0y, u0z, vth0x, vth0y, vth0z
+    return n0, u01, u02, u03, vth01, vth02, vth03
 
 
-def array_moments(eta : 'float[:,:]', moms_spec : 'int[:]', params : 'float[:]', n0 : 'float[:]', u0x : 'float[:]', u0y : 'float[:]', u0z : 'float[:]', vth0x : 'float[:]', vth0y : 'float[:]', vth0z : 'float[:]'):
+def array_moments(eta: 'float[:,:]',
+                  moms_spec: 'int[:]', params: 'float[:]',
+                  n0: 'float[:]',
+                  u01: 'float[:]', u02: 'float[:]', u03: 'float[:]',
+                  vth01: 'float[:]', vth02: 'float[:]', vth03: 'float[:]'):
     r"""
     Point-wise evaluation at every (ip) logical particle positions (eta1, eta2, eta3) of the moments density, mean velocity and thermal velocity:
 
     Parameters
     ----------
         eta : rank2 array[float]
             Array of every particle positions at which to evaluate the moments.
-        
+
         moms_spec : array[int]
-            Specifier for the seven moments n0, u0x, u0y, u0z, vth0x, vth0y, vth0z (in this order).
+            Specifier for the seven moments n0, u01, u02, u03, vth01, vth02, vth03 (in this order).
 
         params : array[float]
             Parameters needed to specify the moments; the order is specified in :ref:`kinetic_moments` in the function's docstrings.
-        
+
         n0    : array[float]
             Array of density moment at ip.
 
-        u0x   : array[float]
+        u01   : array[float]
             Array of 1st comp of mean velocity at ip.
 
-        u0y   : array[float]
-            Array of 2st comp of mean velocity at ip.
+        u02   : array[float]
+            Array of 2nd comp of mean velocity at ip.
 
-        u0z   : array[float]
-            Array of 2st comp of mean velocity at ip.
+        u03   : array[float]
+            Array of 3rd comp of mean velocity at ip.
 
-        vth0x : array[float]
+        vth01 : array[float]
             Array of 1st comp of thermal velocity at ip.
 
-        vth0y : array[float]
-            Array of 1st comp of thermal velocity at ip.
-            
-        vth0z : array[float]
-            Array of 1st comp of thermal velocity at ip.
-    
+        vth02 : array[float]
+            Array of 2nd comp of thermal velocity at ip.
+
+        vth03 : array[float]
+            Array of 3rd comp of thermal velocity at ip.
+
     Notes
     -----
         See :ref:`kinetic_moments` for available moment functions.
     """
 
-    for ip in range(len(eta[:,0])):
-        n0[ip], u0x[ip], u0y[ip], u0z[ip], vth0x[ip], vth0y[ip], vth0z[ip] = moments(eta[ip,:], moms_spec, params)
+    for ip in range(len(eta[:, 0])):
+        n0[ip], u01[ip], u02[ip], u03[ip], vth01[ip], vth02[ip], vth03[ip] = moments(
+            eta[ip, :], moms_spec, params)
```

### Comparing `struphy-1.9.9/src/struphy/linear_algebra/core.py` & `struphy-2.0.0/src/struphy/linear_algebra/core.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/linear_algebra/iterative_solvers.py` & `struphy-2.0.0/src/struphy/linear_algebra/iterative_solvers.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/linear_algebra/linalg_kron.py` & `struphy-2.0.0/src/struphy/linear_algebra/linalg_kron.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/linear_algebra/schur_solver.py` & `struphy-2.0.0/src/struphy/linear_algebra/schur_solver.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/linear_algebra/stencil_dot_kernels.py` & `struphy-2.0.0/src/struphy/linear_algebra/stencil_dot_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/linear_algebra/stencil_transpose_kernels.py` & `struphy-2.0.0/src/struphy/linear_algebra/stencil_transpose_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/models/base.py` & `struphy-2.0.0/src/struphy/models/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                 val['kinetic_data']['markers'][:n_markers_on_proc] = val['obj'].markers[markers_on_proc]
 
     def update_distr_function(self):
         '''
         Writes distribution function slices that are supposed to be saved into corresponding array.
         '''
 
-        dim_to_int = {'e1': 0, 'e2': 1, 'e3': 2, 'vx': 3, 'vy': 4, 'vz': 5}
+        dim_to_int = {'e1': 0, 'e2': 1, 'e3': 2, 'v1': 3, 'v2': 4, 'v3': 5}
 
         for val in self.kinetic.values():
 
             if 'f' in val['params']['save_data']:
 
                 for slice_i, edges in val['bin_edges'].items():
 
@@ -282,23 +282,23 @@
 
         # initialize particles
         if len(self.kinetic) > 0:
 
             for val in self.kinetic.values():
                 val['obj'].mpi_sort_markers(do_test=True)
 
-                if val['params']['markers']['type'] == 'full_f':
+                typ = val['params']['markers']['type']
+                if typ == 'full_f':
                     val['obj'].initialize_weights(val['params']['init'])
-                elif val['params']['markers']['type'] == 'delta_f':
+                elif typ == 'delta_f':
                     val['obj'].initialize_weights(val['params']['init'])
-                elif val['params']['markers']['type'] == 'control_variate':
+                elif typ == 'control_variate':
                     val['obj'].initialize_weights(
                         val['params']['init'], val['params']['background'])
                 else:
-                    typ = val['params']['markers']['type']
                     raise NotImplementedError(
                         f'Type {typ} for distribution function is not known!')
 
                 if val['space'] == 'Particles5D':
                     val['obj'].save_magnetic_moment(self.derham)
 
     def initialize_from_restart(self, data):
@@ -531,15 +531,15 @@
                 Z_bulk = params['kinetic'][cls.bulk_species()
                                            ]['phys_params']['Z']
                 A_bulk = params['kinetic'][cls.bulk_species()
                                            ]['phys_params']['A']
 
             # compute units
             units_basic, units_der, units_dimless = derive_units(
-                Z_bulk, A_bulk, params['units']['x'], params['units']['x'], params['units']['n'], cls.timescale())
+                Z_bulk, A_bulk, params['units']['x'], params['units']['B'], params['units']['n'], cls.timescale())
 
             if verbose:
                 print(f'Unit of time:'.ljust(25),
                       '{:4.3e}'.format(units_basic['t']) + ' s')
                 print(f'Unit of velocity:'.ljust(25),
                       '{:4.3e}'.format(units_der['v']) + ' m/s')
                 print(f'Unit of magnetic field:'.ljust(25),
@@ -553,57 +553,19 @@
                 print(f'Unit of pressure:'.ljust(25),
                       '{:4.3e}'.format(units_der['p'] * 1e-5) + ' bar')
 
                 # dimensionless quantities
                 print('\nRelevant dimensionless quantities:')
                 print(f'alpha:'.ljust(25), '{:7.3f}'.format(
                     units_dimless['alpha']))
+                print(f'kappa:'.ljust(25), '{:7.3f}'.format(
+                    units_dimless['kappa']))
 
             return units_basic, units_der, units_dimless
 
-    # def print_species_params(self):
-    #    '''Compute and print plasma parameters for each species of the model.
-    #    Computed are min, max and volume average of
-    #
-    #        - pressure
-    #        - temperature
-    #        - thermal speed
-    #        - Alfven speed
-    #        - plasma frequency
-    #        - cyclotron frequency
-    #        - transit frequency
-    #        - Alfven frequency
-    #    '''
-#
-    #    species_params = {}
-#
-    #    # plasma size
-    #    h = 1/20
-    #    eta1 = np.linspace(h/2., 1.-h/2., 20)
-    #    eta2 = np.linspace(h/2., 1.-h/2., 20)
-    #    eta3 = np.linspace(h/2., 1.-h/2., 20)
-    #
-    #    plasma_volume = np.mean(
-    #        np.abs(self.domain.jacobian_det(eta1, eta2, eta3)))
-    #
-    #    transit_length = plasma_volume**(1/3)
-    #
-    #    species_params['plasma volume'] = plasma_volume
-    #    species_params['transit length'] = transit_length
-#
-    #    # physics constants
-    #    e = 1.602176634e-19  # elementary charge (C)
-    #    m_p = 1.67262192369e-27  # proton mass (kg)
-    #    mu0 = 1.25663706212e-6  # magnetic constant (N*A^-2)
-    #    eps0 = 8.8541878128e-12  # vacuum permittivity (F*m^-1)
-    #    kB = 1.380649e-23  # Boltzmann constant (J*K^-1)
-    #
-    #    # species parameters
-    #    # TODO
-
     ###################
     # Private methods :
     ###################
 
     def _init_variable_dicts(self):
         """
         Initialize em-fields, fluid and kinetic dictionaries for information on the model variables.
@@ -804,30 +766,31 @@
 
         h = 1/20
         eta1 = np.linspace(h/2., 1.-h/2., 20)
         eta2 = np.linspace(h/2., 1.-h/2., 20)
         eta3 = np.linspace(h/2., 1.-h/2., 20)
 
         # global parameters
+        # plasma volume (hat x^3)
+        vol1 = np.mean(np.abs(self.domain.jacobian_det(eta1, eta2, eta3))) 
         # plasma volume (m⁻³)
-        plasma_volume = np.mean(np.abs(self.domain.jacobian_det(eta1, eta2, eta3))) \
-            * units_basic['x']**3
+        plasma_volume = vol1 * units_basic['x']**3
         # transit length (m)
         transit_length = plasma_volume**(1/3)
         # magnetic field (T)
         magnetic_field = np.mean(self.mhd_equil.absB0(eta1, eta2, eta3)
                                  * np.abs(self.domain.jacobian_det(eta1, eta2, eta3))) \
-            / plasma_volume*units_basic['B']
+            / vol1 * units_basic['B']
 
         print('\nGlobal characteristics of the simulation:')
         print(f'Plasma volume:'.ljust(25),
               '{:4.3e}'.format(plasma_volume) + units['plasma volume'])
         print(f'Transit length:'.ljust(25),
               '{:4.3e}'.format(transit_length) + units['transit length'])
-        print(f'Magnetic field:'.ljust(25),
+        print(f'Volume-averaged magnetic field:'.ljust(25),
               '{:4.3e}'.format(magnetic_field) + units['magnetic field'])
 
         # species dependent parameters
         if len(self.fluid) > 0:
 
             for species, val in self.fluid.items():
                 characteristics[species] = {}
```

### Comparing `struphy-1.9.9/src/struphy/models/main.py` & `struphy-2.0.0/src/struphy/models/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 def main(model_name, parameters, path_out, restart=False, runtime=300, save_step=1):
     """
     Run a Struphy model.
 
     Parameters
     ----------
     model_name : str
-        The name of the model to run.
+        The name of the model to run. Type "struphy run --help" in your terminal to see a list of available models.
 
     parameters : dict | str
         The simulation parameters. Can either be a dictionary OR a string (path of .yml parameter file)
 
     path_out : str
         The output directory. Will create a folder if it does not exist OR cleans the folder for new runs.
 
@@ -19,21 +19,20 @@
     runtime : int, optional
         Maximum run time of simulation in minutes. Will finish the time integration once this limit is reached (default=300).
 
     save_step : int, optional
         When to save data output: every time step (save_step=1), every second time step (save_step=2), etc (default=1).
     """
 
-    from struphy.models import models
+    from struphy.models import fluid, kinetic, hybrid, toy
     from struphy.models.utilities import pre_processing
     from struphy.models.output_handling import DataContainer
 
     import numpy as np
     import time
-    import yaml
 
     from mpi4py import MPI
 
     comm = MPI.COMM_WORLD
     rank = comm.Get_rank()
     size = comm.Get_size()
 
@@ -47,15 +46,20 @@
                             path_out,
                             restart,
                             runtime,
                             rank,
                             size)
 
     # instantiate STRUPHY model (will only allocate model objects and associated memory)
-    model = getattr(models, model_name)(params, comm)
+    objs = [fluid, kinetic, hybrid, toy]
+    for obj in objs:
+        try:
+            model = getattr(obj, model_name)(params, comm)
+        except AttributeError: 
+            pass
 
     # print plasma parameters to screen
     if rank == 0:
         model.print_plasma_params()
 
     # data object for saving (will either create new hdf5 files if restart==False or open existing files if restart==True)
     data = DataContainer(path_out, comm=comm)
@@ -69,21 +73,29 @@
     for key, val in time_state.items():
         key_time = 'time/' + key
         key_time_restart = 'restart/time/' + key
         data.add_data({key_time: val})
         data.add_data({key_time_restart: val})
 
     # start a new simulation (set initial conditions according to parameter file)
+    time_params = params['time']
+
     if not restart:
         model.initialize_from_params()
+        total_steps = str(
+            int(round(time_params['Tend']/time_params['dt'])))
 
     # restart of an existing simulation (overwrite time quantities and load restart data from hdf5 files)
     else:
         time_state['value'][0] = data.file['restart/time/value'][-1]
         time_state['index'][0] = data.file['restart/time/index'][-1]
+
+        total_steps = str(
+            int(round((time_params['Tend'] - time_state['value'][0])/time_params['dt'])))
+
         model.initialize_from_restart(data)
 
     # list of model methods for diagnostics
     model_updates = []
     for method in dir(model):
         if 'update' in method:
             model_updates.append(getattr(model, method))
@@ -96,16 +108,14 @@
     save_keys_all, save_keys_end = model.initialize_data_output(data, size)
 
     if rank == 0:
         print('\nInitial time series saved.')
         model.print_scalar_quantities()
 
     # ======================== main time loop ======================
-    time_params = params['time']
-
     if rank == 0:
         split_algo = time_params['split_algo']
         print(
             f'\nStart time integration with {split_algo} splitting algorithm')
         print()
 
     # time loop
@@ -149,69 +159,73 @@
 
             # extract FEM coefficients
             for key, val in model.em_fields.items():
                 if 'params' not in key:
                     # in-place extraction of FEM coefficients from field.vector --> field.vector_stencil!
                     val['obj'].extract_coeffs(update_ghost_regions=False)
 
-            for species, val in model.fluid.items():
+            for _, val in model.fluid.items():
                 for variable, subval in val.items():
                     if 'params' not in variable:
                         # in-place extraction of FEM coefficients from field.vector --> field.vector_stencil!
                         subval['obj'].extract_coeffs(
                             update_ghost_regions=False)
 
             # save data (everything but restart data)
             data.save_data(keys=save_keys_all)
 
             # print current time and scalar quantities to screen
             if rank == 0:
-                total_steps = str(
-                    int(round(time_params['Tend']/time_params['dt'])))
                 step = str(time_state['index'][0]).zfill(len(total_steps))
 
-                message = 'time: {:15.11f}'.format(time_state['value'][0])
-                message += ' | ' + 'time step: ' + step
-                message += ' | ' + 'final time: ' + str(time_params['Tend'])
+                message = 'time: {0:12.8f}/{1:12.8f}'.format(time_state['value'][0], time_params['Tend'])
+                message += ' | ' + 'time step: ' + step + '/' + str(total_steps) 
 
                 print(message, end='\n')
                 model.print_scalar_quantities()
                 print()
     # ===================================================================
 
+    with open(path_out + '/meta.txt', 'a') as f:
+        f.write('wall-clock time [min]:'.ljust(30) +
+                str((end_simulation - start_simulation)/60.) + '\n')
+
 
 if __name__ == '__main__':
 
     import argparse
     import os
     import struphy
 
     libpath = struphy.__path__[0]
+    
+    with open(os.path.join(libpath, 'io_path.txt')) as f:
+        io_path = f.readlines()[0]
 
     parser = argparse.ArgumentParser(description='Run an Struphy model.')
 
     # model
     parser.add_argument('model',
                         type=str,
                         metavar='model',
                         help='the name of the model to run (default=Maxwell)')
 
     # input (absolute path)
     parser.add_argument('-i', '--input',
                         type=str,
                         metavar='FILE',
                         help='absolute path of parameter file (.yml) (default=<struphy_path>/io/inp/parameters.yml)',
-                        default=os.path.join(libpath, 'io/inp/parameters.yml'))
+                        default=os.path.join(io_path, 'io/inp/parameters.yml'))
 
     # output (absolute path)
     parser.add_argument('-o', '--output',
                         type=str,
                         metavar='DIR',
                         help='absolute path of output folder (default=<struphy_path>/io/out/sim_1)',
-                        default=os.path.join(libpath, 'io/out/sim_1'))
+                        default=os.path.join(io_path, 'io/out/sim_1'))
 
     # restart
     parser.add_argument('-r', '--restart',
                         help='restart the simulation in the output folder specified under -o',
                         action='store_true')
 
     # runtime
```

### Comparing `struphy-1.9.9/src/struphy/models/output_handling.py` & `struphy-2.0.0/src/struphy/models/output_handling.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,40 +34,41 @@
         else:
             if file_name.find(".hdf5") == -1:
                 self._file_name = file_name + '.hdf5'
             else:
                 self._file_name = file_name
 
         # file path
-        file_path = os.path.join(path_out, self._file_name)
-        
+        file_path = os.path.join(path_out, 'data/', self._file_name)
+
         # check if file already exists
         file_exists = os.path.exists(file_path)
-        
+
         # open/create file
         self._file = h5py.File(file_path, 'a')
-        
+
         # dictionary with pairs (dataset key : object ID)
         self._dset_dict = {}
-        
+
         # get dataset keys if file already exists and set None object IDs
         if file_exists:
             dataset_keys = []
 
-            self._file.visit(lambda key : dataset_keys.append(key) if isinstance(self._file[key], h5py.Dataset) else None)
+            self._file.visit(lambda key: dataset_keys.append(
+                key) if isinstance(self._file[key], h5py.Dataset) else None)
 
             for key in dataset_keys:
                 self._dset_dict[key] = None
 
     @property
     def file_name(self):
         """ The hdf5 file name.
         """
         return self._file_name
-    
+
     @property
     def file(self):
         """ The hdf5 file.
         """
         return self._file
 
     @property
@@ -88,29 +89,29 @@
 
         for key, val in data_dict.items():
 
             assert isinstance(val, np.ndarray)
 
             # if dataset already exists, check for compatibility with given array
             if key in self._dset_dict:
-                
+
                 dataset_shape = self.file[key].shape
-                
+
                 # scalar values are saved as 1d arrays of size 1
                 if len(dataset_shape) == 1:
                     assert val.ndim == 1, 'for scalar quantities, a 1d array with a single entry must used!'
                     assert val.size == 1, 'for scalar quantities, a 1d array with a single entry must used!'
-                
+
                 # other values
                 else:
                     assert dataset_shape[1:] == val.shape
-                
+
             # create new dataset otherwise and save array
             else:
-            
+
                 # scalar values are saved as 1d arrays of size 1
                 if val.size == 1:
                     assert val.ndim == 1
                     self._file.create_dataset(
                         key, (1,), maxshape=(None,), dtype=val.dtype, chunks=True)
                     self._file[key][0] = val[0]
                 else:
```

### Comparing `struphy-1.9.9/src/struphy/models/utilities.py` & `struphy-2.0.0/src/struphy/models/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import numpy as np
 
 
 def derive_units(Z_bulk=1, A_bulk=1., x=1., B=1., n=1., time_scale='alfvén'):
     """
     Computes derived physics units of Struphy quantities.
-    
+
     Parameters
     ---------
     Z_bulk : int
         Charge number of bulkd species.
-        
+
     A_bulk : int
         Mass number of bulk species.
-        
+
     x : float
         Unit of length (in meters).
-        
+
     B : float
         Unit of magnetic field (in Tesla).
-        
+
     n : float
         Unit of particle number density (in 1e20 per cubic meter).
-        
+
     time_scale : str
         Time scale to be used (determined by some characteristic velocity: "alfvén", "cyclotron" or "light").
-        
+
     Returns
     -------
     units_basic : dict
         Basic units for time, length, mass and magnetic field.
-        
+
     units_der : dict
         Derived units for velocity, pressure, mass density and particle density.
-        
+
     units_dimless :  dict
         Some dimensionless quantities:
             * alpha = omega_p / omega_c, ratio of bulk plasma to bulk cyclotron frequency.
     """
 
     # physics constants
     e = 1.602176634e-19  # elementary charge (C)
@@ -46,49 +46,51 @@
     kB = 1.380649e-23  # Boltzmann constant (J/K)
     c = 299792458  # speed of light (m/s)
 
     # prescribed units
     x_unit = x * 1
     B_unit = B * 1
     n_unit = n * 1e20
-    
+
     # basic units in SI units (time, length, particle density and magnetic field)
     units_basic = {}
-    
+
     if time_scale == 'light':
         v_unit = 1*c
     elif time_scale == 'alfvén':
         v_unit = B_unit / np.sqrt(n_unit * A_bulk * mH * mu0)
     elif time_scale == 'cyclotron':
         v_unit = Z_bulk * e * B_unit / (A_bulk * mH) / (2*np.pi) * x_unit
-    
+
     units_basic['t'] = x_unit / v_unit
     units_basic['x'] = x_unit
     units_basic['m'] = A_bulk * mH * n_unit * x_unit**3
     units_basic['B'] = B_unit
-       
+
     # derived units
     units_der = {}
 
     units_der['v'] = units_basic['x'] / units_basic['t']
-    units_der['p'] = units_basic['m'] / (units_basic['x'] * units_basic['t']**2)
+    units_der['p'] = units_basic['m'] / \
+        (units_basic['x'] * units_basic['t']**2)
     units_der['rho'] = units_basic['m'] / units_basic['x']**3
     units_der['n'] = units_basic['m'] / units_basic['x']**3 / (A_bulk * mH)
-    
+
     # relevant dimensionless quantities
     units_dimless = {}
-    
+
     # unit of bulk plasma frequency
     omega_p = np.sqrt(n_unit * (Z_bulk * e)**2 / (eps0 * A_bulk * mH))
 
     # unit of bulk cyclotron frequency
     omega_c = Z_bulk * e * B_unit / (A_bulk * mH)
 
     # relevant unit parameters
     units_dimless['alpha'] = omega_p / omega_c
+    units_dimless['kappa'] = omega_c * units_basic['t']
 
     return units_basic, units_der, units_dimless
 
 
 def setup_domain_mhd(params):
     """
     Creates the domain object and MHD equilibrium for a given parameter file.
@@ -147,72 +149,73 @@
 
     return domain, mhd
 
 
 def setup_electric_background(params, domain):
     """
     Creates an electric background field for a given parameter file.
-    
+
     Parameters
     ----------
     params : dict
         The full simulation parameter dictionary.
-        
+
     domain : struphy.geometry.base.Domain
         The Struphy domain object for evaluating the mapping F : [0, 1]^3 --> R^3 and the corresponding metric coefficients.
-        
+
     Returns
     -------
     electric_background : struphy.fields_background.electric_equil.base.EquilibriumElectric
         The electric background object.
     """
-    
+
     from struphy.fields_background.electric_equil import analytical
-        
+
     if 'electric_equilibrium' in params:
-        
+
         electric_type = params['electric_equilibrium']['type']
         electric_class = getattr(analytical, electric_type)
-        electric_background = electric_class(params['electric_equilibrium'][electric_type], domain)
-        
+        electric_background = electric_class(
+            params['electric_equilibrium'][electric_type], domain)
+
     else:
         electric_background = None
-        
+
     return electric_background
 
 
 def setup_derham(params_grid, comm, domain=None, mpi_dims_mask=None):
     """
     Creates the 3d derham sequence for given grid parameters.
-    
+
     Parameters
     ----------
     params_grid : dict
         Grid parameters dictionary.
-        
+
     comm : mpi4py.MPI.Intracomm
         MPI communicator used for parallelization.
-        
+
     domain : struphy.geometry.base.Domain, optional
         The Struphy domain object for evaluating the mapping F : [0, 1]^3 --> R^3 and the corresponding metric coefficients.
-        
+
     mpi_dims_mask: list of bool
         True if the dimension is to be used in the domain decomposition (=default for each dimension). 
         If mpi_dims_mask[i]=False, the i-th dimension will not be decomposed.
-        
+
     Returns
     -------
     derham : struphy.psydac_api.psydac_derham.Derham
         Discrete de Rham sequence on the logical unit cube.
     """
 
     from struphy.psydac_api.psydac_derham import Derham
 
     # number of grid cells
-    Nel = params_grid['Nel']  
+    Nel = params_grid['Nel']
     # spline degrees
     p = params_grid['p']
     # spline types (clamped vs. periodic)
     spl_kind = params_grid['spl_kind']
     # boundary conditions (Homogeneous Dirichlet or None)
     bc = params_grid['bc']
     # Number of quadrature points per histopolation cell
@@ -229,18 +232,19 @@
     derham = Derham(Nel, p, spl_kind, bc,
                     quad_order=quad_order,
                     nq_pr=nq_pr,
                     comm=comm,
                     mpi_dims_mask=mpi_dims_mask,
                     with_projectors=True,
                     polar_ck=polar_ck,
-                    domain=domain)   
+                    domain=domain)
 
     if comm.Get_rank() == 0:
-        print('MPI processes per direction:', derham.domain_decomposition.nprocs)
+        print('MPI processes per direction:',
+              derham.domain_decomposition.nprocs)
         print('')
 
     return derham
 
 
 def pre_processing(model_name, parameters, path_out, restart, max_sim_time, mpi_rank, mpi_size):
     """
@@ -272,24 +276,26 @@
 
     import os
     import shutil
     import datetime
     import sysconfig
     import glob
     import yaml
-    from struphy.models import models
+    from struphy.models import fluid, kinetic, hybrid, toy
 
     # prepare output folder
     if mpi_rank == 0:
         print('')
 
         # create output folder if it does not exit
         if not os.path.exists(path_out):
             os.mkdir(path_out)
             print('\nCreated folder ' + path_out)
+            os.mkdir(os.path.join(path_out, 'data/'))
+            print('\nCreated folder ' + os.path.join(path_out, 'data/'))
 
         # clean output folder if it already exists
         else:
 
             # remove post_processing folder
             folder = os.path.join(path_out, 'post_processing')
             if os.path.exists(folder):
@@ -304,20 +310,26 @@
 
             # remove profiling file
             file = os.path.join(path_out, 'profile_tmp')
             if os.path.exists(file):
                 os.remove(file)
                 print('Removed file ' + file)
 
-            # remove hdf5 files (if NOT a restart)
+            # remove .png files (if NOT a restart)
             if not restart:
-                files = glob.glob(os.path.join(path_out, '*.hdf5'))
+                files = glob.glob(os.path.join(path_out, '*.png'))
+                for n, file in enumerate(files):
+                    os.remove(file)
+                    if n < 10:  # print only ten statements in case of many processes
+                        print('Removed file ' + file)
+                        
+                files = glob.glob(os.path.join(path_out, 'data', '*.hdf5'))
                 for n, file in enumerate(files):
                     os.remove(file)
-                    if n < 10:  # print only forty statements in case of many processes
+                    if n < 10:  # print only ten statements in case of many processes
                         print('Removed file ' + file)
 
     # save "parameters" dictionary as .yml file
     if isinstance(parameters, dict):
         parameters_path = os.path.join(path_out, 'parameters.yml')
 
         # write parameters to file and save it in output folder
@@ -327,20 +339,20 @@
             params_file.close()
 
         params = parameters
 
     # OR load parameters if "parameters" is a string (path)
     else:
         parameters_path = parameters
-        
+
         with open(parameters) as file:
             params = yaml.load(file, Loader=yaml.FullLoader)
 
     if mpi_rank == 0:
-        
+
         # copy parameter file to output folder
         if parameters_path != os.path.join(path_out, 'parameters.yml'):
             shutil.copy2(parameters_path, os.path.join(
                 path_out, 'parameters.yml'))
 
         # print simulation info
         print('')
@@ -365,15 +377,21 @@
         print(f'spline degrees      :', params['grid']['p'])
         print(f'periodic bcs        :', params['grid']['spl_kind'])
         print(f'hom. Dirichlet bc   :', params['grid']['bc'])
         print(f'GL quad pts (L2)    :', params['grid']['nq_el'])
         print(f'GL quad pts (hist)  :', params['grid']['nq_pr'])
 
         # print units info
-        getattr(models, model_name).model_units(params, verbose=True)
+        objs = [fluid, kinetic, hybrid, toy]
+        for obj in objs:
+            try:
+                model = getattr(obj, model_name)
+            except:
+                pass
+        model.model_units(params, verbose=True)
         print('')
 
         # write meta data to output folder
         with open(path_out + '/meta.txt', 'w') as f:
             f.write('date of simulation: '.ljust(30) +
                     str(datetime.datetime.now()) + '\n')
             f.write('platform: '.ljust(30) + sysconfig.get_platform() + '\n')
@@ -381,10 +399,9 @@
                     sysconfig.get_python_version() + '\n')
             f.write('model_name: '.ljust(30) + model_name + '\n')
             f.write('processes: '.ljust(30) + str(mpi_size) + '\n')
             f.write('output folder:'.ljust(30) + path_out + '\n')
             f.write('restart:'.ljust(30) + str(restart) + '\n')
             f.write(
                 'max wall-clock time [min]:'.ljust(30) + str(max_sim_time) + '\n')
-            f.write('# processes: '.ljust(30) + str(mpi_size) + '\n')
 
-    return params
+    return params
```

### Comparing `struphy-1.9.9/src/struphy/pic/accum_kernels.py` & `struphy-2.0.0/src/struphy/pic/accum_kernels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from pyccel.decorators import stack_array
 
-from numpy import zeros, empty, sqrt, shape, floor
+from numpy import zeros, empty, sqrt, shape, floor, log
 
 import struphy.geometry.map_eval as map_eval
 import struphy.b_splines.bsplines_kernels as bsp
 import struphy.b_splines.bspline_evaluation_3d as eval_3d
 import struphy.linear_algebra.core as linalg
 import struphy.pic.mat_vec_filler as mvf
 import struphy.pic.filler_kernels as fk
 
-from struphy.kinetic_background.f0_kernels import maxwellian_6d
-
 
 def _docstring():
     '''
     MODULE DOCSTRING for :ref:`accumulators`.
 
     The module contains model-specific accumulation routines (pyccelized), to be defined by the user.
 
@@ -308,15 +306,18 @@
                                   pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                                   starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                                   kind_map: 'int', params_map: 'float[:]',
                                   p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                                   ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                                   cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
                                   vec: 'float[:,:,:]',
-                                  f0_values: 'float[:]'):  # model specific argument
+                                  f0_values: 'float[:]',  # model specific argument
+                                  f0_params: 'float[:]',  # model specific argument
+                                  alpha: 'float',  # model specific argument
+                                  kappa: 'float'):  # model specific argument
     r"""
     Accumulates the charge density in V0 
 
     .. math::
 
         \rho_p^\mu &= \alpha^2 \sqrt{f_0(\mathbf{\eta}_p, \mathbf{v}_p)} w_p [ DF^{-1}(\mathbf{\eta}_p) \mathbf{v}_p ]_\mu \,.
 
@@ -355,16 +356,16 @@
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
         f0 = f0_values[ip]
 
-        # filling = w_p * sqrt{f_0} / N
-        filling = markers[ip, 6] * sqrt(f0) / n_markers_tot
+        # filling = alpha^2 * kappa * w_p * sqrt{f_0}
+        filling = alpha**2 * kappa * markers[ip, 6] * sqrt(f0) * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2
 
         # spans (i.e. index for non-vanishing B-spline basis functions)
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
 
         # compute bn, bd, i.e. values for non-vanishing B-/splines at position eta
@@ -392,37 +393,41 @@
                           mat13: 'float[:,:,:,:,:,:]',
                           mat22: 'float[:,:,:,:,:,:]',
                           mat23: 'float[:,:,:,:,:,:]',
                           mat33: 'float[:,:,:,:,:,:]',
                           vec1: 'float[:,:,:]',
                           vec2: 'float[:,:,:]',
                           vec3: 'float[:,:,:]',
-                          f0_values: 'float[:]',     # model specific argument
-                          f0_params: 'float[:]',   # model specific argument
-                          alpha: 'float'):  # model specific argument
+                          f0_values: 'float[:]',  # model specific argument
+                          f0_params: 'float[:]',  # model specific argument
+                          alpha: 'float',  # model specific argument
+                          kappa: 'float'):  # model specific argument
     r"""
     Accumulates into V1 with the filling functions
 
     .. math::
 
-        A_p^{\mu, \nu} &= \frac{\alpha^2}{v_{\text{th}}^2} \frac{1}{N\, s_0} f_0(\mathbf{\eta}_p, \mathbf{v}_p)
+        A_p^{\mu, \nu} &= \frac{\alpha^2 \kappa^2}{v_{\text{th}}^2} \frac{1}{N\, s_0} f_0(\mathbf{\eta}_p, \mathbf{v}_p)
             [ DF^{-1}(\mathbf{\eta}_p) v_p ]_\mu [ DF^{-1}(\mathbf{\eta}_p) \mathbf{v}_p ]_\nu \,,
 
-        B_p^\mu &= \alpha^2 \sqrt{f_0(\mathbf{\eta}_p, \mathbf{v}_p)} w_p [ DF^{-1}(\mathbf{\eta}_p) \mathbf{v}_p ]_\mu \,.
+        B_p^\mu &= \alpha^2 \kappa \sqrt{f_0(\mathbf{\eta}_p, \mathbf{v}_p)} w_p [ DF^{-1}(\mathbf{\eta}_p) \mathbf{v}_p ]_\mu \,.
 
     Parameters
     ----------
         f0_values ; array[float]
             Value of f0 for each particle.
 
         f0_params : array[float]
             Parameters needed to specify the moments; the order is specified in :ref:`kinetic_moments` for the respective functions available.
 
         alpha : float
-            = Omega_c / Omega_p ; Parameter determining the coupling strength between particles and fields
+            = Omega_p / Omega_c ; Parameter determining the coupling strength between particles and fields
+
+        kappa : float
+            = 2 * pi * Omega_c / omega ; Parameter determining the coupling strength between particles and fields
 
     Note
     ----
         The above parameter list contains only the model specific input arguments.
     """
 
     # allocate for metric coeffs
@@ -466,33 +471,196 @@
         v[1] = (markers[ip, 4] - f0_params[2]) / f0_params[5]**2
         v[2] = (markers[ip, 5] - f0_params[3]) / f0_params[6]**2
 
         # filling functions
         linalg.matrix_inv(df, df_inv)
         linalg.matrix_vector(df_inv, v, df_inv_times_v)
 
-        # filling_m = alpha^2 * f0 / (N * s_0 * v_th_1^2 * v_th_2^2 * v_th_3^2) * (DF^{-1} v_p)_mu * (DF^{-1} \V_th (v_p - u))_nu
+        # filling_m = alpha^2 * kappa^2 * f0 / (N * s_0 * v_th_1^2 * v_th_2^2 * v_th_3^2) * (DF^{-1} \V_th (v_p - u))_mu * (DF^{-1} \V_th (v_p - u))_nu
         linalg.outer(df_inv_times_v, df_inv_times_v, filling_m)
-        filling_m[:, :] *= alpha**2 * f0 * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2 / (n_markers_tot * markers[ip, 7])
+        filling_m[:, :] *= alpha**2 * kappa**2 * f0 * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2 / (n_markers_tot * markers[ip, 7])
 
-        # filling_v = alpha^2 * w_p * sqrt{f_0} DL^{-1} * \V_th * (v_p - u)
-        filling_v[:] = alpha**2 * sqrt(f0) * markers[ip, 6] * df_inv_times_v[:] * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2
+        # filling_v = alpha^2 * kappa * w_p * sqrt{f_0} DL^{-1} * \V_th * (v_p - u)
+        filling_v[:] = alpha**2 * kappa * sqrt(f0) * markers[ip, 6] * df_inv_times_v[:] * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2
 
         # call the appropriate matvec filler
-        mvf.m_v_fill_b_v1_symm(pn, tn1, tn2, tn3, starts1,
+        mvf.m_v_fill_b_v1_symm(pn,
+                               tn1, tn2, tn3,
+                               starts1,
                                eta1, eta2, eta3,
                                mat11, mat12, mat13, mat22, mat23, mat33,
                                filling_m[0, 0], filling_m[0, 1], filling_m[0, 2],
                                filling_m[1, 1], filling_m[1, 2], filling_m[2, 2],
                                vec1, vec2, vec3,
                                filling_v[0], filling_v[1], filling_v[2])
 
     #$ omp end parallel
 
 
+def delta_f_vlasov_maxwell_poisson(markers: 'float[:,:]', n_markers_tot: 'int',
+                                   pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                   starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                   kind_map: 'int', params_map: 'float[:]',
+                                   p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                   ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                   cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                   vec: 'float[:,:,:]',
+                                   f0_values: 'float[:]',  # model specific argument
+                                   f0_params: 'float[:]',  # model specific argument
+                                   alpha: 'float',  # model specific argument
+                                   kappa: 'float'):  # model specific argument
+    r"""
+    Accumulates the charge density in V0 
+
+    .. math::
+
+        \rho_p^\mu &= \alpha^2 \sqrt{f_0(\mathbf{\eta}_p, \mathbf{v}_p)} w_p [ DF^{-1}(\mathbf{\eta}_p) \mathbf{v}_p ]_\mu \,.
+
+    Parameters
+    ----------
+        f0_values ; array[float]
+            Value of f0 for each particle.
+
+        f0_params : array[float]
+            Parameters needed to specify the moments; the order is specified in :ref:`kinetic_moments` for the respective functions available.
+
+        alpha : float
+            = Omega_c / Omega_p ; Parameter determining the coupling strength between particles and fields
+
+    Note
+    ----
+        The above parameter list contains only the model specific input arguments.
+    """
+
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    #$ omp parallel private (ip, eta1, eta2, eta3, f0, filling)
+    #$ omp for reduction ( + :vec)
+    for ip in range(n_markers):
+
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        # marker positions
+        eta1 = markers[ip, 0]
+        eta2 = markers[ip, 1]
+        eta3 = markers[ip, 2]
+
+        f0 = f0_values[ip]
+
+        # filling = alpha^2 * kappa * (1 / (N * s_0) * (f_0 / log(f_0) - f_0) - w_p / log(f_0))
+        filling = alpha**2 * kappa * ((f0 / log(f0) - f0) / (n_markers_tot * markers[ip, 7]) - markers[ip, 6] / log(f0))  * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2
+
+        # call the appropriate matvec filler
+        mvf.scalar_fill_b_v0(pn, tn1, tn2, tn3,
+                             starts0, eta1, eta2, eta3,
+                             vec, filling)
+
+    #$ omp end parallel
+
+
+@stack_array('df', 'df_t', 'df_inv', 'v', 'df_inv_times_v', 'filling_v')
+def delta_f_vlasov_maxwell(markers: 'float[:,:]', n_markers_tot: 'int',
+                           pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                           starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                           kind_map: 'int', params_map: 'float[:]',
+                           p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                           ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                           cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                           vec1: 'float[:,:,:]',
+                           vec2: 'float[:,:,:]',
+                           vec3: 'float[:,:,:]',
+                           f0_values: 'float[:]',  # model specific argument
+                           f0_params: 'float[:]',  # model specific argument
+                           alpha: 'float',  # model specific argument
+                           kappa: 'float'):  # model specific argument
+    r"""
+    Accumulates into V1 with the filling functions
+
+    .. math::
+
+        A_p^{\mu, \nu} &= \frac{\alpha^2}{v_{\text{th}}^2} \frac{1}{N\, s_0} f_0(\mathbf{\eta}_p, \mathbf{v}_p)
+            [ DF^{-1}(\mathbf{\eta}_p) v_p ]_\mu [ DF^{-1}(\mathbf{\eta}_p) \mathbf{v}_p ]_\nu \,,
+
+        B_p^\mu &= \alpha^2 \sqrt{f_0(\mathbf{\eta}_p, \mathbf{v}_p)} w_p [ DF^{-1}(\mathbf{\eta}_p) \mathbf{v}_p ]_\mu \,.
+
+    Parameters
+    ----------
+        f0_values ; array[float]
+            Value of f0 for each particle.
+
+        f0_params : array[float]
+            Parameters needed to specify the moments; the order is specified in :ref:`kinetic_moments` for the respective functions available.
+
+        alpha : float
+            = Omega_c / Omega_p ; Parameter determining the coupling strength between particles and fields
+
+    Note
+    ----
+        The above parameter list contains only the model specific input arguments.
+    """
+
+    # allocate for metric coeffs
+    df = empty((3, 3), dtype=float)
+    df_inv = empty((3, 3), dtype=float)
+
+    # allocate for filling
+    v = empty(3, dtype=float)
+    df_inv_times_v = empty(3, dtype=float)
+    filling_v = empty(3, dtype=float)
+
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    #$ omp parallel private (ip, eta1, eta2, eta3, f0, df, df_inv, v, df_inv_times_v, filling_v)
+    #$ omp for reduction ( + : mat11, mat12, mat13, mat22, mat23, mat33, vec1, vec2, vec3)
+    for ip in range(n_markers):
+
+        # only do something if particle is a "true" particle (i.e. not a hole)
+        if markers[ip, 0] == -1.:
+            continue
+
+        # marker positions
+        eta1 = markers[ip, 0]
+        eta2 = markers[ip, 1]
+        eta3 = markers[ip, 2]
+
+        f0 = f0_values[ip]
+
+        # evaluate Jacobian, result in df
+        map_eval.df(eta1, eta2, eta3,
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map, p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # compute shifted and stretched velocity
+        v[0] = (markers[ip, 3] - f0_params[1]) / f0_params[4]**2
+        v[1] = (markers[ip, 4] - f0_params[2]) / f0_params[5]**2
+        v[2] = (markers[ip, 5] - f0_params[3]) / f0_params[6]**2
+
+        # filling functions
+        linalg.matrix_inv(df, df_inv)
+        linalg.matrix_vector(df_inv, v, df_inv_times_v)
+
+        # filling_v = alpha^2 / (N * s_0) * (f_0 / ln(f_0) - f_0) * DL^{-1} * \V_th * (v_p - u)
+        filling_v[:] = alpha**2 * kappa / (n_markers_tot * markers[ip, 7]) * (f0 / log(f0) - f0 ) * df_inv_times_v[:] * f0_params[4]**2 * f0_params[5]**2 * f0_params[6]**2
+
+        # call the appropriate matvec filler
+        mvf.vec_fill_b_v1(pn, tn1, tn2, tn3, starts1,
+                          eta1, eta2, eta3,
+                          vec1, vec2, vec3,
+                          filling_v[0], filling_v[1], filling_v[2])
+
+    #$ omp end parallel
+
+
 @stack_array('g_inv', 'tmp1', 'tmp2', 'b', 'b_prod', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def cc_lin_mhd_6d_1(markers: 'float[:,:]', n_markers_tot: 'int',
                     pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                     starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                     kind_map: 'int', params_map: 'float[:]',
                     p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                     ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
@@ -1264,25 +1432,27 @@
                      mat13: 'float[:,:,:,:,:,:]',
                      mat22: 'float[:,:,:,:,:,:]',
                      mat23: 'float[:,:,:,:,:,:]',
                      mat33: 'float[:,:,:,:,:,:]',
                      vec1: 'float[:,:,:]',
                      vec2: 'float[:,:,:]',
                      vec3: 'float[:,:,:]',
-                     kappa: float,    # model specific argument
-                     b1: 'float[:,:,:]',          # model specific argument
-                     b2: 'float[:,:,:]',          # model specific argument 
-                     b3: 'float[:,:,:]',          # model specific argument 
-                     norm_b11: 'float[:,:,:]',       # model specific argument    
-                     norm_b12: 'float[:,:,:]',       # model specific argument
-                     norm_b13: 'float[:,:,:]',       # model specific argument
+                     kappa: float,                  # model specific argument
+                     b1: 'float[:,:,:]',            # model specific argument
+                     b2: 'float[:,:,:]',            # model specific argument 
+                     b3: 'float[:,:,:]',            # model specific argument 
+                     norm_b11: 'float[:,:,:]',      # model specific argument    
+                     norm_b12: 'float[:,:,:]',      # model specific argument
+                     norm_b13: 'float[:,:,:]',      # model specific argument
                      curl_norm_b1: 'float[:,:,:]',  # model specific argument
                      curl_norm_b2: 'float[:,:,:]',  # model specific argument
                      curl_norm_b3: 'float[:,:,:]',  # model specific argument
-                     basis_u : 'int', scale_mat : 'float', scale_vec : 'float'): # model specific argument
+                     basis_u : 'int',               # model specific argument
+                     scale_mat : 'float',           # model specific argument
+                     scale_vec : 'float'):          # model specific argument
 
     r"""Accumulates into V1 with the filling functions
 
     .. math::
 
         A_p^{\mu, \nu} &= w_p * [G^{-1}(\eta_p) * B2_{\times}(\eta_p) * B2_{\times}(\eta_p)^\top * G^{-1}(\eta_p) * v^2_{\parallel,p} * \left( 1/B^*_\parallel \right)^2 * |1/\sqrt{g} \hat \nabla \times \hat b^1_0|_p^2]_{\mu, \nu}
 
@@ -1337,29 +1507,27 @@
     tmp_m = empty((3, 3), dtype=float)
 
     tmp_v = empty(3, dtype=float)
 
     # get number of markers
     n_markers_loc = shape(markers)[0]
     
-    #$ omp parallel firstprivate(b_prod) private(ip, eta1, eta2, eta3, span1, span2, span3, bn1, bn2, bn3, bd1, bd2, bd3, b, b_Star, norm_b1, curl_norm_b, df, det_df, weight, v, df_inv, df_inv_t, g_inv, tmp1, tmp2, tmp_t, tmp_m, tmp_v, filling_m, filling_v) 
-    #$ omp for reduction ( + : mat11, mat12, mat13, mat22, mat23, mat33)
     for ip in range(n_markers_loc):
         
         # only do something if particle is a "true" particle (i.e. not a hole)
         if markers[ip, 0] == -1.:
             continue
 
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
         # marker weight and velocity
-        weight = markers[ip, 6]
+        weight = markers[ip, 5]
         v = markers[ip, 3]
 
         # b-field evaluation
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
 
@@ -1479,16 +1647,14 @@
                                  mat22, mat23, 
                                  mat33, 
                                  filling_m[0, 0], filling_m[0, 1], filling_m[0, 2], 
                                  filling_m[1, 1], filling_m[1, 2], 
                                  filling_m[2, 2],
                                  vec1, vec2, vec3,
                                  filling_v[0], filling_v[1], filling_v[2])
-            
-    #$ omp end parallel
     
     mat11 /= n_markers_tot
     mat12 /= n_markers_tot
     mat13 /= n_markers_tot
     mat22 /= n_markers_tot
     mat23 /= n_markers_tot
     mat33 /= n_markers_tot
@@ -1581,15 +1747,15 @@
 
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
         # marker weight and velocity
-        weight = markers[ip, 6]
+        weight = markers[ip, 5]
         v = markers[ip, 3]
         mu = markers[ip, 4]
 
         # b-field evaluation
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
@@ -1634,17 +1800,14 @@
         curl_norm_b[2] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, curl_norm_b3, starts2[2])
 
         # grad_PB; 1form
         grad_PB[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_PB1, starts1[0])
         grad_PB[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_PB2, starts1[1])
         grad_PB[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_PB3, starts1[2])
 
-        #TODO:check
-        grad_PB /= kappa
-
         # b_star; 2form transformed into H1vec
         b_star[:] = (b + curl_norm_b*v/kappa)/det_df
 
         # calculate abs_b_star_para
         abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
 
         # operator bx() as matrix
@@ -1829,15 +1992,15 @@
 
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
         # marker weight and velocity
-        weight = markers[ip, 6]
+        weight = markers[ip, 5]
         v = markers[ip, 3]
         mu = markers[ip, 4]
 
         # b-field evaluation
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
@@ -1882,17 +2045,14 @@
         curl_norm_b[2] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, curl_norm_b3, starts2[2])
 
         # grad_PB; 1form
         grad_PB[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_PB1, starts1[0])
         grad_PB[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_PB2, starts1[1])
         grad_PB[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_PB3, starts1[2])
 
-        #TODO:check
-        grad_PB /= kappa
-
         # b_star; 2form transformed into H1vec
         b_star[:] = (b + curl_norm_b*v/kappa)/det_df
 
         # calculate abs_b_star_para
         abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
 
         # operator bx() as matrix
@@ -2031,15 +2191,15 @@
 
         # marker positions
         eta1 = markers[ip, 0] # mid
         eta2 = markers[ip, 1] # mid
         eta3 = markers[ip, 2] # mid
 
         # marker weight and velocity
-        weight = markers[ip, 6]
+        weight = markers[ip, 5]
         mu = markers[ip, 4]
 
         # b-field evaluation
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
 
@@ -2048,17 +2208,14 @@
         bsp.b_d_splines_slim(tn3, pn[2], eta3, span3, bn3, bd3)
 
         # grad_PB; 1form
         grad_PB[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_PB1, starts1[0])
         grad_PB[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_PB2, starts1[1])
         grad_PB[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_PB3, starts1[2])
 
-        #TODO:check
-        grad_PB /= kappa
-
         tmp[:,:] = ((markers[ip, 18], markers[ip, 19], markers[ip, 20]),
                     (markers[ip, 19], markers[ip, 21], markers[ip, 22]),
                     (markers[ip, 20], markers[ip, 22], markers[ip, 23])) 
 
         if basis_u == 0:
             
             linalg.matrix_vector(tmp, grad_PB, tmp_v1)
@@ -2216,15 +2373,15 @@
 
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
         # marker weight and velocity
-        weight = markers[ip, 6]
+        weight = markers[ip, 5]
         v = markers[ip, 3]
         mu = markers[ip, 4]
 
         # b-field evaluation
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
@@ -2269,17 +2426,14 @@
         curl_norm_b[2] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, curl_norm_b3, starts2[2])
 
         # grad_PB; 1form
         grad_PB[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_PB1, starts1[0])
         grad_PB[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_PB2, starts1[1])
         grad_PB[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_PB3, starts1[2])
 
-        #TODO:check
-        grad_PB /= kappa
-
         # b_star; 2form transformed into H1vec
         b_star[:] = (b + curl_norm_b*v/kappa)/det_df
 
         # calculate abs_b_star_para
         abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
 
         # operator bx() as matrix
@@ -2396,16 +2550,14 @@
 
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
     bd3 = empty(pn[2], dtype=float)
 
     # get number of markers
     n_markers_loc = shape(markers)[0]
-
-    mH = 1.67262192369e-27 # proton mass (kg)
     
     for ip in range(n_markers_loc):
         
         # only do something if particle is a "true" particle (i.e. not a hole)
         if markers[ip, 0] == -1.:
             continue
 
@@ -2502,15 +2654,15 @@
 
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
         # marker weight and velocity
-        weight = markers[ip, 6]
+        weight = markers[ip, 5]
         mu = markers[ip, 4]
 
         # b-field evaluation
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
 
@@ -2578,15 +2730,14 @@
                             vec1, vec2, vec3,
                             filling_v[0], filling_v[1], filling_v[2])
 
     vec1 /= n_markers_tot
     vec2 /= n_markers_tot
     vec3 /= n_markers_tot
 
-
 @stack_array('df', 'df_t', 'df_inv', 'g_inv', 'filling_m', 'filling_v', 'tmp1', 'tmp2', 'tmp_t', 'tmp_m', 'tmp_v', 'b', 'b_prod', 'norm_b2_prod', 'b_star', 'curl_norm_b', 'norm_b1', 'norm_b2', 'grad_PB', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def cc_lin_mhd_5d_J2(markers: 'float[:,:]', n_markers_tot: 'int',
                     pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                     starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                     kind_map: 'int', params_map: 'float[:]',
                     p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                     ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
@@ -2696,15 +2847,15 @@
 
         # marker positions
         eta1 = markers[ip, 0]
         eta2 = markers[ip, 1]
         eta3 = markers[ip, 2]
 
         # marker weight and velocity
-        weight = markers[ip, 6]
+        weight = markers[ip, 5]
         v = markers[ip, 3]
         mu = markers[ip, 4]
 
         # b-field evaluation
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
@@ -2748,17 +2899,14 @@
         curl_norm_b[1] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2] - 1, bd1, bn2, bd3, span1, span2, span3, curl_norm_b2, starts2[1])
         curl_norm_b[2] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1] - 1, pn[2], bd1, bd2, bn3, span1, span2, span3, curl_norm_b3, starts2[2])
 
         # grad_PB; 1form
         grad_PB[0] = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3, span1, span2, span3, grad_PB1, starts1[0])
         grad_PB[1] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3, span1, span2, span3, grad_PB2, starts1[1])
         grad_PB[2] = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, grad_PB3, starts1[2])
-
-        #TODO:check
-        grad_PB /= kappa
         
         # b_star; 2form transformed into H1vec
         b_star[:] = (b + curl_norm_b*v/kappa)/det_df
 
         # calculate abs_b_star_para
         abs_b_star_para = linalg.scalar_dot(norm_b1, b_star)
 
@@ -2866,8 +3014,8 @@
     mat13 /= n_markers_tot
     mat22 /= n_markers_tot
     mat23 /= n_markers_tot
     mat33 /= n_markers_tot
     
     vec1 /= n_markers_tot
     vec2 /= n_markers_tot
-    vec3 /= n_markers_tot
+    vec3 /= n_markers_tot
```

### Comparing `struphy-1.9.9/src/struphy/pic/filler_kernels.py` & `struphy-2.0.0/src/struphy/pic/filler_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/pic/mat_vec_filler.py` & `struphy-2.0.0/src/struphy/pic/mat_vec_filler.py`

 * *Files 16% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """
 
     print('This is just the docstring function.')
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def mat_fill_b_v1_diag(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts1 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float):
+def mat_fill_b_v1_diag(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -135,15 +135,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -161,36 +161,36 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3, 
-                bd1, bn2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3,
+                bd1, bn2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3, 
-                bn1, bd2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3,
+                bn1, bd2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3, 
-                bn1, bn2, bd3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3,
+                bn1, bn2, bd3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def m_v_fill_b_v1_diag(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts1 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v1_diag(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -205,29 +205,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat22, mat33 : array[float]
             (mu=1, nu=1)-, (mu=2, nu=2)- and (mu=3, nu=3)-block of the block matrix V1 -> V1 that is written to.
 
         fill11, fill22, fill33 : float
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat22 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2, and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -245,36 +245,36 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix and vector entries
-    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3, 
-                    bd1, bn2, bn3, bd1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts1[0], pn, 
+    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3,
+                    bd1, bn2, bn3, bd1, bn2, bn3,
+                    span1, span2, span3,
+                    starts1[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3, 
-                    bn1, bd2, bn3, bn1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts1[1], pn, 
+
+    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3,
+                    bn1, bd2, bn3, bn1, bd2, bn3,
+                    span1, span2, span3,
+                    starts1[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3, 
-                    bn1, bn2, bd3, bn1, bn2, bd3, 
-                    span1, span2, span3, 
+
+    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3,
+                    bn1, bn2, bd3, bn1, bn2, bd3,
+                    span1, span2, span3,
                     starts1[2], pn,
                     mat33, fill33, vec3, fill3)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def mat_fill_b_v2_diag(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts2 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float):
+def mat_fill_b_v2_diag(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -297,15 +297,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -323,36 +323,36 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3, 
-                bn1, bd2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3,
+                bn1, bd2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3, 
-                bd1, bn2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3,
+                bd1, bn2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3, 
-                bd1, bd2, bn3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3,
+                bd1, bd2, bn3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def m_v_fill_b_v2_diag(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts2 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v2_diag(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -367,29 +367,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat22, mat33 : array[float]
             (mu=1, nu=1)-, (mu=2, nu=2)- and (mu=3, nu=3)-block of the block matrix V2 -> V2 that is written to.
 
         fill11, fill22, fill33 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat22 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V2 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -407,36 +407,36 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix and vector entries
-    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3, 
-                    bn1, bd2, bd3, bn1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts2[0], pn, 
+    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3,
+                    bn1, bd2, bd3, bn1, bd2, bd3,
+                    span1, span2, span3,
+                    starts2[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3, 
-                    bd1, bn2, bd3, bd1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts2[1], pn, 
+
+    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3,
+                    bd1, bn2, bd3, bd1, bn2, bd3,
+                    span1, span2, span3,
+                    starts2[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3, 
-                    bd1, bd2, bn3, bd1, bd2, bn3, 
-                    span1, span2, span3, 
+
+    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3,
+                    bd1, bd2, bn3, bd1, bd2, bn3,
+                    span1, span2, span3,
                     starts2[2], pn,
                     mat33, fill33, vec3, fill3)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def mat_fill_b_v1_asym(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts1 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float):
+def mat_fill_b_v1_asym(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V1 -> V1. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -459,15 +459,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -485,36 +485,36 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def m_v_fill_b_v1_asym(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts1 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v1_asym(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V1 -> V1. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -529,29 +529,29 @@
             (logical) position of the particle in each direction.
 
         mat12, mat13, mat23 : array[float]
             (mu=1, nu=2)-, (mu=1, nu=3)-, and (mu=2, nu=3)-block of the block matrix V1 -> V1 that is written to.
 
         fill12, fill13, fill23 : float
             Numbers that will be multiplied by the basis functions of V1 and written to mat12, mat13 and mat23.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -569,42 +569,42 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pn2, pn3, pn1, pd2, pn3, 
-                    bd1, bn2, bn3, bn1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts1[0], pn, 
+    fk.fill_mat_vec(pd1, pn2, pn3, pn1, pd2, pn3,
+                    bd1, bn2, bn3, bn1, bd2, bn3,
+                    span1, span2, span3,
+                    starts1[0], pn,
                     mat12, fill12, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pn2, pd3, 
-                    bn1, bd2, bn3, bn1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts1[1], pn, 
+
+    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pn2, pd3,
+                    bn1, bd2, bn3, bn1, bn2, bd3,
+                    span1, span2, span3,
+                    starts1[1], pn,
                     mat23, fill23, vec2, fill2)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_vec(pn1, pn2, pd3, 
-                bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[2], 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_vec(pn1, pn2, pd3,
+                bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2],
                 vec3, fill3)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def mat_fill_b_v2_asym(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts2 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float):
+def mat_fill_b_v2_asym(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V2 -> V2. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -627,15 +627,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -653,36 +653,36 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def m_v_fill_b_v2_asym(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts2 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v2_asym(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V2 -> V2. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -697,29 +697,29 @@
             (logical) position of the particle in each direction.
 
         mat12, mat13, mat23 : array[float]
             (mu=1, nu=2)-, (mu=1, nu=3)-, and (mu=2, nu=3)-block of the block matrix V2 -> V2 that is written to.
 
         fill12, fill13, fill23 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat12, mat13 and mat23.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V2 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -737,42 +737,42 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pd2, pd3, pd1, pn2, pd3, 
-                    bn1, bd2, bd3, bd1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts2[0], pn, 
+    fk.fill_mat_vec(pn1, pd2, pd3, pd1, pn2, pd3,
+                    bn1, bd2, bd3, bd1, bn2, bd3,
+                    span1, span2, span3,
+                    starts2[0], pn,
                     mat12, fill12, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pd2, pn3, 
-                    bd1, bn2, bd3, bd1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts2[1], pn, 
+
+    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pd2, pn3,
+                    bd1, bn2, bd3, bd1, bd2, bn3,
+                    span1, span2, span3,
+                    starts2[1], pn,
                     mat23, fill23, vec2, fill2)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_vec(pd1, pd2, pn3, 
-                bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[2], 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_vec(pd1, pd2, pn3,
+                bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2],
                 vec3, fill3)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def mat_fill_b_v1_symm(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts1 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float):
+def mat_fill_b_v1_symm(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -795,15 +795,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -821,54 +821,54 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3, 
-                bd1, bn2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3,
+                bd1, bn2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3, 
-                bn1, bd2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3,
+                bn1, bd2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3, 
-                bn1, bn2, bd3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3,
+                bn1, bn2, bd3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat33, fill33)
-    
+
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def m_v_fill_b_v1_symm(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts1 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v1_symm(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -883,29 +883,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
             (mu=1, nu=1)-, (mu=1, nu=2)-, (mu=1, nu=3), (mu=2, nu=2)-, (mu=2, nu=3)- and (mu=3, nu=3)-block of the block matrix V1 -> V1 that is written to.
 
         fill11, fill12, fill13, fill22, fill23, fill33 : float
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat12, mat13, mat22, mat23 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -923,54 +923,54 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3, 
-                    bd1, bn2, bn3, bd1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts1[0], pn, 
+    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3,
+                    bd1, bn2, bn3, bd1, bn2, bn3,
+                    span1, span2, span3,
+                    starts1[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3, 
-                    bn1, bd2, bn3, bn1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts1[1], pn, 
+
+    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3,
+                    bn1, bd2, bn3, bn1, bd2, bn3,
+                    span1, span2, span3,
+                    starts1[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3, 
-                    bn1, bn2, bd3, bn1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts1[2], pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3,
+                    bn1, bn2, bd3, bn1, bn2, bd3,
+                    span1, span2, span3,
+                    starts1[2], pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat13, fill13)
 
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def mat_fill_b_v2_symm(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts2 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float):
+def mat_fill_b_v2_symm(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -993,15 +993,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -1019,54 +1019,54 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3, 
-                bn1, bd2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3,
+                bn1, bd2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3, 
-                bd1, bn2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3,
+                bd1, bn2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3, 
-                bd1, bd2, bn3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3,
+                bd1, bd2, bn3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat33, fill33)
-    
+
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def m_v_fill_b_v2_symm(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts2 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v2_symm(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -1081,29 +1081,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
             (mu=1, nu=1)-, (mu=1, nu=2)-, (mu=1, nu=3), (mu=2, nu=2)-, (mu=2, nu=3)- and (mu=3, nu=3)-block of the block matrix V2 -> V2 that is written to.
 
         fill11, fill12, fill13, fill22, fill23, fill33 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat12, mat13, mat22, mat23 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -1121,54 +1121,54 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3, 
-                    bn1, bd2, bd3, bn1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts2[0], pn, 
+    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3,
+                    bn1, bd2, bd3, bn1, bd2, bd3,
+                    span1, span2, span3,
+                    starts2[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3, 
-                    bd1, bn2, bd3, bd1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts2[1], pn, 
+
+    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3,
+                    bd1, bn2, bd3, bd1, bn2, bd3,
+                    span1, span2, span3,
+                    starts2[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3, 
-                    bd1, bd2, bn3, bd1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts2[2], pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3,
+                    bd1, bd2, bn3, bd1, bd2, bn3,
+                    span1, span2, span3,
+                    starts2[2], pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat13, fill13)
 
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def mat_fill_b_v1_full(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts1 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float):
+def mat_fill_b_v1_full(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -1191,15 +1191,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -1217,72 +1217,72 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3, 
-                bd1, bn2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3,
+                bd1, bn2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pd2, pn3, pd1, pn2, pn3, 
-                bn1, bd2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pd2, pn3, pd1, pn2, pn3,
+                bn1, bd2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat21, fill21)
 
-    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3, 
-                bn1, bd2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3,
+                bn1, bd2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pd3, pd1, pn2, pn3, 
-                bn1, bn2, bd3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pd1, pn2, pn3,
+                bn1, bn2, bd3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pd2, pn3, 
-                bn1, bn2, bd3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pd2, pn3,
+                bn1, bn2, bd3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat32, fill32)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3, 
-                bn1, bn2, bd3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3,
+                bn1, bn2, bd3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat33, fill33)
-    
+
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def m_v_fill_b_v1_full(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts1 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v1_full(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -1297,29 +1297,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V1 -> V1 that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -1337,72 +1337,72 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3, 
-                    bd1, bn2, bn3, bd1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts1[0], pn, 
+    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3,
+                    bd1, bn2, bn3, bd1, bn2, bn3,
+                    span1, span2, span3,
+                    starts1[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3, 
-                    bn1, bd2, bn3, bn1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts1[1], pn, 
+
+    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3,
+                    bn1, bd2, bn3, bn1, bd2, bn3,
+                    span1, span2, span3,
+                    starts1[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3, 
-                    bn1, bn2, bd3, bn1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts1[2], pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3,
+                    bn1, bn2, bd3, bn1, bn2, bd3,
+                    span1, span2, span3,
+                    starts1[2], pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pd2, pn3, pd1, pn2, pn3, 
-                bn1, bd2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pd2, pn3, pd1, pn2, pn3,
+                bn1, bd2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat21, fill21)
 
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pd3, pd1, pn2, pn3, 
-                bn1, bn2, bd3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pd1, pn2, pn3,
+                bn1, bn2, bd3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pd2, pn3, 
-                bn1, bn2, bd3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pd2, pn3,
+                bn1, bn2, bd3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat32, fill32)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def mat_fill_b_v2_full(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts2 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float):
+def mat_fill_b_v2_full(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -1417,29 +1417,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V2 -> V2 that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V2 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -1457,72 +1457,72 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3, 
-                bn1, bd2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3,
+                bn1, bd2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pn2, pd3, pn1, pd2, pd3, 
-                bd1, bn2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pn2, pd3, pn1, pd2, pd3,
+                bd1, bn2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat21, fill21)
 
-    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3, 
-                bd1, bn2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3,
+                bd1, bn2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pn3, pn1, pd2, pd3, 
-                bd1, bd2, bn3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pn1, pd2, pd3,
+                bd1, bd2, bn3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pn2, pd3, 
-                bd1, bd2, bn3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pn2, pd3,
+                bd1, bd2, bn3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat32, fill32)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3, 
-                bd1, bd2, bn3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3,
+                bd1, bd2, bn3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
-def m_v_fill_b_v2_full(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts2 : 'int[:,:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]',  fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v2_full(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]',  fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -1537,29 +1537,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V2 -> V2 that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V2 and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
@@ -1577,85 +1577,85 @@
 
     # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
     bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
     bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
     bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3, 
-                    bn1, bd2, bd3, bn1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts2[0], pn, 
+    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3,
+                    bn1, bd2, bd3, bn1, bd2, bd3,
+                    span1, span2, span3,
+                    starts2[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3, 
-                    bd1, bn2, bd3, bd1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts2[1], pn, 
+
+    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3,
+                    bd1, bn2, bd3, bd1, bn2, bd3,
+                    span1, span2, span3,
+                    starts2[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3, 
-                    bd1, bd2, bn3, bd1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts2[2], pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3,
+                    bd1, bd2, bn3, bd1, bd2, bn3,
+                    span1, span2, span3,
+                    starts2[2], pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pn2, pd3, pn1, pd2, pd3, 
-                bd1, bn2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pn2, pd3, pn1, pd2, pd3,
+                bd1, bn2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat21, fill21)
 
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pn3, pn1, pd2, pd3, 
-                bd1, bd2, bn3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pn1, pd2, pd3,
+                bd1, bd2, bn3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pn2, pd3, 
-                bd1, bd2, bn3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pn2, pd3,
+                bd1, bd2, bn3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat32, fill32)
 
 
 @pure
-def mat_fill_v1_diag(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float):
+def mat_fill_v1_diag(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts1 : array[int]
             Start indices of the current process in space V1.
 
         mat11, mat22, mat33 : array[float]
@@ -1665,119 +1665,119 @@
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat22 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3, 
-                bd1, bn2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3,
+                bd1, bn2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3, 
-                bn1, bd2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3,
+                bn1, bd2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3, 
-                bn1, bn2, bd3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3,
+                bn1, bn2, bd3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v1_diag(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v1_diag(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts1 : array[int]
             Start indices of the current process in space V1.
 
         mat11, mat22, mat33 : array[float]
             (mu=1, nu=1)-, (mu=2, nu=2)- and (mu=3, nu=3)-block of the block matrix V1 -> V1 that is written to.
 
         fill11, fill22, fill33 : float
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat22 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2, and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix and vector entries
-    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3, 
-                    bd1, bn2, bn3, bd1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts1[0], pn, 
+    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3,
+                    bd1, bn2, bn3, bd1, bn2, bn3,
+                    span1, span2, span3,
+                    starts1[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3, 
-                    bn1, bd2, bn3, bn1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts1[1], pn, 
+
+    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3,
+                    bn1, bd2, bn3, bn1, bd2, bn3,
+                    span1, span2, span3,
+                    starts1[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3, 
-                    bn1, bn2, bd3, bn1, bn2, bd3, 
-                    span1, span2, span3, 
+
+    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3,
+                    bn1, bn2, bd3, bn1, bn2, bd3,
+                    span1, span2, span3,
                     starts1[2], pn,
                     mat33, fill33, vec3, fill3)
 
 
 @pure
-def mat_fill_v2_diag(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]', mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float):
+def mat_fill_v2_diag(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]', mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts2 : array[int]
             Start indices of the current process in space V2.
 
         mat11, mat22, mat33 : array[float]
@@ -1787,119 +1787,119 @@
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat22 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3, 
-                bn1, bd2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3,
+                bn1, bd2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3, 
-                bd1, bn2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3,
+                bd1, bn2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3, 
-                bd1, bd2, bn3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3,
+                bd1, bd2, bn3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v2_diag(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]', mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v2_diag(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]', mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts2 : array[int]
             Start indices of the current process in space V2.
 
         mat11, mat22, mat33 : array[float]
             (mu=1, nu=1)-, (mu=2, nu=2)- and (mu=3, nu=3)-block of the block matrix V2 -> V2 that is written to.
 
         fill11, fill22, fill33 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat22 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V2 and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix and vector entries
-    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3, 
-                    bn1, bd2, bd3, bn1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts2[0], pn, 
+    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3,
+                    bn1, bd2, bd3, bn1, bd2, bd3,
+                    span1, span2, span3,
+                    starts2[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3, 
-                    bd1, bn2, bd3, bd1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts2[1], pn, 
+
+    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3,
+                    bd1, bn2, bd3, bd1, bn2, bd3,
+                    span1, span2, span3,
+                    starts2[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3, 
-                    bd1, bd2, bn3, bd1, bd2, bn3, 
-                    span1, span2, span3, 
+
+    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3,
+                    bd1, bd2, bn3, bd1, bd2, bn3,
+                    span1, span2, span3,
                     starts2[2], pn,
                     mat33, fill33, vec3, fill3)
 
 
 @pure
-def mat_fill_v1_asym(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float):
+def mat_fill_v1_asym(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V1 -> V1. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts1 : array[int]
             Start indices of the current process in space V1.
 
         mat12, mat13, mat23 : array[float]
@@ -1909,125 +1909,125 @@
             Numbers that will be multiplied by the basis functions of V1 and written to mat12, mat13 and mat23.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
 
 
 @pure
-def m_v_fill_v1_asym(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v1_asym(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V1 -> V1. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts1 : array[int]
             Start indices of the current process in space V1.
 
         mat12, mat13, mat23 : array[float]
             (mu=1, nu=2)-, (mu=1, nu=3)-, and (mu=2, nu=3)-block of the block matrix V1 -> V1 that is written to.
 
         fill12, fill13, fill23 : float
             Numbers that will be multiplied by the basis functions of V1 and written to mat12, mat13 and mat23.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pn2, pn3, pn1, pd2, pn3, 
-                    bd1, bn2, bn3, bn1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts1[0], pn, 
+    fk.fill_mat_vec(pd1, pn2, pn3, pn1, pd2, pn3,
+                    bd1, bn2, bn3, bn1, bd2, bn3,
+                    span1, span2, span3,
+                    starts1[0], pn,
                     mat12, fill12, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pn2, pd3, 
-                    bn1, bd2, bn3, bn1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts1[1], pn, 
+
+    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pn2, pd3,
+                    bn1, bd2, bn3, bn1, bn2, bd3,
+                    span1, span2, span3,
+                    starts1[1], pn,
                     mat23, fill23, vec2, fill2)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_vec(pn1, pn2, pd3, 
-                bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[2], 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_vec(pn1, pn2, pd3,
+                bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2],
                 vec3, fill3)
 
 
 @pure
-def mat_fill_v2_asym(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float):
+def mat_fill_v2_asym(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V2 -> V2. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts2 : array[int]
             Start indices of the current process in space V2.
 
         mat12, mat13, mat23 : array[float]
@@ -2037,125 +2037,125 @@
             Numbers that will be multiplied by the basis functions of V2 and written to mat12, mat13 and mat23.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
 
 
 @pure
-def m_v_fill_v2_asym(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v2_asym(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V2 -> V2. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts2 : array[int]
             Start indices of the current process in space V2.
 
         mat12, mat13, mat23 : array[float]
             (mu=1, nu=2)-, (mu=1, nu=3)-, and (mu=2, nu=3)-block of the block matrix V2 -> V2 that is written to.
 
         fill12, fill13, fill23 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat12, mat13 and mat23.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V2 and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pd2, pd3, pd1, pn2, pd3, 
-                    bn1, bd2, bd3, bd1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts2[0], pn, 
+    fk.fill_mat_vec(pn1, pd2, pd3, pd1, pn2, pd3,
+                    bn1, bd2, bd3, bd1, bn2, bd3,
+                    span1, span2, span3,
+                    starts2[0], pn,
                     mat12, fill12, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pd2, pn3, 
-                    bd1, bn2, bd3, bd1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts2[1], pn, 
+
+    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pd2, pn3,
+                    bd1, bn2, bd3, bd1, bd2, bn3,
+                    span1, span2, span3,
+                    starts2[1], pn,
                     mat23, fill23, vec2, fill2)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_vec(pd1, pd2, pn3, 
-                bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[2], 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_vec(pd1, pd2, pn3,
+                bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2],
                 vec3, fill3)
 
 
 @pure
-def mat_fill_v1_symm(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float):
+def mat_fill_v1_symm(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts1 : array[int]
             Start indices of the current process in space V1.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
@@ -2165,155 +2165,155 @@
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat12, mat13, mat22, mat23 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3, 
-                bd1, bn2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3,
+                bd1, bn2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3, 
-                bn1, bd2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3,
+                bn1, bd2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3, 
-                bn1, bn2, bd3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3,
+                bn1, bn2, bd3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v1_symm(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v1_symm(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts1 : array[int]
             Start indices of the current process in space V1.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
             (mu=1, nu=1)-, (mu=1, nu=2)-, (mu=1, nu=3), (mu=2, nu=2)-, (mu=2, nu=3)- and (mu=3, nu=3)-block of the block matrix V1 -> V1 that is written to.
 
         fill11, fill12, fill13, fill22, fill23, fill33 : float
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat12, mat13, mat22, mat23 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3, 
-                    bd1, bn2, bn3, bd1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts1[0], pn, 
+    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3,
+                    bd1, bn2, bn3, bd1, bn2, bn3,
+                    span1, span2, span3,
+                    starts1[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3, 
-                    bn1, bd2, bn3, bn1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts1[1], pn, 
+
+    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3,
+                    bn1, bd2, bn3, bn1, bd2, bn3,
+                    span1, span2, span3,
+                    starts1[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3, 
-                    bn1, bn2, bd3, bn1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts1[2], pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3,
+                    bn1, bn2, bd3, bn1, bn2, bd3,
+                    span1, span2, span3,
+                    starts1[2], pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat13, fill13)
 
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
 
 
 @pure
-def mat_fill_v2_symm(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]', mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float):
+def mat_fill_v2_symm(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]', mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts2 : array[int]
             Start indices of the current process in space V2.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
@@ -2323,155 +2323,155 @@
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat12, mat13, mat22, mat23 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3, 
-                bn1, bd2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3,
+                bn1, bd2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3, 
-                bd1, bn2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3,
+                bd1, bn2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3, 
-                bd1, bd2, bn3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3,
+                bd1, bd2, bn3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v2_symm(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v2_symm(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts2 : array[int]
             Start indices of the current process in space V2.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
             (mu=1, nu=1)-, (mu=1, nu=2)-, (mu=1, nu=3), (mu=2, nu=2)-, (mu=2, nu=3)- and (mu=3, nu=3)-block of the block matrix V2 -> V2 that is written to.
 
         fill11, fill12, fill13, fill22, fill23, fill33 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat12, mat13, mat22, mat23 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3, 
-                    bn1, bd2, bd3, bn1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts2[0], pn, 
+    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3,
+                    bn1, bd2, bd3, bn1, bd2, bd3,
+                    span1, span2, span3,
+                    starts2[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3, 
-                    bd1, bn2, bd3, bd1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts2[1], pn, 
+
+    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3,
+                    bd1, bn2, bd3, bd1, bn2, bd3,
+                    span1, span2, span3,
+                    starts2[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3, 
-                    bd1, bd2, bn3, bd1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts2[2], pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3,
+                    bd1, bd2, bn3, bd1, bd2, bn3,
+                    span1, span2, span3,
+                    starts2[2], pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat13, fill13)
 
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
 
 
 @pure
-def mat_fill_v1_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float):
+def mat_fill_v1_full(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts1 : array[int]
             Start indices of the current process in space V1.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat13, mat23, mat33 : array[float]
@@ -2481,191 +2481,191 @@
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat12, mat13, mat12, mat22, mat23, mat13, mat23 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3, 
-                bd1, bn2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+    fk.fill_mat(pd1, pn2, pn3, pd1, pn2, pn3,
+                bd1, bn2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pd2, pn3, pd1, pn2, pn3, 
-                bn1, bd2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pd2, pn3, pd1, pn2, pn3,
+                bn1, bd2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat21, fill21)
 
-    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3, 
-                bn1, bd2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+    fk.fill_mat(pn1, pd2, pn3, pn1, pd2, pn3,
+                bn1, bd2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pd3, pd1, pn2, pn3, 
-                bn1, bn2, bd3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pd1, pn2, pn3,
+                bn1, bn2, bd3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pd2, pn3, 
-                bn1, bn2, bd3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pd2, pn3,
+                bn1, bn2, bd3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat32, fill32)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3, 
-                bn1, bn2, bd3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pn2, pd3,
+                bn1, bn2, bd3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v1_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]',  fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v1_full(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]',  fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V1 -> V1. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts1 : array[int]
             Start indices of the current process in space V1.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V1 -> V1 that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V1 and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V1 and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3, 
-                    bd1, bn2, bn3, bd1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts1[0], pn, 
+    fk.fill_mat_vec(pd1, pn2, pn3, pd1, pn2, pn3,
+                    bd1, bn2, bn3, bd1, bn2, bn3,
+                    span1, span2, span3,
+                    starts1[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3, 
-                    bn1, bd2, bn3, bn1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts1[1], pn, 
+
+    fk.fill_mat_vec(pn1, pd2, pn3, pn1, pd2, pn3,
+                    bn1, bd2, bn3, bn1, bd2, bn3,
+                    span1, span2, span3,
+                    starts1[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3, 
-                    bn1, bn2, bd3, bn1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts1[2], pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pd3, pn1, pn2, pd3,
+                    bn1, bn2, bd3, bn1, bn2, bd3,
+                    span1, span2, span3,
+                    starts1[2], pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3, 
-                bd1, bn2, bn3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pd2, pn3,
+                bd1, bn2, bn3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3, 
-                bd1, bn2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pd2, pn3, pd1, pn2, pn3, 
-                bn1, bd2, bn3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pn3, pn1, pn2, pd3,
+                bd1, bn2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pd2, pn3, pd1, pn2, pn3,
+                bn1, bd2, bn3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat21, fill21)
 
-    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3, 
-                bn1, bd2, bn3, bn1, bn2, bd3, 
-                span1, span2, span3, 
-                starts1[1], pn, 
+    fk.fill_mat(pn1, pd2, pn3, pn1, pn2, pd3,
+                bn1, bd2, bn3, bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pd3, pd1, pn2, pn3, 
-                bn1, bn2, bd3, bd1, bn2, bn3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pd1, pn2, pn3,
+                bn1, bn2, bd3, bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pn1, pn2, pd3, pn1, pd2, pn3, 
-                bn1, bn2, bd3, bn1, bd2, bn3, 
-                span1, span2, span3, 
-                starts1[2], pn, 
+
+    fk.fill_mat(pn1, pn2, pd3, pn1, pd2, pn3,
+                bn1, bn2, bd3, bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[2], pn,
                 mat32, fill32)
 
 
 @pure
-def mat_fill_v2_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float):
+def mat_fill_v2_full(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts2 : array[int]
             Start indices of the current process in space V2.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
@@ -2675,178 +2675,178 @@
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3, 
-                bn1, bd2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+    fk.fill_mat(pn1, pd2, pd3, pn1, pd2, pd3,
+                bn1, bd2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pn2, pd3, pn1, pd2, pd3, 
-                bd1, bn2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pn2, pd3, pn1, pd2, pd3,
+                bd1, bn2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat21, fill21)
 
-    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3, 
-                bd1, bn2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+    fk.fill_mat(pd1, pn2, pd3, pd1, pn2, pd3,
+                bd1, bn2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pn3, pn1, pd2, pd3, 
-                bd1, bd2, bn3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pn1, pd2, pd3,
+                bd1, bd2, bn3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pn2, pd3, 
-                bd1, bd2, bn3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pn2, pd3,
+                bd1, bd2, bn3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat32, fill32)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3, 
-                bd1, bd2, bn3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pd2, pn3,
+                bd1, bd2, bn3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v2_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]',  fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v2_full(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]',  fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V2 -> V2. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts2 : array[int]
             Start indices of the current process in space V2.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V2 -> V2 that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V2 and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V2 and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3, 
-                    bn1, bd2, bd3, bn1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts2[0], pn, 
+    fk.fill_mat_vec(pn1, pd2, pd3, pn1, pd2, pd3,
+                    bn1, bd2, bd3, bn1, bd2, bd3,
+                    span1, span2, span3,
+                    starts2[0], pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3, 
-                    bd1, bn2, bd3, bd1, bn2, bd3, 
-                    span1, span2, span3, 
-                    starts2[1], pn, 
+
+    fk.fill_mat_vec(pd1, pn2, pd3, pd1, pn2, pd3,
+                    bd1, bn2, bd3, bd1, bn2, bd3,
+                    span1, span2, span3,
+                    starts2[1], pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3, 
-                    bd1, bd2, bn3, bd1, bd2, bn3, 
-                    span1, span2, span3, 
-                    starts2[2], pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pn3, pd1, pd2, pn3,
+                    bd1, bd2, bn3, bd1, bd2, bn3,
+                    span1, span2, span3,
+                    starts2[2], pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3, 
-                bn1, bd2, bd3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pn2, pd3,
+                bn1, bd2, bd3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[0], pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3, 
-                bn1, bd2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[0], pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pn2, pd3, pn1, pd2, pd3, 
-                bd1, bn2, bd3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+
+    fk.fill_mat(pn1, pd2, pd3, pd1, pd2, pn3,
+                bn1, bd2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[0], pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pn2, pd3, pn1, pd2, pd3,
+                bd1, bn2, bd3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat21, fill21)
 
-    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3, 
-                bd1, bn2, bd3, bd1, bd2, bn3, 
-                span1, span2, span3, 
-                starts2[1], pn, 
+    fk.fill_mat(pd1, pn2, pd3, pd1, pd2, pn3,
+                bd1, bn2, bd3, bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[1], pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pn3, pn1, pd2, pd3, 
-                bd1, bd2, bn3, bn1, bd2, bd3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pn1, pd2, pd3,
+                bd1, bd2, bn3, bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pd1, pd2, pn3, pd1, pn2, pd3, 
-                bd1, bd2, bn3, bd1, bn2, bd3, 
-                span1, span2, span3, 
-                starts2[2], pn, 
+
+    fk.fill_mat(pd1, pd2, pn3, pd1, pn2, pd3,
+                bd1, bd2, bn3, bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[2], pn,
                 mat32, fill32)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def mat_fill_b_v0(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat : 'float[:,:,:,:,:,:]', fill : float):
+def mat_fill_b_v0(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat: 'float[:,:,:,:,:,:]', fill: float):
     """
     Adds the contribution of one particle to the elements of an accumulation matrix V0 -> V0. The result is returned in mat.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -2886,24 +2886,24 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat, fill)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def m_v_fill_b_v0(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat : 'float[:,:,:,:,:,:]', fill_m : float, vec : 'float[:,:,:]', fill_v : float):
+def m_v_fill_b_v0(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat: 'float[:,:,:,:,:,:]', fill_m: float, vec: 'float[:,:,:]', fill_v: float):
     """
     Adds the contribution of one particle to the elements of an accumulation matrix V0 -> V0. The result is returned in mat.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -2949,24 +2949,24 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix and vector entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat, fill_m, vec, fill_v)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def mat_fill_b_v3(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat : 'float[:,:,:,:,:,:]', fill : float):
+def mat_fill_b_v3(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat: 'float[:,:,:,:,:,:]', fill: float):
     """
     Adds the contribution of one particle to the elements of an accumulation matrix V3 -> V3. The result is returned in mat.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -2989,15 +2989,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -3010,24 +3010,24 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat, fill)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def m_v_fill_b_v3(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat : 'float[:,:,:,:,:,:]', fill_m : float, vec : 'float[:,:,:]', fill_v : float):
+def m_v_fill_b_v3(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat: 'float[:,:,:,:,:,:]', fill_m: float, vec: 'float[:,:,:]', fill_v: float):
     """
     Adds the contribution of one particle to the elements of an accumulation matrix V3 -> V3. The result is returned in mat.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3056,15 +3056,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -3077,34 +3077,34 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix and vector entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat, fill_m, vec, fill_v)
 
 
 @pure
-def mat_fill_v0(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', mat : 'float[:,:,:,:,:,:]', fill : float):
+def mat_fill_v0(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', mat: 'float[:,:,:,:,:,:]', fill: float):
     """
     Adds the contribution of one particle to the elements of an accumulation matrix V0 -> V0. The result is returned in mat.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
 
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat : array[float]
@@ -3114,39 +3114,39 @@
             Number that will be multiplied by the basis functions of V0 and written to mat.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat, fill)
 
 
 @pure
-def m_v_fill_v0(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', mat : 'float[:,:,:,:,:,:]', fill_m : float, vec : 'float[:,:,:]', fill_v : float):
+def m_v_fill_v0(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', mat: 'float[:,:,:,:,:,:]', fill_m: float, vec: 'float[:,:,:]', fill_v: float):
     """
     Adds the contribution of one particle to the elements of an accumulation matrix V0 -> V0. The result is returned in mat.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat : array[float]
             Matrix V0 -> V0 that is written to.
 
         fill_m : float
@@ -3159,36 +3159,36 @@
             Number that is multiplied by the basis functions of V0 and written to vec.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix and vector entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat, fill_m, vec, fill_v)
 
 
 @pure
-def mat_fill_v3(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]', mat : 'float[:,:,:,:,:,:]', fill : float):
+def mat_fill_v3(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]', mat: 'float[:,:,:,:,:,:]', fill: float):
     """
     Adds the contribution of one particle to the elements of an accumulation block matrix V3 -> V3. The result is returned in mat.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat : array[float]
@@ -3198,40 +3198,40 @@
             Number that will be multiplied by the basis functions of V3 and written to mat.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn[0] - 1
     pd2 = pn[1] - 1
     pd3 = pn[2] - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat, fill)
 
 
 @pure
-def m_v_fill_v3(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]', mat : 'float[:,:,:,:,:,:]', fill_m : float, vec : 'float[:,:,:]', fill_v : float):
+def m_v_fill_v3(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]', mat: 'float[:,:,:,:,:,:]', fill_m: float, vec: 'float[:,:,:]', fill_v: float):
     """
     Adds the contribution of one particle to the elements of an accumulation matrix V3 -> V3. The result is returned in mat.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat : array[float]
@@ -3247,30 +3247,30 @@
             Number that is multiplied by the basis functions of V3 and written to vec.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn[0] - 1
     pd2 = pn[1] - 1
     pd3 = pn[2] - 1
-    
+
     # fill matrix and vector entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat, fill_m, vec, fill_v)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def mat_fill_b_v0vec_diag(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float):
+def mat_fill_b_v0vec_diag(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3310,36 +3310,36 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def m_v_fill_b_v0vec_diag(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v0vec_diag(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3354,18 +3354,18 @@
             (logical) position of the particle in each direction.
 
         mat11, mat22, mat33 : array[float]
             (mu=1, nu=1)-, (mu=2, nu=2)- and (mu=3, nu=3)-block of the block matrix V0vec -> V0vec that is written to.
 
         fill11, fill22, fill33 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat22 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2, and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn)
@@ -3385,36 +3385,36 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat33, fill33, vec3, fill3)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def mat_fill_b_v3vec_diag(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float):
+def mat_fill_b_v3vec_diag(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3437,15 +3437,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn[0] - 1
     pd2 = pn[1] - 1
     pd3 = pn[2] - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -3458,36 +3458,36 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def m_v_fill_b_v3vec_diag(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v3vec_diag(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3502,29 +3502,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat22, mat33 : array[float]
             (mu=1, nu=1)-, (mu=2, nu=2)- and (mu=3, nu=3)-block of the block matrix V3vec -> V3vec that is written to.
 
         fill11, fill22, fill33 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat22 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -3537,36 +3537,36 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat33, fill33, vec3, fill3)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def mat_fill_b_v0vec_asym(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float):
+def mat_fill_b_v0vec_asym(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3606,36 +3606,36 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def m_v_fill_b_v0vec_asym(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v0vec_asym(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3650,18 +3650,18 @@
             (logical) position of the particle in each direction.
 
         mat12, mat13, mat23 : array[float]
             (mu=1, nu=2)-, (mu=1, nu=3)-, and (mu=2, nu=3)-block of the block matrix V0vec -> V0vec that is written to.
 
         fill12, fill13, fill23 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat12, mat13 and mat23.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn)
@@ -3681,42 +3681,42 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat12, fill12, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat23, fill23, vec2, fill2)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_vec(pn1, pn2, pn3, 
-                bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_vec(pn1, pn2, pn3,
+                bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0,
                 vec3, fill3)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def mat_fill_b_v3vec_asym(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float):
+def mat_fill_b_v3vec_asym(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3739,15 +3739,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -3760,36 +3760,36 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def m_v_fill_b_v3vec_asym(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v3vec_asym(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3804,29 +3804,29 @@
             (logical) position of the particle in each direction.
 
         mat12, mat13, mat23 : array[float]
             (mu=1, nu=2)-, (mu=1, nu=3)-, and (mu=2, nu=3)-block of the block matrix V3vec -> V3vec that is written to.
 
         fill12, fill13, fill23 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat12, mat13 and mat23.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -3839,42 +3839,42 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat12, fill12, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat23, fill23, vec2, fill2)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_vec(pd1, pd2, pd3, 
-                bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_vec(pd1, pd2, pd3,
+                bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3,
                 vec3, fill3)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def mat_fill_b_v0vec_symm(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float):
+def mat_fill_b_v0vec_symm(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3897,15 +3897,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
     bn3 = empty(pn[2] + 1, dtype=float)
 
     # spans (i.e. index for non-vanishing B-spline basis functions)
     span1 = bsp.find_span(tn1, pn1, eta1)
@@ -3914,54 +3914,54 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def m_v_fill_b_v0vec_symm(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v0vec_symm(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -3976,18 +3976,18 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
             (mu=1, nu=1)-, (mu=1, nu=2)-, (mu=1, nu=3), (mu=2, nu=2)-, (mu=2, nu=3)- and (mu=3, nu=3)-block of the block matrix V0vec -> V0vec that is written to.
 
         fill11, fill12, fill13, fill22, fill23, fill33 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat12, mat13, mat22, mat23 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn)
@@ -4007,54 +4007,54 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat13, fill13)
 
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def mat_fill_b_v3vec_symm(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float):
+def mat_fill_b_v3vec_symm(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -4077,15 +4077,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -4098,54 +4098,54 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def m_v_fill_b_v3vec_symm(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v3vec_symm(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -4160,29 +4160,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
             (mu=1, nu=1)-, (mu=1, nu=2)-, (mu=1, nu=3), (mu=2, nu=2)-, (mu=2, nu=3)- and (mu=3, nu=3)-block of the block matrix V3vec -> V3vec that is written to.
 
         fill11, fill12, fill13, fill22, fill23, fill33 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat12, mat13, mat22, mat23 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -4195,54 +4195,54 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat13, fill13)
 
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def mat_fill_b_v0vec_full(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float):
+def mat_fill_b_v0vec_full(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -4265,15 +4265,15 @@
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # non-vanishing B-splines at particle position
     bn1 = empty(pn[0] + 1, dtype=float)
     bn2 = empty(pn[1] + 1, dtype=float)
     bn3 = empty(pn[2] + 1, dtype=float)
 
     # spans (i.e. index for non-vanishing B-spline basis functions)
     span1 = bsp.find_span(tn1, pn1, eta1)
@@ -4282,72 +4282,72 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat21, fill21)
 
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat32, fill32)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bn1', 'bn2', 'bn3')
-def m_v_fill_b_v0vec_full(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts0 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]',  fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v0vec_full(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]',  fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -4362,18 +4362,18 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V0vec -> V0vec that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : B-splines (pn)
@@ -4393,72 +4393,72 @@
 
     # compute bn, i.e. values for non-vanishing B-splines at position eta
     bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
     bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
     bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat21, fill21)
 
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat32, fill32)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def mat_fill_b_v3vec_full(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float):
+def mat_fill_b_v3vec_full(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -4473,29 +4473,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V3vec -> V3vec that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -4508,72 +4508,72 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat21, fill21)
 
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat32, fill32)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat33, fill33)
 
 
 @pure
 @stack_array('bd1', 'bd2', 'bd3')
-def m_v_fill_b_v3vec_full(pn : 'int[:]', tn1 : 'float[:]', tn2 : 'float[:]', tn3 : 'float[:]', starts3 : 'int[:]', eta1 : float, eta2 : float, eta3 : float, mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]',  fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_b_v3vec_full(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts3: 'int[:]', eta1: float, eta2: float, eta3: float, mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]',  fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
@@ -4588,29 +4588,29 @@
             (logical) position of the particle in each direction.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V3vec -> V3vec that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     from numpy import empty
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
     # non-vanishing D-splines at particle position
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
@@ -4623,82 +4623,82 @@
 
     # compute bd, i.e. values for non-vanishing D-splines at position eta
     bsp.d_splines_slim(tn1, pn1, eta1, span1, bd1)
     bsp.d_splines_slim(tn2, pn2, eta2, span2, bd2)
     bsp.d_splines_slim(tn3, pn3, eta3, span3, bd3)
 
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat21, fill21)
 
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat32, fill32)
 
-    
+
 @pure
-def mat_fill_v0vec_diag(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float):
+def mat_fill_v0vec_diag(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
 
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat11, mat22, mat33 : array[float]
@@ -4708,105 +4708,105 @@
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat22 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v0vec_diag(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v0vec_diag(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
 
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat11, mat22, mat33 : array[float]
             (mu=1, nu=1)-, (mu=2, nu=2)- and (mu=3, nu=3)-block of the block matrix V0vec -> V0vec that is written to.
 
         fill11, fill22, fill33 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat22 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2, and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix and vector entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
                     starts0, pn,
                     mat33, fill33, vec3, fill3)
 
 
 @pure
-def mat_fill_v3vec_diag(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]', mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float):
+def mat_fill_v3vec_diag(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]', mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat11, mat22, mat33 : array[float]
@@ -4816,113 +4816,113 @@
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat22 and mat33.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v3vec_diag(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]', mat11 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill22 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v3vec_diag(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]', mat11: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill22: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the diagonal elements (mu,nu)=(1,1), (mu,nu)=(2,2) and (mu,nu)=(3,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat22 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat11, mat22, mat33 : array[float]
             (mu=1, nu=1)-, (mu=2, nu=2)- and (mu=3, nu=3)-block of the block matrix V3vec -> V3vec that is written to.
 
         fill11, fill22, fill33 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat22 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix and vector entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
                     starts3, pn,
                     mat33, fill33, vec3, fill3)
-    
+
 
 @pure
-def mat_fill_v0vec_asym(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float):
+def mat_fill_v0vec_asym(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
 
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat12, mat13, mat23 : array[float]
@@ -4932,111 +4932,111 @@
             Numbers that will be multiplied by the basis functions of V0vec and written to mat12, mat13 and mat23.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
 
 
 @pure
-def m_v_fill_v0vec_asym(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v0vec_asym(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
 
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat12, mat13, mat23 : array[float]
             (mu=1, nu=2)-, (mu=1, nu=3)-, and (mu=2, nu=3)-block of the block matrix V0vec -> V0vec that is written to.
 
         fill12, fill13, fill23 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat12, mat13 and mat23.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat12, fill12, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat23, fill23, vec2, fill2)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_vec(pn1, pn2, pn3, 
-                bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_vec(pn1, pn2, pn3,
+                bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0,
                 vec3, fill3)
 
 
 @pure
-def mat_fill_v3vec_asym(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float):
+def mat_fill_v3vec_asym(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V3 -> V3. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat12, mat13, mat23 : array[float]
@@ -5046,119 +5046,119 @@
             Numbers that will be multiplied by the basis functions of V3vec and written to mat12, mat13 and mat23.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
 
 
 @pure
-def m_v_fill_v3vec_asym(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', fill12 : float, fill13 : float, fill23 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v3vec_asym(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', fill12: float, fill13: float, fill23: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the antisymmetric elements (mu,nu)=(1,2), (mu,nu)=(1,3) and (mu,nu)=(2,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat12, mat13 and mat23.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat12, mat13, mat23 : array[float]
             (mu=1, nu=2)-, (mu=1, nu=3)-, and (mu=2, nu=3)-block of the block matrix V3vec -> V3vec that is written to.
 
         fill12, fill13, fill23 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat12, mat13 and mat23.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat12, fill12, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat23, fill23, vec2, fill2)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_vec(pd1, pd2, pd3, 
-                bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_vec(pd1, pd2, pd3,
+                bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3,
                 vec3, fill3)
 
 
 @pure
-def mat_fill_v0vec_symm(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float):
+def mat_fill_v0vec_symm(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
 
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
@@ -5168,141 +5168,141 @@
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat12, mat13, mat22, mat23 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v0vec_symm(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v0vec_symm(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
 
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
             (mu=1, nu=1)-, (mu=1, nu=2)-, (mu=1, nu=3), (mu=2, nu=2)-, (mu=2, nu=3)- and (mu=3, nu=3)-block of the block matrix V0vec -> V0vec that is written to.
 
         fill11, fill12, fill13, fill22, fill23, fill33 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat12, mat13, mat22, mat23 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat13, fill13)
 
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
 
 
 @pure
-def mat_fill_v3vec_symm(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]', mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float):
+def mat_fill_v3vec_symm(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]', mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
@@ -5312,511 +5312,512 @@
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat12, mat13, mat22, mat23 and mat33.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v3vec_symm(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]', mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v3vec_symm(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]', mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat12, mat13, mat22, mat23 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat11, mat12, mat13, mat22, mat23, mat33 : array[float]
             (mu=1, nu=1)-, (mu=1, nu=2)-, (mu=1, nu=3), (mu=2, nu=2)-, (mu=2, nu=3)- and (mu=3, nu=3)-block of the block matrix V3vec -> V3vec that is written to.
 
         fill11, fill12, fill13, fill22, fill23, fill33 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat12, mat13, mat22, mat23 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat13, fill13)
 
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
 
 
 @pure
-def mat_fill_v0vec_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float):
+def mat_fill_v0vec_full(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
-            
+
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat13, mat23, mat33 : array[float]
             All 9 blocks of the block matrix V0vec -> V0vec that is written to.
 
         fill11, fill12, fill13, fill12, fill23, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat12, mat13, mat12, mat22, mat23, mat13, mat23 and mat33.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix entries
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat21, fill21)
 
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat32, fill32)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat33, fill33)
 
+
 @pure
-def m_v_fill_v0vec_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]',  fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v0vec_full(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]',  fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V0vec -> V0vec. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bn1, bn2, bn3 : array[float]
             Evaluated B-splines at particle position in each direction.
 
         starts0 : array[int]
             Start indices of the current process in space V0.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V0vec -> V0vec that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V0vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : B-splines (pn)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3, 
-                    bn1, bn2, bn3, bn1, bn2, bn3, 
-                    span1, span2, span3, 
-                    starts0, pn, 
+
+    fk.fill_mat_vec(pn1, pn2, pn3, pn1, pn2, pn3,
+                    bn1, bn2, bn3, bn1, bn2, bn3,
+                    span1, span2, span3,
+                    starts0, pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat21, fill21)
 
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3, 
-                bn1, bn2, bn3, bn1, bn2, bn3, 
-                span1, span2, span3, 
-                starts0, pn, 
+
+    fk.fill_mat(pn1, pn2, pn3, pn1, pn2, pn3,
+                bn1, bn2, bn3, bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0, pn,
                 mat32, fill32)
 
 
 @pure
-def mat_fill_v3vec_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float):
+def mat_fill_v3vec_full(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V3vec -> V3vec that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat11, fill11)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat21, fill21)
 
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat22, fill22)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat32, fill32)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat33, fill33)
 
 
 @pure
-def m_v_fill_v3vec_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts3 : 'int[:]',  mat11 : 'float[:,:,:,:,:,:]', mat12 : 'float[:,:,:,:,:,:]', mat13 : 'float[:,:,:,:,:,:]', mat21 : 'float[:,:,:,:,:,:]', mat22 : 'float[:,:,:,:,:,:]', mat23 : 'float[:,:,:,:,:,:]', mat31 : 'float[:,:,:,:,:,:]', mat32 : 'float[:,:,:,:,:,:]', mat33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill21 : float, fill22 : float, fill23 : float, fill31 : float, fill32 : float, fill33 : float, vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]',  fill1 : float, fill2 : float, fill3 : float):
+def m_v_fill_v3vec_full(pn: 'int[:]', span1: int, span2: int, span3: int, bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts3: 'int[:]',  mat11: 'float[:,:,:,:,:,:]', mat12: 'float[:,:,:,:,:,:]', mat13: 'float[:,:,:,:,:,:]', mat21: 'float[:,:,:,:,:,:]', mat22: 'float[:,:,:,:,:,:]', mat23: 'float[:,:,:,:,:,:]', mat31: 'float[:,:,:,:,:,:]', mat32: 'float[:,:,:,:,:,:]', mat33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill21: float, fill22: float, fill23: float, fill31: float, fill32: float, fill33: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]',  fill1: float, fill2: float, fill3: float):
     """
     Adds the contribution of one particle to the generic elements (mu,nu) of an accumulation block matrix V3vec -> V3vec. The result is returned in mat11, mat12, mat13, mat21, mat22, mat23, mat31, mat32 and mat33.
 
     Parameters 
     ----------
         pn : array[int]
             Spline degrees in each direction.
 
         span1, span2, span3 : int
             Spline knot span indices in each direction.
-            
+
         bd1, bd2, bd3 : array[float]
             Evaluated D-splines at particle position in each direction.
 
         starts3 : array[int]
             Start indices of the current process in space V3.
 
         mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32, mat33 : array[float]
             All 9 blocks of the block matrix V3vec -> V3vec that is written to.
 
         fill11, fill12, fill13, fill21, fill22, fill23, fill31, fill32, fill33 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to mat11, mat12, mat13, mat12, mat22, mat23, mat31, mat32 and mat33.
-            
+
         vec1, vec2, vec3 : array[float]
             mu=1, mu=2 and mu=3-component of the vector that is written to.
-            
+
         fill1, fill2, fill3 : float
             Numbers that will be multiplied by the basis functions of V3vec and written to vec1, vec2 and vec3.
     """
 
     # degrees of the basis functions : D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix entries
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat11, fill11, vec1, fill1)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat22, fill22, vec2, fill2)
-    
-    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3, 
-                    bd1, bd2, bd3, bd1, bd2, bd3, 
-                    span1, span2, span3, 
-                    starts3, pn, 
+
+    fk.fill_mat_vec(pd1, pd2, pd3, pd1, pd2, pd3,
+                    bd1, bd2, bd3, bd1, bd2, bd3,
+                    span1, span2, span3,
+                    starts3, pn,
                     mat33, fill33, vec3, fill3)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat12, fill12)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
-                mat13, fill13)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
+                mat13, fill13)
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat21, fill21)
 
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat23, fill23)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat31, fill31)
-    
-    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3, 
-                bd1, bd2, bd3, bd1, bd2, bd3, 
-                span1, span2, span3, 
-                starts3, pn, 
+
+    fk.fill_mat(pd1, pd2, pd3, pd1, pd2, pd3,
+                bd1, bd2, bd3, bd1, bd2, bd3,
+                span1, span2, span3,
+                starts3, pn,
                 mat32, fill32)
 
 
 @pure
-def m_v_fill_v1_pressure_full(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', mat11_11 : 'float[:,:,:,:,:,:]', mat12_11 : 'float[:,:,:,:,:,:]', mat13_11 : 'float[:,:,:,:,:,:]', mat22_11 : 'float[:,:,:,:,:,:]', mat23_11 : 'float[:,:,:,:,:,:]', mat33_11 : 'float[:,:,:,:,:,:]', mat11_12 : 'float[:,:,:,:,:,:]', mat12_12 : 'float[:,:,:,:,:,:]', mat13_12 : 'float[:,:,:,:,:,:]', mat22_12 : 'float[:,:,:,:,:,:]', mat23_12 : 'float[:,:,:,:,:,:]', mat33_12 : 'float[:,:,:,:,:,:]', mat11_13 : 'float[:,:,:,:,:,:]', mat12_13 : 'float[:,:,:,:,:,:]', mat13_13 : 'float[:,:,:,:,:,:]', mat22_13 : 'float[:,:,:,:,:,:]', mat23_13 : 'float[:,:,:,:,:,:]', mat33_13 : 'float[:,:,:,:,:,:]', mat11_22 : 'float[:,:,:,:,:,:]', mat12_22 : 'float[:,:,:,:,:,:]', mat13_22 : 'float[:,:,:,:,:,:]', mat22_22 : 'float[:,:,:,:,:,:]', mat23_22 : 'float[:,:,:,:,:,:]', mat33_22 : 'float[:,:,:,:,:,:]', mat11_23 : 'float[:,:,:,:,:,:]', mat12_23 : 'float[:,:,:,:,:,:]', mat13_23 : 'float[:,:,:,:,:,:]', mat22_23 : 'float[:,:,:,:,:,:]', mat23_23 : 'float[:,:,:,:,:,:]', mat33_23 : 'float[:,:,:,:,:,:]', mat11_33 : 'float[:,:,:,:,:,:]', mat12_33 : 'float[:,:,:,:,:,:]', mat13_33 : 'float[:,:,:,:,:,:]', mat22_33 : 'float[:,:,:,:,:,:]', mat23_33 : 'float[:,:,:,:,:,:]', mat33_33 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1_1 : 'float[:,:,:]', vec2_1 : 'float[:,:,:]',  vec3_1 : 'float[:,:,:]', vec1_2 : 'float[:,:,:]', vec2_2 : 'float[:,:,:]',  vec3_2 : 'float[:,:,:]', vec1_3 : 'float[:,:,:]', vec2_3 : 'float[:,:,:]',  vec3_3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float, vx : float, vy : float, vz : float):
+def m_v_fill_v1_pressure_full(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', mat11_11: 'float[:,:,:,:,:,:]', mat12_11: 'float[:,:,:,:,:,:]', mat13_11: 'float[:,:,:,:,:,:]', mat22_11: 'float[:,:,:,:,:,:]', mat23_11: 'float[:,:,:,:,:,:]', mat33_11: 'float[:,:,:,:,:,:]', mat11_12: 'float[:,:,:,:,:,:]', mat12_12: 'float[:,:,:,:,:,:]', mat13_12: 'float[:,:,:,:,:,:]', mat22_12: 'float[:,:,:,:,:,:]', mat23_12: 'float[:,:,:,:,:,:]', mat33_12: 'float[:,:,:,:,:,:]', mat11_13: 'float[:,:,:,:,:,:]', mat12_13: 'float[:,:,:,:,:,:]', mat13_13: 'float[:,:,:,:,:,:]', mat22_13: 'float[:,:,:,:,:,:]', mat23_13: 'float[:,:,:,:,:,:]', mat33_13: 'float[:,:,:,:,:,:]', mat11_22: 'float[:,:,:,:,:,:]', mat12_22: 'float[:,:,:,:,:,:]', mat13_22: 'float[:,:,:,:,:,:]', mat22_22: 'float[:,:,:,:,:,:]', mat23_22: 'float[:,:,:,:,:,:]', mat33_22: 'float[:,:,:,:,:,:]', mat11_23: 'float[:,:,:,:,:,:]', mat12_23: 'float[:,:,:,:,:,:]', mat13_23: 'float[:,:,:,:,:,:]', mat22_23: 'float[:,:,:,:,:,:]', mat23_23: 'float[:,:,:,:,:,:]', mat33_23: 'float[:,:,:,:,:,:]', mat11_33: 'float[:,:,:,:,:,:]', mat12_33: 'float[:,:,:,:,:,:]', mat13_33: 'float[:,:,:,:,:,:]', mat22_33: 'float[:,:,:,:,:,:]', mat23_33: 'float[:,:,:,:,:,:]', mat33_33: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1_1: 'float[:,:,:]', vec2_1: 'float[:,:,:]',  vec3_1: 'float[:,:,:]', vec1_2: 'float[:,:,:]', vec2_2: 'float[:,:,:]',  vec3_2: 'float[:,:,:]', vec1_3: 'float[:,:,:]', vec2_3: 'float[:,:,:]',  vec3_3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float, vx: float, vy: float, vz: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. 
     The result is returned in mat11_xy, mat12_xy, mat13_xy, mat22_xy, mat23_xy, mat33_xy, vec1_x, vec2_x, vec3_x (x and y denotes components of velocity for the accumulation of the pressure tensor).
 
     Parameters 
     ----------
         pn : array[int]
@@ -5850,68 +5851,68 @@
             Component of the particle velocity.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix and vector entries
     fk.fill_mat_vec_pressure_full(pd1, pn2, pn3, pd1, pn2, pn3,
                                   bd1, bn2, bn3, bd1, bn2, bn3,
                                   span1, span2, span3,
                                   starts1[0], pn,
-                                  mat11_11, mat11_12, mat11_13, mat11_22, mat11_23, mat11_33, fill11, 
-                                  vec1_1, vec1_2, vec1_3, fill1, 
+                                  mat11_11, mat11_12, mat11_13, mat11_22, mat11_23, mat11_33, fill11,
+                                  vec1_1, vec1_2, vec1_3, fill1,
                                   vx, vy, vz)
-    
+
     fk.fill_mat_vec_pressure_full(pn1, pd2, pn3, pn1, pd2, pn3,
                                   bn1, bd2, bn3, bn1, bd2, bn3,
                                   span1, span2, span3,
                                   starts1[1], pn,
-                                  mat22_11, mat22_12, mat22_13, mat22_22, mat22_23, mat22_33, fill22, 
-                                  vec2_1, vec2_2, vec2_3, fill2, 
+                                  mat22_11, mat22_12, mat22_13, mat22_22, mat22_23, mat22_33, fill22,
+                                  vec2_1, vec2_2, vec2_3, fill2,
                                   vx, vy, vz)
-    
+
     fk.fill_mat_vec_pressure_full(pn1, pn2, pd3, pn1, pn2, pd3,
                                   bn1, bn2, bd3, bn1, bn2, bd3,
                                   span1, span2, span3,
                                   starts1[2], pn,
-                                  mat33_11, mat33_12, mat33_13, mat33_22, mat33_23, mat33_33, fill33, 
-                                  vec3_1, vec3_2, vec3_3, fill3, 
+                                  mat33_11, mat33_12, mat33_13, mat33_22, mat33_23, mat33_33, fill33,
+                                  vec3_1, vec3_2, vec3_3, fill3,
                                   vx, vy, vz)
-    
+
     fk.fill_mat_pressure_full(pd1, pn2, pn3, pn1, pd2, pn3,
                               bd1, bn2, bn3, bn1, bd2, bn3,
                               span1, span2, span3,
                               starts1[0], pn,
-                              mat12_11, mat12_12, mat12_13, mat12_22, mat12_23, mat12_33, fill12, 
+                              mat12_11, mat12_12, mat12_13, mat12_22, mat12_23, mat12_33, fill12,
                               vx, vy, vz)
-    
+
     fk.fill_mat_pressure_full(pd1, pn2, pn3, pn1, pn2, pd3,
                               bd1, bn2, bn3, bn1, bn2, bd3,
                               span1, span2, span3,
                               starts1[0], pn,
-                              mat13_11, mat13_12, mat13_13, mat13_22, mat13_23, mat13_33, fill13, 
+                              mat13_11, mat13_12, mat13_13, mat13_22, mat13_23, mat13_33, fill13,
                               vx, vy, vz)
-    
+
     fk.fill_mat_pressure_full(pn1, pd2, pn3, pn1, pn2, pd3,
                               bn1, bd2, bn3, bn1, bn2, bd3,
                               span1, span2, span3,
                               starts1[1], pn,
-                              mat23_11, mat23_12, mat23_13, mat23_22, mat23_23, mat23_33, fill23, 
+                              mat23_11, mat23_12, mat23_13, mat23_22, mat23_23, mat23_33, fill23,
                               vx, vy, vz)
 
 
 @pure
-def m_v_fill_v1_pressure(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', mat11_11 : 'float[:,:,:,:,:,:]', mat12_11 : 'float[:,:,:,:,:,:]', mat13_11 : 'float[:,:,:,:,:,:]', mat22_11 : 'float[:,:,:,:,:,:]', mat23_11 : 'float[:,:,:,:,:,:]', mat33_11 : 'float[:,:,:,:,:,:]', mat11_12 : 'float[:,:,:,:,:,:]', mat12_12 : 'float[:,:,:,:,:,:]', mat13_12 : 'float[:,:,:,:,:,:]', mat22_12 : 'float[:,:,:,:,:,:]', mat23_12 : 'float[:,:,:,:,:,:]', mat33_12 : 'float[:,:,:,:,:,:]', mat11_22 : 'float[:,:,:,:,:,:]', mat12_22 : 'float[:,:,:,:,:,:]', mat13_22 : 'float[:,:,:,:,:,:]', mat22_22 : 'float[:,:,:,:,:,:]', mat23_22 : 'float[:,:,:,:,:,:]', mat33_22 : 'float[:,:,:,:,:,:]', fill11 : float, fill12 : float, fill13 : float, fill22 : float, fill23 : float, fill33 : float, vec1_1 : 'float[:,:,:]', vec2_1 : 'float[:,:,:]',  vec3_1 : 'float[:,:,:]', vec1_2 : 'float[:,:,:]', vec2_2 : 'float[:,:,:]',  vec3_2 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float, vx : float, vy : float):
+def m_v_fill_v1_pressure(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', mat11_11: 'float[:,:,:,:,:,:]', mat12_11: 'float[:,:,:,:,:,:]', mat13_11: 'float[:,:,:,:,:,:]', mat22_11: 'float[:,:,:,:,:,:]', mat23_11: 'float[:,:,:,:,:,:]', mat33_11: 'float[:,:,:,:,:,:]', mat11_12: 'float[:,:,:,:,:,:]', mat12_12: 'float[:,:,:,:,:,:]', mat13_12: 'float[:,:,:,:,:,:]', mat22_12: 'float[:,:,:,:,:,:]', mat23_12: 'float[:,:,:,:,:,:]', mat33_12: 'float[:,:,:,:,:,:]', mat11_22: 'float[:,:,:,:,:,:]', mat12_22: 'float[:,:,:,:,:,:]', mat13_22: 'float[:,:,:,:,:,:]', mat22_22: 'float[:,:,:,:,:,:]', mat23_22: 'float[:,:,:,:,:,:]', mat33_22: 'float[:,:,:,:,:,:]', fill11: float, fill12: float, fill13: float, fill22: float, fill23: float, fill33: float, vec1_1: 'float[:,:,:]', vec2_1: 'float[:,:,:]',  vec3_1: 'float[:,:,:]', vec1_2: 'float[:,:,:]', vec2_2: 'float[:,:,:]',  vec3_2: 'float[:,:,:]', fill1: float, fill2: float, fill3: float, vx: float, vy: float):
     """
     Adds the contribution of one particle to the symmetric elements (mu,nu)=(1,1), (mu,nu)=(1,2), (mu,nu)=(1,3), (mu,nu)=(2,2), (mu,nu)=(2,3) and (mu,nu)=(3,3) of an accumulation block matrix V1 -> V1. 
     The result is returned in mat11_xy, mat12_xy, mat13_xy, mat22_xy, mat23_xy, mat33_xy, vec1_x, vec2_x, vec3_x (x and y denotes components of velocity for the accumulation of the pressure tensor).
 
     Parameters 
     ----------
         pn : array[int]
@@ -5945,174 +5946,375 @@
             Component of the particle velocity.
     """
 
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
-    
+
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
-    
+
     # fill matrix and vector entries
     fk.fill_mat_vec_pressure(pd1, pn2, pn3, pd1, pn2, pn3,
                              bd1, bn2, bn3, bd1, bn2, bn3,
                              span1, span2, span3,
                              starts1[0], pn,
-                             mat11_11, mat11_12, mat11_22, fill11, 
-                             vec1_1, vec1_2, fill1, 
+                             mat11_11, mat11_12, mat11_22, fill11,
+                             vec1_1, vec1_2, fill1,
                              vx, vy)
-    
+
     fk.fill_mat_vec_pressure(pn1, pd2, pn3, pn1, pd2, pn3,
                              bn1, bd2, bn3, bn1, bd2, bn3,
                              span1, span2, span3,
                              starts1[1], pn,
-                             mat22_11, mat22_12, mat22_22, fill22, 
-                             vec2_1, vec2_2, fill2, 
+                             mat22_11, mat22_12, mat22_22, fill22,
+                             vec2_1, vec2_2, fill2,
                              vx, vy)
-    
+
     fk.fill_mat_vec_pressure(pn1, pn2, pd3, pn1, pn2, pd3,
                              bn1, bn2, bd3, bn1, bn2, bd3,
                              span1, span2, span3,
                              starts1[2], pn,
-                             mat33_11, mat33_12, mat33_22, fill33, 
-                             vec3_1, vec3_2, fill3, 
+                             mat33_11, mat33_12, mat33_22, fill33,
+                             vec3_1, vec3_2, fill3,
                              vx, vy)
-    
+
     fk.fill_mat_pressure(pd1, pn2, pn3, pn1, pd2, pn3,
                          bd1, bn2, bn3, bn1, bd2, bn3,
                          span1, span2, span3,
                          starts1[0], pn,
-                         mat12_11, mat12_12, mat12_22, fill12, 
+                         mat12_11, mat12_12, mat12_22, fill12,
                          vx, vy)
-    
+
     fk.fill_mat_pressure(pd1, pn2, pn3, pn1, pn2, pd3,
                          bd1, bn2, bn3, bn1, bn2, bd3,
                          span1, span2, span3,
                          starts1[0], pn,
-                         mat13_11, mat13_12, mat13_22, fill13, 
+                         mat13_11, mat13_12, mat13_22, fill13,
                          vx, vy)
-    
+
     fk.fill_mat_pressure(pn1, pd2, pn3, pn1, pn2, pd3,
                          bn1, bd2, bn3, bn1, bn2, bd3,
                          span1, span2, span3,
                          starts1[1], pn,
-                         mat23_11, mat23_12, mat23_22, fill23, 
+                         mat23_11, mat23_12, mat23_22, fill23,
                          vx, vy)
 
 
 @pure
 def hybrid_density(Nel: 'int[:]', pn: 'int[:]', cell_left: 'int[:]', cell_number: 'int[:]', span1: 'int', span2: 'int', span3: 'int', starts0: 'int[:]', ie1: 'int', ie2: 'int', ie3: 'int', temp1: 'float[:]', temp4: 'float[:]', quad: 'int[:]', quad_pts_x: 'float[:]', quad_pts_y: 'float[:]', quad_pts_z: 'float[:]', compact: 'float[:]', eta1: 'float', eta2: 'float', eta3: 'float', mat: 'float[:,:,:,:,:,:]', weight: 'float', p_shape: 'int[:]', p_size: 'float[:]', grids_shapex: 'float[:]', grids_shapey: 'float[:]', grids_shapez: 'float[:]'):
 
-    fk.hy_density(Nel, pn, cell_left, cell_number, span1, span2, span3, starts0, ie1, ie2, ie3, temp1, temp4, quad, quad_pts_x, quad_pts_y, quad_pts_z, compact, eta1, eta2, eta3, mat, weight, p_shape, p_size, grids_shapex, grids_shapey, grids_shapez)
+    fk.hy_density(Nel, pn, cell_left, cell_number, span1, span2, span3, starts0, ie1, ie2, ie3, temp1, temp4, quad, quad_pts_x,
+                  quad_pts_y, quad_pts_z, compact, eta1, eta2, eta3, mat, weight, p_shape, p_size, grids_shapex, grids_shapey, grids_shapez)
+
+
+@pure
+def vec_fill_v0(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
+    """TODO
+    """
+
+    # degrees of the basis functions : B-splines (pn) and D-splines (pd)
+    pn1 = pn[0]
+    pn2 = pn[1]
+    pn3 = pn[2]
+
+    # fill vector entries
+    fk.fill_vec(pn1, pn2, pn3,
+                bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0,
+                vec1, fill1)
+
+    fk.fill_vec(pn1, pn2, pn3,
+                bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0,
+                vec2, fill2)
+
+    fk.fill_vec(pn1, pn2, pn3,
+                bn1, bn2, bn3,
+                span1, span2, span3,
+                starts0,
+                vec3, fill3)
+
+
+@pure
+def vec_fill_v1(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts1: 'int[:,:]', vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
+    """TODO
+    """
+
+    # degrees of the basis functions : B-splines (pn) and D-splines (pd)
+    pn1 = pn[0]
+    pn2 = pn[1]
+    pn3 = pn[2]
+
+    pd1 = pn1 - 1
+    pd2 = pn2 - 1
+    pd3 = pn3 - 1
+
+    # fill vector entries
+    fk.fill_vec(pd1, pn2, pn3,
+                bd1, bn2, bn3,
+                span1, span2, span3,
+                starts1[0],
+                vec1, fill1)
+
+    fk.fill_vec(pn1, pd2, pn3,
+                bn1, bd2, bn3,
+                span1, span2, span3,
+                starts1[1],
+                vec2, fill2)
+
+    fk.fill_vec(pn1, pn2, pd3,
+                bn1, bn2, bd3,
+                span1, span2, span3,
+                starts1[2],
+                vec3, fill3)
+
+
+@pure
+def vec_fill_v2(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]', starts2: 'int[:,:]', vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
+    """TODO
+    """
+
+    # degrees of the basis functions : B-splines (pn) and D-splines (pd)
+    pn1 = pn[0]
+    pn2 = pn[1]
+    pn3 = pn[2]
+
+    pd1 = pn1 - 1
+    pd2 = pn2 - 1
+    pd3 = pn3 - 1
+
+    # fill vector entries
+    fk.fill_vec(pn1, pd2, pd3,
+                bn1, bd2, bd3,
+                span1, span2, span3,
+                starts2[0],
+                vec1, fill1)
+
+    fk.fill_vec(pd1, pn2, pd3,
+                bd1, bn2, bd3,
+                span1, span2, span3,
+                starts2[1],
+                vec2, fill2)
+
+    fk.fill_vec(pd1, pd2, pn3,
+                bd1, bd2, bn3,
+                span1, span2, span3,
+                starts2[2],
+                vec3, fill3)
+
+
+@pure
+def scalar_fill_v0(pn: 'int[:]', span1: int, span2: int, span3: int, bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]', starts0: 'int[:]', vec: 'float[:,:,:]', fill: float):
+    """TODO
+    """
+
+    # degrees of the basis functions : B-splines (pn) and D-splines (pd)
+    pn1 = pn[0]
+    pn2 = pn[1]
+    pn3 = pn[2]
+
+    fk.fill_vec(pn1, pn2, pn3, bn1, bn2, bn3, span1,
+                span2, span3, starts0, vec, fill)
 
 
 @pure
-def vec_fill_v0(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+@stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
+def vec_fill_b_v0(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """TODO
     """
 
+    from numpy import empty
+
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
 
+    # non-vanishing B-splines at particle position
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    # spans (i.e. index for non-vanishing B-spline basis functions)
+    span1 = bsp.find_span(tn1, pn1, eta1)
+    span2 = bsp.find_span(tn2, pn2, eta2)
+    span3 = bsp.find_span(tn3, pn3, eta3)
+
+    # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
+    bsp.b_splines_slim(tn1, pn1, eta1, span1, bn1)
+    bsp.b_splines_slim(tn2, pn2, eta2, span2, bn2)
+    bsp.b_splines_slim(tn3, pn3, eta3, span3, bn3)
+
     # fill vector entries
     fk.fill_vec(pn1, pn2, pn3,
                 bn1, bn2, bn3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts0,
                 vec1, fill1)
 
     fk.fill_vec(pn1, pn2, pn3,
                 bn1, bn2, bn3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts0,
                 vec2, fill2)
 
     fk.fill_vec(pn1, pn2, pn3,
                 bn1, bn2, bn3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts0,
                 vec3, fill3)
 
 
 @pure
-def vec_fill_v1(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts1 : 'int[:,:]', vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+@stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
+def vec_fill_b_v1(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts1: 'int[:,:]', eta1: float, eta2: float, eta3: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """TODO
     """
 
+    from numpy import empty
+
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
 
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
+    # non-vanishing B-splines at particle position
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    # non-vanishing D-splines at particle position
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # spans (i.e. index for non-vanishing B-spline basis functions)
+    span1 = bsp.find_span(tn1, pn1, eta1)
+    span2 = bsp.find_span(tn2, pn2, eta2)
+    span3 = bsp.find_span(tn3, pn3, eta3)
+
+    # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
+    bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
+    bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
+    bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
+
     # fill vector entries
     fk.fill_vec(pd1, pn2, pn3,
                 bd1, bn2, bn3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts1[0],
                 vec1, fill1)
 
     fk.fill_vec(pn1, pd2, pn3,
                 bn1, bd2, bn3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts1[1],
                 vec2, fill2)
 
     fk.fill_vec(pn1, pn2, pd3,
                 bn1, bn2, bd3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts1[2],
                 vec3, fill3)
 
 
 @pure
-def vec_fill_v2(pn : 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', bd1 : 'float[:]', bd2 : 'float[:]', bd3 : 'float[:]', starts2 : 'int[:,:]', vec1 : 'float[:,:,:]', vec2 : 'float[:,:,:]',  vec3 : 'float[:,:,:]', fill1 : float, fill2 : float, fill3 : float):
+@stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
+def vec_fill_b_v2(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts2: 'int[:,:]', eta1: float, eta2: float, eta3: float, vec1: 'float[:,:,:]', vec2: 'float[:,:,:]',  vec3: 'float[:,:,:]', fill1: float, fill2: float, fill3: float):
     """TODO
     """
 
+    from numpy import empty
+
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
 
     pd1 = pn1 - 1
     pd2 = pn2 - 1
     pd3 = pn3 - 1
 
+    # non-vanishing B-splines at particle position
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    # non-vanishing D-splines at particle position
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # spans (i.e. index for non-vanishing B-spline basis functions)
+    span1 = bsp.find_span(tn1, pn1, eta1)
+    span2 = bsp.find_span(tn2, pn2, eta2)
+    span3 = bsp.find_span(tn3, pn3, eta3)
+
+    # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
+    bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
+    bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
+    bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
+
     # fill vector entries
     fk.fill_vec(pn1, pd2, pd3,
                 bn1, bd2, bd3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts2[0],
                 vec1, fill1)
 
     fk.fill_vec(pd1, pn2, pd3,
                 bd1, bn2, bd3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts2[1],
                 vec2, fill2)
 
     fk.fill_vec(pd1, pd2, pn3,
                 bd1, bd2, bn3,
-                span1, span2, span3, 
+                span1, span2, span3,
                 starts2[2],
                 vec3, fill3)
 
 
 @pure
-def scalar_fill_v0(pn: 'int[:]', span1 : int, span2 : int, span3 : int, bn1 : 'float[:]', bn2 : 'float[:]', bn3 : 'float[:]', starts0 : 'int[:]', vec : 'float[:,:,:]', fill : float):
+@stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
+def scalar_fill_b_v0(pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]', starts0: 'int[:]', eta1: float, eta2: float, eta3: float, vec: 'float[:,:,:]', fill: float):
     """TODO
     """
 
+    from numpy import empty
+
     # degrees of the basis functions : B-splines (pn) and D-splines (pd)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
 
-    fk.fill_vec(pn1, pn2, pn3, bn1, bn2, bn3, span1, span2, span3, starts0, vec, fill)
+    # non-vanishing B-splines at particle position
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    # non-vanishing D-splines at particle position
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    # spans (i.e. index for non-vanishing B-spline basis functions)
+    span1 = bsp.find_span(tn1, pn1, eta1)
+    span2 = bsp.find_span(tn2, pn2, eta2)
+    span3 = bsp.find_span(tn3, pn3, eta3)
+
+    # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
+    bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
+    bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
+    bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
+
+    fk.fill_vec(pn1, pn2, pn3, bn1, bn2, bn3, span1,
+                span2, span3, starts0, vec, fill)
```

### Comparing `struphy-1.9.9/src/struphy/pic/particles.py` & `struphy-2.0.0/src/struphy/pic/particles.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                           'domain_array': None
                           }
 
         self._params = set_defaults(params, params_default)
 
         self._name = name
         self._domain = params['domain']
-        self._bc =     params['bc_type']
+        self._bc = params['bc_type']
         self._domain_decomp = params['domain_array']
 
         assert params['comm'] is not None
         self._mpi_comm = params['comm']
         self._mpi_size = params['comm'].Get_size()
         self._mpi_rank = params['comm'].Get_rank()
 
@@ -189,15 +189,15 @@
         return self._markers[~self._holes]
 
     @property
     def domain(self):
         """ struphy.geometry.domains
         """
         return self._domain
-    
+
     @property
     def bc(self):
         """ Kinetic boundary conditions in each direction.
         """
         return self._bc
 
     def create_marker_array(self):
@@ -223,38 +223,40 @@
             ppc = Np/n_cells
 
         Np = int(Np)
         assert Np >= self._mpi_size
 
         # array of number of markers on each process at loading stage
         self._n_mks_load = np.zeros(self._mpi_size, dtype=int)
-        self._mpi_comm.Allgather(np.array([int(ppc*n_cells_loc)]), self._n_mks_load)
+        self._mpi_comm.Allgather(np.array([int(ppc*n_cells_loc)]),
+                                 self._n_mks_load)
 
         # add deviation from Np to rank 0
         self._n_mks_load[0] += Np - np.sum(self._n_mks_load)
 
         # check if all markers are there
         assert np.sum(self._n_mks_load) == Np
         self._n_mks = Np
 
         # number of markers on the local process at loading stage
         n_mks_load_loc = self._n_mks_load[self._mpi_rank]
 
         # create markers array (3 x positions, vdim x velocities, weight, s0, w0, ..., ID) with eps send/receive buffer
-        markers_size = round(n_mks_load_loc*(1 + 1/np.sqrt(n_mks_load_loc) + self.params['eps']))
+        markers_size = round(n_mks_load_loc *
+                             (1 + 1/np.sqrt(n_mks_load_loc) + self.params['eps']))
         self._markers = np.zeros((markers_size, self.n_cols), dtype=float)
 
     def draw_markers(self):
         """ Draw markers. 
         """
 
         # number of markers on the local process at loading stage
         n_mks_load_loc = self.n_mks_load[self._mpi_rank]
 
-        # cumulative sum of number of markers on each process at loading stage. 
+        # cumulative sum of number of markers on each process at loading stage.
         n_mks_load_cum_sum = np.cumsum(self.n_mks_load)
 
         # load markers from external .hdf5 file
         if self._params['loading']['type'] == 'external':
 
             if self._mpi_rank == 0:
                 file = h5py.File(self._params['loading']['dir_markers'], 'r')
@@ -395,58 +397,61 @@
 
         bckgr_params : dict (optional)
             Dictionary of the form {type : class_name, class_name : params_dict} defining the background.
         """
         if self._use_control_variate:
             assert bckgr_params is not None, 'When control variate is used, background parameters must be given!'
 
-        # compute s0 and save at vdim+4
-        self._markers[~self._holes, self.vdim+4] = self.s0(*self.markers_wo_holes[:, :self.vdim+3].T)
+        # compute s0 and save at vdim + 4
+        self._markers[~self._holes, self.vdim + 4] = \
+            self.s0(*self.markers_wo_holes[:, :self.vdim + 3].T)
 
         # load distribution function (with given parameters or default parameters)
         fun_name = fun_params['type']
 
         if fun_name in fun_params:
             f_init = getattr(analytical, fun_name)(**fun_params[fun_name])
         else:
             f_init = getattr(analytical, fun_name)()
 
-        # compute w0 and save at vdim+5
-        self._markers[~self._holes, self.vdim+5] = f_init(
-            *self.markers_wo_holes[:, :self.vdim+3].T)/self.markers_wo_holes[:, self.vdim+4]
+        # compute w0 and save at vdim + 5
+        self._markers[~self._holes, self.vdim + 5] = f_init(
+            *self.markers_wo_holes[:, :self.vdim + 3].T) / self.markers_wo_holes[:, self.vdim + 4]
 
-        # compute weights and save at vdim+3
+        # compute weights and save at vdim + 3
         if self._use_control_variate:
             fun_name = bckgr_params['type']
 
             if fun_name in bckgr_params:
                 f_bckgr = getattr(analytical, fun_name)(
                     **bckgr_params[fun_name])
             else:
                 f_bckgr = getattr(analytical, fun_name)()
 
-            self._markers[~self._holes, self.vdim+3] = self.markers_wo_holes[:, self.vdim+5] - \
-                f_bckgr(*self.markers_wo_holes[:, :self.vdim+3].T) / \
-                self.markers_wo_holes[:, self.vdim+4]
+            self._markers[~self._holes, self.vdim + 3] = self.markers_wo_holes[:, self.vdim + 5] - \
+                f_bckgr(*self.markers_wo_holes[:, :self.vdim + 3].T) / \
+                self.markers_wo_holes[:, self.vdim + 4]
         else:
-            self._markers[~self._holes, self.vdim+3] = self.markers_wo_holes[:, self.vdim+5]
+            self._markers[~self._holes, self.vdim + 3] = \
+                self.markers_wo_holes[:, self.vdim + 5]
 
     def update_weights(self, f0):
         """
         Updates the marker weights according to w0 - control*f0(eta, v)/s0, where control=True or control=False.
 
         Parameters
         ----------
         f0 : callable
-            The distribution function used as a control variate. Is called as f0(eta1, eta2, eta3, vx, vy, vz).
+            The distribution function used as a control variate. Is called as f0(eta1, eta2, eta3, v1, v2, v3).
         """
 
         if self._use_control_variate:
-            self._markers[~self._holes, self.vdim+3] = self.markers_wo_holes[:, self.vdim+5] - \
-                f0(*self.markers_wo_holes[:, :self.vdim+3].T)/self.markers_wo_holes[:, self.vdim+4]
+            self._markers[~self._holes, self.vdim + 3] = self.markers_wo_holes[:, self.vdim + 5] - \
+                f0(*self.markers_wo_holes[:, :self.vdim + 3].T) / \
+                self.markers_wo_holes[:, self.vdim + 4]
 
     def binning(self, components, bin_edges, domain=None):
         """
         Computes the distribution function via marker binning in logical space using numpy's histogramdd.
 
         Parameters
         ----------
@@ -513,17 +518,17 @@
 
         assert n_dim == 1 or n_dim == 2
 
         f_slice = self.binning(components, bin_edges, domain)
 
         bin_centers = [bi[:-1] + (bi[1] - bi[0])/2 for bi in bin_edges]
 
-        #labels = {0 : '$\eta_1$', 1 : '$\eta_2$', 2 : '$\eta_3$', 3 : '$v_x$', 4 : '$v_y$', 5 : '$v_z$'}
+        # labels = {0 : '$\eta_1$', 1 : '$\eta_2$', 2 : '$\eta_3$', 3 : '$v_x$', 4 : '$v_y$', 5 : '$v_z$'}
 
-        indices = np.nonzero(components)[0]
+        # indices = np.nonzero(components)[0]
 
         if n_dim == 1:
             plt.plot(bin_centers[0], f_slice)
             # plt.xlabel(labels[indices[0]])
         else:
             plt.contourf(bin_centers[0], bin_centers[1], f_slice, levels=20)
             plt.colorbar()
@@ -542,29 +547,30 @@
         """
 
         self.comm.Barrier()
 
         for axis, bc in enumerate(self.bc):
 
             # sorting out particles outside of the logical unit cube
-            is_outside_cube = np.logical_or(self.markers[:,axis] > 1.,
-                                            self.markers[:,axis] < 0.)
-            
+            is_outside_cube = np.logical_or(self.markers[:, axis] > 1.,
+                                            self.markers[:, axis] < 0.)
+
             # exclude holes
             is_outside_cube[self.holes] = False
 
             # indices or particles that are outside of the logical unit cube
             outside_inds = np.nonzero(is_outside_cube)[0]
 
             # apply boundary conditions
             if bc == 'remove':
                 self.markers[outside_inds, :-1] = -1.
 
             elif bc == 'periodic':
-                self.markers[outside_inds, axis] = self.markers[outside_inds, axis]%1.
+                self.markers[outside_inds, axis] = \
+                    self.markers[outside_inds, axis] % 1.
 
             elif bc == 'reflect':
                 reflect(self.markers, *self.domain.args_map, outside_inds, axis)
 
             else:
                 raise NotImplementedError('Given bc_type is not implemented!')
 
@@ -588,34 +594,35 @@
     """
 
     def __init__(self, name, **params):
 
         # base class params
         base_params = {}
 
-        list_base_params = ['type', 'ppc', 'Np', 'eps', 'bc_type', 'loading', 'comm', 'domain', 'domain_array']
+        list_base_params = ['type', 'ppc', 'Np', 'eps',
+                            'bc_type', 'loading', 'comm', 'domain', 'domain_array']
 
         for key, val in params.items():
             if key in list_base_params:
                 base_params[key] = val
 
         super().__init__(name, **base_params)
 
     @property
     def n_cols(self):
         """Number of the columns at each markers.
         """
         return 16
-    
+
     @property
     def vdim(self):
         """Dimension of the velocity space.
         """
         return 3
-    
+
     def svol(self, eta1, eta2, eta3, *v):
         """ 
         Sampling density function as volume form.
 
         Parameters
         ----------
         eta1, eta2, eta3 : array_like
@@ -630,20 +637,20 @@
             The volume-form sampling density.
         -------
         """
         # load sampling density svol = s6 = s3 (normalized to 1 in logical space!)
         Maxwellian6DUniform = getattr(analytical, 'Maxwellian6DUniform')
 
         s3 = Maxwellian6DUniform(n=1.,
-                                 ux=self._params['loading']['moments'][0],
-                                 uy=self._params['loading']['moments'][1],
-                                 uz=self._params['loading']['moments'][2],
-                                 vthx=self._params['loading']['moments'][3],
-                                 vthy=self._params['loading']['moments'][4],
-                                 vthz=self._params['loading']['moments'][5])
+                                 u1=self._params['loading']['moments'][0],
+                                 u2=self._params['loading']['moments'][1],
+                                 u3=self._params['loading']['moments'][2],
+                                 vth1=self._params['loading']['moments'][3],
+                                 vth2=self._params['loading']['moments'][4],
+                                 vth3=self._params['loading']['moments'][5])
         
         return s3(eta1, eta2, eta3, *v)
 
     def s0(self, eta1, eta2, eta3, *v, remove_holes=True):
         """ 
         Sampling density function as 0 form.
 
@@ -684,15 +691,16 @@
     """
 
     def __init__(self, name, **params):
 
         # base class params
         base_params = {}
 
-        list_base_params = ['type', 'ppc', 'Np', 'eps', 'bc_type', 'loading', 'comm', 'domain', 'domain_array']
+        list_base_params = ['type', 'ppc', 'Np', 'eps',
+                            'bc_type', 'loading', 'comm', 'domain', 'domain_array']
 
         for key, val in params.items():
             if key in list_base_params:
                 base_params[key] = val
 
         super().__init__(name, **base_params)
 
@@ -701,46 +709,46 @@
 
         list_child_params = ['A', 'Z', 'mhd_equil', 'units_basic']
 
         for key, val in params.items():
             if key in list_child_params:
                 child_params[key] = val
 
-        params_default = {'A': 1, 
+        params_default = {'A': 1,
                           'Z': 1,
                           'mhd_equil': None,
                           'units_basic': None
                           }
 
         child_params = set_defaults(child_params, params_default)
 
         self._mhd_equil = params['mhd_equil']
 
         # compute kappa
-        ee = 1.602176634e-19 # elementary charge (C)
-        mH = 1.67262192369e-27 # proton mass (kg)
+        ee = 1.602176634e-19  # elementary charge (C)
+        mH = 1.67262192369e-27  # proton mass (kg)
 
         Ah = child_params['A']
         Zh = child_params['Z']
-        
+
         omega_ch = (Zh*ee*child_params['units_basic']['B'])/(Ah*mH)
         self._kappa = omega_ch*child_params['units_basic']['t']
 
     @property
     def n_cols(self):
         """Number of the columns at each markers.
         """
         return 25
-    
+
     @property
     def vdim(self):
         """Dimension of the velocity space.
         """
         return 2
-    
+
     def svol(self, eta1, eta2, eta3, *v):
         """ 
         Sampling density function as volume-form.
 
         Parameters
         ----------
         eta1, eta2, eta3 : array_like
@@ -759,15 +767,15 @@
         Maxwellian5DUniform = getattr(analytical, 'Maxwellian5DUniform')
 
         s5 = Maxwellian5DUniform(n=1.,
                                  u_parallel=self.params['loading']['moments'][0],
                                  u_perp=self.params['loading']['moments'][1],
                                  vth_parallel=self.params['loading']['moments'][2],
                                  vth_perp=self.params['loading']['moments'][3])
-        
+
         return s5(eta1, eta2, eta3, *v)
 
     def s3(self, eta1, eta2, eta3, *v):
         """
         Sampling density function as 3-form.
 
         Parameters
@@ -788,17 +796,17 @@
         etas = (np.vstack((eta1, eta2, eta3)).T).copy()
         bv = self._mhd_equil.bv(etas)
         curlb = self._mhd_equil.jv(etas)/self._mhd_equil.absB0(etas)
         unit_b1 = self._mhd_equil.unit_b1(etas)
 
         # contra-variant components of B* = B + 1/kappa*v_parallel*curlb0
         bstar = bv + 1/self._kappa*v[0]*curlb
-
+        
         # B*_parallel = b0 . B*
-        jacobian_det = np.einsum('ij,ij->j',unit_b1, bstar)/v[1]
+        jacobian_det = np.einsum('ij,ij->j', unit_b1, bstar)/v[1]
 
         return self.svol(eta1, eta2, eta3, *v)/np.abs(jacobian_det)
 
     def s0(self, eta1, eta2, eta3, *v, remove_holes=True):
         """ 
         Sampling density function as 0-form.
```

### Comparing `struphy-1.9.9/src/struphy/pic/particles_to_grid.py` & `struphy-2.0.0/src/struphy/pic/particles_to_grid.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/pic/pusher.py` & `struphy-2.0.0/src/struphy/pic/pusher.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/pic/pusher_kernels.py` & `struphy-2.0.0/src/struphy/pic/pusher_kernels.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 import struphy.linear_algebra.core as linalg
 import struphy.geometry.map_eval as map_eval
 import struphy.b_splines.bsplines_kernels as bsp
 import struphy.b_splines.bsplines_kernels_particles as bspparticle
 import struphy.b_splines.bspline_evaluation_3d as eval_3d
 
 from struphy.pic.pusher_utilities import aux_fun_x_v_stat_e
-from struphy.kinetic_background.f0_kernels import maxwellian_6d
 
-from numpy import zeros, empty, shape, sqrt, cos, sin, floor
+from numpy import zeros, empty, shape, sqrt, cos, sin, floor, log
 
 
 @stack_array('df', 'df_inv', 'df_inv_t', 'e_form', 'e_cart', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def push_v_with_efield(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
@@ -28,15 +27,15 @@
         \frac{\mathbf v^{n+1}_p - \mathbf v^n_p}{\Delta t} = DF^{-\top} \hat{\mathbf E}^1(\eta^n_p)
 
     for each marker :math:`p` in markers array, where :math:`\hat{\mathbf E}^1 in H(\textnormal{curl})`.
 
     Parameters
     ----------
         e1_1, e1_2, e1_3: array[float]
-            3d array of FE coeffs of B-field as 2-form.
+            3d array of FE coeffs of E-field as 1-form.
     '''
 
     # allocate metric coeffs
     df = empty((3, 3), dtype=float)
     dfinv = empty((3, 3), dtype=float)
     dfinvt = empty((3, 3), dtype=float)
 
@@ -98,15 +97,15 @@
         e_form[2] = eval_3d.eval_spline_mpi_kernel(
             pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3, span1, span2, span3, e1_3, starts1[2])
 
         # electric field: Cartesian components
         linalg.matrix_vector(dfinvt, e_form, e_cart)
 
         # update velocities
-        markers[ip, 3:6] += dt*e_cart
+        markers[ip, 3:6] += dt * e_cart
 
     #$ omp end parallel
 
 
 @stack_array('df', 'b_form', 'b_cart', 'b_norm', 'e', 'v', 'vperp', 'vxb_norm', 'b_normxvperp', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def push_vxb_analytic(markers: 'float[:,:]', dt: float, stage: int,
                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
@@ -654,16 +653,14 @@
                                     markers[ip, 4] += dt * ww[0] * thermal * temp6[1]
                                     markers[ip, 5] += dt * ww[0] * thermal * temp6[2]
 
 
     #$ omp end parallel
 
 
-
-
 @stack_array('df', 'dfinv', 'dfinv_t', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3')
 def push_hybrid_xp_ap(markers: 'float[:,:]', dt: float, stage: int,
                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                       starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                       kind_map: int, params_map: 'float[:]',
                       p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                       ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
@@ -2432,26 +2429,26 @@
 
         # update markers for the next stage
         markers[ip, 0:3] = (markers[ip, 9:12] + dt*k/2 *
                             cont + dt*markers[ip, 12:15] * last)
 
 
 @stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'df', 'df_inv', 'v', 'df_inv_v')
-def push_weights_with_efield(markers: 'float[:,:]', dt: float, stage: int,
-                             pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
-                             starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
-                             kind_map: int, params_map: 'float[:]',
-                             p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
-                             ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
-                             cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
-                             e1_1: 'float[:,:,:]', e1_2: 'float[:,:,:]', e1_3: 'float[:,:,:]',
-                             f0_values: 'float[:]', f0_params: 'float[:]',
-                             n_markers_tot: 'int'):
+def push_weights_with_efield_lin_vm(markers: 'float[:,:]', dt: float, stage: int,
+                                    pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                    starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                    kind_map: int, params_map: 'float[:]',
+                                    p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                    ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                    cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                    e1_1: 'float[:,:,:]', e1_2: 'float[:,:,:]', e1_3: 'float[:,:,:]',
+                                    f0_values: 'float[:]', f0_params: 'float[:]',
+                                    n_markers_tot: 'int', kappa: 'float'):
     r'''
-    updates the single weights in the e_W substep of the linearized Vlasov Maxwell system;
+    updates the single weights in the e_W substep of the Vlasov Maxwell system with delta-f;
     c.f. struphy.propagators.propagators.StepEfieldWeights
 
     Parameters :
     ------------
         e1_1, e1_2, e1_3: array[float]
             3d array of FE coeffs of E-field as 1-form.
 
@@ -2460,14 +2457,17 @@
 
         f0_params : array[float]
             Parameters needed to specify the moments; the order is specified in :ref:`struphy.kinetic_background.moments_kernels`
             for the respective functions available.
 
         n_markers_tot : int
             total number of particles
+
+        kappa : float
+            = 2 * pi * Omega_c / omega ; Parameter determining the coupling strength between particles and fields
     '''
 
     # total number of basis functions : B-splines (pn) and D-splines (pn-1)
     pn1 = pn[0]
     pn2 = pn[1]
     pn3 = pn[2]
 
@@ -2534,17 +2534,131 @@
         e_vec_1 = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3,
                                                  span1, span2, span3, e1_1, starts1[0])
         e_vec_2 = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3,
                                                  span1, span2, span3, e1_2, starts1[1])
         e_vec_3 = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3,
                                                  span1, span2, span3, e1_3, starts1[2])
 
-        # w_{n+1} = w_n + dt / (2 * N * s_0) * sqrt(f_0) * ( DF^{-1} \V_th (v_p - u) ) \cdot ( e_{n+1} + e_n )
+        # w_{n+1} = w_n + dt * kappa / (2 * N * s_0) * sqrt(f_0) * ( DF^{-1} \V_th (v_p - u) ) \cdot ( e_{n+1} + e_n )
         update = (df_inv_v[0] * e_vec_1 + df_inv_v[1] * e_vec_2 + df_inv_v[2] * e_vec_3) * \
-            sqrt(f0) * dt / (2 * n_markers_tot * markers[ip, 7])
+            sqrt(f0) * dt * kappa / (2 * n_markers_tot * markers[ip, 7])
+        markers[ip, 6] += update
+
+    #$ omp end parallel
+
+
+@stack_array('bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'df', 'df_inv', 'v', 'df_inv_v')
+def push_weights_with_efield_deltaf_vm(markers: 'float[:,:]', dt: float, stage: int,
+                                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                                       starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                                       kind_map: int, params_map: 'float[:]',
+                                       p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                                       ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                                       cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                                       e1_1: 'float[:,:,:]', e1_2: 'float[:,:,:]', e1_3: 'float[:,:,:]',
+                                       f0_values: 'float[:]', f0_params: 'float[:]',
+                                       n_markers_tot: 'int', kappa: 'float'):
+    r'''
+    updates the single weights in the e_W substep of the linearized Vlasov Maxwell system;
+    c.f. struphy.propagators.propagators.StepEfieldWeights
+
+    Parameters :
+    ------------
+    e1_1, e1_2, e1_3: array[float]
+        3d array of FE coeffs of E-field as 1-form.
+
+    f0_values ; array[float]
+        Value of f0 for each particle.
+
+    f0_params : array[float]
+        Parameters needed to specify the moments; the order is specified in :ref:`struphy.kinetic_background.moments_kernels`
+        for the respective functions available.
+
+    n_markers_tot : int
+        total number of particles
+
+    kappa : float
+        = 2 * pi * Omega_c / omega ; Parameter determining the coupling strength between particles and fields
+    '''
+
+    # total number of basis functions : B-splines (pn) and D-splines (pn-1)
+    pn1 = pn[0]
+    pn2 = pn[1]
+    pn3 = pn[2]
+
+    # non-vanishing N-splines at particle position
+    bn1 = empty(pn[0] + 1, dtype=float)
+    bn2 = empty(pn[1] + 1, dtype=float)
+    bn3 = empty(pn[2] + 1, dtype=float)
+
+    # non-vanishing D-splines at particle position
+    bd1 = empty(pn[0], dtype=float)
+    bd2 = empty(pn[1], dtype=float)
+    bd3 = empty(pn[2], dtype=float)
+
+    df = empty((3, 3), dtype=float)
+    df_inv = empty((3, 3), dtype=float)
+    v = empty(3, dtype=float)
+    df_inv_v = empty(3, dtype=float)
+
+    # get number of markers
+    n_markers = shape(markers)[0]
+
+    #$ omp parallel private (ip, eta1, eta2, eta3, df, df_inv, v, df_inv_v, span1, span2, span3, bn1, bn2, bn3, bd1, bd2, bd3, f0, e_vec_1, e_vec_2, e_vec_3, update)
+    #$ omp for
+    for ip in range(n_markers):
+        if markers[ip, 0] == -1:
+            continue
+
+        # position
+        eta1 = markers[ip, 0]
+        eta2 = markers[ip, 1]
+        eta3 = markers[ip, 2]
+
+        # spans (i.e. index for non-vanishing basis functions)
+        span1 = bsp.find_span(tn1, pn1, eta1)
+        span2 = bsp.find_span(tn2, pn2, eta2)
+        span3 = bsp.find_span(tn3, pn3, eta3)
+
+        # compute bn, bd, i.e. values for non-vanishing B-/D-splines at position eta
+        bsp.b_d_splines_slim(tn1, pn1, eta1, span1, bn1, bd1)
+        bsp.b_d_splines_slim(tn2, pn2, eta2, span2, bn2, bd2)
+        bsp.b_d_splines_slim(tn3, pn3, eta3, span3, bn3, bd3)
+
+        f0 = f0_values[ip]
+
+        # Compute Jacobian matrix
+        map_eval.df(eta1, eta2, eta3,
+                    kind_map, params_map,
+                    t1_map, t2_map, t3_map,
+                    p_map,
+                    ind1_map, ind2_map, ind3_map,
+                    cx, cy, cz,
+                    df)
+
+        # compute shifted and stretched velocity
+        v[0] = (markers[ip, 3] - f0_params[1]) / f0_params[4]**2
+        v[1] = (markers[ip, 4] - f0_params[2]) / f0_params[5]**2
+        v[2] = (markers[ip, 5] - f0_params[3]) / f0_params[6]**2
+
+        # invert Jacobian matrix
+        linalg.matrix_inv(df, df_inv)
+        linalg.matrix_vector(df_inv, v, df_inv_v)
+
+        # E-field (1-form)
+        e_vec_1 = eval_3d.eval_spline_mpi_kernel(pn[0] - 1, pn[1], pn[2], bd1, bn2, bn3,
+                                                 span1, span2, span3, e1_1, starts1[0])
+        e_vec_2 = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1] - 1, pn[2], bn1, bd2, bn3,
+                                                 span1, span2, span3, e1_2, starts1[1])
+        e_vec_3 = eval_3d.eval_spline_mpi_kernel(pn[0], pn[1], pn[2] - 1, bn1, bn2, bd3,
+                                                 span1, span2, span3, e1_3, starts1[2])
+
+        # w_{n+1} = w_n + dt * kappa / (N * s_0) (e_n - dt^2 / 2 * accum_vec) \cdot (DL^{-1} \V_th (v_p - u)) (f_0 / log(f_0) - f_0)
+        update = (df_inv_v[0] * e_vec_1 + df_inv_v[1] * e_vec_2 + df_inv_v[2] * e_vec_3) * \
+            dt * kappa * (f0 / log(f0) - f0) / (n_markers_tot * markers[ip, 7])
         markers[ip, 6] += update
 
     #$ omp end parallel
 
 
 @stack_array('particle', 'df', 'df_inv', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'taus')
 def push_x_v_static_efield(markers: 'float[:,:]', dt: float, stage: int,
@@ -2553,39 +2667,43 @@
                            kind_map: int, params_map: 'float[:]',
                            p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                            ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                            cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
                            loc1: 'float[:]', loc2: 'float[:]', loc3: 'float[:]',
                            weight1: 'float[:]', weight2: 'float[:]', weight3: 'float[:]',
                            e1_1: 'float[:,:,:]', e1_2: 'float[:,:,:]', e1_3: 'float[:,:,:]',
+                           kappa: 'float',
                            eps: 'float[:]', maxiter: int):
     r"""
     particle pusher for ODE
 
     .. math::
         \frac{\text{d} \mathbf{\eta}}{\text{d} t} & = DL^{-1} \mathbf{v} \,
 
-        \frac{\text{d} \mathbf{v}}{\text{d} t} & = DL^{-T} \mathbf{E}_0(\mathbf{\eta})
+        \frac{\text{d} \mathbf{v}}{\text{d} t} & = \kappa \, DL^{-T} \mathbf{E}_0(\mathbf{\eta})
 
     Parameters 
     ----------
-        loc1, loc2, loc3 : array
-            contain the positions of the Legendre-Gauss quadrature points of necessary order to integrate basis splines exactly in each direction
+    loc1, loc2, loc3 : array
+        contain the positions of the Legendre-Gauss quadrature points of necessary order to integrate basis splines exactly in each direction
 
-        weight1, weight2, weight3 : array
-            contain the values of the weights for the Legendre-Gauss quadrature in each direction
+    weight1, weight2, weight3 : array
+        contain the values of the weights for the Legendre-Gauss quadrature in each direction
 
-        e1_1, e1_2, e1_3: array[float]
-            3d array of FE coeffs of the background E-field as 1-form.
+    e1_1, e1_2, e1_3: array[float]
+        3d array of FE coeffs of the background E-field as 1-form.
+
+    kappa : float
+        = 2 * pi * Omega_c / omega ; Parameter determining the coupling strength between particles and fields
 
-        eps: array
-            determines the accuracy for the position (0th element) and velocity (1st element) with which the implicit scheme is executed
+    eps: array
+        determines the accuracy for the position (0th element) and velocity (1st element) with which the implicit scheme is executed
 
-        maxiter : integer
-            sets the maximum number of iterations for the iterative scheme
+    maxiter : integer
+        sets the maximum number of iterations for the iterative scheme
     """
 
     particle = zeros(9, dtype=float)
 
     # get number of markers
     n_markers = shape(markers)[0]
 
@@ -2648,14 +2766,15 @@
                                           n_quad1, n_quad2, n_quad3,
                                           df, df_inv,
                                           bn1, bn2, bn3, bd1, bd2, bd3,
                                           taus,
                                           dt2,
                                           loc1, loc2, loc3, weight1, weight2, weight3,
                                           e1_1, e1_2, e1_3,
+                                          kappa,
                                           eps, maxiter)
                 run = run + temp
 
         # write the results in the particles array
         markers[ip, :] = particle[:]
 
     #$ omp end parallel
@@ -2818,14 +2937,15 @@
         # accumulation for last stage
         markers[ip, 13:16] += dt*b[stage]*k
 
         # update positions for intermediate stages or last stage
         markers[ip, 0:3] = markers[ip, 9:12] + \
             dt*a[stage]*k + last*markers[ip, 13:16]
 
+
 def push_gc2_explicit_stage(markers: 'float[:,:]', dt: float, stage: int,
                             pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                             starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                             kind_map: int, params_map: 'float[:]',
                             p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                             ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                             cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -2960,14 +3080,15 @@
 
         # update positions for intermediate stages or last stage
         markers[ip, 0:3] = markers[ip, 9:12] + \
             dt*a[stage]*k + last*markers[ip, 13:16]
         markers[ip, 3] = markers[ip, 12] + dt * \
             a[stage]*k_v + last*markers[ip, 16]
 
+
 def push_gc_explicit_stage(markers: 'float[:,:]', dt: float, stage: int,
                            pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                            starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                            kind_map: int, params_map: 'float[:]',
                            p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                            ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                            cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -3130,14 +3251,15 @@
 
         # update positions for intermediate stages or last stage
         markers[ip, 0:3] = markers[ip, 9:12] + \
             dt*a[stage]*k + last*markers[ip, 13:16]
         markers[ip, 3] = markers[ip, 12] + dt * \
             a[stage]*k_v + last*markers[ip, 16]
 
+
 def push_gc1_discrete_gradients(markers: 'float[:,:]', dt: float, stage: int, tol: float,
                                 domain_array: 'float[:]',
                                 pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                                 starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                                 kind_map: int, params_map: 'float[:]',
                                 p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                                 ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
@@ -3243,14 +3365,15 @@
             markers[ip, 23] = -1.
             markers[ip, 20] = stage
 
             continue
 
         markers[ip, 0:4] = (markers[ip, 0:4] + markers[ip, 9:13])/2.
 
+
 def push_gc2_discrete_gradients(markers: 'float[:,:]', dt: float, stage: int, tol: float,
                                 domain_array: 'float[:]',
                                 pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                                 starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                                 kind_map: int, params_map: 'float[:]',
                                 p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                                 ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
@@ -3346,14 +3469,15 @@
         if diff < tol:
             markers[ip, 23] = -1.
             markers[ip, 20] = stage
             continue
 
         markers[ip, 0:4] = (markers[ip, 0:4] + markers[ip, 9:13])/2.
 
+
 def push_gc1_discrete_gradients_faster(markers: 'float[:,:]', dt: float, stage: int, tol: float,
                                        domain_array: 'float[:]',
                                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                                        kind_map: int, params_map: 'float[:]',
                                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
@@ -3458,14 +3582,15 @@
             markers[ip, 23] = -1.
             markers[ip, 20] = stage
 
             continue
 
         markers[ip, 0:3] = (markers[ip, 0:3] + markers[ip, 9:12])/2.
 
+
 def push_gc2_discrete_gradients_faster(markers: 'float[:,:]', dt: float, stage: int, tol: float,
                                        domain_array: 'float[:]',
                                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                                        kind_map: int, params_map: 'float[:]',
                                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
@@ -3562,14 +3687,15 @@
         if diff < tol:
             markers[ip, 23] = -1.
             markers[ip, 20] = stage
             continue
 
         markers[ip, 0:3] = (markers[ip, 0:3] + markers[ip, 9:12])/2.
 
+
 def push_gc_cc_J1_H1vec(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -3612,15 +3738,14 @@
 
         # only do something if particle is a "true" particle (i.e. not a hole)
         if markers[ip, 0] == -1.:
             continue
 
         eta[:] = markers[ip, 0:3]
         v = markers[ip, 3]
-        mu = markers[ip, 4]
 
         # evaluate Jacobian, result in df
         map_eval.df(eta[0], eta[1], eta[2],
                     kind_map, params_map,
                     t1_map, t2_map, t3_map, p_map,
                     ind1_map, ind2_map, ind3_map,
                     cx, cy, cz,
@@ -3669,14 +3794,15 @@
         linalg.cross(b, u, e)
 
         # curl_norm_b dot electric field
         temp = linalg.scalar_dot(e, curl_norm_b) / det_df
 
         markers[ip, 3] += temp/abs_b_star_para*v*dt
 
+
 def push_gc_cc_J1_Hcurl(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -3723,15 +3849,14 @@
 
         # only do something if particle is a "true" particle (i.e. not a hole)
         if markers[ip, 0] == -1.:
             continue
 
         eta[:] = markers[ip, 0:3]
         v = markers[ip, 3]
-        mu = markers[ip, 4]
 
         # evaluate Jacobian, result in df
         map_eval.df(eta[0], eta[1], eta[2],
                     kind_map, params_map,
                     t1_map, t2_map, t3_map, p_map,
                     ind1_map, ind2_map, ind3_map,
                     cx, cy, cz,
@@ -3788,14 +3913,15 @@
         linalg.cross(b, u0, e)
 
         # curl_norm_b dot electric field
         temp = linalg.scalar_dot(e, curl_norm_b) / det_df
 
         markers[ip, 3] += temp/abs_b_star_para*v*dt
 
+
 def push_gc_cc_J1_Hdiv(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -3838,15 +3964,14 @@
 
         # only do something if particle is a "true" particle (i.e. not a hole)
         if markers[ip, 0] == -1.:
             continue
 
         eta[:] = markers[ip, 0:3]
         v = markers[ip, 3]
-        mu = markers[ip, 4]
 
         # evaluate Jacobian, result in df
         map_eval.df(eta[0], eta[1], eta[2],
                     kind_map, params_map,
                     t1_map, t2_map, t3_map, p_map,
                     ind1_map, ind2_map, ind3_map,
                     cx, cy, cz,
@@ -3898,14 +4023,15 @@
         linalg.cross(b, u, e)
 
         # curl_norm_b dot electric field
         temp = linalg.scalar_dot(e, curl_norm_b) / det_df
 
         markers[ip, 3] += temp/abs_b_star_para*v*dt
 
+
 def push_gc_cc_J2_dg_H1vec(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -3933,16 +4059,16 @@
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
     bd3 = empty(pn[2], dtype=float)
 
     # containers for fields
     tmp1 = empty((3,3), dtype=float)
     tmp2 = empty((3,3), dtype=float)
-    b_prod = empty((3,3), dtype=float)
-    norm_b2_prod = empty((3,3), dtype=float)
+    b_prod = zeros((3,3), dtype=float)
+    norm_b2_prod = zeros((3,3), dtype=float)
     e = empty(3, dtype=float)
     u = empty(3, dtype=float)
     b = empty(3, dtype=float)
     b_star = empty(3, dtype=float)
     norm_b1 = empty(3, dtype=float)
     norm_b2 = empty(3, dtype=float)
     curl_norm_b = empty(3, dtype=float)
@@ -4036,14 +4162,15 @@
         linalg.matrix_matrix(tmp1, g_inv, tmp2)
         linalg.matrix_matrix(tmp2, b_prod, tmp1)
 
         linalg.matrix_vector(tmp1, u, e)
 
         markers[ip, 0:3] = markers[ip, 9:12]- e/abs_b_star_para*dt
 
+
 def push_gc_cc_J2_dg_faster_H1vec(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -4103,14 +4230,15 @@
                     (markers[ip, 19], markers[ip, 21], markers[ip, 22]),
                     (markers[ip, 20], markers[ip, 22], markers[ip, 23])) 
 
         linalg.matrix_vector(tmp, u, e)
 
         markers[ip, 0:3] = markers[ip, 9:12] - e*dt
 
+
 def push_gc_cc_J2_dg_faster_Hcurl(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -4170,14 +4298,15 @@
                     (markers[ip, 19], markers[ip, 21], markers[ip, 22]),
                     (markers[ip, 20], markers[ip, 22], markers[ip, 23])) 
 
         linalg.matrix_vector(tmp, u, e)
 
         markers[ip, 0:3] = markers[ip, 9:12] - e*dt
 
+
 def push_gc_cc_J2_dg_faster_Hdiv(markers: 'float[:,:]', dt: float, stage: int,
                        pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                        starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
                        kind_map: int, params_map: 'float[:]',
                        p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
                        ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
                        cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
@@ -4237,28 +4366,29 @@
                     (markers[ip, 19], markers[ip, 21], markers[ip, 22]),
                     (markers[ip, 20], markers[ip, 22], markers[ip, 23])) 
 
         linalg.matrix_vector(tmp, u, e)
 
         markers[ip, 0:3] = markers[ip, 9:12] - e*dt
 
+
 def push_gc_cc_J2_stage_H1vec(markers: 'float[:,:]', dt: float, stage: int,
-                       pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
-                       starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
-                       kind_map: int, params_map: 'float[:]',
-                       p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
-                       ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
-                       cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
-                       kappa: float,
-                       b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
-                       norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
-                       norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
-                       curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
-                       u1: 'float[:,:,:]', u2: 'float[:,:,:]', u3: 'float[:,:,:]',
-                       a: 'float[:]', b: 'float[:]', c: 'float[:]'):
+                              pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
+                              starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
+                              kind_map: int, params_map: 'float[:]',
+                              p_map: 'int[:]', t1_map: 'float[:]', t2_map: 'float[:]', t3_map: 'float[:]',
+                              ind1_map: 'int[:,:]', ind2_map: 'int[:,:]', ind3_map: 'int[:,:]',
+                              cx: 'float[:,:,:]', cy: 'float[:,:,:]', cz: 'float[:,:,:]',
+                              kappa: float,
+                              b1: 'float[:,:,:]', b2: 'float[:,:,:]', b3: 'float[:,:,:]',
+                              norm_b11: 'float[:,:,:]', norm_b12: 'float[:,:,:]', norm_b13: 'float[:,:,:]',
+                              norm_b21: 'float[:,:,:]', norm_b22: 'float[:,:,:]', norm_b23: 'float[:,:,:]',
+                              curl_norm_b1: 'float[:,:,:]', curl_norm_b2: 'float[:,:,:]', curl_norm_b3: 'float[:,:,:]',
+                              u1: 'float[:,:,:]', u2: 'float[:,:,:]', u3: 'float[:,:,:]',
+                              a: 'float[:]', b: 'float[:]', c: 'float[:]'):
     r'''
     TODO
     '''
 
     # allocate metric coeffs
     df = empty((3, 3), dtype=float)
     df_inv   = empty((3, 3), dtype=float)
@@ -4273,15 +4403,15 @@
     bd1 = empty(pn[0], dtype=float)
     bd2 = empty(pn[1], dtype=float)
     bd3 = empty(pn[2], dtype=float)
 
     # containers for fields
     tmp1 = empty((3,3), dtype=float)
     tmp2 = empty((3,3), dtype=float)
-    b_prod = empty((3,3), dtype=float)
+    b_prod = zeros((3,3), dtype=float)
     norm_b2_prod = empty((3,3), dtype=float)
     e = empty(3, dtype=float)
     u = empty(3, dtype=float)
     bb = empty(3, dtype=float)
     b_star = empty(3, dtype=float)
     norm_b1 = empty(3, dtype=float)
     norm_b2 = empty(3, dtype=float)
@@ -4386,9 +4516,9 @@
 
         linalg.matrix_vector(tmp1, u, e)
 
         e /= abs_b_star_para
 
         # markers[ip, :3] -= e/abs_b_star_para*dt
 
-        markers[ip, 12:15] -= dt*b[stage]*e
-        markers[ip, 0:3] = markers[ip, 9:12] + dt*a[stage]*e + last*markers[ip, 12:15]
+        markers[ip, 13:16] -= dt*b[stage]*e
+        markers[ip, 0:3] = markers[ip, 9:12] + dt*a[stage]*e + last*markers[ip, 13:16]
```

### Comparing `struphy-1.9.9/src/struphy/pic/pusher_utilities.py` & `struphy-2.0.0/src/struphy/pic/pusher_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,22 +173,22 @@
 @pure
 def quicksort(a: 'float[:]', lo: 'int', hi: 'int'):
     """
     Implementation of the quicksort sorting algorithm. Ref?
 
     Parameters
     ----------
-        a : array
-            list that is to be sorted
+    a : array
+        list that is to be sorted
 
-        lo : integer
-            lower index from which the sort to start
+    lo : integer
+        lower index from which the sort to start
 
-        hi : integer
-            upper index until which the sort is to be done
+    hi : integer
+        upper index until which the sort is to be done
     """
     i = lo
     j = hi
     while i < hi:
         pivot = a[(lo + hi) // 2]
         while i <= j:
             while a[i] < pivot:
@@ -209,28 +209,28 @@
 
 def find_taus(eta: 'float', eta_next: 'float', Nel: 'int', breaks: 'float[:]', uniform: 'int', tau_list: 'float[:]'):
     """
     Find the values of tau for which the particle crosses the cell boundaries while going from eta to eta_next
 
     Parameters
     ----------
-        eta : float
-            old position
+    eta : float
+        old position
 
-        eta_next : float
-            new position
+    eta_next : float
+        new position
 
-        Nel : integer
-            contains the number of elements in this direction
+    Nel : integer
+        contains the number of elements in this direction
 
-        breaks : array
-            break points in this direction
+    breaks : array
+        break points in this direction
 
-        uniform : integer
-            0 if the grid is non-uniform, 1 if the grid is uniform
+    uniform : integer
+        0 if the grid is non-uniform, 1 if the grid is uniform
     """
 
     if uniform == 1:
         index = int(floor(eta * Nel))
         index_next = int(floor(eta_next * Nel))
         length = int(abs(index_next - index))
 
@@ -265,40 +265,41 @@
                        bn1: 'float[:]', bn2: 'float[:]', bn3: 'float[:]',
                        bd1: 'float[:]', bd2: 'float[:]', bd3: 'float[:]',
                        taus: 'float[:]',
                        dt: 'float',
                        loc1: 'float[:]', loc2: 'float[:]', loc3: 'float[:]',
                        weight1: 'float[:]', weight2: 'float[:]', weight3: 'float[:]',
                        e1_1: 'float[:,:,:]', e1_2: 'float[:,:,:]', e1_3: 'float[:,:,:]',
+                       kappa: 'float',
                        eps: 'float[:]', maxiter: 'int') -> 'int':
     """
     Auxiliary function for the pusher_x_v_static_efield, introduced to enable time-step splitting if scheme does not converge for the standard dt
 
     Parameters
     ----------
-        particle : array
-            shape(7), contains the values for the positions [0:3], velocities [3:6], and weights [8]
+    particle : array
+        shape(7), contains the values for the positions [0:3], velocities [3:6], and weights [8]
 
-        dt2 : double
-            time stepping of substep
+    dt2 : double
+        time stepping of substep
 
-        loc1, loc2, loc3 : array
-            contain the positions of the Legendre-Gauss quadrature points of necessary order to integrate basis splines exactly in each direction
+    loc1, loc2, loc3 : array
+        contain the positions of the Legendre-Gauss quadrature points of necessary order to integrate basis splines exactly in each direction
 
-        weight1, weight2, weight3 : array
-            contain the values of the weights for the Legendre-Gauss quadrature in each direction
+    weight1, weight2, weight3 : array
+        contain the values of the weights for the Legendre-Gauss quadrature in each direction
 
-        e1_1, e1_2, e1_3: array[float]
-            3d array of FE coeffs of the background E-field as 1-form.
+    e1_1, e1_2, e1_3: array[float]
+        3d array of FE coeffs of the background E-field as 1-form.
 
-        eps: array
-            determines the accuracy for the position (0th element) and velocity (1st element) with which the implicit scheme is executed
+    eps: array
+        determines the accuracy for the position (0th element) and velocity (1st element) with which the implicit scheme is executed
 
-        maxiter : integer
-            sets the maximum number of iterations for the iterative scheme
+    maxiter : integer
+        sets the maximum number of iterations for the iterative scheme
     """
 
     # Find number of elements in each direction
     Nel = empty(3, dtype=int)
     Nel[0] = len(tn1)
     Nel[1] = len(tn2)
     Nel[2] = len(tn3)
@@ -336,20 +337,20 @@
     v3_curr = v3
 
     # Use Euler method as a predictor for positions
     map_eval.df(eta1, eta2, eta3, kind_map, params_map, t1_map, t2_map,
                 t3_map, p_map, ind1_map, ind2_map, ind3_map, cx, cy, cz, df)
     linalg.matrix_inv(df, df_inv)
 
-    v1_curv = df_inv[0, 0] * (v1_curr + v1) + df_inv[0, 1] * \
-        (v2_curr + v2) + df_inv[0, 2] * (v3_curr + v3)
-    v2_curv = df_inv[1, 0] * (v1_curr + v1) + df_inv[1, 1] * \
-        (v2_curr + v2) + df_inv[1, 2] * (v3_curr + v3)
-    v3_curv = df_inv[2, 0] * (v1_curr + v1) + df_inv[2, 1] * \
-        (v2_curr + v2) + df_inv[2, 2] * (v3_curr + v3)
+    v1_curv = kappa * (df_inv[0, 0] * (v1_curr + v1) + df_inv[0, 1] * \
+        (v2_curr + v2) + df_inv[0, 2] * (v3_curr + v3))
+    v2_curv = kappa * (df_inv[1, 0] * (v1_curr + v1) + df_inv[1, 1] * \
+        (v2_curr + v2) + df_inv[1, 2] * (v3_curr + v3))
+    v3_curv = kappa * (df_inv[2, 0] * (v1_curr + v1) + df_inv[2, 1] * \
+        (v2_curr + v2) + df_inv[2, 2] * (v3_curr + v3))
 
     eta1_next = (eta1 + dt * v1_curv / 2.) % 1
     eta2_next = (eta2 + dt * v2_curv / 2.) % 1
     eta3_next = (eta3 + dt * v3_curv / 2.) % 1
 
     # set some initial value for v_next
     v1_next = v1_curr
@@ -379,20 +380,20 @@
                     cx, cy, cz, df)
 
         # evaluate inverse Jacobian matrix
         linalg.matrix_inv(df, df_inv)
 
         # ======================================================================================
         # update the positions and place them back into the computational domain
-        v1_curv = df_inv[0, 0] * (v1_curr + v1) + df_inv[0, 1] * \
-            (v2_curr + v2) + df_inv[0, 2] * (v3_curr + v3)
-        v2_curv = df_inv[1, 0] * (v1_curr + v1) + df_inv[1, 1] * \
-            (v2_curr + v2) + df_inv[1, 2] * (v3_curr + v3)
-        v3_curv = df_inv[2, 0] * (v1_curr + v1) + df_inv[2, 1] * \
-            (v2_curr + v2) + df_inv[2, 2] * (v3_curr + v3)
+        v1_curv = kappa * (df_inv[0, 0] * (v1_curr + v1) + df_inv[0, 1] * \
+            (v2_curr + v2) + df_inv[0, 2] * (v3_curr + v3))
+        v2_curv = kappa * (df_inv[1, 0] * (v1_curr + v1) + df_inv[1, 1] * \
+            (v2_curr + v2) + df_inv[1, 2] * (v3_curr + v3))
+        v3_curv = kappa * (df_inv[2, 0] * (v1_curr + v1) + df_inv[2, 1] * \
+            (v2_curr + v2) + df_inv[2, 2] * (v3_curr + v3))
 
         # x_{n+1} = x_n + dt/2 * DF^{-1}(x_{n+1}/2 + x_n/2) * (v_{n+1} + v_n)
         eta1_next = (eta1 + dt * v1_curv / 2.) % 1
         eta2_next = (eta2 + dt * v2_curv / 2.) % 1
         eta3_next = (eta3 + dt * v3_curv / 2.) % 1
 
         # ======================================================================================
@@ -411,15 +412,16 @@
         length3 = int(abs(index3_next - index3))
 
         length = length1 + length2 + length3
 
         taus[0] = 0.0
         taus[length + 1] = 1.0
 
-        find_taus(eta1_curr, eta1_next, Nel[0], tn1, 1, taus[1:length1 + 1])
+        find_taus(eta1_curr, eta1_next,
+                  Nel[0], tn1, 1, taus[1:length1 + 1])
         find_taus(eta2_curr, eta2_next,
                   Nel[1], tn2, 1, taus[length1 + 1:length1 + length2 + 1])
         find_taus(eta3_curr, eta3_next,
                   Nel[2], tn3, 1, taus[length1 + length2 + 1:length + 1])
 
         if length != 0:
             quicksort(taus[0:length + 1], 1, length)
@@ -565,20 +567,23 @@
                             i3 = ie3 + il3
                             bi3 = bi2 * bd3[il3] * e1_3[i1 - starts3[0] + pn1,
                                                         i2 - starts3[1] + pn2, i3 - starts3[2] + pn3]
 
                             temp3 += bi3 * weight3[n]
 
         # v_{n+1} = v_n + dt * DF^{-T}(x_n) * int_0^1 d tau ( E(x_n + tau*(x_{n+1} - x_n) ) )
-        v1_next = v1 + dt * (df_inv[0, 0] * temp1 +
-                             df_inv[1, 0] * temp2 + df_inv[2, 0] * temp3)
-        v2_next = v2 + dt * (df_inv[0, 1] * temp1 +
-                             df_inv[1, 1] * temp2 + df_inv[2, 1] * temp3)
-        v3_next = v3 + dt * (df_inv[0, 2] * temp1 +
-                             df_inv[1, 2] * temp2 + df_inv[2, 2] * temp3)
+        v1_next = v1 + dt * kappa * (df_inv[0, 0] * temp1 +
+                                     df_inv[1, 0] * temp2 +
+                                     df_inv[2, 0] * temp3)
+        v2_next = v2 + dt * kappa * (df_inv[0, 1] * temp1 +
+                                     df_inv[1, 1] * temp2 +
+                                     df_inv[2, 1] * temp3)
+        v3_next = v3 + dt * kappa * (df_inv[0, 2] * temp1 +
+                                     df_inv[1, 2] * temp2 +
+                                     df_inv[2, 2] * temp3)
 
         runs += 1
 
         if runs == maxiter:
             break
 
     if runs < maxiter:
```

### Comparing `struphy-1.9.9/src/struphy/pic/sampling.py` & `struphy-2.0.0/src/struphy/pic/sampling.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/pic/sobol_seq.py` & `struphy-2.0.0/src/struphy/pic/sobol_seq.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/pic/utilities.py` & `struphy-2.0.0/src/struphy/pic/utilities.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/pic/utilities_kernels.py` & `struphy-2.0.0/src/struphy/pic/utilities_kernels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyccel.decorators import stack_array
 
 import struphy.b_splines.bsplines_kernels as bsp
 from struphy.b_splines.bspline_evaluation_3d import eval_spline_mpi_kernel
 import struphy.linear_algebra.core as linalg
 import struphy.geometry.map_eval as map_eval
 
-from numpy import empty, shape, zeros, sqrt, log
+from numpy import empty, shape, zeros, sqrt, log, abs
 
 
 @stack_array('bn1', 'bn2', 'bn3')
 def eval_0_form_at_particles(markers: 'float[:,:]',
                              pn: 'int[:]',
                              tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                              starts: 'int[:]',
@@ -487,15 +487,15 @@
         bsp.b_splines_slim(tn1, pn[0], eta1, span1, bn1)
         bsp.b_splines_slim(tn2, pn[1], eta2, span2, bn2)
         bsp.b_splines_slim(tn3, pn[2], eta3, span3, bn3)
         
         B0 = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, absB, starts0)
 
         # magnetic moment
-        markers[ip,4] = 1/2 * v_perp**2 / B0
+        markers[ip,4] = 1/2 * v_perp**2 / abs(B0)
 
 
 @stack_array('bn1', 'bn2', 'bn3')
 def eval_magnetic_energy(markers: 'float[:,:]',
                          pn: 'int[:]',
                          tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                          starts0: 'int[:]',
@@ -544,15 +544,15 @@
 
         bsp.b_splines_slim(tn1, pn[0], eta1, span1, bn1)
         bsp.b_splines_slim(tn2, pn[1], eta2, span2, bn2)
         bsp.b_splines_slim(tn3, pn[2], eta3, span3, bn3)
 
         B0 = eval_spline_mpi_kernel(pn[0], pn[1], pn[2], bn1, bn2, bn3, span1, span2, span3, PB, starts0)
 
-        markers[ip, 8] = B0*markers[ip, 4]
+        markers[ip, 8] = abs(B0)*markers[ip, 4]
 
 
 @stack_array('df', 'dfinv', 'g', 'g_inv', 'bn1', 'bn2', 'bn3', 'bd1', 'bd2', 'bd3', 'e')
 def push_gc1_discrete_gradients_prepare(markers: 'float[:,:]', dt: float,
                                         domain_array: 'float[:]',
                                         pn: 'int[:]', tn1: 'float[:]', tn2: 'float[:]', tn3: 'float[:]',
                                         starts0: 'int[:]', starts1: 'int[:,:]', starts2: 'int[:,:]', starts3: 'int[:]',
@@ -1514,15 +1514,15 @@
 
         # marker positions
         eta1 = markers[ip, 0] # mid
         eta2 = markers[ip, 1] # mid
         eta3 = markers[ip, 2] # mid
 
         # marker weight and velocity
-        weight = markers[ip, 6]
+        weight = markers[ip, 5]
         mu = markers[ip, 4]
 
         # b-field evaluation
         span1 = bsp.find_span(tn1, pn[0], eta1)
         span2 = bsp.find_span(tn2, pn[1], eta2)
         span3 = bsp.find_span(tn3, pn[2], eta3)
```

### Comparing `struphy-1.9.9/src/struphy/polar/basic.py` & `struphy-2.0.0/src/struphy/polar/basic.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/polar/extraction_operators.py` & `struphy-2.0.0/src/struphy/polar/extraction_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,17 @@
         assert np.all(cx[0] == self.pole[0])
         assert np.all(cy[0] == self.pole[1])
         
         self._n0 = cx.shape[0]
         self._n1 = cx.shape[1]
         self._n2 = derham.nbasis['0'][2]
         
+        assert derham.spl_kind[1] , 'Use of poalr splines requires periodic splines in eta2.'
+        assert self.n1 == derham.Nel[1], f'Polar splines: number of control points {self.n1} in eta2 direction is not consistent with the grid (with {derham.Nel[1]}).'
+        
         self._d0 = self.n0 - 1
         self._d1 = self.n1 - 0
         self._d2 = derham.nbasis['3'][2]
         
         self._n_rings = [(2,), (1, 2), (2, 1), (1,)]
         self._n_polar = [(3,), (0, 2), (2, 0), (0,)]
```

### Comparing `struphy-1.9.9/src/struphy/polar/linear_operators.py` & `struphy-2.0.0/src/struphy/polar/linear_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/post_processing/cprofile_analyser.py` & `struphy-2.0.0/src/struphy/post_processing/cprofile_analyser.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/post_processing/post_processing_tools.py` & `struphy-2.0.0/src/struphy/post_processing/post_processing_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 
-import os, shutil, h5py, yaml
+import os
+import shutil
+import h5py
+import yaml
 
-from struphy.geometry import domains
-from struphy.fields_background.mhd_equil import equils
 from struphy.psydac_api.psydac_derham import Derham
 from struphy.psydac_api.fields import Field
 from struphy.kinetic_background import analytical
 from struphy.models.utilities import setup_domain_mhd
 
 from tqdm import tqdm
 
@@ -15,70 +16,71 @@
 def create_femfields(path, step=1):
     """
     Creates instances of struphy.psydac_api.fields.Field from distributed Struphy data.
 
     Parameters
     ----------
     path : str
-        Absolute path to folder with hdf5 data files.
+        Absolute path of simulation output folder.
 
     step : int, optional
         Whether to create FEM fields at every time step (step=1, default), every second time step (step=2), etc. 
 
     Returns
     -------
     fields : dict
         Nested dictionary holding struphy.psydac_api.field.Field: fields[t][name] contains the Field with the name "name" in the hdf5 file at time t.
 
     space_ids : dict
         The space IDs of the fields (H1, Hcurl, Hdiv, L2 or H1vec). space_ids[name] contains the space ID of the field with the name "name".
 
     model : str
-        From which model in struphy.models.models the data has been obtained.
+        From which model in struphy/models the data has been obtained.
     """
 
     # get model name and # of MPI processes from meta.txt file
     with open(os.path.join(path, 'meta.txt'), 'r') as f:
         lines = f.readlines()
 
-    model = lines[-6].split()[-1]
-    nproc = lines[-1].split()[-1]
+    model = lines[3].split()[-1]
+    nproc = lines[4].split()[-1]
 
     # create Derham sequence from grid parameters
     with open(os.path.join(path, 'parameters.yml'), 'r') as f:
         params = yaml.load(f, Loader=yaml.FullLoader)
-    
+
     derham = Derham(params['grid']['Nel'],
                     params['grid']['p'],
                     params['grid']['spl_kind'])
 
     # get fields names, space IDs and time grid from 0-th rank hdf5 file
-    file = h5py.File(os.path.join(path, 'data_proc0.hdf5'), 'r')
-    
+    file = h5py.File(os.path.join(path, 'data/', 'data_proc0.hdf5'), 'r')
+
     space_ids = {}
-    
+
     for field_name, dset in file['feec'].items():
         space_ids[field_name] = dset.attrs['space_id']
 
     t_grid = file['time/value'][::step].copy()
-    
+
     file.close()
 
     # create one FemField for each snapshot
     fields = {}
     for t in t_grid:
         fields[t] = {}
         for field_name, ID in space_ids.items():
             fields[t][field_name] = Field(field_name, ID, derham)
 
     # get hdf5 data
     for rank in range(int(nproc)):
 
         # open hdf5 file
-        file = h5py.File(os.path.join(path, 'data_proc' + str(rank) + '.hdf5'), 'r')
+        file = h5py.File(os.path.join(
+            path, 'data/', 'data_proc' + str(rank) + '.hdf5'), 'r')
 
         for field_name, dset in tqdm(file['feec'].items()):
 
             # get global start indices, end indices and pads
             gl_s = dset.attrs['starts']
             gl_e = dset.attrs['ends']
             pads = dset.attrs['pads']
@@ -108,18 +110,22 @@
                 else:
                     for comp in range(3):
 
                         s1, s2, s3 = gl_s[comp]
                         e1, e2, e3 = gl_e[comp]
                         p1, p2, p3 = pads[comp]
 
-                        data = dset[str(comp + 1)][n*step, p1:-p1, p2:-p2, p3:-p3].copy()
-
-                        fields[t][field_name].vector[comp][s1:e1 +
-                                                           1, s2:e2 + 1, s3:e3 + 1] = data
+                        data = dset[str(comp + 1)][n * step,
+                                                   p1:-p1,
+                                                   p2:-p2,
+                                                   p3:-p3].copy()
+
+                        fields[t][field_name].vector[comp][s1:e1 + 1,
+                                                           s2:e2 + 1,
+                                                           s3:e3 + 1] = data
                     # update after each data addition, can be made more efficient
                     fields[t][field_name].vector.update_ghost_regions()
 
         file.close()
 
     print('Creation of PSYDAC FemFields done.')
 
@@ -162,50 +168,51 @@
 
     assert isinstance(fields, dict)
     assert isinstance(space_ids, dict)
 
     # domain object according to parameter file and grids
     with open(os.path.join(path, 'parameters.yml'), 'r') as f:
         params = yaml.load(f, Loader=yaml.FullLoader)
-    
+
     domain = setup_domain_mhd(params)[0]
 
     # create logical and physical grids
     assert isinstance(celldivide, list)
     assert len(celldivide) == 3
-        
+
     Nel = params['grid']['Nel']
-    
-    grids_log = [np.linspace(0., 1., Nel_i*n_i + 1) for Nel_i, n_i in zip(Nel, celldivide)]
+
+    grids_log = [np.linspace(0., 1., Nel_i * n_i + 1)
+                 for Nel_i, n_i in zip(Nel, celldivide)]
     grids_phy = [domain(*grids_log)[0],
                  domain(*grids_log)[1],
                  domain(*grids_log)[2]]
 
     # evaluate fields at evaluation grid and push-forward
     point_data_log = {}
     point_data_phy = {}
-    
+
     # one dict for each field
     for name in space_ids:
         point_data_log[name] = {}
         point_data_phy[name] = {}
-    
+
     # time loop
     print('Evaluating fields ...')
     for t in tqdm(fields):
-        
+
         # field loop
         for name, field in fields[t].items():
-            
+
             # space ID
             space_id = space_ids[name]
 
             # field evaluation
             temp_val = field(*grids_log)
-            
+
             point_data_log[name][t] = []
             point_data_phy[name][t] = []
 
             # scalar spaces
             if isinstance(temp_val, np.ndarray):
 
                 point_data_log[name][t].append(temp_val)
@@ -216,15 +223,15 @@
                         temp_val, *grids_log, kind='0_form'))
                 elif space_id == 'L2':
                     point_data_phy[name][t].append(domain.push(
                         temp_val, *grids_log, kind='3_form'))
 
             # vector-valued spaces
             else:
-                
+
                 for j in range(3):
 
                     point_data_log[name][t].append(temp_val[j])
 
                     # push-forward
                     if space_id == 'Hcurl':
                         point_data_phy[name][t].append(domain.push(
@@ -238,124 +245,126 @@
 
     return point_data_log, point_data_phy, grids_log, grids_phy
 
 
 def create_vtk(path, grids_phy, point_data_phy):
     """
     Creates structured virtual toolkit files (.vts) for Paraview from evaluated field data.
-    
+
     Parameters
     ----------
     path : str
         Absolute path of where to store the .vts files. Will then be in path/vtk/step_<step>.vts.
-        
+
     grids_phy : 3-list
         Mapped (physical) grids obtained from struphy.diagnostics.post_processing.eval_femfields.
-        
+
     point_data_phy : dict
         Pushed-forward field data obtained from struphy.diagnostics.post_processing.eval_femfields.
     """
-    
+
     from pyevtk.hl import gridToVTK
-    
+
     # directory for vtk files
     path_vtk = os.path.join(path, 'vtk')
-    
+
     try:
         os.mkdir(path_vtk)
     except:
         shutil.rmtree(path_vtk)
         os.mkdir(path_vtk)
-        
+
     # field names
     names = list(point_data_phy.keys())
-        
+
     # time loop
     tgrid = list(point_data_phy[names[0]].keys())
-    
+
     nt = len(tgrid) - 1
     log_nt = int(np.log10(nt)) + 1
-    
+
     print('Creating vtk ...')
     for n, t in enumerate(tqdm(tgrid)):
-        
+
         point_data_n = {}
-        
+
         for name in names:
-            
+
             points_list = point_data_phy[name][t]
-            
+
             # scalar
             if len(points_list) == 1:
                 point_data_n[name] = points_list[0]
-                
+
             # vector
             else:
                 for j in range(3):
                     point_data_n[name + f'_{j + 1}'] = points_list[j]
-        
-        gridToVTK(os.path.join(path_vtk, 'step_{0:0{1}d}'.format(n, log_nt)), *grids_phy, pointData=point_data_n)
+
+        gridToVTK(os.path.join(path_vtk, 'step_{0:0{1}d}'.format(n, log_nt)),
+                  *grids_phy, pointData=point_data_n)
 
 
 def post_process_markers(path_in, path_out, species, step=1):
     """
     Computes the Cartesian (x, y, z) coordinates of saved markers during a simulation and writes them
     to text files that can be imported to e.g. Paraview (one text file for each time step saved as
     "<name_of_species>_<time_step>.txt" in a directory "kinetic_data/<name_of_species>/orbits/").
 
     Parameters
     ----------
     path_in : str
-        Absolute path to folder with hdf5 data files.
-        
+        Absolute path of simulation output folder.
+
     path_out : str
         Absolute path of where to store the .txt files. Will be in path_out/orbits. 
 
     species : str
         Name of the species for which the post processing should be performed.
-        
+
     step : int, optional
         Whether to do post-processing at every time step (step=1, default), every second time step (step=2), etc. 
     """
 
     # get # of MPI processes from meta.txt file
     with open(os.path.join(path_in, 'meta.txt'), 'r') as f:
         lines = f.readlines()
 
-    nproc = lines[-1].split()[-1]
+    nproc = lines[4].split()[-1]
 
     # create domain for calculating markers' physical coordinates
     with open(os.path.join(path_in, 'parameters.yml'), 'r') as f:
         params = yaml.load(f, Loader=yaml.FullLoader)
-    
+
     domain = setup_domain_mhd(params)[0]
-    
+
     # open hdf5 files and get names and number of saved markers of kinetic species
-    files = [h5py.File(os.path.join(path_in, f'data_proc{i}.hdf5'), 'r') for i in range(int(nproc))]
+    files = [h5py.File(os.path.join(
+        path_in, 'data/', f'data_proc{i}.hdf5'), 'r') for i in range(int(nproc))]
 
     n_IDs = files[0]['kinetic/' + species + '/markers'].shape[1]
 
     # directory for .txt files
     path_orbits = os.path.join(path_out, 'orbits')
-    
+
     try:
         os.mkdir(path_orbits)
     except:
         shutil.rmtree(path_orbits)
         os.mkdir(path_orbits)
 
     t_grid = files[0]['time/value'][::step]
 
     nt = len(t_grid) - 1
     log_nt = int(np.log10(nt)) + 1
 
     print('Evaluation of marker orbits for ' + str(species))
 
     # loop over time grid
-    for n, t in enumerate(tqdm(t_grid)):
+    for n, _ in enumerate(tqdm(t_grid)):
 
         # create text file for this time step and this species
         with open(os.path.join(path_orbits, species + '_{0:0{1}d}.txt'.format(n, log_nt)), 'w') as f_out:
 
             # find markers with right IDs by looping over all hdf5 files and all saved markers
             for ID in range(n_IDs):
 
@@ -370,18 +379,18 @@
                             # compute x, y, z coordinates and write to .txt file
                             X = domain(marker[0], marker[1], marker[2])
 
                             write_string = '{0:0{1}d}'.format(int(ID), 2)
                             write_string += ',' + str(X[0])
                             write_string += ',' + str(X[1])
                             write_string += ',' + str(X[2])
-                                        
+
                             if int(ID) < n_IDs - 1:
                                 write_string += '\n'
-                            
+
                             f_out.write(write_string)
                             break_flag = True
                             break
 
                     if break_flag:
                         break
 
@@ -394,118 +403,155 @@
     """
     Computes and saves distribution function of saved binning data during a simulation
     (saved as f_<slice>.npy in a directory "kinetic_data/<name_of_species>/distribution_function/").
 
     Parameters
     ----------
     path_in : str
-        Absolute path to folder with hdf5 data files.
-        
+        Absolute path of simulation output folder.
+
     path_out : str
         Absolute path of where to store the .txt files. Will be in path_out/orbits. 
 
     species : str
         Name of the species for which the post processing should be performed.
-        
+
     step : int, optional
         Whether to do post-processing at every time step (step=1, default), every second time step (step=2), etc.
-    
+
     marker_type : str
         Which type of markers were simulated.
     """
 
     # get model name and # of MPI processes from meta.txt file
     with open(os.path.join(path_in, 'meta.txt'), 'r') as f:
         lines = f.readlines()
 
-    model = lines[-6].split()[-1]
-    nproc = lines[-1].split()[-1]
-    
+    model = lines[3].split()[-1]
+    nproc = lines[4].split()[-1]
+
     # load parameters
     with open(os.path.join(path_in, 'parameters.yml'), 'r') as f:
         params = yaml.load(f, Loader=yaml.FullLoader)
 
     # open hdf5 files
-    files = [h5py.File(os.path.join(path_in, f'data_proc{i}.hdf5'), 'r') for i in range(int(nproc))]
+    files = [h5py.File(os.path.join(
+        path_in, 'data/', f'data_proc{i}.hdf5'), 'r') for i in range(int(nproc))]
 
     # directory for .npy files
     path_distr = os.path.join(path_out, 'distribution_function')
-    
+
     try:
         os.mkdir(path_distr)
     except:
         shutil.rmtree(path_distr)
         os.mkdir(path_distr)
 
     print('Evaluation of distribution functions for ' + str(species))
 
-    # loop over saved slices and sum up all ranks
+    # Create grids
     for slice_name, dset in tqdm(files[0]['kinetic/' + species + '/f'].items()):
 
+        # create a new folder for each slice
+        path_slice = os.path.join(path_distr, slice_name)
+        os.mkdir(path_slice)
+
+        # Find out all names of slices
+        slice_names = slice_name.split('_')
+
         # save grid
-        for n_gr, (_, gr) in enumerate(files[0]['kinetic/' + species + '/f/' + slice_name].attrs.items()):
-            grid_path = os.path.join(path_distr, 'grid_' + slice_name + '_' + str(n_gr + 1) + '.npy')
-            np.save(grid_path, gr[:])
+        for n_gr, (_, grid) in enumerate(files[0]['kinetic/' + species + '/f/' + slice_name].attrs.items()):
+            grid_path = os.path.join(
+                path_slice, 'grid_' + slice_names[n_gr] + '.npy')
+            np.save(grid_path, grid[:])
+
+    # compute distribution function (and delta f)
+    for k, (slice_name, dset) in enumerate(tqdm(files[0]['kinetic/' + species + '/f'].items())):
+
+        # path to folder of slice
+        path_slice = os.path.join(path_distr, slice_name)
+
+        # Find out all names of slices
+        slice_names = slice_name.split('_')
 
         # load data
         data = dset[::step].copy()
         for rank in range(1, int(nproc)):
-            data += files[rank]['kinetic/' + species + '/f/' + slice_name][::step]
+            data += files[rank]['kinetic/' +
+                                species + '/f/' + slice_name][::step]
 
         assert marker_type in ['full_f', 'control_variate', 'delta_f'], \
             f'Got unexpected marker type: {marker_type}'
 
         if marker_type == 'full_f':
             # save distribution function
-            np.save(os.path.join(path_distr, 'f_' + slice_name + '.npy'), data)
+            np.save(os.path.join(path_slice, 'f_binned.npy'), data)
 
         else:
-
             fun_name = params['kinetic'][species]['background']['type']
-            bckgr_params = params['kinetic'][species]['background'][fun_name]
+            bckgr_params = params['kinetic'][species]['background']
 
             # Get background function
-            if fun_name in bckgr_params:
+            if fun_name in bckgr_params.keys():
                 f_bckgr = getattr(analytical, fun_name)(
                     **bckgr_params[fun_name])
             else:
                 f_bckgr = getattr(analytical, fun_name)()
 
-            # multiplier collecting all non-integrated slices in velocity space
-            data_bckgr = np.ones(data.shape)
+            # load all grids of the variables of f
+            grid_tot = []
+            for coord in ['e', 'v']:
+                for comp in range(1, 4):
+                    current_slice = coord + str(comp)
+                    filename = os.path.join(
+                        path_slice, 'grid_' + current_slice + '.npy')
+
+                    # check if file exists and is in slice_name
+                    if os.path.exists(filename) and current_slice in slice_names:
+                        grid_tot += [np.load(filename)]
+
+                    # otherwise evaluate at zero 
+                    else:
+                        if coord == 'e':
+                            grid_tot += [np.zeros(1)]
+                        elif coord == 'v':
+                            grid_tot += [np.zeros(1)]
 
-            if isinstance(f_bckgr, analytical.Maxwellian6DUniform):
-                for direction in slice_name.split('_'):
-                    if direction[0] == 'v':
-
-                        for k in range(len(slice_name.split('_'))):
-                            slicing = [None] * len(data.shape)
-                            slicing[k + 1] = slice(None)
-                            grid_v = files[0]['kinetic/' + species + '/f/' + slice_name].attrs['bin_centers_' + str(k+1)]
-                            data_bckgr *= getattr(f_bckgr, 'gaussian')(grid_v, u=f_bckgr.params['u' + direction[1]], 
-                                                                       vth=f_bckgr.params['vth' + direction[1]])[tuple(slicing)]
+            grid_eval = np.meshgrid(*grid_tot, indexing='ij')
 
-            else:
-                raise NotImplementedError(f'Post-processing is not yet available for background of type {fun_name}')
+            data_bckgr = f_bckgr(*grid_eval).squeeze()
 
             if marker_type == 'control_variate':
                 data_delta_f = data
 
             elif marker_type == 'delta_f':
 
                 # Linearized Vlasov-Maxwell system
                 if model == "LinearVlasovMaxwell":
                     assert fun_name == 'Maxwellian6DUniform', \
                         'The linearized Vlasov-Maxwell is only implemented for a uniform Maxwellian background!'
 
-                    data_delta_f = np.multiply(data, np.sqrt(data_bckgr))
+                    # h = f_1 / sqrt{f_0}
+                    data_delta_f = np.multiply(data,
+                                               np.sqrt(data_bckgr[tuple([None])]))  # add extra axis at beginning
+
+                # Vlasov-Maxwell system with Delta-f
+                elif model == "DeltaFVlasovMaxwell":
+                    assert fun_name == 'Maxwellian6DUniform', \
+                        'The Vlasov-Maxwell system with Delta-f is only implemented for a uniform Maxwellian background!'
+
+                    # h = f_0 - (f_0 + f_1) * ln(f_0)
+                    data_delta_f = data_bckgr[tuple([None])] - \
+                        np.multiply(data_bckgr[tuple([None])] + data,
+                                    np.log(data_bckgr[tuple([None])]))
 
                 else:
-                    raise NotImplementedError(f'Post-processing for the model {model} has not been implemented yet!')
+                    raise NotImplementedError(
+                        f'Post-processing for the model {model} with {marker_type} has not been implemented yet!')
 
             # save distribution function
-            np.save(os.path.join(path_distr, 'delta_f_' + slice_name + '.npy'), data_delta_f)
-            np.save(os.path.join(path_distr, 'f_' + slice_name + '.npy'), data_delta_f + data_bckgr)
+            np.save(os.path.join(path_slice, 'delta_f_binned.npy'), data_delta_f)
+            np.save(os.path.join(path_slice, 'f_binned.npy'), data_delta_f + data_bckgr)
 
     # close hdf5 files
     for file in files:
         file.close()
```

### Comparing `struphy-1.9.9/src/struphy/post_processing/pproc_struphy.py` & `struphy-2.0.0/src/struphy/post_processing/pproc_struphy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 def main(path, step=1, celldivide=1):
     """
     Post-processing of finished Struphy runs.
-    
+
     Parameters
     ----------
-    paths : str
+    path : str
         Absolute path of simulation output folder to post-process.
-        
+
     step : int, optional
         Whether to do post-processing at every time step (step=1, default), every second time step (step=2), etc.
-        
+
     celldivide : int, optional
         Grid refinement in evaluation of FEM fields. E.g. celldivide=2 evaluates two points per grid cell. 
     """
-    
-    import os, shutil, h5py, pickle, yaml
-    
+
+    import os
+    import shutil
+    import h5py
+    import pickle
+    import yaml
+
     import numpy as np
 
     import struphy.post_processing.post_processing_tools as pproc
 
     print('')
 
     # create post-processing folder
@@ -28,72 +32,91 @@
     try:
         os.mkdir(path_pproc)
     except:
         shutil.rmtree(path_pproc)
         os.mkdir(path_pproc)
 
     # check for fields and kinetic data in hdf5 file that need post processing
-    file = h5py.File(os.path.join(path, 'data_proc0.hdf5'), 'r')
+    file = h5py.File(os.path.join(path, 'data/', 'data_proc0.hdf5'), 'r')
 
     # save time grid at which post-processing data is created
-    np.save(os.path.join(path_pproc, 't_grid.npy'), file['time/value'][::step].copy())
+    np.save(os.path.join(path_pproc, 't_grid.npy'),
+            file['time/value'][::step].copy())
 
     if 'feec' in file.keys():
         exist_fields = True
     else:
         exist_fields = False
 
     kinetic_species = []
     if 'kinetic' in file.keys():
-        exist_kinetic = [[], []]
+        exist_kinetic = {'markers': False, 'f': False}
 
         for name in file['kinetic'].keys():
             kinetic_species += [name]
 
             # check for saved markers
             if 'markers' in file['kinetic'][name]:
-                exist_kinetic[0] += [True]
-            else:
-                exist_kinetic[0] += [False]
+                exist_kinetic['markers'] = True
 
             # check for saved distribution function
             if 'f' in file['kinetic'][name]:
-                exist_kinetic[1] += [True]
-            else:
-                exist_kinetic[1] += [False]
+                exist_kinetic['f'] = True
+
     else:
-        exist_kinetic = False
+        exist_kinetic = None
 
     file.close()
 
     # field post-processing
     if exist_fields:
 
-        fields, space_ids, model = pproc.create_femfields(path, step)
+        fields, space_ids, _ = pproc.create_femfields(path, step)
 
         point_data_log, point_data_phy, grids_log, grids_phy = pproc.eval_femfields(
             path, fields, space_ids, [celldivide, celldivide, celldivide])
 
         # directory for field data
         path_fields = os.path.join(path_pproc, 'fields_data')
-        
+
         try:
             os.mkdir(path_fields)
         except:
             shutil.rmtree(path_fields)
             os.mkdir(path_fields)
 
         # save data dicts for each field
         for name, val in point_data_log.items():
+            
+            aux = name.split('_')
+            # is em field
+            if len(aux) == 1:
+                subfolder = 'em_fields'
+                new_name = name
+                try:
+                    os.mkdir(os.path.join(path_fields, subfolder))
+                except:
+                    pass
+                
+            # is fluid species
+            elif len(aux) == 2:
+                subfolder = aux[0]
+                new_name = aux[1]
+                try:
+                    os.mkdir(os.path.join(path_fields, subfolder))
+                except:
+                    pass
+            else:
+                raise ValueError(f'Naming {name} of feec unknown is not permitted (can only have one underscore).')
 
-            with open(os.path.join(path_fields, name + '_log.bin'), 'wb') as handle:
+            with open(os.path.join(path_fields, subfolder, new_name + '_log.bin'), 'wb') as handle:
                 pickle.dump(val, handle,
                             protocol=pickle.HIGHEST_PROTOCOL)
 
-            with open(os.path.join(path_fields, name + '_phy.bin'), 'wb') as handle:
+            with open(os.path.join(path_fields, subfolder, new_name + '_phy.bin'), 'wb') as handle:
                 pickle.dump(point_data_phy[name], handle,
                             protocol=pickle.HIGHEST_PROTOCOL)
 
         # save grids
         with open(os.path.join(path_fields, 'grids_log.bin'), 'wb') as handle:
             pickle.dump(grids_log, handle,
                         protocol=pickle.HIGHEST_PROTOCOL)
@@ -102,80 +125,82 @@
             pickle.dump(grids_phy, handle,
                         protocol=pickle.HIGHEST_PROTOCOL)
 
         # create vtk files
         pproc.create_vtk(path_fields, grids_phy, point_data_phy)
 
     # kinetic post-processing
-    if np.any(exist_kinetic):
+    if exist_kinetic is not None:
 
         # directory for kinetic data
         path_kinetics = os.path.join(path_pproc, 'kinetic_data')
-        
+
         try:
             os.mkdir(path_kinetics)
         except:
             shutil.rmtree(path_kinetics)
             os.mkdir(path_kinetics)
 
-    # kinetic post-processing for each species
-    for n, species in enumerate(kinetic_species):
+        # kinetic post-processing for each species
+        for n, species in enumerate(kinetic_species):
 
-        # directory for each species
-        path_kinetics_species = os.path.join(path_kinetics, species)
-        
-        try:
-            os.mkdir(path_kinetics_species)
-        except:
-            shutil.rmtree(path_kinetics_species)
-            os.mkdir(path_kinetics_species)
-
-        # markers
-        if exist_kinetic[0][n]:
-            pproc.post_process_markers(path, path_kinetics_species, species, step)
-
-        # distribution function
-        if exist_kinetic[1][n]:
-
-            with open(os.path.join(path, 'parameters.yml'), 'r') as f:
-                params = yaml.load(f, Loader=yaml.FullLoader)
+            # directory for each species
+            path_kinetics_species = os.path.join(path_kinetics, species)
 
             try:
-                marker_type = params['kinetic'][species]['markers']['type']
+                os.mkdir(path_kinetics_species)
             except:
-                marker_type = 'full_f'
+                shutil.rmtree(path_kinetics_species)
+                os.mkdir(path_kinetics_species)
+
+            # markers
+            if exist_kinetic['markers']:
+                pproc.post_process_markers(path, path_kinetics_species, species, step)
+
+            # distribution function
+            if exist_kinetic['f']:
+
+                with open(os.path.join(path, 'parameters.yml'), 'r') as f:
+                    params = yaml.load(f, Loader=yaml.FullLoader)
+
+                try:
+                    marker_type = params['kinetic'][species]['markers']['type']
+                except:
+                    marker_type = 'full_f'
 
-            pproc.post_process_f(path, path_kinetics_species, species, step, marker_type)
+                pproc.post_process_f(path, path_kinetics_species,
+                                    species, step, marker_type)
 
 
 if __name__ == '__main__':
-    
+
     import argparse
     import struphy
 
     libpath = struphy.__path__[0]
-    
-    parser = argparse.ArgumentParser(description='Post-process data of finished Struphy runs to prepare for diagnostics.')
-    
+
+    parser = argparse.ArgumentParser(
+        description='Post-process data of finished Struphy runs to prepare for diagnostics.')
+
     # paths of simulation folders
     parser.add_argument('dir',
                         type=str,
                         metavar='DIR',
                         help='absolute path of simulation ouput folder to post-process')
 
     parser.add_argument('-s', '--step',
                         type=int,
                         metavar='N',
                         help='do post-processing every N-th time step (default=1)',
                         default=1)
-    
+
     parser.add_argument('--celldivide',
                         type=int,
                         metavar='N',
                         help='divide each grid cell by N for field evaluation (default=1)',
                         default=1)
-    
+
     args = parser.parse_args()
-    
+
     main(args.dir,
          args.step,
          args.celldivide)
```

### Comparing `struphy-1.9.9/src/struphy/post_processing/profile_struphy.py` & `struphy-2.0.0/src/struphy/post_processing/profile_struphy.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
         with open(path + 'profile_dict.sav', 'rb') as f:
             dicts_pre += [pickle.load(f)]
 
         with open(path + 'meta.txt', 'r') as f:
             lines = f.readlines()
 
-        nproc += [int(lines[-1].split()[-1])]
+        nproc += [int(lines[4].split()[-1])]
 
         with open(path + 'parameters.yml', 'r') as f:
             params = yaml.load(f, Loader=yaml.FullLoader)
 
         Nel += [params['grid']['Nel']]
 
     # Nicer key names for output:
```

### Comparing `struphy-1.9.9/src/struphy/propagators/base.py` & `struphy-2.0.0/src/struphy/propagators/base.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/propagators/propagators_coupling.py` & `struphy-2.0.0/src/struphy/propagators/propagators_coupling.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import numpy as np
 
 from psydac.linalg.block import BlockVector
 
 from struphy.propagators.base import Propagator
 from struphy.linear_algebra.schur_solver import SchurSolver
 from struphy.pic.particles import Particles6D
-from struphy.pic.particles_to_grid import Accumulator
+from struphy.pic.particles_to_grid import Accumulator, AccumulatorVector
 from struphy.pic.pusher import Pusher
 import struphy.pic.utilities_kernels as utilities
 from struphy.polar.basic import PolarVector
-from struphy.kinetic_background.analytical import Maxwellian, Maxwellian6DUniform
+from struphy.kinetic_background.analytical import Maxwellian, Maxwellian6DUniform, Maxwellian5DUniform
 from struphy.fields_background.mhd_equil.equils import set_defaults
 
 from struphy.psydac_api.linear_operators import CompositeLinearOperator as Compose
-from struphy.psydac_api.linear_operators import SumLinearOperator as Sum
 from struphy.psydac_api.linear_operators import ScalarTimesLinearOperator as Multiply
 from struphy.psydac_api.linear_operators import InverseLinearOperator as Inverse
 from struphy.psydac_api import preconditioner
 from struphy.psydac_api.linear_operators import LinOpWithTransp
 from struphy.psydac_api.mass import WeightedMassOperator
 import struphy.linear_algebra.iterative_solvers as it_solvers
 
+from psydac.linalg.iterative_solvers import pcg
 
-class EfieldWeights(Propagator):
+
+class EfieldWeightsImplicit(Propagator):
     r'''Solve the following Crank-Nicolson step
 
     .. math::
 
         \begin{bmatrix}
             \mathbb{M}_1 \left( \mathbf{e}^{n+1} - \mathbf{e}^n \right) \\
             \mathbf{W}^{n+1} - \mathbf{W}^n
@@ -75,35 +76,37 @@
         self._e = e
 
         assert isinstance(particles, Particles6D)
         self._particles = particles
 
         # parameters
         params_default = {'alpha': 1e2,
+                          'kappa': 1.,
                           'f0': Maxwellian6DUniform(),
                           'type': 'PConjugateGradient',
                           'pc': 'MassMatrixPreconditioner',
                           'tol': 1e-8,
                           'maxiter': 3000,
                           'info': False,
                           'verbose': False}
 
         params = set_defaults(params, params_default)
 
         assert isinstance(params['f0'], Maxwellian6DUniform)
 
         self._alpha = params['alpha']
+        self._kappa = params['kappa']
         self._f0 = params['f0']
         self._f0_params = np.array([self._f0.params['n'],
-                                    self._f0.params['ux'],
-                                    self._f0.params['uy'],
-                                    self._f0.params['uz'],
-                                    self._f0.params['vthx'],
-                                    self._f0.params['vthy'],
-                                    self._f0.params['vthz']])
+                                    self._f0.params['u1'],
+                                    self._f0.params['u2'],
+                                    self._f0.params['u3'],
+                                    self._f0.params['vth1'],
+                                    self._f0.params['vth2'],
+                                    self._f0.params['vth3']])
 
         self._info = params['info']
 
         # Initialize Accumulator object
         self._accum = Accumulator(self.derham, self.domain, 'Hcurl', 'linear_vlasov_maxwell',
                                   add_vector=True, symmetry='symm')
 
@@ -132,60 +135,213 @@
         # Instantiate Schur solver
         self._schur_solver = SchurSolver(_A, _BC, pc=self._pc, solver_name=params['type'],
                                          tol=params['tol'], maxiter=params['maxiter'],
                                          verbose=params['verbose'])
 
         # Instantiate particle pusher
         self._pusher = Pusher(self.derham, self.domain,
-                              'push_weights_with_efield')
+                              'push_weights_with_efield_lin_vm')
 
     @property
     def variables(self):
         return [self._e]
 
     def __call__(self, dt):
-        """
-        TODO
-        """
         # evaluate f0 and accumulate
         f0_values = self._f0(self._particles.markers[:, 0],
                              self._particles.markers[:, 1],
                              self._particles.markers[:, 2],
                              self._particles.markers[:, 3],
                              self._particles.markers[:, 4],
                              self._particles.markers[:, 5])
 
         self._accum.accumulate(self._particles, f0_values,
-                               self._f0_params, self._alpha)
+                               self._f0_params, self._alpha, self._kappa)
 
         # Update Schur solver
         self._schur_solver.BC = - self._accum.operators[0].matrix / 4
 
         # allocate temporary BlockVector during solution
         self._e_temp, info = self._schur_solver(
             self._e, self._accum.vectors[0] / 2., dt)
 
         # Store old weights
         self._old_weights[~self._particles.holes] = self._particles.markers[~self._particles.holes, 6]
 
-        self._e_sum = self._e_temp + self._e
+        # reset _e_sum
+        self._e_sum *= 0.
+
+        # self._e_sum = self._e_temp + self._e
+        self._e_sum += self._e_temp
+        self._e_sum += self._e
 
         # Update weights
         self._pusher(self._particles, dt,
-                     self._e_temp.blocks[0]._data + self._e.blocks[0]._data,
-                     self._e_temp.blocks[1]._data + self._e.blocks[1]._data,
-                     self._e_temp.blocks[2]._data + self._e.blocks[2]._data,
+                     self._e_sum.blocks[0]._data,
+                     self._e_sum.blocks[1]._data,
+                     self._e_sum.blocks[2]._data,
                      f0_values,
                      self._f0_params,
-                     int(self._particles.n_mks))
+                     int(self._particles.n_mks),
+                     self._kappa)
 
         # write new coeffs into self.variables
         max_de, = self.in_place_update(self._e_temp)
 
-        # Print out max differences for weights and efield
+        # Print out max differences for weights and e-field
+        if self._info:
+            print('Status          for StepEfieldWeights:', info['success'])
+            print('Iterations      for StepEfieldWeights:', info['niter'])
+            print('Maxdiff    e1   for StepEfieldWeights:', max_de)
+            max_diff = np.max(np.abs(self._old_weights[~self._particles.holes]
+                                     - self._particles.markers[~self._particles.holes, 6]))
+            print('Maxdiff weights for StepEfieldWeights:', max_diff)
+            print()
+
+
+class EfieldWeightsExplicit(Propagator):
+    r'''Solve the following system analytically
+
+    .. math::
+
+        \begin{align}
+            \frac{\text{d}}{\text{d} t} w_p & = \frac{1}{N \, s_{0, p}} \frac{\kappa}{v_{\text{th}}^2} \left[ DF^{-T} (\mathbb{\Lambda}^1)^T \mathbf{e} \right]
+            \cdot \mathbf{v}_p \left( \frac{f_0}{\ln(f_0)} - f_0 \right) \\[2mm]
+            \frac{\text{d}}{\text{d} t} \mathbb{M}_1 \mathbf{e} & = - \alpha^2 \kappa \sum_p \mathbb{\Lambda}^1 \cdot \left( DF^{-1} \mathbf{v}_p \right)
+            \frac{1}{N \, s_{0, p}} \left( \frac{f_0}{\ln(f_0)} - f_0 \right)
+        \end{align}
+
+    Parameters
+    ---------- 
+    e : psydac.linalg.block.BlockVector
+        FE coefficients of a 1-form.
+
+    particles : struphy.pic.particles.Particles6D
+        Particles object.
+
+    **params : dict
+        Solver- and/or other parameters for this splitting step.
+    '''
+
+    def __init__(self, e, particles, **params):
+
+        from struphy.kinetic_background.analytical import Maxwellian6DUniform
+
+        # pointers to variables
+        assert isinstance(e, (BlockVector, PolarVector))
+        self._e = e
+
+        assert isinstance(particles, Particles6D)
+        self._particles = particles
+
+        # parameters
+        params_default = {'alpha': 1e2,
+                          'kappa': 1.,
+                          'f0': Maxwellian6DUniform(),
+                          'type': 'PConjugateGradient',
+                          'pc': 'MassMatrixPreconditioner',
+                          'tol': 1e-8,
+                          'maxiter': 3000,
+                          'info': False,
+                          'verbose': False}
+
+        params = set_defaults(params, params_default)
+
+        self._params = params
+
+        assert isinstance(params['f0'], Maxwellian6DUniform)
+
+        self._alpha = params['alpha']
+        self._kappa = params['kappa']
+        self._f0 = params['f0']
+        self._f0_params = np.array([self._f0.params['n'],
+                                    self._f0.params['u1'],
+                                    self._f0.params['u2'],
+                                    self._f0.params['u3'],
+                                    self._f0.params['vth1'],
+                                    self._f0.params['vth2'],
+                                    self._f0.params['vth3']])
+
+        self._info = params['info']
+
+        # Initialize Accumulator object
+        self._accum = AccumulatorVector(
+            self.derham, self.domain, 'Hcurl', 'delta_f_vlasov_maxwell')
+
+        # Create buffers to temporarily store _e and its sum with old e
+        self._m1_acc_vec = e.copy()
+        self._e_dt2 = e.copy()
+
+        # store old weights to compute difference
+        self._old_weights = np.empty(particles.markers.shape[0], dtype=float)
+
+        # ================================
+        # ========= Schur Solver =========
+        # ================================
+
+        # Preconditioner
+        if params['pc'] == None:
+            self._pc = None
+        else:
+            pc_class = getattr(preconditioner, params['pc'])
+            self._pc = pc_class(self.mass_ops.M1)
+
+        self._pusher = Pusher(self.derham, self.domain,
+                              'push_weights_with_efield_deltaf_vm')
+
+    @property
+    def variables(self):
+        return [self._e]
+
+    def __call__(self, dt):
+        # evaluate f0 and accumulate
+        f0_values = self._f0(self._particles.markers[:, 0],
+                             self._particles.markers[:, 1],
+                             self._particles.markers[:, 2],
+                             self._particles.markers[:, 3],
+                             self._particles.markers[:, 4],
+                             self._particles.markers[:, 5])
+
+        self._accum.accumulate(self._particles, f0_values,
+                               self._f0_params, self._alpha, self._kappa)
+
+        self._m1_acc_vec, info = pcg(self.mass_ops.M1,
+                                     self._accum.vectors[0],
+                                     self._pc,
+                                     self._e,
+                                     tol=self._params['tol'],
+                                     maxiter=self._params['maxiter'],
+                                     verbose=self._params['verbose']
+                                     )
+
+        # Store old weights
+        self._old_weights[~self._particles.holes] = self._particles.markers[~self._particles.holes, 6]
+
+        # Compute vector for particle pushing
+        self._e_dt2 *= 0.
+        self._e_dt2 -= self._m1_acc_vec
+        self._e_dt2 *= dt / 2
+        self._e_dt2 += self._e
+
+        # Update weights
+        self._pusher(self._particles, dt,
+                     self._e_dt2.blocks[0]._data,
+                     self._e_dt2.blocks[1]._data,
+                     self._e_dt2.blocks[2]._data,
+                     f0_values,
+                     self._f0_params,
+                     int(self._particles.n_mks),
+                     self._kappa)
+
+        # Update e-field and compute max difference
+        self._m1_acc_vec *= dt
+        max_de = np.max(np.abs(self._m1_acc_vec.toarray()))
+        self._e -= self._m1_acc_vec
+
+        # Print out max differences for weights and e-field
         if self._info:
             print('Status          for StepEfieldWeights:', info['success'])
             print('Iterations      for StepEfieldWeights:', info['niter'])
             print('Maxdiff    e1   for StepEfieldWeights:', max_de)
             max_diff = np.max(np.abs(self._old_weights[~self._particles.holes]
                                      - self._particles.markers[~self._particles.holes, 6]))
             print('Maxdiff weights for StepEfieldWeights:', max_diff)
@@ -702,24 +858,24 @@
         self._u = u
 
         # parameters
         params_default = {'u_space': 'Hdiv',
                           'b': None,
                           'b_eq': None,
                           'unit_b1': None,
-                          'f0': Maxwellian6DUniform(),
+                          'f0': Maxwellian5DUniform(),
                           'type': 'PConjugateGradient',
                           'pc': 'MassMatrixPreconditioner',
                           'tol': 1e-8,
                           'maxiter': 3000,
                           'info': False,
                           'verbose': False,
                           'Ab': 1,
                           'Ah': 1,
-                          'kappa': 100.}
+                          'kappa': 1.}
 
         params = set_defaults(params, params_default)
 
         assert params['u_space'] in {'Hcurl', 'Hdiv', 'H1vec'}
 
         if params['u_space'] == 'H1vec':
             self._space_key_int = 0
@@ -735,99 +891,110 @@
 
         assert isinstance(params['b_eq'], (BlockVector, PolarVector))
         self._b_eq = params['b_eq']
 
         assert isinstance(params['unit_b1'], (BlockVector, PolarVector))
         self._unit_b1 = params['unit_b1']
 
-        self._type = params['type']
-        self._pc = params['pc']
-        self._tol = params['tol']
-        self._maxiter = params['maxiter']
         self._info = params['info']
-        self._verbose = params['verbose']
         self._rank = self.derham.comm.Get_rank()
 
-        self._coupling_mat = params['Ah'] / params['Ab'] * params['kappa']**2
-        self._coupling_vec = params['Ah'] / params['Ab'] * params['kappa']
-        self._scale_push = 1*params['kappa']
+        self._coupling_mat = params['Ah'] / params['Ab']
+        self._coupling_vec = params['Ah'] / params['Ab']
+        self._scale_push = 1
 
         self._curl_norm_b = self.derham.curl.dot(self._unit_b1)
         self._curl_norm_b.update_ghost_regions()
 
-        b_full = self._b_eq.copy()
-        if self._b is not None:
-            b_full += self._b
-
-        b_full.update_ghost_regions()
-
         u_id = self.derham.spaces_dict[params['u_space']]
+        self._EuT = self.derham.E[u_id].transpose()
+        self._EbT = self.derham.E['2'].transpose()
 
         # define system [[A B], [C I]] [u_new, v_new] = [[A -B], [-C I]] [u_old, v_old] (without time step size dt)
-        self._A = getattr(self.mass_ops, 'M' + u_id + 'n')
+        _A = getattr(self.mass_ops, 'M' + u_id + 'n')
 
         # preconditioner
         if params['pc'] is None:
-            self._pc = None
+            pc = None
         else:
             pc_class = getattr(preconditioner, params['pc'])
-            self._pc = pc_class(self._A)
+            pc = pc_class(_A)
 
         # Call the accumulation and Pusher class
         self._ACC = Accumulator(self.derham, self.domain, params['u_space'],
                                 'cc_lin_mhd_5d_J1', add_vector=True, symmetry='symm')
         self._pusher = Pusher(self.derham, self.domain,
                               'push_gc_cc_J1_' + params['u_space'])
 
+        # define BC and B dot V of the Schur block matrix [[A, B], [C, I]]
+        _BC = Multiply(-1/4, self._ACC.operators[0])
+
+        # call SchurSolver class
+        self._schur_solver = SchurSolver(_A, _BC, pc=pc, solver_name=params['type'],
+                                         tol=params['tol'], maxiter=params['maxiter'],
+                                         verbose=params['verbose'])
+
+        # temporary vectors to avoid memory allocation
+        self._b_full1 = self._b_eq.space.zeros()
+        self._b_full2 = self._EbT.codomain.zeros()
+
+        self._u_new = self._u.space.zeros()
+
+        self._u_avg1 = self._u.space.zeros()
+        self._u_avg2 = self._EuT.codomain.zeros()
+
     @property
     def variables(self):
         return [self._u]
 
     def __call__(self, dt):
 
         un = self.variables[0]
 
-        # sum up total magnetic field
-        b_full = self._b_eq.copy()
+        # sum up total magnetic field b_full1 = b_eq + b_tilde (in-place)
+        self._b_eq.copy(out=self._b_full1)
+
         if self._b is not None:
-            b_full += self._b
+            self._b_full1 += self._b
 
-        b_full.update_ghost_regions()
+        # extract coefficients to tensor product space (in-place)
+        self._EbT.dot(self._b_full1, out=self._b_full2)
+
+        # update ghost regions because of non-local access in accumulation kernel!
+        self._b_full2.update_ghost_regions()
 
         # acuumulate MAT and VEC
         self._ACC.accumulate(self._particles, self._kappa,
-                             b_full[0]._data, b_full[1]._data, b_full[2]._data,
+                             self._b_full2[0]._data, self._b_full2[1]._data, self._b_full2[2]._data,
                              self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                              self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                              self._space_key_int, self._coupling_mat, self._coupling_vec)
 
-        # define BC and B dot V of the Schur block matrix [[A, B], [C, I]]
-        _BC = Multiply(-1/4, self._ACC.operators[0])
+        # solve linear system for updated u coefficients
+        info = self._schur_solver(
+            un, -self._ACC.vectors[0]/2, dt, out=self._u_new)[1]
 
-        # call SchurSolver class
-        schur_solver = SchurSolver(self._A, _BC, pc=self._pc, solver_name=self._type,
-                                   tol=self._tol, maxiter=self._maxiter,
-                                   verbose=self._verbose)
+        # call pusher kernel with average field (u_new + u_old)/2 and update ghost regions because of non-local access in kernel
+        un.copy(out=self._u_avg1)
+        self._u_avg1 += self._u_new
+        self._u_avg1 /= 2
 
-        # solve linear system for updated u coefficients
-        u_new, info = schur_solver(un, -self._ACC.vectors[0]/2, dt)
+        self._EuT.dot(self._u_avg1, out=self._u_avg2)
 
-        # calculate average u
-        u_avg = (un + u_new)/2
-        u_avg.update_ghost_regions()
+        self._u_avg2.update_ghost_regions()
 
-        self._pusher(self._particles, dt,
+        self._pusher(self._particles, self._scale_push*dt,
                      self._kappa,
-                     b_full[0]._data, b_full[1]._data, b_full[2]._data,
+                     self._b_full2[0]._data, self._b_full2[1]._data, self._b_full2[2]._data,
                      self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                      self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                     u_avg[0]._data, u_avg[1]._data, u_avg[2]._data)
+                     self._u_avg2[0]._data, self._u_avg2[1]._data, self._u_avg2[2]._data)
 
         # write new coeffs into Propagator.variables
-        max_du, = self.in_place_update(u_new)
+        max_du, = self.in_place_update(self._u_new)
 
         if self._info and self._rank == 0:
             print('Status     for CurrentCoupling5DCurrent1:', info['success'])
             print('Iterations for CurrentCoupling5DCurrent1:', info['niter'])
             print('Maxdiff u1 for CurrentCoupling5DCurrent1:', max_du)
             print()
 
@@ -845,98 +1012,91 @@
         self._particles = particles
 
         # pointers to variables
         assert isinstance(u, (BlockVector, PolarVector))
         self._u = u
 
         # parameters
-        params_default = {'b': None,
-                          'u_space': 'Hdiv',
+        params_default = {'u_space': 'Hdiv',
+                          'b': None,
                           'b_eq': None,
                           'unit_b1': None,
                           'unit_b2': None,
                           'abs_b': None,
-                          'f0': Maxwellian6DUniform(),
+                          'f0': Maxwellian5DUniform(),
                           'type': 'PConjugateGradient',
                           'pc': 'MassMatrixPreconditioner',
                           'tol': 1e-8,
                           'maxiter': 3000,
                           'info': False,
                           'verbose': False,
                           'Ab': 1,
                           'Ah': 1,
-                          'kappa': 100.,
+                          'kappa': 1.,
                           'integrator': 'explicit',
                           'method': 'rk4'}
 
         params = set_defaults(params, params_default)
 
         assert params['u_space'] in {'Hcurl', 'Hdiv', 'H1vec'}
+
         if params['u_space'] == 'H1vec':
             self._space_key_int = 0
         else:
             self._space_key_int = int(
                 self.derham.spaces_dict[params['u_space']])
 
         self._kappa = params['kappa']
         self._f0 = params['f0']
+
         assert isinstance(params['b'], (BlockVector, PolarVector))
         self._b = params['b']
+
         assert isinstance(params['b_eq'], (BlockVector, PolarVector))
         self._b_eq = params['b_eq']
+
         assert isinstance(params['unit_b1'], (BlockVector, PolarVector))
         self._unit_b1 = params['unit_b1']
+
         assert isinstance(params['unit_b2'], (BlockVector, PolarVector))
         self._unit_b2 = params['unit_b2']
+
         self._abs_b = params['abs_b']
 
         self._curl_norm_b = self.derham.curl.dot(self._unit_b1)
         self._curl_norm_b.update_ghost_regions()
 
-        self._type = params['type']
-        self._pc = params['pc']
-        self._tol = params['tol']
-        self._maxiter = params['maxiter']
         self._info = params['info']
-        self._verbose = params['verbose']
+
         self._rank = self.derham.comm.Get_rank()
 
-        self._coupling_mat = params['Ah'] / params['Ab'] * params['kappa']**2
-        self._coupling_vec = params['Ah'] / params['Ab'] * params['kappa']
-        self._scale_push = 1*params['kappa']
+        self._coupling_mat = params['Ah'] / params['Ab']
+        self._coupling_vec = params['Ah'] / params['Ab']
+        self._scale_push = 1
 
         u_id = self.derham.spaces_dict[params['u_space']]
-
-        # sum up total magnetic field
-        b_full = self._b_eq.copy()
-        if self._b is not None:
-            b_full += self._b
-
-        b_full.update_ghost_regions()
+        self._EuT = self.derham.E[u_id].transpose()
+        self._E1T = self.derham.E['1'].transpose()
+        self._EbT = self.derham.E['2'].transpose()
 
         self._PB = getattr(self.basis_ops, 'PB')
-        self._PBb = self._PB.dot(b_full)
-        self._PBb.update_ghost_regions()
-
-        self._grad_PBb = self.derham.grad.dot(self._PBb)
-        self._grad_PBb.update_ghost_regions()
 
+        # define system [[A B], [C I]] [u_new, v_new] = [[A -B], [-C I]] [u_old, v_old] (without time step size dt)
         _A = getattr(self.mass_ops, 'M' + u_id + 'n')
 
         # preconditioner
         if params['pc'] is None:
             pc = None
         else:
             pc_class = getattr(preconditioner, params['pc'])
             pc = pc_class(_A)
 
         # Call the accumulation and Pusher class
         self._ACC = Accumulator(
             self.derham, self.domain,  params['u_space'], 'cc_lin_mhd_5d_J2', add_vector=True, symmetry='symm')
-        # self._pusher = Pusher(self.derham, self.domain, 'push_gc_cc_J2_' +  params['u_space'])
 
         # choose algorithm
         if params['method'] == 'forward_euler':
             a = []
             b = [1.]
             c = [0.]
         elif params['method'] == 'heun2':
@@ -964,67 +1124,90 @@
 
         _BC = Multiply(-1/4, self._ACC.operators[0])
 
         self._schur_solver = SchurSolver(_A, _BC, pc=pc, solver_name=params['type'],
                                          tol=params['tol'], maxiter=params['maxiter'],
                                          verbose=params['verbose'])
 
-        self._rank = self.derham.comm.Get_rank()
+        # temporary vectors to avoid memory allocation
+        self._b_full1 = self._b_eq.space.zeros()
+        self._b_full2 = self._EbT.codomain.zeros()
+
+        self._PBb = self._abs_b.space.zeros()
+        self._grad_PBb1 = self._unit_b1.space.zeros()
+        self._grad_PBb2 = self._E1T.codomain.zeros()
+
+        self._u_new = self._u.space.zeros()
+
+        self._u_avg1 = self._u.space.zeros()
+        self._u_avg2 = self._EuT.codomain.zeros()
 
     @property
     def variables(self):
         return [self._u]
 
     def __call__(self, dt):
 
         un = self.variables[0]
 
-        # sum up total magnetic field
-        b_full = self._b_eq.copy()
+        # sum up total magnetic field b_full1 = b_eq + b_tilde (in-place)
+        self._b_eq.copy(out=self._b_full1)
+
         if self._b is not None:
-            b_full += self._b
+            self._b_full1 += self._b
+
+        # extract coefficients to tensor product space (in-place)
+        self._EbT.dot(self._b_full1, out=self._b_full2)
 
-        b_full.update_ghost_regions()
+        # update ghost regions because of non-local access in accumulation kernel!
+        self._b_full2.update_ghost_regions()
 
-        self._PBb = self._PB.dot(b_full)
+        self._PBb = self._PB.dot(self._b_full1)
         self._PBb.update_ghost_regions()
 
-        self._grad_PBb = self.derham.grad.dot(self._PBb)
-        self._grad_PBb.update_ghost_regions()
+        self._grad_PBb1 = self.derham.grad.dot(self._PBb)
+
+        # extract coefficients to tensor product space (in-place)
+        self._E1T.dot(self._grad_PBb1, out=self._grad_PBb2)
+
+        self._grad_PBb2.update_ghost_regions()
 
         # acuumulate MAT and VEC
-        self._ACC.accumulate(self._particles,
-                             self._kappa,
-                             b_full[0]._data, b_full[1]._data, b_full[2]._data,
+        self._ACC.accumulate(self._particles, self._kappa,
+                             self._b_full2[0]._data, self._b_full2[1]._data, self._b_full2[2]._data,
                              self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                              self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
                              self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                             self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
+                             self._grad_PBb2[0]._data, self._grad_PBb2[1]._data, self._grad_PBb2[2]._data,
                              self._space_key_int, self._coupling_mat, self._coupling_vec)
 
         # solve linear system for updated u coefficients
-        u_new, info = self._schur_solver(un, -self._ACC.vectors[0]/2., dt)
+        info = self._schur_solver(
+            un, -self._ACC.vectors[0]/2, dt, out=self._u_new)[1]
+
+        # call pusher kernel with average field (u_new + u_old)/2 and update ghost regions because of non-local access in kernel
+        un.copy(out=self._u_avg1)
+        self._u_avg1 += self._u_new
+        self._u_avg1 /= 2
 
-        # calculate average u
-        u_avg = (un + u_new)/2
-        u_avg.update_ghost_regions()
+        self._EuT.dot(self._u_avg1, out=self._u_avg2)
+
+        self._u_avg2.update_ghost_regions()
 
         self._pusher(self._particles, dt,
                      self._kappa,
-                     b_full[0]._data, b_full[1]._data, b_full[2]._data,
+                     self._b_full2[0]._data, self._b_full2[1]._data, self._b_full2[2]._data,
                      self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                      self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
                      self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                     u_avg[0]._data, u_avg[1]._data, u_avg[2]._data,
+                     self._u_avg2[0]._data, self._u_avg2[1]._data, self._u_avg2[2]._data,
                      self._butcher.a, self._butcher.b, self._butcher.c)
 
-        self._particles.save_magnetic_energy(self.derham, self._PBb)
-
         # write new coeffs into Propagator.variables
-        max_du, = self.in_place_update(u_new)
+        max_du, = self.in_place_update(self._u_new)
 
         if self._info and self._rank == 0:
             print('Status     for CurrentCoupling5DCurrent2:', info['success'])
             print('Iterations for CurrentCoupling5DCurrent2:', info['niter'])
             print('Maxdiff u1 for CurrentCoupling5DCurrent2:', max_du)
             print()
 
@@ -1041,83 +1224,77 @@
         self._particles = particles
 
         # pointers to variables
         assert isinstance(u, (BlockVector, PolarVector))
         self._u = u
 
         # parameters
-        params_default = {'b': None,
-                          'u_space': 'Hdiv',
+        params_default = {'u_space': 'Hdiv',
+                          'b': None,
                           'b_eq': None,
                           'unit_b1': None,
                           'unit_b2': None,
                           'abs_b': None,
-                          'f0': Maxwellian6DUniform(),
+                          'f0': Maxwellian5DUniform(),
                           'type': 'PConjugateGradient',
                           'pc': 'MassMatrixPreconditioner',
                           'tol': 1e-8,
                           'maxiter': 3000,
                           'info': False,
                           'verbose': False,
                           'Ab': 1,
                           'Ah': 1,
-                          'kappa': 100.,
+                          'kappa': 1.,
                           'integrator': 'explicit',
                           'method': 'rk4'}
 
         params = set_defaults(params, params_default)
 
         assert params['u_space'] in {'Hcurl', 'Hdiv', 'H1vec'}
         if params['u_space'] == 'H1vec':
             self._space_key_int = 0
         else:
             self._space_key_int = int(
                 self.derham.spaces_dict[params['u_space']])
 
         self._kappa = params['kappa']
         self._f0 = params['f0']
+
         assert isinstance(params['b'], (BlockVector, PolarVector))
         self._b = params['b']
+
         assert isinstance(params['b_eq'], (BlockVector, PolarVector))
         self._b_eq = params['b_eq']
+
         assert isinstance(params['unit_b1'], (BlockVector, PolarVector))
         self._unit_b1 = params['unit_b1']
+
         assert isinstance(params['unit_b2'], (BlockVector, PolarVector))
         self._unit_b2 = params['unit_b2']
+
         self._abs_b = params['abs_b']
 
         self._curl_norm_b = self.derham.curl.dot(self._unit_b1)
         self._curl_norm_b.update_ghost_regions()
 
         self._type = params['type']
         self._pc = params['pc']
         self._tol = params['tol']
         self._maxiter = params['maxiter']
         self._info = params['info']
         self._verbose = params['verbose']
         self._rank = self.derham.comm.Get_rank()
 
-        self._coupling_mat = params['Ah'] / params['Ab'] * params['kappa']**2
-        self._coupling_vec = params['Ah'] / params['Ab'] * params['kappa']
-        self._scale_push = 1*params['kappa']
+        self._coupling_mat = params['Ah'] / params['Ab']
+        self._coupling_vec = params['Ah'] / params['Ab']
+        self._scale_push = 1
 
         u_id = self.derham.spaces_dict[params['u_space']]
 
-        # sum up total magnetic field
-        b_full = self._b_eq.copy()
-        if self._b is not None:
-            b_full += self._b
-
-        b_full.update_ghost_regions()
-
         self._PB = getattr(self.basis_ops, 'PB')
-        self._PBb = self._PB.dot(b_full)
-        self._PBb.update_ghost_regions()
-        self._grad_PBb = self.derham.grad.dot(self._PBb)
-        self._grad_PBb.update_ghost_regions()
 
         self._A = getattr(self.mass_ops, 'M' + u_id + 'n')
 
         # preconditioner
         if params['pc'] is None:
             self._pc = None
         else:
@@ -1143,52 +1320,62 @@
         self._rhs1 = u.space.zeros()
         self._rhs2 = u.space.zeros()
         self._u_old = u.space.zeros()
         self._u_temp = u.space.zeros()
         self._u_pusher = u.space.zeros()
         self._u_diff = u.space.zeros()
         self._u_new = u.space.zeros()
+        self._b_full = self._b_eq.space.zeros()
+        self._PBb = self._abs_b.space.zeros()
+        self._grad_PBb = self._unit_b1.space.zeros()
+        self._en_fB_old = np.empty(1, dtype=float)
+        self._en_fB_loc = np.empty(1, dtype=float)
+        self._sum_H_diff_loc = np.empty(1, dtype=float)
+        self._u_norm_loc = np.empty(1, dtype=float)
+        self._denominator = np.empty(1, dtype=float)
+        self._accum_gradI_const_loc = np.empty(1, dtype=float)
+        self._gradI_const = np.empty(1, dtype=float)
 
     @property
     def variables(self):
         return [self._u]
 
     def __call__(self, dt):
 
         # save old u
         self.variables[0].copy(out=self._u_old)
 
+        self._u_old.update_ghost_regions()
+
         # sum up total magnetic field
-        b_full = self._b_eq.copy()
         if self._b is not None:
-            b_full += self._b
+            self._b_full += self._b
 
-        b_full.update_ghost_regions()
+        self._b_full.update_ghost_regions()
 
-        self._PBb = self._PB.dot(b_full)
-        self._PBb.update_ghost_regions()
+        self._PBb = self._PB.dot(self._b_full)
 
         self._grad_PBb = self.derham.grad.dot(self._PBb)
         self._grad_PBb.update_ghost_regions()
 
         # reorganize particles
         self._particles.mpi_sort_markers()
 
         #####################################
-        #discrete gradient solver(mid point)#
+        # discrete gradient solver(mid point)#
         #####################################
         # eval initial particle energy
         self._particles.save_magnetic_energy(self.derham, self._PBb)
-        en_fB_old = self._particles.markers[~self._particles.holes, 6].dot(
-            self._particles.markers[~self._particles.holes, 5])/self._particles.n_mks*self._coupling_vec
+        self._en_fB_old = self._particles.markers[~self._particles.holes, 5].dot(
+            self._particles.markers[~self._particles.holes, 8])/self._particles.n_mks
 
         # ------------ initial guess of u ------------#
         # accumulate S*gradI
         self._ACC_prepare.accumulate(self._particles, self._kappa,
-                                     b_full[0]._data, b_full[1]._data, b_full[2]._data,
+                                     self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
                                      self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                                      self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
                                      self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                                      self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
                                      self._space_key_int, self._coupling_vec)
 
         # print('maximum accum result', np.max(np.unique(self._ACC_prepare.vectors[0].toarray_local())))
@@ -1210,67 +1397,70 @@
         # save old etas in columns 9-11
         self._particles.markers[~self._particles.holes,
                                 9:12] = self._particles.markers[~self._particles.holes, 0:3]
 
         # initial guess of eta is stored in columns 0:3
         self._pusher._pusher(self._particles.markers, dt, 0, *self._pusher._args_fem, *self.domain.args_map,
                              self._kappa,
-                             b_full[0]._data, b_full[1]._data, b_full[2]._data,
+                             self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
                              self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                              self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
                              self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                              self._u_old[0]._data, self._u_old[1]._data, self._u_old[2]._data)
 
         self._particles.mpi_sort_markers()
 
         # print('H initial guess', np.max(self._particles.markers[~self._particles.holes,0:3]))
 
         # ------------ fixed point iteration ------------#
-        for stage in range(10):
+        for stage in range(20):
+
+            print(self._particles.markers[~self._particles.holes, 0:8])
 
             self._u_new.copy(out=self._u_temp)
 
             # save eta diff at markers[ip, 15:18]
             utilities.check_eta_diff(self._particles.markers)
             # self._particles.markers[~self._particles.holes, 15:18] = self._particles.markers[~self._particles.holes, 0:3] - self._particles.markers[~self._particles.holes, 9:12]
 
-            sum_H_diff_loc = np.sum(
+            self._sum_H_diff_loc = np.sum(
                 self._particles.markers[~self._particles.holes, 15:18]**2)
-            u_norm_loc = np.sum(
+            self._u_norm_loc = np.sum(
                 (self._u_new.toarray_local() - self._u_old.toarray_local())**2)
-            denominator = sum_H_diff_loc + u_norm_loc
+            self._denominator = self._sum_H_diff_loc + self._u_norm_loc
 
             # eval particle magnetic energy
             self._particles.save_magnetic_energy(self.derham, self._PBb)
-            en_fB_loc = self._particles.markers[~self._particles.holes, 6].dot(
-                self._particles.markers[~self._particles.holes, 5])/self._particles.n_mks*self._coupling_vec
+            self._en_fB_loc = self._particles.markers[~self._particles.holes, 5].dot(
+                self._particles.markers[~self._particles.holes, 8])/self._particles.n_mks
 
             # move particle to the mid point position and then the real position is saved at markers[ip, 12:15]
             utilities.check_eta_mid(self._particles.markers)
             self._particles.markers[~self._particles.holes, 0:3], self._particles.markers[~self._particles.holes,
                                                                                           12:15] = self._particles.markers[~self._particles.holes, 12:15].copy(), self._particles.markers[~self._particles.holes, 0:3].copy()
             self._particles.mpi_sort_markers()
 
             # Accumulate
-            accum_gradI_const_loc = utilities.accum_gradI_const(self._particles.markers, self._particles.n_mks, *self._pusher._args_fem,
-                                                                self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
-                                                                self._coupling_vec)[0]
+            self._accum_gradI_const_loc = utilities.accum_gradI_const(self._particles.markers, self._particles.n_mks, *self._pusher._args_fem,
+                                                                      self._grad_PBb[0]._data, self._grad_PBb[
+                                                                          1]._data, self._grad_PBb[2]._data,
+                                                                      self._coupling_vec)[0]
 
             # gradI_const = (en_u - en_u_old - u_diff.dot(self._A.dot(u_mid)) + np.sum(en_fB) - np.sum(en_fB_old) - np.sum(accum_gradI_const))/denominator
-            gradI_const = (en_fB_loc - en_fB_old -
-                           accum_gradI_const_loc)/denominator
+            self._gradI_const = (
+                self._en_fB_loc - self._en_fB_old - self._accum_gradI_const_loc)/self._denominator
 
             # Accumulate
             self._ACC.accumulate(self._particles, self._kappa,
-                                 b_full[0]._data, b_full[1]._data, b_full[2]._data,
+                                 self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
                                  self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                                  self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
                                  self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                                  self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data,
-                                 gradI_const,
+                                 self._gradI_const,
                                  self._space_key_int, self._coupling_vec)
 
             # update u
             # solve linear system A*u^k_n+1 = A*u_n + ACC.vector
             self._A.dot(self._u_old, out=self._rhs1)
             self._rhs1 += dt*self._ACC.vectors[0]
 
@@ -1293,51 +1483,50 @@
             # calculate average u
             self._u_old.copy(out=self._u_pusher)
             self._u_pusher += self._u_temp
             self._u_pusher /= 2
 
             self._u_temp.copy(out=self._u_diff)
             self._u_diff -= self._u_old
-            self._u_diff *= gradI_const
+            self._u_diff *= self._gradI_const
 
             self._u_diff.update_ghost_regions()
 
             self._u_pusher += Inverse(self._A, pc=self._pc,
                                       tol=1e-18).dot(self._u_diff)
 
             self._u_pusher.update_ghost_regions()
 
             self._pusher._pusher(self._particles.markers, dt, 0, *self._pusher._args_fem, *self.domain.args_map,
                                  self._kappa,
-                                 b_full[0]._data, b_full[1]._data, b_full[2]._data,
+                                 self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
                                  self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
                                  self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
                                  self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
                                  self._u_pusher[0]._data, self._u_pusher[1]._data, self._u_pusher[2]._data)
 
             self._particles.mpi_sort_markers()
 
             print('stage', stage+1)
 
-            u_norm_loc = np.sum(
+            self._u_norm_loc = np.sum(
                 (self._u_new.toarray_local() - self._u_temp.toarray_local())**2)
-            print('u differences',  np.sqrt(u_norm_loc))
+            print('u differences',  np.sqrt(self._u_norm_loc))
 
-            sum_H_diff_loc = np.sum(
+            self._sum_H_diff_loc = np.sum(
                 (self._particles.markers[~self._particles.holes, 0:3] - self._particles.markers[~self._particles.holes, 12:15])**2)
-            print('H differences', np.sqrt(sum_H_diff_loc))
+            print('H differences', np.sqrt(self._sum_H_diff_loc))
 
-            diff = np.sqrt(u_norm_loc + sum_H_diff_loc)
+            diff = np.sqrt(self._u_norm_loc + self._sum_H_diff_loc)
             print('diff', diff)
+
             if diff < 1e-15:
                 print('converged!')
                 break
 
-        self._particles.save_magnetic_energy(self.derham, self._PBb)
-
         # write new coeffs into Propagator.variables
         max_du, = self.in_place_update(self._u_new)
 
         if self._info and self._rank == 0:
             print('Status     for StepPressurecoupling:', info['success'])
             print('Iterations for StepPressurecoupling:', info['niter'])
             print('Maxdiff u1 for StepPressurecoupling:', max_du)
```

### Comparing `struphy-1.9.9/src/struphy/propagators/propagators_fields.py` & `struphy-2.0.0/src/struphy/propagators/propagators_fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import numpy as np
 from numpy import zeros
 
 from struphy.propagators.base import Propagator
 from struphy.linear_algebra.schur_solver import SchurSolver
 from struphy.pic.particles_to_grid import Accumulator
 from struphy.polar.basic import PolarVector
-from struphy.kinetic_background.analytical import Maxwellian, Maxwellian6DUniform
+from struphy.kinetic_background.analytical import Maxwellian, Maxwellian6DUniform, Maxwellian5DUniform
 from struphy.fields_background.mhd_equil.equils import set_defaults
 
 from struphy.psydac_api.linear_operators import CompositeLinearOperator as Compose
 from struphy.psydac_api.linear_operators import SumLinearOperator as Sum
 from struphy.psydac_api.linear_operators import ScalarTimesLinearOperator as Multiply
 from struphy.psydac_api.linear_operators import InverseLinearOperator as Inverse
 from struphy.psydac_api import preconditioner
 from struphy.psydac_api.mass import WeightedMassOperator
 import struphy.linear_algebra.iterative_solvers as it_solvers
 from psydac.linalg.iterative_solvers import pcg
 
-from psydac.api.settings import PSYDAC_BACKEND_GPYCCEL
 from psydac.linalg.stencil import StencilVector
 from psydac.linalg.block import BlockVector
 import struphy.psydac_api.utilities as util
 
 
 class Maxwell(Propagator):
     r'''Crank-Nicolson step
@@ -355,14 +354,218 @@
             print('Status     for ShearAlfvén:', info['success'])
             print('Iterations for ShearAlfvén:', info['niter'])
             print('Maxdiff up for ShearAlfvén:', max_du)
             print('Maxdiff b2 for ShearAlfvén:', max_db)
             print()
 
 
+class ShearAlfvénB1(Propagator):
+    r'''Crank-Nicolson step for shear Alfvén part in Extended MHD equations,
+
+    .. math::
+
+        \begin{bmatrix} \mathbf u^{n+1} - \mathbf u^n \\ \mathbf b^{n+1} - \mathbf b^n \end{bmatrix} 
+        = \frac{\Delta t}{2} \begin{bmatrix} 0 & (\mathbb M^\rho_2)^{-1} \mathcal {T^2}^\top \mathbb C \mathbb M_1^{-1}\\ - \mathbb M_1^{-1} \mathbb C^\top \mathcal {T^2} (\mathbb M^\rho_2)^{-1} & 0 \end{bmatrix} 
+        \begin{bmatrix} {\mathbb M^\rho_2}(\mathbf u^{n+1} + \mathbf u^n) \\ \mathbb M_1(\mathbf b^{n+1} + \mathbf b^n) \end{bmatrix} ,
+
+    where :math:`\mathbb M^\rho_2` is a weighted mass matrix in 2-space, the weight being :math:`\rho_0`,
+    the MHD equilibirum density. The solution of the above system is based on the :ref:`Schur complement <schur_solver>`.
+
+    Parameters
+    ---------- 
+    u : psydac.linalg.block.BlockVector
+        FE coefficients of MHD velocity as 2-form.
+
+    b : psydac.linalg.block.BlockVector
+        FE coefficients of magnetic field as 1-form.
+
+        **params : dict
+            Solver- and/or other parameters for this splitting step.
+    '''
+
+    def __init__(self, u, b, **params):
+
+        # pointers to variables
+        assert isinstance(u, (BlockVector, PolarVector))
+        assert isinstance(b, (BlockVector, PolarVector))
+        self._u = u
+        self._b = b
+
+        # parameters
+        params_default = {'type': 'PConjugateGradient',
+                          'pc': 'MassMatrixPreconditioner',
+                          'tol': 1e-8,
+                          'maxiter': 3000,
+                          'info': False,
+                          'verbose': False}
+
+        params = set_defaults(params, params_default)
+
+        self._info = params['info']
+        self._rank = self.derham.comm.Get_rank()
+
+        # define block matrix [[A B], [C I]] (without time step size dt in the diagonals)
+        _A = self.mass_ops.M2n
+        self._M1inv = Inverse(self.mass_ops.M1, tol=1e-8)
+        self._B = Multiply(1/2, Compose(self.mass_ops.M2B,
+                           self.derham.curl))
+        #I still have to invert M1
+        self._C = Multiply(1/2, Compose(self._M1inv,self.derham.curl.T, self.mass_ops.M2B))
+
+        # Preconditioner
+        if params['pc'] is None:
+            pc = None
+        else:
+            pc_class = getattr(preconditioner, params['pc'])
+            pc = pc_class(getattr(self.mass_ops, 'M2n'))
+
+        # instantiate Schur solver (constant in this case)
+        _BC = Compose(self._B, self._C)
+
+        self._schur_solver = SchurSolver(_A, _BC, pc=pc, solver_name=params['type'],
+                                         tol=params['tol'], maxiter=params['maxiter'],
+                                         verbose=params['verbose'])
+
+        # allocate dummy vectors to avoid temporary array allocations
+        self._u_tmp1 = u.space.zeros()
+        self._u_tmp2 = u.space.zeros()
+        self._b_tmp1 = b.space.zeros()
+
+        self._byn = self._B.codomain.zeros()
+
+    @property
+    def variables(self):
+        return [self._u, self._b]
+
+    def __call__(self, dt):
+
+        # current variables
+        un = self.variables[0]
+        bn = self.variables[1]
+
+        # solve for new u coeffs
+        self._B.dot(bn, out=self._byn)
+
+        info = self._schur_solver(un, self._byn, dt, out=self._u_tmp1)[1]
+
+        # new b coeffs
+        un.copy(out=self._u_tmp2)
+        self._u_tmp2 += self._u_tmp1
+        self._C.dot(self._u_tmp2, out=self._b_tmp1)
+        self._b_tmp1 *= -dt
+        self._b_tmp1 += bn
+
+        # write new coeffs into self.variables
+        max_du, max_db = self.in_place_update(self._u_tmp1, self._b_tmp1)
+
+        if self._info and self._rank == 0:
+            print('Status     for ShearAlfvénB1:', info['success'])
+            print('Iterations for ShearAlfvénB1:', info['niter'])
+            print('Maxdiff up for ShearAlfvénB1:', max_du)
+            print('Maxdiff b2 for ShearAlfvénB1:', max_db)
+            print()
+
+
+class Hall(Propagator):
+    r'''Crank-Nicolson step for Hall part in Extended MHD equations,
+
+    .. math::
+
+        \mathbf b^{n+1} - \mathbf b^n 
+        = \frac{\Delta t}{2} \mathbb M_1^{-1} \mathbb C^\top  \mathbb M^{\mathcal{T},\rho}_2  \mathbb C  (\mathbf b^{n+1} + \mathbf b^n)  ,
+
+    where :math:`\mathbb M^{\mathcal{T},\rho}_2` is a weighted mass matrix in 2-space, the weight being :math:`\frac{\mathcal{T}}{\rho_0}`,
+    the MHD equilibirum density :math:`\rho_0` as a 0-form, and rotation matrix :math:`\mathcal{T} \vec v = \vec B^2_{\textnormal{eq}} \times \vec v\,,`. 
+    The solution of the above system is based on the Pre-conditioned Biconjugate Gradient Stabilized algortihm (PBiConjugateGradientStab).
+
+    Parameters
+    ---------- 
+    b : psydac.linalg.block.BlockVector
+        FE coefficients of magnetic field as 1-form.
+
+        **params : dict
+            Solver- and/or other parameters for this splitting step.
+    '''
+
+    def __init__(self, b, **params):
+
+        # pointers to variables
+        assert isinstance(b, (BlockVector, PolarVector))
+        self._b = b
+
+        # parameters
+        params_default = {'type': 'PBiConjugateGradientStab',
+                          'pc': 'MassMatrixPreconditioner',
+                          'tol': 1e-8,
+                          'maxiter': 3000,
+                          'info': False,
+                          'verbose': False,
+                          'kappa': 1.0}
+
+        params = set_defaults(params, params_default)
+
+        self._info = params['info']
+        self._rank = self.derham.comm.Get_rank()
+        self._tol = params['tol']
+        self._maxiter = params['maxiter']
+        self._verbose = params['verbose']
+        self._kappa = params['kappa']
+
+        # mass matrix in system (M - dt/2 * A)*b^(n + 1) = (M + dt/2 * A)*b^n
+        id_M = 'M1'
+        id_M2Bn = 'M2Bn'
+        self._M = getattr(self.mass_ops, id_M)
+        self._M2Bn = getattr(self.mass_ops, id_M2Bn)
+        self._A = Multiply(self._kappa, Compose(self.derham.curl.T,self._M2Bn,self.derham.curl))
+
+        # Preconditioner
+        if params['pc'] is None:
+            self._pc = None
+        else:
+            pc_class = getattr(preconditioner, params['pc'])
+            self._pc = pc_class(getattr(self.mass_ops, id_M))
+            
+        # Instantiate linear solver
+        self._solver = getattr(it_solvers, params['type'])(self._M.domain)
+
+        # allocate dummy vectors to avoid temporary array allocations
+        self._rhs_b = self._M.codomain.zeros()
+        self._b_new = b.space.zeros()
+
+    @property
+    def variables(self):
+        return [self._b]
+
+    def __call__(self, dt):
+
+        # current variables
+        bn = self.variables[0]
+
+        # define system (M - dt/2 * A)*b^(n + 1) = (M + dt/2 * A)*b^n
+        lhs = Sum(self._M, Multiply(-dt/2.0, self._A))
+        rhs = Sum(self._M, Multiply(dt/2.0, self._A))
+
+        # solve linear system for updated u coefficients (in-place)
+        rhs.dot(bn, out=self._rhs_b)
+
+        info = self._solver.solve(lhs, self._rhs_b, self._pc,
+                                  x0=bn, tol=self._tol,
+                                  maxiter=self._maxiter, verbose=self._verbose,
+                                  out=self._b_new)[1]
+
+        # write new coeffs into self.variables
+        max_db = self.in_place_update(self._b_new)
+
+        if self._info and self._rank == 0:
+            print('Status     for Hall:', info['success'])
+            print('Iterations for Hall:', info['niter'])
+            print('Maxdiff b1 for Hall:', max_db)
+            print()
+
+
 class Magnetosonic(Propagator):
     r'''Crank-Nicolson step for magnetosonic part in MHD equations:
 
     .. math::
 
         \begin{bmatrix} \mathbf u^{n+1} - \mathbf u^n \\ \mathbf p^{n+1} - \mathbf p^n \end{bmatrix} 
         = \frac{\Delta t}{2} \begin{bmatrix} 0 & (\mathbb M^\rho_\alpha)^{-1} {\mathcal U^\alpha}^\top \mathbb D^\top \mathbb M_3 \\ - \mathbb D \mathcal S^\alpha - (\gamma - 1) \mathcal K^\alpha \mathbb D \mathcal U^\alpha & 0 \end{bmatrix} 
@@ -518,14 +721,290 @@
             print('Iterations for Magnetosonic:', info['niter'])
             print('Maxdiff n3 for Magnetosonic:', max_dn)
             print('Maxdiff up for Magnetosonic:', max_du)
             print('Maxdiff p3 for Magnetosonic:', max_dp)
             print()
 
 
+class SonicIon(Propagator):
+    r'''Crank-Nicolson step for Ion sonic part in Extended MHD equations:
+
+    .. math::
+
+        \begin{bmatrix} \mathbf u^{n+1} - \mathbf u^n \\ \mathbf p^{n+1}_i - \mathbf p^n_i \end{bmatrix} 
+        = \frac{\Delta t}{2} \begin{bmatrix} 0 & (\mathbb M^\rho_2)^{-1} \mathbb D^\top \mathbb M_3 \\ - \gamma \mathcal K^3 \mathbb D & 0 \end{bmatrix} 
+        \begin{bmatrix} (\mathbf u^{n+1} + \mathbf u^n) \\ (\mathbf p^{n+1}_i + \mathbf p^n_i) \end{bmatrix} ,
+
+    where :math:`\mathbb M^\rho_2`  is a weighted mass matrix in 2-space, 
+    the weight being the MHD equilibirum density :math:`\rho_0`. Furthermore, :math:`\mathcal K^3` is the basis projection operator given by :
+    
+    .. math::
+
+        \mathcal{K}^3_{ijk,mno} := \hat{\Pi}^3_{ijk} \left[ \frac{\hat{p}^3_{\text{eq}}}{\sqrt{g}}\Lambda^3_{mno} \right] \,.
+    The solution of the above system is based on the :ref:`Schur complement <schur_solver>`.
+
+    Decoupled density update:
+
+    .. math::
+
+        \boldsymbol{\rho}^{n+1} = \boldsymbol{\rho}^n - \frac{\Delta t}{2} \mathcal Q \mathbb D  (\mathbf u^{n+1} + \mathbf u^n) \,.
+
+    Parameters
+    ---------- 
+    n : psydac.linalg.stencil.StencilVector
+        FE coefficients of a discrete 3-form.
+
+    u : psydac.linalg.block.BlockVector
+        FE coefficients of MHD velocity 2-form.
+
+    p : psydac.linalg.stencil.StencilVector
+        FE coefficients of a discrete 3-form.
+
+        **params : dict
+            Solver- and/or other parameters for this splitting step.
+    '''
+
+    def __init__(self, n, u, p, **params):
+
+        # pointers to variables
+        assert isinstance(n, (StencilVector, PolarVector))
+        assert isinstance(u, (BlockVector, PolarVector))
+        assert isinstance(p, (StencilVector, PolarVector))
+        self._n = n
+        self._u = u
+        self._p = p
+
+        # parameters
+        params_default = {'type': 'PBiConjugateGradientStab',
+                          'pc': 'MassMatrixPreconditioner',
+                          'tol': 1e-8,
+                          'maxiter': 3000,
+                          'info': False,
+                          'verbose': False}
+
+        params = set_defaults(params, params_default)
+
+        self._info = params['info']
+        self._bc = self.derham.bc
+        self._rank = self.derham.comm.Get_rank()
+
+        # define block matrix [[A B], [C I]] (without time step size dt in the diagonals)
+        id_Mn = 'M2n' 
+        id_K, id_Q = 'K3', 'Q3'
+        
+        _A = getattr(self.mass_ops, id_Mn)
+        _K = getattr(self.basis_ops, id_K)
+
+        self._B = Multiply(-1/2., Compose(self.derham.div.T, self.mass_ops.M3))
+        self._C = Multiply(5/6., Compose(_K, self.derham.div))
+
+        self._QD = Compose(getattr(self.basis_ops, id_Q) ,self.derham.div)
+
+        # preconditioner
+        if params['pc'] is None:
+            pc = None
+        else:
+            pc_class = getattr(preconditioner, params['pc'])
+            pc = pc_class(getattr(self.mass_ops, id_Mn))
+
+        # instantiate Schur solver (constant in this case)
+        _BC = Compose(self._B, self._C)
+
+        self._schur_solver = SchurSolver(_A, _BC, pc=pc, solver_name=params['type'],
+                                         tol=params['tol'], maxiter=params['maxiter'],
+                                         verbose=params['verbose'])
+
+        # allocate dummy vectors to avoid temporary array allocations
+        self._u_tmp1 = u.space.zeros()
+        self._u_tmp2 = u.space.zeros()
+        self._p_tmp1 = p.space.zeros()
+        self._n_tmp1 = n.space.zeros()
+
+        self._byn1 = self._B.codomain.zeros()
+
+    @property
+    def variables(self):
+        return [self._n, self._u, self._p]
+
+    def __call__(self, dt):
+
+        # current variables
+        nn = self.variables[0]
+        un = self.variables[1]
+        pn = self.variables[2]
+
+        # solve for new u coeffs
+        self._B.dot(pn, out=self._byn1)
+
+        info = self._schur_solver(un, self._byn1, dt, out=self._u_tmp1)[1]
+
+        # new p, n, b coeffs
+        un.copy(out=self._u_tmp2)
+        self._u_tmp2 += self._u_tmp1
+        self._C.dot(self._u_tmp2, out=self._p_tmp1)
+        self._p_tmp1 *= -dt
+        self._p_tmp1 += pn
+
+        self._QD.dot(self._u_tmp2, out=self._n_tmp1)
+        self._n_tmp1 *= -dt/2.0
+        self._n_tmp1 += nn
+
+        # write new coeffs into self.variables
+        max_dn, max_du, max_dp = self.in_place_update(self._n_tmp1,
+                                                      self._u_tmp1,
+                                                      self._p_tmp1)
+
+        if self._info and self._rank == 0:
+            print('Status     for Magnetosonic:', info['success'])
+            print('Iterations for Magnetosonic:', info['niter'])
+            print('Maxdiff n3 for Magnetosonic:', max_dn)
+            print('Maxdiff up for Magnetosonic:', max_du)
+            print('Maxdiff p3 for Magnetosonic:', max_dp)
+            print()
+
+
+class SonicElectron(Propagator):
+    r'''Crank-Nicolson step for Electron sonic part in Extended MHD equations:
+
+    .. math::
+
+        \begin{bmatrix} \mathbf u^{n+1} - \mathbf u^n \\ \mathbf p^{n+1}_i - \mathbf p^n_i \end{bmatrix} 
+        = \frac{\Delta t}{2} \begin{bmatrix} 0 & (\mathbb M^\rho_2)^{-1} \mathbb D^\top \mathbb M_3 \\ - \gamma \mathcal K^3 \mathbb D & 0 \end{bmatrix} 
+        \begin{bmatrix} (\mathbf u^{n+1} + \mathbf u^n) \\ (\mathbf p^{n+1}_i + \mathbf p^n_i) \end{bmatrix} ,
+
+    where :math:`\mathbb M^\rho_2`  is a weighted mass matrix in 2-space, 
+    the weight being the MHD equilibirum density :math:`\rho_0`. Furthermore, :math:`\mathcal K^3` is the basis projection operator given by :
+    
+    .. math::
+
+        \mathcal{K}^3_{ijk,mno} := \hat{\Pi}^3_{ijk} \left[ \frac{\hat{p}^3_{\text{eq}}}{\sqrt{g}}\Lambda^3_{mno} \right] \,.
+    The solution of the above system is based on the :ref:`Schur complement <schur_solver>`.
+
+    Decoupled density update:
+
+    .. math::
+
+        \boldsymbol{\rho}^{n+1} = \boldsymbol{\rho}^n - \frac{\Delta t}{2} \mathcal Q \mathbb D  (\mathbf u^{n+1} + \mathbf u^n) \,.
+
+    Parameters
+    ---------- 
+    n : psydac.linalg.stencil.StencilVector
+        FE coefficients of a discrete 3-form.
+
+    u : psydac.linalg.block.BlockVector
+        FE coefficients of MHD velocity 2-form.
+
+    p : psydac.linalg.stencil.StencilVector
+        FE coefficients of a discrete 3-form.
+
+        **params : dict
+            Solver- and/or other parameters for this splitting step.
+    '''
+
+    def __init__(self, n, u, p, **params):
+
+        # pointers to variables
+        assert isinstance(n, (StencilVector, PolarVector))
+        assert isinstance(u, (BlockVector, PolarVector))
+        assert isinstance(p, (StencilVector, PolarVector))
+        self._n = n
+        self._u = u
+        self._p = p
+
+        # parameters
+        params_default = {'type': 'PBiConjugateGradientStab',
+                          'pc': 'MassMatrixPreconditioner',
+                          'tol': 1e-8,
+                          'maxiter': 3000,
+                          'info': False,
+                          'verbose': False}
+
+        params = set_defaults(params, params_default)
+
+        self._info = params['info']
+        self._bc = self.derham.bc
+        self._rank = self.derham.comm.Get_rank()
+
+        # define block matrix [[A B], [C I]] (without time step size dt in the diagonals)
+        id_Mn = 'M2n' 
+        # ONCE THE CODE SUPPORTS HAVING A DIFFERENT EQUILIBRIUM ELECTRON PRESSURE TO THE EQUILIBRIUM ION PRESSURE; WE MUST ADD A NEW PROJECTION MATRIX Ke3 THAT TAKES THE EQUILIBRIUM ELECTRON PRESSURE
+        #INSTEAD OF THE EQUILIBRIUM ION PRESSURE: AND USE HERE Ke3, NOT K3.
+        id_K, id_Q = 'K3', 'Q3'
+        
+        _A = getattr(self.mass_ops, id_Mn)
+        _K = getattr(self.basis_ops, id_K)
+
+        self._B = Multiply(-1/2., Compose(self.derham.div.T, self.mass_ops.M3))
+        self._C = Multiply(5/6., Compose(_K, self.derham.div))
+
+        self._QD = Compose(getattr(self.basis_ops, id_Q) ,self.derham.div)
+
+        # preconditioner
+        if params['pc'] is None:
+            pc = None
+        else:
+            pc_class = getattr(preconditioner, params['pc'])
+            pc = pc_class(getattr(self.mass_ops, id_Mn))
+
+        # instantiate Schur solver (constant in this case)
+        _BC = Compose(self._B, self._C)
+
+        self._schur_solver = SchurSolver(_A, _BC, pc=pc, solver_name=params['type'],
+                                         tol=params['tol'], maxiter=params['maxiter'],
+                                         verbose=params['verbose'])
+
+        # allocate dummy vectors to avoid temporary array allocations
+        self._u_tmp1 = u.space.zeros()
+        self._u_tmp2 = u.space.zeros()
+        self._p_tmp1 = p.space.zeros()
+        self._n_tmp1 = n.space.zeros()
+
+        self._byn1 = self._B.codomain.zeros()
+
+    @property
+    def variables(self):
+        return [self._n, self._u, self._p]
+
+    def __call__(self, dt):
+
+        # current variables
+        nn = self.variables[0]
+        un = self.variables[1]
+        pn = self.variables[2]
+
+        # solve for new u coeffs
+        self._B.dot(pn, out=self._byn1)
+
+        info = self._schur_solver(un, self._byn1, dt, out=self._u_tmp1)[1]
+
+        # new p, n, b coeffs
+        un.copy(out=self._u_tmp2)
+        self._u_tmp2 += self._u_tmp1
+        self._C.dot(self._u_tmp2, out=self._p_tmp1)
+        self._p_tmp1 *= -dt
+        self._p_tmp1 += pn
+
+        self._QD.dot(self._u_tmp2, out=self._n_tmp1)
+        self._n_tmp1 *= -dt/2.0
+        self._n_tmp1 += nn
+
+        # write new coeffs into self.variables
+        max_dn, max_du, max_dp = self.in_place_update(self._n_tmp1,
+                                                      self._u_tmp1,
+                                                      self._p_tmp1)
+
+        if self._info and self._rank == 0:
+            print('Status     for Magnetosonic:', info['success'])
+            print('Iterations for Magnetosonic:', info['niter'])
+            print('Maxdiff n3 for Magnetosonic:', max_dn)
+            print('Maxdiff up for Magnetosonic:', max_du)
+            print('Maxdiff p3 for Magnetosonic:', max_dp)
+            print()
+
+
 class FaradayExtended(Propagator):
     r'''Equations: Faraday's law
 
     .. math::
         \begin{align*}
         & \frac{\partial {\mathbf A}}{\partial t} = - \frac{\nabla \times (\nabla \times {\mathbf A} + {\mathbf B}_0) }{n} \times (\nabla \times {\mathbf A} + {\mathbf B}_0) - \frac{\int ({\mathbf A} - {\mathbf p}f \mathrm{d}{\mathbf p})}{n} \times (\nabla \times {\mathbf A} + {\mathbf B}_0), \\
         & n = \int f \mathrm{d}{\mathbf p}.
@@ -642,28 +1121,28 @@
 
         self._L2 = Multiply(-dt/2, Compose(self._Minv,
                             Sum(self._accum_potential._operators[0].matrix, self._CMC)))
         self._RHS = -(self._L2.dot(self._a)) - dt*(self._Minv.dot(
             self._accum_potential._vectors[0] - Compose(self.derham.curl.transpose(), self._M2).dot(self._beq)))
         self._rhs = self._M1.dot(self._a)
 
-        for loop in range(10):
-            #print('+++++=====++++++', self._accum_density._operators[0].matrix._data)
+        for _ in range(10):
+            # print('+++++=====++++++', self._accum_density._operators[0].matrix._data)
             # set mid-value used in the fixed iteration
             curla_mid = self.derham.curl.dot(
                 0.5*(self._a_old + self._a)) + self._beq
             curla_mid.update_ghost_regions()
             # initialize the curl A
             # remember to check ghost region of curla_mid
             util.create_weight_weightedmatrix_hybrid(
                 curla_mid, self._weight_pre, self.derham, self._accum_density, self.domain)
-            #self._weight = [[None, self._weight_pre[2], -self._weight_pre[1]], [None, None, self._weight_pre[0]], [None, None, None]]
+            # self._weight = [[None, self._weight_pre[2], -self._weight_pre[1]], [None, None, self._weight_pre[0]], [None, None, None]]
             self._weight = [[0.0*self._weight_pre[0], 0.0*self._weight_pre[2], 0.0*self._weight_pre[1]], [0.0*self._weight_pre[2], 0.0 *
                                                                                                           self._weight_pre[1], 0.0*self._weight_pre[0]], [0.0*self._weight_pre[1], 0.0*self._weight_pre[0], 0.0*self._weight_pre[2]]]
-            #self._weight = [[self._weight_pre[0], self._weight_pre[2], self._weight_pre[1]], [self._weight_pre[2], self._weight_pre[1], self._weight_pre[0]], [self._weight_pre[1], self._weight_pre[0], self._weight_pre[2]]]
+            # self._weight = [[self._weight_pre[0], self._weight_pre[2], self._weight_pre[1]], [self._weight_pre[2], self._weight_pre[1], self._weight_pre[0]], [self._weight_pre[1], self._weight_pre[0], self._weight_pre[2]]]
             HybridM1 = self.mass_ops.assemble_weighted_mass(
                 self._weight, 'Hcurl', 'Hcurl')
 
             # next prepare for solving linear system
             _LHS = Sum(self._M1, Compose(HybridM1, self._L2))
             _RHS2 = HybridM1.dot(self._RHS) + self._rhs
 
@@ -910,24 +1389,24 @@
         self._u = u
         self._b = b
 
         # parameters
         params_default = {'particles': None,
                           'u_space': 'Hdiv',
                           'b_eq': None,
-                          'f0': Maxwellian6DUniform(),
+                          'f0': Maxwellian5DUniform(),
                           'type': 'PConjugateGradient',
                           'pc': 'MassMatrixPreconditioner',
                           'tol': 1e-8,
                           'maxiter': 3000,
                           'info': False,
                           'verbose': False,
                           'Ab': 1,
                           'Ah': 1,
-                          'kappa': 100}
+                          'kappa': 1.}
 
         params = set_defaults(params, params_default)
 
         assert isinstance(params['particles'], Particles5D)
         self._particles = params['particles']
 
         assert params['u_space'] in {'Hcurl', 'Hdiv', 'H1vec'}
@@ -979,21 +1458,14 @@
         # allocate dummy vectors to avoid temporary array allocations
         self._u_tmp1 = u.space.zeros()
         self._u_tmp2 = u.space.zeros()
         self._b_tmp1 = b.space.zeros()
 
         self._byn = self._B.codomain.zeros()
 
-        # allocate dummy vectors to avoid temporary array allocations
-        self._u_tmp1 = u.space.zeros()
-        self._u_tmp2 = u.space.zeros()
-        self._b_tmp1 = b.space.zeros()
-
-        self._byn = self._B.codomain.zeros()
-
     @property
     def variables(self):
         return [self._u, self._b]
 
     def __call__(self, dt):
 
         # current variables
@@ -1015,17 +1487,14 @@
         self._C.dot(self._u_tmp2, out=self._b_tmp1)
         self._b_tmp1 *= -dt
         self._b_tmp1 += bn
 
         # write new coeffs into self.variables
         max_du, max_db = self.in_place_update(self._u_tmp1, self._b_tmp1)
 
-        self._particles.save_magnetic_energy(
-            self.derham, self._PB.dot(self._b + self._b_eq))
-
         if self._info and self._rank == 0:
             print('Status     for ShearAlfvén:', info['success'])
             print('Iterations for ShearAlfvén:', info['niter'])
             print('Maxdiff up for ShearAlfvén:', max_du)
             print('Maxdiff b2 for ShearAlfvén:', max_db)
             print()
 
@@ -1045,55 +1514,57 @@
         self._p = p
 
         # parameters
         params_default = {'b': self.derham.Vh['2'].zeros(),
                           'particles': None,
                           'u_space': 'Hdiv',
                           'unit_b1': None,
-                          'f0': Maxwellian6DUniform(),
+                          'f0': Maxwellian5DUniform(),
                           'type': 'PBiConjugateGradientStab',
                           'pc': 'MassMatrixPreconditioner',
                           'tol': 1e-8,
                           'maxiter': 3000,
                           'info': False,
                           'verbose': False,
                           'Ab': 1,
                           'Ah': 1,
-                          'kappa': 100}
+                          'kappa': 1}
 
         params = set_defaults(params, params_default)
 
         assert isinstance(params['particles'], Particles5D)
         self._particles = params['particles']
 
         assert params['u_space'] in {'Hcurl', 'Hdiv', 'H1vec'}
         if params['u_space'] == 'H1vec':
             self._space_key_int = 0
         else:
             self._space_key_int = int(
                 self.derham.spaces_dict[params['u_space']])
 
         self._f0 = params['f0']
+
         assert isinstance(params['b'], (BlockVector, PolarVector))
         self._b = params['b']
+
         assert isinstance(params['unit_b1'], (BlockVector, PolarVector))
         self._unit_b1 = params['unit_b1']
 
         assert params['u_space'] in {'Hcurl', 'Hdiv', 'H1vec'}
 
         self._curl_norm_b = self.derham.curl.dot(self._unit_b1)
         self._curl_norm_b.update_ghost_regions()
         self._bc = self.derham.bc
         self._info = params['info']
         self._rank = self.derham.comm.Get_rank()
 
-        self._scale_vec = params['Ah'] / params['Ab']
+        self._coupling_const = params['Ah'] / params['Ab']
 
         self._ACC = Accumulator(self.derham, self.domain,
-                                params['u_space'], 'cc_lin_mhd_5d_M', add_vector=True)
+                                params['u_space'], 'cc_lin_mhd_5d_curlM', add_vector=False)
 
         # define block matrix [[A B], [C I]] (without time step size dt in the diagonals)
         id_Mn = 'M' + self.derham.spaces_dict[params['u_space']] + 'n'
         id_MJ = 'M' + self.derham.spaces_dict[params['u_space']] + 'J'
 
         if params['u_space'] == 'Hcurl':
             id_S, id_U, id_K, id_Q = 'S1', 'U1', 'K3', 'Q1'
@@ -1155,20 +1626,20 @@
         un = self.variables[1]
         pn = self.variables[2]
 
         # accumulate
         self._ACC.accumulate(self._particles,
                              self._b[0]._data, self._b[1]._data, self._b[2]._data,
                              self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
-                             self._space_key_int, self._scale_vec)
+                             self._space_key_int, self._coupling_const)
 
         # solve for new u coeffs
         self._B.dot(pn, out=self._byn1)
         self._MJ.dot(self._b, out=self._byn2)
-        self._byn2 -= self._ACC.vectors[0]
+        self._byn2 -= self._ACC.vectors[0].dot(self._b)
         self._byn2 *= 1/2
         self._byn1 -= self._byn2
 
         info = self._schur_solver(un, self._byn1, dt, out=self._u_tmp1)[1]
 
         # new p, n, b coeffs
         un.copy(out=self._u_tmp2)
```

### Comparing `struphy-1.9.9/src/struphy/propagators/propagators_markers.py` & `struphy-2.0.0/src/struphy/propagators/propagators_markers.py`

 * *Files 6% similar despite different names*

```diff
@@ -347,15 +347,15 @@
         TODO
         """
         # get density from particles
         self._accum_density.accumulate(self._particles, array(self.derham.Nel), array(self._nqs), array(
             self._pts_x), array(self._pts_y), array(self._pts_z), array(self._p_shape), array(self._p_size))
         if not self._accum_density._operators[0].matrix.ghost_regions_in_sync:
             self._accum_density._operators[0].matrix.update_ghost_regions()
-        #print('++++++check_density+++++++++', self._accum_density._operators[0].matrix._data)
+        # print('++++++check_density+++++++++', self._accum_density._operators[0].matrix._data)
         self._pusher_lnn(self._particles, dt, array(self._p_shape), array(self._p_size), array(self.derham.Nel), array(self._pts_x), array(self._pts_y), array(
             self._pts_z), array(self._wts_x), array(self._wts_y), array(self._wts_z), self._accum_density._operators[0].matrix._data, self._thermal, array(self._nqs))
 
         if not self._a[0].ghost_regions_in_sync:
             self._a[0].update_ghost_regions()
         if not self._a[1].ghost_regions_in_sync:
             self._a[1].update_ghost_regions()
@@ -750,26 +750,26 @@
 class StepStaticEfield(Propagator):
     r'''Solve the following system
 
     .. math::
 
         \frac{\text{d} \mathbf{\eta}_p}{\text{d} t} & = DL^{-1} \mathbf{v}_p \,,
 
-        \frac{\text{d} \mathbf{v}_p}{\text{d} t} & = DL^{-T} \mathbf{E}_0
+        \frac{\text{d} \mathbf{v}_p}{\text{d} t} & = \kappa \, DL^{-T} \mathbf{E}
 
     which is solved by an average discrete gradient method, implicitly iterating
     over :math:`k` (for every particle :math:`p`):
 
     .. math::
 
         \mathbf{\eta}^{n+1}_{k+1} = \mathbf{\eta}^n + \frac{\Delta t}{2} DL^{-1}
         \left( \frac{\mathbf{\eta}^{n+1}_k + \mathbf{\eta}^n }{2} \right) \left( \mathbf{v}^{n+1}_k + \mathbf{v}^n \right) \,,
 
-        \mathbf{v}^{n+1}_{k+1} = \mathbf{v}^n + \Delta t DL^{-1}\left(\mathbf{\eta}^n\right)
-        \int_0^1 \left[ \mathbb{\Lambda}\left( \eta^n + \tau (\mathbf{\eta}^{n+1}_k - \mathbf{\eta}^n) \right) \right]^T \mathbf{e}_0 \, \text{d} \tau
+        \mathbf{v}^{n+1}_{k+1} = \mathbf{v}^n + \Delta t \, \kappa \, DL^{-1}\left(\mathbf{\eta}^n\right)
+        \int_0^1 \left[ \mathbb{\Lambda}\left( \eta^n + \tau (\mathbf{\eta}^{n+1}_k - \mathbf{\eta}^n) \right) \right]^T \mathbf{e} \, \text{d} \tau
 
     Parameters
     ----------
     particles : struphy.pic.particles.Particles6D
         Holdes the markers to push.
 
     **params : dict
@@ -781,21 +781,23 @@
         from numpy import polynomial, floor
 
         # pointer to variable
         assert isinstance(particles, Particles6D)
         self._particles = particles
 
         # parameters
-        params_default = {'e_eq': BlockVector(
-            self.derham.Vh_fem['1'].vector_space)}
+        params_default = {'e_field': BlockVector(
+            self.derham.Vh_fem['1'].vector_space),
+            'kappa': 1e2}
 
         params = set_defaults(params, params_default)
+        self.kappa = params['kappa']
 
-        assert isinstance(params['e_eq'], (BlockVector, PolarVector))
-        self._e_eq = params['e_eq']
+        assert isinstance(params['e_field'], (BlockVector, PolarVector))
+        self._e_field = params['e_field']
 
         pn1 = self.derham.p[0]
         pd1 = pn1 - 1
         pn2 = self.derham.p[1]
         pd2 = pn2 - 1
         pn3 = self.derham.p[2]
         pd3 = pn3 - 1
@@ -821,15 +823,16 @@
 
     def __call__(self, dt):
         """
         TODO
         """
         self._pusher(self._particles, dt,
                      self._loc1, self._loc2, self._loc3, self._weight1, self._weight2, self._weight3,
-                     self._e_eq.blocks[0]._data, self._e_eq.blocks[1]._data, self._e_eq.blocks[2]._data,
+                     self._e_field.blocks[0]._data, self._e_field.blocks[1]._data, self._e_field.blocks[2]._data,
+                     self.kappa,
                      array([1e-10, 1e-10]), 100)
 
 
 class StepPushDriftKinetic1(Propagator):
     r"""Solves
 
     .. math::
@@ -863,15 +866,15 @@
     def __init__(self, particles, **params):
 
         # pointer to variable
         assert isinstance(particles, Particles5D)
         self._particles = particles
 
         # parameters
-        params_default = {'kappa': 100.,
+        params_default = {'kappa': 1.,
                           'b': None,
                           'b_eq': None,
                           'unit_b1': None,
                           'unit_b2': None,
                           'abs_b': None,
                           'integrator': 'implicit',
                           'method': 'discrete_gradient_faster',
@@ -898,16 +901,16 @@
         self._b_full = self._b_eq.copy()
         if self._b is not None:
             self._b_full += self._b
 
         self._b_full.update_ghost_regions()
 
         # define gradient of absolute value of parallel magnetic field
-        PB = getattr(self.basis_ops, 'PB')
-        self._PBb = PB.dot(self._b_full)
+        self._PB = getattr(self.basis_ops, 'PB')
+        self._PBb = self._PB.dot(self._b_full)
         self._PBb.update_ghost_regions()
 
         self._grad_PBb = self.derham.grad.dot(self._PBb)
         self._grad_PBb.update_ghost_regions()
 
         if params['integrator'] == 'explicit':
 
@@ -974,19 +977,39 @@
     def variables(self):
         return self._particles
 
     def __call__(self, dt):
         """
         TODO
         """
+
+        # sum up total magnetic field
+        self._b_full = self._b_eq.copy()
+        if self._b is not None:
+            self._b_full += self._b
+
+        self._b_full.update_ghost_regions()
+
+        # define gradient of absolute value of parallel magnetic field
+        self._PBb = self._PB.dot(self._b_full)
+        self._PBb.update_ghost_regions()
+
+        self._grad_PBb = self.derham.grad.dot(self._PBb)
+        self._grad_PBb.update_ghost_regions()
+
+        self._pusher_inputs = (self._kappa, self._PBb._data,
+                               self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
+                               self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
+                               self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
+                               self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
+                               self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data)
+
         self._pusher(self._particles, dt,
                      *self._pusher_inputs, mpi_sort='each', verbose=False)
 
-        self._particles.save_magnetic_energy(self.derham, self._PBb)
-
 
 class StepPushDriftKinetic2(Propagator):
     r"""Solves
 
     .. math::
 
         \dot{\mathbf X} &= \frac{1}{B^*_\parallel} \frac{1}{\sqrt{g}(\eta_p(t))}\hat{\mathbf{B}}^{*2} v_\parallel \,,
@@ -1013,15 +1036,15 @@
     def __init__(self, particles, **params):
 
         # pointer to variable
         assert isinstance(particles, Particles5D)
         self._particles = particles
 
         # parameters
-        params_default = {'kappa': 100.,
+        params_default = {'kappa': 1.,
                           'b': None,
                           'b_eq': None,
                           'unit_b1': None,
                           'unit_b2': None,
                           'abs_b': None,
                           'integrator': 'implicit',
                           'method': 'discrete_gradient_faster',
@@ -1048,16 +1071,16 @@
         self._b_full = self._b_eq.copy()
         if self._b is not None:
             self._b_full += self._b
 
         self._b_full.update_ghost_regions()
 
         # define gradient of absolute value of parallel magnetic field
-        PB = getattr(self.basis_ops, 'PB')
-        self._PBb = PB.dot(self._b_full)
+        self._PB = getattr(self.basis_ops, 'PB')
+        self._PBb = self._PB.dot(self._b_full)
         self._PBb.update_ghost_regions()
 
         self._grad_PBb = self.derham.grad.dot(self._PBb)
         self._grad_PBb.update_ghost_regions()
 
         if params['integrator'] == 'explicit':
 
@@ -1124,11 +1147,30 @@
     def variables(self):
         return self._particles
 
     def __call__(self, dt):
         """
         TODO
         """
+        # sum up total magnetic field
+        self._b_full = self._b_eq.copy()
+        if self._b is not None:
+            self._b_full += self._b
+
+        self._b_full.update_ghost_regions()
+
+        # define gradient of absolute value of parallel magnetic field
+        self._PBb = self._PB.dot(self._b_full)
+        self._PBb.update_ghost_regions()
+
+        self._grad_PBb = self.derham.grad.dot(self._PBb)
+        self._grad_PBb.update_ghost_regions()
+
+        self._pusher_inputs = (self._kappa, self._PBb._data,
+                               self._b_full[0]._data, self._b_full[1]._data, self._b_full[2]._data,
+                               self._unit_b1[0]._data, self._unit_b1[1]._data, self._unit_b1[2]._data,
+                               self._unit_b2[0]._data, self._unit_b2[1]._data, self._unit_b2[2]._data,
+                               self._curl_norm_b[0]._data, self._curl_norm_b[1]._data, self._curl_norm_b[2]._data,
+                               self._grad_PBb[0]._data, self._grad_PBb[1]._data, self._grad_PBb[2]._data)
+
         self._pusher(self._particles, dt,
                      *self._pusher_inputs, mpi_sort='each', verbose=False)
-
-        self._particles.save_magnetic_energy(self.derham, self._PBb)
```

### Comparing `struphy-1.9.9/src/struphy/propagators/solvers.py` & `struphy-2.0.0/src/struphy/propagators/solvers.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac-0.1-py3-none-any.whl` & `struphy-2.0.0/src/struphy/psydac-0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/banded_to_stencil_kernels.py` & `struphy-2.0.0/src/struphy/psydac_api/banded_to_stencil_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/basis_projection_kernels.py` & `struphy-2.0.0/src/struphy/psydac_api/basis_projection_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/basis_projection_ops.py` & `struphy-2.0.0/src/struphy/psydac_api/basis_projection_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,29 @@
 
             self._Q2 = self.assemble_basis_projection_operator(
                 fun, 'Hdiv', 'Hdiv')
 
         return self._Q2
 
     @property
+    def Q3(self):
+        r'''Basis projection operator
+
+        .. math::
+
+            \mathcal{Q}^3_{ijk,mno} := \hat{\Pi}^3_{ijk} \left[ \frac{\hat{\rho}^3_{\text{eq}}}{\sqrt{g}}\Lambda^3_{mno} \right] \,.
+        '''
+        if not hasattr(self, '_Q3'):
+            fun = [[lambda e1, e2, e3: self.weights['eq_mhd'].n3(
+                e1, e2, e3) / self.sqrt_g(e1, e2, e3)]]
+            self._Q3 = self.assemble_basis_projection_operator(fun, 'L2', 'L2')
+
+        return self._Q3
+
+    @property
     def Tv(self):
         r'''Basis projection operator 
 
         .. math::
 
             \mathcal{T}^v_{(\mu, ijk), (\nu, mno)} := \hat{\Pi}^1_{(\mu, ijk)} \left[\mathcal R^B_{\mu,\nu} \Lambda^0_{(\nu, mno)} \right] \,.
```

### Comparing `struphy-1.9.9/src/struphy/psydac_api/fields.py` & `struphy-2.0.0/src/struphy/psydac_api/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         init_type = init_params['type']
 
         if init_type is not None:
             fun_params = init_params[init_type]
 
             # white noise in logical space for different components
             if init_type == 'noise':
-                
+
                 # component(s) to perturb
                 if isinstance(fun_params['comps'][self._name], bool):
                     comps = [fun_params['comps'][self._name]]
                 else:
                     comps = fun_params['comps'][self._name]
 
                 # set white noise FE coefficients
@@ -323,38 +323,38 @@
 
                 # select function and project project
                 if hasattr(funs, self.name):
                     self.vector = self.derham.P[self.space_key](
                         getattr(funs, self.name))
 
         # apply boundary operator (in-place)
-        self.derham.B[self.space_key].dot(self._vector.copy(), out=self._vector)
+        self.derham.B[self.space_key].dot(
+            self._vector.copy(), out=self._vector)
 
         # update ghost regions
         self._vector.update_ghost_regions()
 
     def initialize_coeffs_from_restart_file(self, file, species=None):
         """
         TODO
         """
-        
+
         if species is None:
             key = 'restart/' + self.name
         else:
             key = 'restart/' + species + '_' + self.name
-        
+
         if isinstance(self.vector, StencilVector):
             self.vector._data[:] = file[key][-1]
         else:
             for n in range(3):
                 self.vector[n]._data[:] = file[key + '/' + str(n + 1)][-1]
-            
+
         self._vector.update_ghost_regions()
-    
-    
+
     def __call__(self, eta1, eta2, eta3, squeeze_output=False):
         """
         Evaluates the spline function on the local domain.
 
         Parameters
         ----------
             eta1, eta2, eta3 : array-like
```

### Comparing `struphy-1.9.9/src/struphy/psydac_api/linear_operators.py` & `struphy-2.0.0/src/struphy/psydac_api/linear_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/mass.py` & `struphy-2.0.0/src/struphy/psydac_api/mass.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,14 +363,82 @@
                 for n in range(3):
                     fun[-1] += [lambda e1, e2, e3, m=m,
                                 n=n: rot_J(e1, e2, e3)[:, :, :, m, n]]
 
             self._MvJ = self.assemble_weighted_mass(fun, 'Hdiv', 'H1vec')
 
         return self._MvJ
+    
+    @property
+    def M2B(self):
+        r"""
+        Mass matrix 
+
+        .. math::
+
+            \mathbb M^{2,B}_{(\mu,ijk), (\nu,mno)} = \int \Lambda^2_{\mu,ijk}\, \mathcal R^J_{\alpha, \nu}\, \Lambda^2_{\nu, mno} \, \frac{1}{\sqrt g}\,  \textnormal d \boldsymbol\eta. 
+
+        with the rotation matrix
+
+        .. math::
+
+            \mathcal R^J_{\alpha, \nu} := \epsilon_{\alpha \beta \nu}\, B^2_{\textnormal{eq}, \beta}\,,\qquad s.t. \qquad \mathcal R^J \vec v = \vec B^2_{\textnormal{eq}} \times \vec v\,,
+
+        where :math:`\epsilon_{\alpha \beta \nu}` stands for the Levi-Civita tensor and :math:`B^2_{\textnormal{eq}, \beta}` is the :math:`\beta`-component of the MHD equilibrium magnetic field (2-form).
+        """
+
+        if not hasattr(self, '_M2B'):
+
+            rot_B = RotationMatrix(
+                self.weights['eq_mhd'].b2_1, self.weights['eq_mhd'].b2_2, self.weights['eq_mhd'].b2_3)
+
+            fun = []
+            for m in range(3):
+                fun += [[]]
+                for n in range(3):
+                    fun[-1] += [lambda e1, e2, e3, m=m,
+                                n=n: rot_B(e1, e2, e3)[:, :, :, m, n] / self.sqrt_g(e1, e2, e3)]
+
+            self._M2B = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv')
+
+        return self._M2B
+    
+    @property
+    def M2Bn(self):
+        r"""
+        Mass matrix 
+
+        .. math::
+
+            \mathbb M^{2,BN}_{(\mu,ijk), (\nu,mno)} = \int \Lambda^2_{\mu,ijk}\, \mathcal R^J_{\alpha, \nu}\, \Lambda^2_{\nu, mno} \, \frac{1}{n^0_{\textnormal{eq}}(\boldsymbol \eta)}\, \frac{1}{\sqrt g}\,  \textnormal d \boldsymbol\eta. 
+
+        with the rotation matrix
+
+        .. math::
+
+            \mathcal R^J_{\alpha, \nu} := \epsilon_{\alpha \beta \nu}\, B^2_{\textnormal{eq}, \beta}\,,\qquad s.t. \qquad \mathcal R^J \vec v = \vec B^2_{\textnormal{eq}} \times \vec v\,,
+
+        where :math:`\epsilon_{\alpha \beta \nu}` stands for the Levi-Civita tensor and :math:`B^2_{\textnormal{eq}, \beta}` is the :math:`\beta`-component of the MHD equilibrium magnetic field (2-form).
+        """
+
+        if not hasattr(self, '_M2BN'):
+
+            rot_B = RotationMatrix(
+                self.weights['eq_mhd'].b2_1, self.weights['eq_mhd'].b2_2, self.weights['eq_mhd'].b2_3)
+
+            fun = []
+            for m in range(3):
+                fun += [[]]
+                for n in range(3):
+                    fun[-1] += [lambda e1, e2, e3, m=m,
+                                n=n: rot_B(e1, e2, e3)[:, :, :, m, n] / (self.sqrt_g(e1, e2, e3) * self.weights['eq_mhd'].n0(e1, e2, e3, squeeze_out=False))]
+
+            self._M2BN = self.assemble_weighted_mass(fun, 'Hdiv', 'Hdiv')
+
+        return self._M2BN
 
     #######################################
     # Wrapper around WeightedMassOperator #
     #######################################
     def assemble_weighted_mass(self, fun: list, V_id: str, W_id: str):
         r""" Weighted mass matrix :math:`V^\alpha_h \to V^\beta_h` with given (matrix-valued) weight function :math:`W(\boldsymbol \eta)`:
```

### Comparing `struphy-1.9.9/src/struphy/psydac_api/mass_kernels.py` & `struphy-2.0.0/src/struphy/psydac_api/mass_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/preconditioner.py` & `struphy-2.0.0/src/struphy/psydac_api/preconditioner.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/projectors.py` & `struphy-2.0.0/src/struphy/psydac_api/projectors.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/psydac_derham.py` & `struphy-2.0.0/src/struphy/psydac_api/psydac_derham.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/quadrature_evaluation_kernels.py` & `struphy-2.0.0/src/struphy/psydac_api/quadrature_evaluation_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/utilities.py` & `struphy-2.0.0/src/struphy/psydac_api/utilities.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/psydac_api/utilities_kernels.py` & `struphy-2.0.0/src/struphy/psydac_api/utilities_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_accumulation.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_accumulation.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_basis_operators.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_basis_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_draw_parallel.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_draw_parallel.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_eval_spline_mpi.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_eval_spline_mpi.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_iterative_solvers.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_iterative_solvers.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_mass_matrices.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_mass_matrices.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_mat_vec_filler.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_mat_vec_filler.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/accumulation_kernels_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/mappings_3d_fast.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_pos.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_2d.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_3d.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/pusher_vel_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_2d.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_2d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_polar.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_polar.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_psydac_basics.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_psydac_basics.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_psydac_derham.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_psydac_derham.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_pushers.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_pushers.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_stencil_dot_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/test_stencil_transpose_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_mpi/xx_test_send_ghost_regions.py` & `struphy-2.0.0/src/struphy/tests/tests_mpi/xx_test_send_ghost_regions.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_bsplines_kernels.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_bsplines_kernels.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_domain.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_domain.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_gvec_equil.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_gvec_equil.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_legacy_polar_splines.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_legacy_polar_splines.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_numerical_MHD_equil.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_numerical_MHD_equil.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_projectors_global.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_projectors_global.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_prop_solvers.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_prop_solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     mass_ops = WeightedMassOperators(derham, domain)
 
     Propagator.derham = derham
     Propagator.domain = domain
     Propagator.mass_ops = mass_ops
 
     # Create Poisson solver
-    poisson_solver = PoissonSolver(rho=rho_vec, x0=sol_vec, **solver_params)
+    poisson_solver = PoissonSolver(rho=rho_vec, **solver_params)
 
     # Solve Poisson equation
     poisson_solver(0.1)
 
     # Compare to analytical solution
     compare_arrays(
         poisson_solver._phi,
```

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_psydac_basis_operators.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_basis_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_psydac_linear_operators.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_linear_operators.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_psydac_mapping.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_psydac_mapping.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/test_spline_space_1d.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/test_spline_space_1d.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_psydac_lin_ops.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_psydac_lin_ops.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_GVEC.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_GVEC.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_codes.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_codes.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_cprofiler.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_cprofiler.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_divB.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_divB.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_filler_kernel.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_filler_kernel.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_mappings.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mappings.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_mat_vec_filler.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mat_vec_filler.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_mhd_equil.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_mhd_equil.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_paraview.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_paraview.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_polar_splines_3D.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_polar_splines_3D.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_preconditioner.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_preconditioner.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_psydac_lin_ops_loop.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_psydac_lin_ops_loop.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_spline_evaluation.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_spline_evaluation.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_spline_interpolation.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_spline_interpolation.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy/tests/tests_serial/xx_test_template_gvec.py` & `struphy-2.0.0/src/struphy/tests/tests_serial/xx_test_template_gvec.py`

 * *Files identical despite different names*

### Comparing `struphy-1.9.9/src/struphy.egg-info/PKG-INFO` & `struphy-2.0.0/src/struphy.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struphy
-Version: 1.9.9
+Version: 2.0.0
 Summary: Multi-model plasma physics package
 Author: Max Planck Institute for Plasma Physics
 Author-email: stefan.possanner@ipp.mpg.de, florian.holderied@ipp.mpg.de
 License: Copyright 2019 (c) Struphy dev team | Max Planck Institute for Plasma Physics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and 
         associated documentation files (the "Software"), to deal in the Software without restriction, 
@@ -17,69 +17,89 @@
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT 
         NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. 
         IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
         WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
         SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
-        In addition, we ask you to cite the following reference inscientific publications which contain
+        In addition, we ask you to cite the following reference in scientific publications which contain
         results obtained with this software and developments:
         
         F. Holderied, S. Possanner, X. Wang, 
         "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell",
         J. Comp. Phys. 433 (2021) 110143
         
 Project-URL: homepage, https://struphy.pages.mpcdf.de/struphy/
 Project-URL: documentation, https://struphy.pages.mpcdf.de/struphy/
 Project-URL: repository, https://gitlab.mpcdf.mpg.de/struphy/struphy
 Project-URL: changelog, https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/CHANGELOG.md
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/struphy/struphy/-/issues
 Keywords: plasma physics, fusion, numerical modeling, partial differential equations, energetic particles
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # STRUPHY - STRUcture-Preserving HYbrid codes
 
 A Python package for energetic particles in plasma.
 
 The package is developed since 2019 at [Max Planck Institute for Plasma Physics](https://www.ipp.mpg.de/) 
 in the division [NMPP (Numerical Methods for Plasma Physics)](https://www.ipp.mpg.de/ippcms/de/for/bereiche/numerik).
 
 ## What you can do with struphy
 
-* Solve a variety of [plasma physics PDEs](https://struphy.pages.mpcdf.de/struphy/sections/models.html) with fluid and/or kinetic components on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
-* [Post process](https://struphy.pages.mpcdf.de/struphy/sections/userguide.html#post-processing) data and generate `.vtk` files for 3d views
-* Add your own [model equations](https://struphy.pages.mpcdf.de/struphy/sections/developers.html#model-equations) or [physics feature](https://struphy.pages.mpcdf.de/struphy/sections/developers.html#how-to-add) 
+* Investigate plasma physics problems with multiple [models equations](https://struphy.pages.mpcdf.de/struphy/sections/models.html) containing fluid and/or kinetic components 
+* Simulate each model on [curved domains](https://struphy.pages.mpcdf.de/struphy/sections/domains.html) 
+* Load a variety of [MHD equilibira](https://struphy.pages.mpcdf.de/struphy/sections/mhd_equils.html) and [kinetic backgrounds](https://struphy.pages.mpcdf.de/struphy/sections/kinetic_backgrounds.html)
+* Use [diagnostic tools](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html) to visualize results
+* Compare simulations to analytic [dispersion relations](https://struphy.pages.mpcdf.de/struphy/sections/diagnostics.html#module-struphy.dispersion_relations.analytic)
+* Solve the [MHD eigenvalue problem](https://struphy.pages.mpcdf.de/struphy/index.html) in axisymmetric toroidal geometries
+* [Improve Struphy](https://struphy.pages.mpcdf.de/struphy/sections/developers.html) by adding
+    * model equations
+    * domains (geometry)
+    * MHD equilibria
+    * kinetic backgrounds
+    * diagnostic tools
+    * dispersion relations
+    * other physics features (e.g. collision operators etc.)
 
 ## Algorithmic features
 
 * Particle-in-cell method for kinetic species
 * Discrete differential forms based on high-order B-spline finite elements ([Psydac library](https://github.com/pyccel/psydac)) for fields/fluids
 * Exact conservation laws
 * Polar splines to treat a polar singularity 
 * Kernels are pre-compiled with [Pyccel](https://github.com/pyccel/pyccel) to achieve near-Fortran performance
 * MPI/OpenMP hybrid parallelization  
 
 ## Installation
 
-* See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+See the [struphy documentation](https://struphy.pages.mpcdf.de/struphy/index.html).
+
+## Tutorials
+
+* [Turorial 01](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_01_units_run_main.ipynb): Learn about Struphy model's normalization (units), simulation parameters and the Struphy main execution file.
+
+* [Tutorial 02](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_02_postproc_standard_plotting.ipynb): Learn about the data generated by Struphy simulations, data post processing and simple plotting 
+of field/fluid and kinetic variables.
+
+* [Tutorial 03](https://gitlab.mpcdf.mpg.de/struphy/struphy/-/blob/devel/notebooks/tutorial_03_plot_poloidal_planes.ipynb): Learn about plotting field/fluid variables in toroidal geometry.
 
 ## Key references
 
 * F. Holderied, S. Possanner, X. Wang, "MHD-kinetic hybrid code based on structure-preserving finite elements with particles-in-cell", [J. Comp. Phys. 433 (2021) 110143](https://www.sciencedirect.com/science/article/pii/S0021999121000358?via%3Dihub)
 
 * F. Holderied, S. Possanner, "Magneto-hydrodynamic eigenvalue solver for axis-symmetric equilibria based on smooth polar splines", [J. Comp. Phys. 464 (2022) 111329](https://www.sciencedirect.com/science/article/pii/S0021999122003916?via%3Dihub)
 
 * F. Holderied, "STRUPHY: a structure-preserving hybrid MHD-kinetic code for the interaction of energetic particles with Alfvén waves in magnetized plasmas", [PhD thesis (2022)](https://mediatum.ub.tum.de/?id=1656539)
 
 ## License
 
-Copyright 2022 (c) struphy dev team | CONTRIBUTING.md | Max Planck Institute for Plasma Physics
+Copyright 2019 (c) Struphy dev team | Max Planck Institute for Plasma Physics
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `struphy-1.9.9/src/struphy.egg-info/SOURCES.txt` & `struphy-2.0.0/src/struphy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 src/struphy/examples/TAE_tokamak.py
 src/struphy/examples/__init__.py
 src/struphy/examples/_draw_parallel.py
 src/struphy/examples/_mhd_eigenvalues_cylinder.py
 src/struphy/examples/_mhd_eigenvalues_slab.py
 src/struphy/examples/_sendrecv.py
 src/struphy/examples/gc_orbits_tokamak.py
+src/struphy/examples/linearextendedmhd.py
 src/struphy/examples/linearmhd.py
 src/struphy/examples/linearmhdvlasov_cc.py
 src/struphy/examples/linearmhdvlasov_pc.py
 src/struphy/examples/maxwell.py
 src/struphy/examples/orbits_tokamak.py
 src/struphy/fields_background/__init__.py
 src/struphy/fields_background/electric_equil/__init__.py
@@ -153,22 +154,23 @@
 src/struphy/io/inp/__init__.py
 src/struphy/io/inp/parameters.yml
 src/struphy/io/inp/examples/__init__.py
 src/struphy/io/inp/examples/params_TAE_tokamak.yml
 src/struphy/io/inp/examples/params_gc_orbits_tokamak.yml
 src/struphy/io/inp/examples/params_hybridmhdvlasovcc.yml
 src/struphy/io/inp/examples/params_hybridmhdvlasovpc.yml
+src/struphy/io/inp/examples/params_linearextendedmhd.yml
 src/struphy/io/inp/examples/params_linearmhd.yml
-src/struphy/io/inp/examples/params_linvlasovmaxwell.yml
 src/struphy/io/inp/examples/params_linvlasovmaxwell_landau.yml
 src/struphy/io/inp/examples/params_linvlasovmaxwell_weibel.yml
 src/struphy/io/inp/examples/params_maxwell.yml
 src/struphy/io/inp/examples/params_orbits_tokamak.yml
 src/struphy/io/inp/tests/__init__.py
 src/struphy/io/inp/tests/params_cc_linmhd_5d.yml
+src/struphy/io/inp/tests/params_deltafvlasovmaxwell.yml
 src/struphy/io/inp/tests/params_hybrid_fA.yml
 src/struphy/io/inp/tests/params_hybridmhdvlasovcc.yml
 src/struphy/io/inp/tests/params_hybridmhdvlasovcc_control.yml
 src/struphy/io/inp/tests/params_hybridmhdvlasovcc_gvec.yml
 src/struphy/io/inp/tests/params_hybridmhdvlasovpc.yml
 src/struphy/io/inp/tests/params_linearmhd.yml
 src/struphy/io/inp/tests/params_linearmhd_gvec.yml
@@ -195,17 +197,20 @@
 src/struphy/linear_algebra/iterative_solvers.py
 src/struphy/linear_algebra/linalg_kron.py
 src/struphy/linear_algebra/schur_solver.py
 src/struphy/linear_algebra/stencil_dot_kernels.py
 src/struphy/linear_algebra/stencil_transpose_kernels.py
 src/struphy/models/__init__.py
 src/struphy/models/base.py
+src/struphy/models/fluid.py
+src/struphy/models/hybrid.py
+src/struphy/models/kinetic.py
 src/struphy/models/main.py
-src/struphy/models/models.py
 src/struphy/models/output_handling.py
+src/struphy/models/toy.py
 src/struphy/models/utilities.py
 src/struphy/pic/__init__.py
 src/struphy/pic/accum_kernels.py
 src/struphy/pic/filler_kernels.py
 src/struphy/pic/mat_vec_filler.py
 src/struphy/pic/particles.py
 src/struphy/pic/particles_to_grid.py
@@ -274,14 +279,15 @@
 src/struphy/tests/tests_mpi/test_pic_legacy_files/spline_evaluation_3d.py
 src/struphy/tests/tests_serial/__init__.py
 src/struphy/tests/tests_serial/test_bsplines_kernels.py
 src/struphy/tests/tests_serial/test_domain.py
 src/struphy/tests/tests_serial/test_gvec_equil.py
 src/struphy/tests/tests_serial/test_legacy_mhd_projectors.py
 src/struphy/tests/tests_serial/test_legacy_polar_splines.py
+src/struphy/tests/tests_serial/test_mhd_equils.py
 src/struphy/tests/tests_serial/test_numerical_MHD_equil.py
 src/struphy/tests/tests_serial/test_projectors_global.py
 src/struphy/tests/tests_serial/test_prop_solvers.py
 src/struphy/tests/tests_serial/test_psydac_basis_operators.py
 src/struphy/tests/tests_serial/test_psydac_linear_operators.py
 src/struphy/tests/tests_serial/test_psydac_mapping.py
 src/struphy/tests/tests_serial/test_spline_space_1d.py
```

