# Comparing `tmp/ansys-mapdl-core-0.64.1.tar.gz` & `tmp/ansys_mapdl_core-0.65.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-mapdl-core-0.64.1.tar", last modified: Wed Apr  5 05:11:43 2023, max compression
+gzip compressed data, was "ansys_mapdl_core-0.65.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys-mapdl-core-0.64.1.tar` & `ansys_mapdl_core-0.65.0.tar`

### file list

```diff
@@ -1,485 +1,521 @@
--rw-r--r--   0        0        0     1089 2023-04-05 05:10:59.422384 ansys-mapdl-core-0.64.1/LICENSE
--rw-r--r--   0        0        0    10464 2023-04-05 05:10:59.422384 ansys-mapdl-core-0.64.1/README.rst
--rw-r--r--   0        0        0     4509 2023-04-05 05:10:59.606383 ansys-mapdl-core-0.64.1/pyproject.toml
--rw-r--r--   0        0        0     2492 2023-04-05 05:10:59.606383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 05:10:59.606383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/__init__.py
--rw-r--r--   0        0        0      134 2023-04-05 05:10:59.606383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/__init__.py
--rw-r--r--   0        0        0     7083 2023-04-05 05:10:59.606383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/abbreviations.py
--rw-r--r--   0        0        0    65022 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/array_param.py
--rw-r--r--   0        0        0    24293 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/macro_files.py
--rw-r--r--   0        0        0    33278 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/matrix_op.py
--rw-r--r--   0        0        0    49087 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/parameter_definition.py
--rw-r--r--   0        0        0      877 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/process_controls.py
--rw-r--r--   0        0        0       65 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux12_/__init__.py
--rw-r--r--   0        0        0     1800 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux12_/general_radiation.py
--rw-r--r--   0        0        0     4381 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux12_/radiation_mat.py
--rw-r--r--   0        0        0    15390 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux12_/radiosity_solver.py
--rw-r--r--   0        0        0     5782 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux15_.py
--rw-r--r--   0        0        0       34 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux2_/__init__.py
--rw-r--r--   0        0        0     2783 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux2_/bin_dump.py
--rw-r--r--   0        0        0    13843 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux2_/bin_manip.py
--rw-r--r--   0        0        0     4949 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux3_.py
--rw-r--r--   0        0        0    11323 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/conn.py
--rw-r--r--   0        0        0       78 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/__init__.py
--rw-r--r--   0        0        0    22459 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/components.py
--rw-r--r--   0        0        0    17248 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/coord_sys.py
--rw-r--r--   0        0        0     4715 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/picking.py
--rw-r--r--   0        0        0    53650 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/selecting.py
--rw-r--r--   0        0        0    13775 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/setup.py
--rw-r--r--   0        0        0    16923 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/working_plane.py
--rw-r--r--   0        0        0       20 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/display_/__init__.py
--rw-r--r--   0        0        0     9516 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/display_/setup.py
--rw-r--r--   0        0        0       73 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/__init__.py
--rw-r--r--   0        0        0    21774 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/annotation.py
--rw-r--r--   0        0        0    11407 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/graphs.py
--rw-r--r--   0        0        0    42963 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/labeling.py
--rw-r--r--   0        0        0    10248 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/scaling.py
--rw-r--r--   0        0        0    53850 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/setup.py
--rw-r--r--   0        0        0    22511 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/style.py
--rw-r--r--   0        0        0    18352 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/views.py
--rw-r--r--   0        0        0     3162 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/hidden.py
--rw-r--r--   0        0        0    50786 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/inq_func.py
--rw-r--r--   0        0        0    10067 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/map_cmd.py
--rw-r--r--   0        0        0       19 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/misc/__init__.py
--rw-r--r--   0        0        0      992 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/misc/misc.py
--rw-r--r--   0        0        0     2975 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/parse.py
--rw-r--r--   0        0        0      248 2023-04-05 05:10:59.610383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/__init__.py
--rw-r--r--   0        0        0    26912 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/animation.py
--rw-r--r--   0        0        0    21848 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/controls.py
--rw-r--r--   0        0        0    31418 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/element_table.py
--rw-r--r--   0        0        0     7015 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/failure_criteria.py
--rw-r--r--   0        0        0    11070 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/listing.py
--rw-r--r--   0        0        0    15600 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/load_case.py
--rw-r--r--   0        0        0    11457 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/magnetics_calc.py
--rw-r--r--   0        0        0    36235 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/path_operations.py
--rw-r--r--   0        0        0    38181 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/results.py
--rw-r--r--   0        0        0    32317 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/setup.py
--rw-r--r--   0        0        0    96414 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/special.py
--rw-r--r--   0        0        0     4431 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/status.py
--rw-r--r--   0        0        0    16032 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/surface_operations.py
--rw-r--r--   0        0        0     8201 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/trace_points.py
--rw-r--r--   0        0        0       77 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/__init__.py
--rw-r--r--   0        0        0     9792 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/controls.py
--rw-r--r--   0        0        0     5716 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/display.py
--rw-r--r--   0        0        0     4351 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/listing.py
--rw-r--r--   0        0        0    22683 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/operations.py
--rw-r--r--   0        0        0    33525 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/setup.py
--rw-r--r--   0        0        0    20246 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/special.py
--rw-r--r--   0        0        0     2904 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/status.py
--rw-r--r--   0        0        0      441 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/__init__.py
--rw-r--r--   0        0        0    42817 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/areas.py
--rw-r--r--   0        0        0     4341 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/artificially_matched_layers.py
--rw-r--r--   0        0        0    62005 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/booleans.py
--rw-r--r--   0        0        0    22650 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/constraint_equations.py
--rw-r--r--   0        0        0    15817 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/coupled_dof.py
--rw-r--r--   0        0        0    38580 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/database.py
--rw-r--r--   0        0        0     4096 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/digitizing.py
--rw-r--r--   0        0        0    16260 2023-04-05 05:10:59.614383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/element_type.py
--rw-r--r--   0        0        0   102587 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/elements.py
--rw-r--r--   0        0        0   158286 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/explicit_dynamics.py
--rw-r--r--   0        0        0     3745 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/hard_points.py
--rw-r--r--   0        0        0    32528 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/keypoints.py
--rw-r--r--   0        0        0    52765 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/lines.py
--rw-r--r--   0        0        0    26805 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/material_data_tables.py
--rw-r--r--   0        0        0    38458 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/materials.py
--rw-r--r--   0        0        0   136306 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/meshing.py
--rw-r--r--   0        0        0    12362 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/morphing.py
--rw-r--r--   0        0        0    43541 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/nodes.py
--rw-r--r--   0        0        0    35522 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/primitives.py
--rw-r--r--   0        0        0     9440 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/real_constants.py
--rw-r--r--   0        0        0    59811 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/sections.py
--rw-r--r--   0        0        0    43269 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/special_purpose.py
--rw-r--r--   0        0        0    15604 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/status.py
--rw-r--r--   0        0        0     9685 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/superelements.py
--rw-r--r--   0        0        0    44600 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/volumes.py
--rw-r--r--   0        0        0       55 2023-04-05 05:10:59.618383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/__init__.py
--rw-r--r--   0        0        0    15305 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/generation.py
--rw-r--r--   0        0        0     3067 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/preparation.py
--rw-r--r--   0        0        0     1154 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/setup.py
--rw-r--r--   0        0        0     4692 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/use_pass.py
--rw-r--r--   0        0        0       66 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/__init__.py
--rw-r--r--   0        0        0    26143 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/files.py
--rw-r--r--   0        0        0     3481 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/list_controls.py
--rw-r--r--   0        0        0     5122 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/processor_entry.py
--rw-r--r--   0        0        0    25874 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/run_controls.py
--rw-r--r--   0        0        0      763 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/all_others.py
--rw-r--r--   0        0        0   157108 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/analysis_options.py
--rw-r--r--   0        0        0     3320 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/birth_and_death.py
--rw-r--r--   0        0        0    56005 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/dynamic_options.py
--rw-r--r--   0        0        0    34700 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/fe_body_loads.py
--rw-r--r--   0        0        0    29784 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/fe_constraints.py
--rw-r--r--   0        0        0    15694 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/fe_forces.py
--rw-r--r--   0        0        0    23544 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/fe_surface_loads.py
--rw-r--r--   0        0        0     8378 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/gap_conditions.py
--rw-r--r--   0        0        0    33877 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/inertia.py
--rw-r--r--   0        0        0     8882 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/load_step_operations.py
--rw-r--r--   0        0        0    36881 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/load_step_options.py
--rw-r--r--   0        0        0     6753 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/master_dof.py
--rw-r--r--   0        0        0    55158 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/miscellaneous_loads.py
--rw-r--r--   0        0        0     4065 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_convergence_controls.py
--rw-r--r--   0        0        0     6518 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_definition_commands.py
--rw-r--r--   0        0        0    12413 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_global_controls.py
--rw-r--r--   0        0        0     7669 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_interface_mapping.py
--rw-r--r--   0        0        0     9429 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_load_transfer.py
--rw-r--r--   0        0        0     7905 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_time_controls.py
--rw-r--r--   0        0        0    58898 2023-04-05 05:10:59.622383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/nonlinear_options.py
--rw-r--r--   0        0        0    15629 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/ocean.py
--rw-r--r--   0        0        0    10287 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/radiosity.py
--rw-r--r--   0        0        0    12029 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/rezoning.py
--rw-r--r--   0        0        0    18965 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solid_body_loads.py
--rw-r--r--   0        0        0    18072 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solid_constraints.py
--rw-r--r--   0        0        0     4405 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solid_forces.py
--rw-r--r--   0        0        0    10519 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solid_surface_loads.py
--rw-r--r--   0        0        0    12380 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solution_status.py
--rw-r--r--   0        0        0    61309 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/spectrum_options.py
--rw-r--r--   0        0        0     2435 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/twod_to_3d_analysis.py
--rw-r--r--   0        0        0      720 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_version.py
--rw-r--r--   0        0        0    24139 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/commands.py
--rw-r--r--   0        0        0     4583 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/common_grpc.py
--rw-r--r--   0        0        0    36769 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/convert.py
--rw-r--r--   0        0        0      208 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/database/__init__.py
--rw-r--r--   0        0        0    14174 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/database/database.py
--rw-r--r--   0        0        0    10848 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/database/elems.py
--rw-r--r--   0        0        0    16557 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/database/nodes.py
--rw-r--r--   0        0        0     5900 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/errors.py
--rw-r--r--   0        0        0      171 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/__init__.py
--rw-r--r--   0        0        0     5342 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/downloads.py
--rw-r--r--   0        0        0     1001 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/examples.py
--rwxr-xr-x   0        0        0     1259 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm1.dat
--rwxr-xr-x   0        0        0     1136 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm10.dat
--rwxr-xr-x   0        0        0     2398 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm100.dat
--rwxr-xr-x   0        0        0     2310 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm101.dat
--rwxr-xr-x   0        0        0     2288 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm102.dat
--rwxr-xr-x   0        0        0     3460 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm103.dat
--rwxr-xr-x   0        0        0     2186 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm104.dat
--rwxr-xr-x   0        0        0     1910 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm105.dat
--rwxr-xr-x   0        0        0     1158 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm106.dat
--rwxr-xr-x   0        0        0     1367 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm107.dat
--rwxr-xr-x   0        0        0     1334 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm108.dat
--rwxr-xr-x   0        0        0     1706 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm109.dat
--rwxr-xr-x   0        0        0     1775 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm11.dat
--rwxr-xr-x   0        0        0     2079 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm110.dat
--rwxr-xr-x   0        0        0     1526 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm111.dat
--rwxr-xr-x   0        0        0     1655 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm112.dat
--rwxr-xr-x   0        0        0     1906 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm113.dat
--rwxr-xr-x   0        0        0     2179 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm114.dat
--rwxr-xr-x   0        0        0     1710 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm115.dat
--rwxr-xr-x   0        0        0     2274 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm116.dat
--rwxr-xr-x   0        0        0     4258 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm117.dat
--rwxr-xr-x   0        0        0     3342 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm118.dat
--rwxr-xr-x   0        0        0     4270 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm119.dat
--rwxr-xr-x   0        0        0     2179 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm12.dat
--rwxr-xr-x   0        0        0     2347 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm120.dat
--rwxr-xr-x   0        0        0     5210 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm121.dat
--rwxr-xr-x   0        0        0     1157 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm122.dat
--rwxr-xr-x   0        0        0     1271 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm123.dat
--rwxr-xr-x   0        0        0     1840 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm124.dat
--rwxr-xr-x   0        0        0     2193 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm125.dat
--rwxr-xr-x   0        0        0     2215 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm126.dat
--rwxr-xr-x   0        0        0     2706 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm127.dat
--rwxr-xr-x   0        0        0     1613 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm128.dat
--rwxr-xr-x   0        0        0     2143 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm129.dat
--rwxr-xr-x   0        0        0     1304 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm13.dat
--rwxr-xr-x   0        0        0     2681 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm130.dat
--rwxr-xr-x   0        0        0     1316 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm131.dat
--rwxr-xr-x   0        0        0     1822 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm132.dat
--rwxr-xr-x   0        0        0     1919 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm133.dat
--rwxr-xr-x   0        0        0     4248 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm134.dat
--rwxr-xr-x   0        0        0     1248 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm135.dat
--rwxr-xr-x   0        0        0     4147 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm136.dat
--rwxr-xr-x   0        0        0     1606 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm137.dat
--rwxr-xr-x   0        0        0     1206 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm138.dat
--rwxr-xr-x   0        0        0     5171 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm139.dat
--rwxr-xr-x   0        0        0     1366 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm14.dat
--rwxr-xr-x   0        0        0     2083 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm140.dat
--rwxr-xr-x   0        0        0     9573 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm141.dat
--rwxr-xr-x   0        0        0     3492 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm142.dat
--rwxr-xr-x   0        0        0    14718 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm143.dat
--rwxr-xr-x   0        0        0     7102 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm144.dat
--rwxr-xr-x   0        0        0     1597 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm145.dat
--rwxr-xr-x   0        0        0     2712 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm146.dat
--rwxr-xr-x   0        0        0     2204 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm147.dat
--rwxr-xr-x   0        0        0     2427 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm148.dat
--rwxr-xr-x   0        0        0     9424 2023-04-05 05:10:59.626383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm149.dat
--rwxr-xr-x   0        0        0     3289 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm15.dat
--rwxr-xr-x   0        0        0     3048 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm150.dat
--rwxr-xr-x   0        0        0     1844 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm151.dat
--rwxr-xr-x   0        0        0     2211 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm152.dat
--rwxr-xr-x   0        0        0     4596 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm153.dat
--rwxr-xr-x   0        0        0     1297 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm154.dat
--rwxr-xr-x   0        0        0     2617 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm155.dat
--rwxr-xr-x   0        0        0     2085 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm156.dat
--rwxr-xr-x   0        0        0     2343 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm157.dat
--rwxr-xr-x   0        0        0     1726 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm158.dat
--rwxr-xr-x   0        0        0     1741 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm159.dat
--rwxr-xr-x   0        0        0     3791 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm16.dat
--rwxr-xr-x   0        0        0     1989 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm160.dat
--rwxr-xr-x   0        0        0     1323 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm161.dat
--rwxr-xr-x   0        0        0     1289 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm162.dat
--rwxr-xr-x   0        0        0     1856 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm163.dat
--rwxr-xr-x   0        0        0     1340 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm164.dat
--rwxr-xr-x   0        0        0     4809 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm165.dat
--rwxr-xr-x   0        0        0     5306 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm166.dat
--rwxr-xr-x   0        0        0     6982 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm167.dat
--rwxr-xr-x   0        0        0     3247 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm168.dat
--rwxr-xr-x   0        0        0     2946 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm169.dat
--rwxr-xr-x   0        0        0     5454 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm17.dat
--rwxr-xr-x   0        0        0     1864 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm170.dat
--rwxr-xr-x   0        0        0     3287 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm171.dat
--rwxr-xr-x   0        0        0     3481 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm172.dat
--rwxr-xr-x   0        0        0     2328 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm173.dat
--rwxr-xr-x   0        0        0     3216 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm174.dat
--rwxr-xr-x   0        0        0     7192 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm175.dat
--rwxr-xr-x   0        0        0    10653 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm176.dat
--rwxr-xr-x   0        0        0    13034 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm177.dat
--rwxr-xr-x   0        0        0     2400 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm178.dat
--rwxr-xr-x   0        0        0     3944 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm179.dat
--rwxr-xr-x   0        0        0     2572 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm18.dat
--rwxr-xr-x   0        0        0     1734 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm180.dat
--rwxr-xr-x   0        0        0     1308 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm181.dat
--rwxr-xr-x   0        0        0     2336 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm182.dat
--rwxr-xr-x   0        0        0     2110 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm183.dat
--rwxr-xr-x   0        0        0     8756 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm184.dat
--rwxr-xr-x   0        0        0     7860 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm185.dat
--rwxr-xr-x   0        0        0     7664 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm186.dat
--rwxr-xr-x   0        0        0     4063 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm187.dat
--rwxr-xr-x   0        0        0     6561 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm188.dat
--rwxr-xr-x   0        0        0     2768 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm189.dat
--rwxr-xr-x   0        0        0     2378 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm19.dat
--rwxr-xr-x   0        0        0     3974 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm190.dat
--rwxr-xr-x   0        0        0     8625 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm191.dat
--rwxr-xr-x   0        0        0     1966 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm192.dat
--rwxr-xr-x   0        0        0     1568 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm193.dat
--rwxr-xr-x   0        0        0     1799 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm194.dat
--rwxr-xr-x   0        0        0     2052 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm195.dat
--rwxr-xr-x   0        0        0     2394 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm196.dat
--rwxr-xr-x   0        0        0     3069 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm197.dat
--rwxr-xr-x   0        0        0     6858 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm198.dat
--rwxr-xr-x   0        0        0     4458 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm199.dat
--rwxr-xr-x   0        0        0     1621 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm2.dat
--rwxr-xr-x   0        0        0     2886 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm20.dat
--rwxr-xr-x   0        0        0     5701 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm200.dat
--rwxr-xr-x   0        0        0     6376 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm201.dat
--rwxr-xr-x   0        0        0     2019 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm202.dat
--rwxr-xr-x   0        0        0     3016 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm203.dat
--rwxr-xr-x   0        0        0     3646 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm204.dat
--rwxr-xr-x   0        0        0     3330 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm205.dat
--rwxr-xr-x   0        0        0     5126 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm206.dat
--rwxr-xr-x   0        0        0     6365 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm207.dat
--rwxr-xr-x   0        0        0     1933 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm208.dat
--rwxr-xr-x   0        0        0    12274 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm209.dat
--rwxr-xr-x   0        0        0     2714 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm21.dat
--rwxr-xr-x   0        0        0     9377 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm210.dat
--rwxr-xr-x   0        0        0     8476 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm211.dat
--rwxr-xr-x   0        0        0     6047 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm212.dat
--rwxr-xr-x   0        0        0     7773 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm213.dat
--rwxr-xr-x   0        0        0     2056 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm214.dat
--rwxr-xr-x   0        0        0     1748 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm215.dat
--rwxr-xr-x   0        0        0     2981 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm216.dat
--rwxr-xr-x   0        0        0     2034 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm217.dat
--rwxr-xr-x   0        0        0    11580 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm218.dat
--rwxr-xr-x   0        0        0     3850 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm219.dat
--rwxr-xr-x   0        0        0     1126 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm22.dat
--rwxr-xr-x   0        0        0     2333 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm220.dat
--rwxr-xr-x   0        0        0     2033 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm221.dat
--rwxr-xr-x   0        0        0     2638 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm222.dat
--rwxr-xr-x   0        0        0     5854 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm223.dat
--rwxr-xr-x   0        0        0     3550 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm224.dat
--rwxr-xr-x   0        0        0     3006 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm225.dat
--rwxr-xr-x   0        0        0     9693 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm226.dat
--rwxr-xr-x   0        0        0     2644 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm227.dat
--rwxr-xr-x   0        0        0    11948 2023-04-05 05:10:59.630383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm228.dat
--rwxr-xr-x   0        0        0     6269 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm229.dat
--rwxr-xr-x   0        0        0     6440 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm23.dat
--rwxr-xr-x   0        0        0     2506 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm230.dat
--rwxr-xr-x   0        0        0     7488 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm231.dat
--rwxr-xr-x   0        0        0     2702 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm232.dat
--rwxr-xr-x   0        0        0     3332 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm233.dat
--rwxr-xr-x   0        0        0     2505 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm234.dat
--rwxr-xr-x   0        0        0     3668 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm235.dat
--rwxr-xr-x   0        0        0     5828 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm236.dat
--rwxr-xr-x   0        0        0     6539 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm237.dat
--rwxr-xr-x   0        0        0     3570 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm238.dat
--rwxr-xr-x   0        0        0     8213 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm239.dat
--rwxr-xr-x   0        0        0     1314 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm24.dat
--rwxr-xr-x   0        0        0     2368 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm240.dat
--rwxr-xr-x   0        0        0     8192 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm241.dat
--rwxr-xr-x   0        0        0     3120 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm242.dat
--rwxr-xr-x   0        0        0     2532 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm243.dat
--rwxr-xr-x   0        0        0     2788 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm244.dat
--rwxr-xr-x   0        0        0     3386 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm245.dat
--rwxr-xr-x   0        0        0     6740 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm246.dat
--rwxr-xr-x   0        0        0     7893 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm247.dat
--rwxr-xr-x   0        0        0    10983 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm248.dat
--rwxr-xr-x   0        0        0     7633 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm249.dat
--rwxr-xr-x   0        0        0     3932 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm25.dat
--rwxr-xr-x   0        0        0     7520 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm250.dat
--rwxr-xr-x   0        0        0     8080 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm251.dat
--rwxr-xr-x   0        0        0     4160 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm252.dat
--rwxr-xr-x   0        0        0     3738 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm253.dat
--rwxr-xr-x   0        0        0     8494 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm254.dat
--rwxr-xr-x   0        0        0     4159 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm255.dat
--rwxr-xr-x   0        0        0     7257 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm256.dat
--rwxr-xr-x   0        0        0     8647 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm257.dat
--rwxr-xr-x   0        0        0     7153 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm258.dat
--rwxr-xr-x   0        0        0    20705 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm259.dat
--rwxr-xr-x   0        0        0     6028 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm26.dat
--rwxr-xr-x   0        0        0     8138 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm260.dat
--rwxr-xr-x   0        0        0     5004 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm261.dat
--rwxr-xr-x   0        0        0     2767 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm262.dat
--rwxr-xr-x   0        0        0    17283 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm263.dat
--rwxr-xr-x   0        0        0     7791 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm264.dat
--rwxr-xr-x   0        0        0     6050 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm265.dat
--rwxr-xr-x   0        0        0    10152 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm266.dat
--rwxr-xr-x   0        0        0     5481 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm267.dat
--rwxr-xr-x   0        0        0     3292 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm268.dat
--rwxr-xr-x   0        0        0     2798 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm269.dat
--rwxr-xr-x   0        0        0     1748 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm27.dat
--rwxr-xr-x   0        0        0     4546 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm270.dat
--rwxr-xr-x   0        0        0     5089 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm271.dat
--rwxr-xr-x   0        0        0    19367 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm272.dat
--rwxr-xr-x   0        0        0     5448 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm273.dat
--rwxr-xr-x   0        0        0     3911 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm274.dat
--rwxr-xr-x   0        0        0     8074 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm275.dat
--rwxr-xr-x   0        0        0     3462 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm276.dat
--rwxr-xr-x   0        0        0     2857 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm277.dat
--rwxr-xr-x   0        0        0     3930 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm278.dat
--rwxr-xr-x   0        0        0     8865 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm279.dat
--rwxr-xr-x   0        0        0     2087 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm28.dat
--rwxr-xr-x   0        0        0     4009 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm280.dat
--rwxr-xr-x   0        0        0    11179 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm281.dat
--rwxr-xr-x   0        0        0     5487 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm282.dat
--rwxr-xr-x   0        0        0     4608 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm283.dat
--rwxr-xr-x   0        0        0     4853 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm29.dat
--rwxr-xr-x   0        0        0     1679 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm3.dat
--rwxr-xr-x   0        0        0     2534 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm30.dat
--rwxr-xr-x   0        0        0     1634 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm31.dat
--rwxr-xr-x   0        0        0     2881 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm32.dat
--rwxr-xr-x   0        0        0     6611 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm33.dat
--rwxr-xr-x   0        0        0     6409 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm34.dat
--rwxr-xr-x   0        0        0     1980 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm35.dat
--rwxr-xr-x   0        0        0     4297 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm36.dat
--rwxr-xr-x   0        0        0     3948 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm37.dat
--rwxr-xr-x   0        0        0     4667 2023-04-05 05:10:59.634383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm38.dat
--rwxr-xr-x   0        0        0     5129 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm39.dat
--rwxr-xr-x   0        0        0     1457 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm4.dat
--rwxr-xr-x   0        0        0     2909 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm40.dat
--rwxr-xr-x   0        0        0     2692 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm41.dat
--rwxr-xr-x   0        0        0     3005 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm42.dat
--rwxr-xr-x   0        0        0     2772 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm43.dat
--rwxr-xr-x   0        0        0     2861 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm44.dat
--rwxr-xr-x   0        0        0     1045 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm45.dat
--rwxr-xr-x   0        0        0     3215 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm46.dat
--rwxr-xr-x   0        0        0     1491 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm47.dat
--rwxr-xr-x   0        0        0     1536 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm48.dat
--rwxr-xr-x   0        0        0     3272 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm49.dat
--rwxr-xr-x   0        0        0     2875 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm5.dat
--rwxr-xr-x   0        0        0     1456 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm50.dat
--rwxr-xr-x   0        0        0    13101 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm51.dat
--rwxr-xr-x   0        0        0     1863 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm52.dat
--rwxr-xr-x   0        0        0     2268 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm53.dat
--rwxr-xr-x   0        0        0     5967 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm54.dat
--rwxr-xr-x   0        0        0     1721 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm55.dat
--rwxr-xr-x   0        0        0     5900 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm56.dat
--rwxr-xr-x   0        0        0     5777 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm57.dat
--rwxr-xr-x   0        0        0     1869 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm58.dat
--rwxr-xr-x   0        0        0     2129 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm59.dat
--rwxr-xr-x   0        0        0     2488 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm6.dat
--rwxr-xr-x   0        0        0     1672 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm60.dat
--rwxr-xr-x   0        0        0     1305 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm61.dat
--rwxr-xr-x   0        0        0     4598 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm62.dat
--rwxr-xr-x   0        0        0     3612 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm63.dat
--rwxr-xr-x   0        0        0     1685 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm64.dat
--rwxr-xr-x   0        0        0     3053 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm65.dat
--rwxr-xr-x   0        0        0     4452 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm66.dat
--rwxr-xr-x   0        0        0     1553 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm67.dat
--rwxr-xr-x   0        0        0     2415 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm68.dat
--rwxr-xr-x   0        0        0     1816 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm69.dat
--rwxr-xr-x   0        0        0     6360 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm7.dat
--rwxr-xr-x   0        0        0     2165 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm70.dat
--rwxr-xr-x   0        0        0     2359 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm71.dat
--rwxr-xr-x   0        0        0     2798 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm72.dat
--rwxr-xr-x   0        0        0     2012 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm73.dat
--rwxr-xr-x   0        0        0     2168 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm74.dat
--rwxr-xr-x   0        0        0     2371 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm75.dat
--rwxr-xr-x   0        0        0     2394 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm76.dat
--rwxr-xr-x   0        0        0     2758 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm77.dat
--rwxr-xr-x   0        0        0     2150 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm78.dat
--rwxr-xr-x   0        0        0     2362 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm79.dat
--rwxr-xr-x   0        0        0     3514 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm8.dat
--rwxr-xr-x   0        0        0     2412 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm80.dat
--rwxr-xr-x   0        0        0     3967 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm81.dat
--rwxr-xr-x   0        0        0     9680 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm82.dat
--rwxr-xr-x   0        0        0     2361 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm83.dat
--rwxr-xr-x   0        0        0     2243 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm84.dat
--rwxr-xr-x   0        0        0     2850 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm85.dat
--rwxr-xr-x   0        0        0     1434 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm86.dat
--rwxr-xr-x   0        0        0     1561 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm87.dat
--rwxr-xr-x   0        0        0     1620 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm88.dat
--rwxr-xr-x   0        0        0     2116 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm89.dat
--rwxr-xr-x   0        0        0     2464 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm9.dat
--rwxr-xr-x   0        0        0     2579 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm90.dat
--rwxr-xr-x   0        0        0     2830 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm91.dat
--rwxr-xr-x   0        0        0     1395 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm92.dat
--rwxr-xr-x   0        0        0     1108 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm93.dat
--rwxr-xr-x   0        0        0     1542 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm94.dat
--rwxr-xr-x   0        0        0     3494 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm95.dat
--rwxr-xr-x   0        0        0     3026 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm96.dat
--rwxr-xr-x   0        0        0     2578 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm97.dat
--rwxr-xr-x   0        0        0     2034 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm98.dat
--rwxr-xr-x   0        0        0     1607 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm99.dat
--rwxr-xr-x   0        0        0    11868 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc1.dat
--rwxr-xr-x   0        0        0     9617 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc2.dat
--rwxr-xr-x   0        0        0     4766 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc3.dat
--rwxr-xr-x   0        0        0     6787 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc4.dat
--rwxr-xr-x   0        0        0     5775 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc5.dat
--rwxr-xr-x   0        0        0     6120 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc6.dat
--rwxr-xr-x   0        0        0     4152 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc7.dat
--rwxr-xr-x   0        0        0     4320 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc8.dat
--rwxr-xr-x   0        0        0    11304 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmd1.dat
--rwxr-xr-x   0        0        0     4372 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmd2.dat
--rwxr-xr-x   0        0        0    11914 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmd3.dat
--rwxr-xr-x   0        0        0     2600 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme1.dat
--rwxr-xr-x   0        0        0     1771 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme2.dat
--rwxr-xr-x   0        0        0     3360 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme3.dat
--rwxr-xr-x   0        0        0     3447 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme4.dat
--rwxr-xr-x   0        0        0     2452 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme5.dat
--rwxr-xr-x   0        0        0     3670 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme6.dat
--rwxr-xr-x   0        0        0      639 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif_files.py
--rw-r--r--   0        0        0     1455 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/wing.dat
--rw-r--r--   0        0        0       70 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/__init__.py
--rw-r--r--   0        0        0    20036 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/component_queries.py
--rw-r--r--   0        0        0     2523 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/connectivity_queries.py
--rw-r--r--   0        0        0     2973 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/core.py
--rw-r--r--   0        0        0     5878 2023-04-05 05:10:59.638383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/geometry_queries.py
--rw-r--r--   0        0        0     4495 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/inline_functions.py
--rw-r--r--   0        0        0     7220 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/line_queries.py
--rw-r--r--   0        0        0     3021 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/nearest_queries.py
--rw-r--r--   0        0        0     7010 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/normals_queries.py
--rw-r--r--   0        0        0     4285 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/scalar_queries.py
--rw-r--r--   0        0        0    16111 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/selection_queries.py
--rw-r--r--   0        0        0     3999 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/jupyter.py
--rw-r--r--   0        0        0    25522 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/krylov.py
--rw-r--r--   0        0        0    74171 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/launcher.py
--rw-r--r--   0        0        0    17782 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/licensing.py
--rw-r--r--   0        0        0    20215 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/logging.py
--rw-r--r--   0        0        0   142533 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl.py
--rw-r--r--   0        0        0     7620 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_console.py
--rw-r--r--   0        0        0    13258 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_corba.py
--rw-r--r--   0        0        0    29313 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_geometry.py
--rw-r--r--   0        0        0   110168 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_grpc.py
--rw-r--r--   0        0        0      258 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_types.py
--rwxr-xr-x   0        0        0    60954 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/math.py
--rw-r--r--   0        0        0        0 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mesh/__init__.py
--rw-r--r--   0        0        0     7669 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mesh/mesh.py
--rw-r--r--   0        0        0    24033 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mesh_grpc.py
--rw-r--r--   0        0        0    40380 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/misc.py
--rw-r--r--   0        0        0    23198 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/parameters.py
--rw-r--r--   0        0        0    37509 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/plotting.py
--rwxr-xr-x   0        0        0    20596 2023-04-05 05:10:59.642383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/pool.py
--rw-r--r--   0        0        0   130583 2023-04-05 05:10:59.646383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/post.py
--rw-r--r--   0        0        0     8039 2023-04-05 05:10:59.646383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/solution.py
--rw-r--r--   0        0        0     1267 2023-04-05 05:10:59.646383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/theme.py
--rw-r--r--   0        0        0    16086 2023-04-05 05:10:59.646383 ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/xpl.py
--rw-r--r--   0        0        0    13991 1970-01-01 00:00:00.000000 ansys-mapdl-core-0.64.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-06-02 09:30:43.135172 ansys_mapdl_core-0.65.0/LICENSE
+-rw-r--r--   0        0        0    10472 2023-06-02 09:30:43.135172 ansys_mapdl_core-0.65.0/README.rst
+-rw-r--r--   0        0        0     4553 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/pyproject.toml
+-rw-r--r--   0        0        0     2341 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/__init__.py
+-rw-r--r--   0        0        0      134 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/__init__.py
+-rw-r--r--   0        0        0     7083 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/abbreviations.py
+-rw-r--r--   0        0        0    65022 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/array_param.py
+-rw-r--r--   0        0        0    24293 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/macro_files.py
+-rw-r--r--   0        0        0    33278 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/matrix_op.py
+-rw-r--r--   0        0        0    49087 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/parameter_definition.py
+-rw-r--r--   0        0        0      877 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/process_controls.py
+-rw-r--r--   0        0        0       65 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/__init__.py
+-rw-r--r--   0        0        0     1800 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/general_radiation.py
+-rw-r--r--   0        0        0     4381 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/radiation_mat.py
+-rw-r--r--   0        0        0    15390 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/radiosity_solver.py
+-rw-r--r--   0        0        0     5782 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux15_.py
+-rw-r--r--   0        0        0       34 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/__init__.py
+-rw-r--r--   0        0        0     2783 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/bin_dump.py
+-rw-r--r--   0        0        0    13843 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/bin_manip.py
+-rw-r--r--   0        0        0     4949 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux3_.py
+-rw-r--r--   0        0        0    11323 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/conn.py
+-rw-r--r--   0        0        0       78 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/__init__.py
+-rw-r--r--   0        0        0    22459 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/components.py
+-rw-r--r--   0        0        0    17248 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/coord_sys.py
+-rw-r--r--   0        0        0     4715 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/picking.py
+-rw-r--r--   0        0        0    53650 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/selecting.py
+-rw-r--r--   0        0        0    13775 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/setup.py
+-rw-r--r--   0        0        0    16923 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/working_plane.py
+-rw-r--r--   0        0        0       20 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/display_/__init__.py
+-rw-r--r--   0        0        0     9516 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/display_/setup.py
+-rw-r--r--   0        0        0       73 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/__init__.py
+-rw-r--r--   0        0        0    21774 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/annotation.py
+-rw-r--r--   0        0        0    11407 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/graphs.py
+-rw-r--r--   0        0        0    42963 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/labeling.py
+-rw-r--r--   0        0        0    10248 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/scaling.py
+-rw-r--r--   0        0        0    53850 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/setup.py
+-rw-r--r--   0        0        0    22511 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/style.py
+-rw-r--r--   0        0        0    18352 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/views.py
+-rw-r--r--   0        0        0     3162 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/hidden.py
+-rw-r--r--   0        0        0    50786 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/inq_func.py
+-rw-r--r--   0        0        0    10067 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/map_cmd.py
+-rw-r--r--   0        0        0       19 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/misc/__init__.py
+-rw-r--r--   0        0        0      992 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/misc/misc.py
+-rw-r--r--   0        0        0     2975 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/parse.py
+-rw-r--r--   0        0        0      248 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/__init__.py
+-rw-r--r--   0        0        0    26912 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/animation.py
+-rw-r--r--   0        0        0    21848 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/controls.py
+-rw-r--r--   0        0        0    31418 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/element_table.py
+-rw-r--r--   0        0        0     7015 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/failure_criteria.py
+-rw-r--r--   0        0        0    11070 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/listing.py
+-rw-r--r--   0        0        0    15600 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/load_case.py
+-rw-r--r--   0        0        0    11457 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/magnetics_calc.py
+-rw-r--r--   0        0        0    36235 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/path_operations.py
+-rw-r--r--   0        0        0    38181 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/results.py
+-rw-r--r--   0        0        0    32317 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/setup.py
+-rw-r--r--   0        0        0    96414 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/special.py
+-rw-r--r--   0        0        0     4431 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/status.py
+-rw-r--r--   0        0        0    16032 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/surface_operations.py
+-rw-r--r--   0        0        0     8201 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/trace_points.py
+-rw-r--r--   0        0        0       77 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/__init__.py
+-rw-r--r--   0        0        0     9792 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/controls.py
+-rw-r--r--   0        0        0     5716 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/display.py
+-rw-r--r--   0        0        0     4351 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/listing.py
+-rw-r--r--   0        0        0    22683 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/operations.py
+-rw-r--r--   0        0        0    33525 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/setup.py
+-rw-r--r--   0        0        0    20246 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/special.py
+-rw-r--r--   0        0        0     2904 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/status.py
+-rw-r--r--   0        0        0      441 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/__init__.py
+-rw-r--r--   0        0        0    42817 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/areas.py
+-rw-r--r--   0        0        0     4341 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/artificially_matched_layers.py
+-rw-r--r--   0        0        0    62005 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/booleans.py
+-rw-r--r--   0        0        0    22650 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/constraint_equations.py
+-rw-r--r--   0        0        0    15817 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/coupled_dof.py
+-rw-r--r--   0        0        0    38580 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/database.py
+-rw-r--r--   0        0        0     4096 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/digitizing.py
+-rw-r--r--   0        0        0    16260 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/element_type.py
+-rw-r--r--   0        0        0   102587 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/elements.py
+-rw-r--r--   0        0        0   158286 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/explicit_dynamics.py
+-rw-r--r--   0        0        0     3745 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/hard_points.py
+-rw-r--r--   0        0        0    32528 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/keypoints.py
+-rw-r--r--   0        0        0    52765 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/lines.py
+-rw-r--r--   0        0        0    26805 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/material_data_tables.py
+-rw-r--r--   0        0        0    38458 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/materials.py
+-rw-r--r--   0        0        0   136306 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/meshing.py
+-rw-r--r--   0        0        0    12362 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/morphing.py
+-rw-r--r--   0        0        0    43541 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/nodes.py
+-rw-r--r--   0        0        0    35522 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/primitives.py
+-rw-r--r--   0        0        0     9440 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/real_constants.py
+-rw-r--r--   0        0        0    59811 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/sections.py
+-rw-r--r--   0        0        0    43269 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/special_purpose.py
+-rw-r--r--   0        0        0    15604 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/status.py
+-rw-r--r--   0        0        0     9685 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/superelements.py
+-rw-r--r--   0        0        0    44600 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/volumes.py
+-rw-r--r--   0        0        0       55 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/__init__.py
+-rw-r--r--   0        0        0    15305 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/generation.py
+-rw-r--r--   0        0        0     3067 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/preparation.py
+-rw-r--r--   0        0        0     1154 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/setup.py
+-rw-r--r--   0        0        0     4692 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/use_pass.py
+-rw-r--r--   0        0        0       66 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/__init__.py
+-rw-r--r--   0        0        0    26143 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/files.py
+-rw-r--r--   0        0        0     3481 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/list_controls.py
+-rw-r--r--   0        0        0     5122 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/processor_entry.py
+-rw-r--r--   0        0        0    25874 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/run_controls.py
+-rw-r--r--   0        0        0      763 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/all_others.py
+-rw-r--r--   0        0        0   157108 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/analysis_options.py
+-rw-r--r--   0        0        0     3320 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/birth_and_death.py
+-rw-r--r--   0        0        0    56005 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/dynamic_options.py
+-rw-r--r--   0        0        0    34700 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_body_loads.py
+-rw-r--r--   0        0        0    29784 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_constraints.py
+-rw-r--r--   0        0        0    15694 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_forces.py
+-rw-r--r--   0        0        0    23544 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_surface_loads.py
+-rw-r--r--   0        0        0     8378 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/gap_conditions.py
+-rw-r--r--   0        0        0    33877 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/inertia.py
+-rw-r--r--   0        0        0     8882 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/load_step_operations.py
+-rw-r--r--   0        0        0    36881 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/load_step_options.py
+-rw-r--r--   0        0        0     6753 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/master_dof.py
+-rw-r--r--   0        0        0    55158 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/miscellaneous_loads.py
+-rw-r--r--   0        0        0     4065 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_convergence_controls.py
+-rw-r--r--   0        0        0     6518 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_definition_commands.py
+-rw-r--r--   0        0        0    12413 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_global_controls.py
+-rw-r--r--   0        0        0     7669 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_interface_mapping.py
+-rw-r--r--   0        0        0     9429 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_load_transfer.py
+-rw-r--r--   0        0        0     7905 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_time_controls.py
+-rw-r--r--   0        0        0    58898 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/nonlinear_options.py
+-rw-r--r--   0        0        0    15629 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/ocean.py
+-rw-r--r--   0        0        0    10287 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/radiosity.py
+-rw-r--r--   0        0        0    12029 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/rezoning.py
+-rw-r--r--   0        0        0    18965 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_body_loads.py
+-rw-r--r--   0        0        0    18072 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_constraints.py
+-rw-r--r--   0        0        0     4405 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_forces.py
+-rw-r--r--   0        0        0    10519 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_surface_loads.py
+-rw-r--r--   0        0        0    12380 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solution_status.py
+-rw-r--r--   0        0        0    61309 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/spectrum_options.py
+-rw-r--r--   0        0        0     2435 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/twod_to_3d_analysis.py
+-rw-r--r--   0        0        0      720 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_version.py
+-rw-r--r--   0        0        0    24307 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/commands.py
+-rw-r--r--   0        0        0     4583 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/common_grpc.py
+-rw-r--r--   0        0        0    36769 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/convert.py
+-rw-r--r--   0        0        0      209 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/__init__.py
+-rw-r--r--   0        0        0    14261 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/database.py
+-rw-r--r--   0        0        0    10848 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/elems.py
+-rw-r--r--   0        0        0    16557 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/nodes.py
+-rw-r--r--   0        0        0     4532 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/docs.py
+-rw-r--r--   0        0        0     5900 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/errors.py
+-rw-r--r--   0        0        0      171 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/__init__.py
+-rw-r--r--   0        0        0     5342 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/downloads.py
+-rw-r--r--   0        0        0     1001 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/examples.py
+-rwxr-xr-x   0        0        0     1294 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm1.dat
+-rwxr-xr-x   0        0        0     1143 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm10.dat
+-rwxr-xr-x   0        0        0     2429 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm100.dat
+-rwxr-xr-x   0        0        0     2341 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm101.dat
+-rwxr-xr-x   0        0        0     2354 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm102.dat
+-rwxr-xr-x   0        0        0     3467 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm103.dat
+-rwxr-xr-x   0        0        0     2193 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm104.dat
+-rwxr-xr-x   0        0        0     1941 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm105.dat
+-rwxr-xr-x   0        0        0     1165 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm106.dat
+-rwxr-xr-x   0        0        0     1374 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm107.dat
+-rwxr-xr-x   0        0        0     1365 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm108.dat
+-rwxr-xr-x   0        0        0     1713 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm109.dat
+-rwxr-xr-x   0        0        0     1782 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm11.dat
+-rwxr-xr-x   0        0        0     2110 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm110.dat
+-rwxr-xr-x   0        0        0     1533 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm111.dat
+-rwxr-xr-x   0        0        0     1662 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm112.dat
+-rwxr-xr-x   0        0        0     1913 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm113.dat
+-rwxr-xr-x   0        0        0     2232 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm114.dat
+-rwxr-xr-x   0        0        0     1740 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm115.dat
+-rwxr-xr-x   0        0        0     2338 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm116.dat
+-rwxr-xr-x   0        0        0     4303 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm117.dat
+-rwxr-xr-x   0        0        0     3349 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm118.dat
+-rwxr-xr-x   0        0        0     4277 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm119.dat
+-rwxr-xr-x   0        0        0     2152 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm12.dat
+-rwxr-xr-x   0        0        0     2354 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm120.dat
+-rwxr-xr-x   0        0        0     5119 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm121.dat
+-rwxr-xr-x   0        0        0     1164 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm122.dat
+-rwxr-xr-x   0        0        0     1278 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm123.dat
+-rwxr-xr-x   0        0        0     1871 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm124.dat
+-rwxr-xr-x   0        0        0     2200 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm125.dat
+-rwxr-xr-x   0        0        0     2246 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm126.dat
+-rwxr-xr-x   0        0        0     2732 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm127.dat
+-rwxr-xr-x   0        0        0     1620 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm128.dat
+-rwxr-xr-x   0        0        0     2150 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm129.dat
+-rwxr-xr-x   0        0        0     1311 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm13.dat
+-rwxr-xr-x   0        0        0     2688 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm130.dat
+-rwxr-xr-x   0        0        0     1323 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm131.dat
+-rwxr-xr-x   0        0        0     1862 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm132.dat
+-rwxr-xr-x   0        0        0     1926 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm133.dat
+-rwxr-xr-x   0        0        0     4300 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm134.dat
+-rwxr-xr-x   0        0        0     1292 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm135.dat
+-rwxr-xr-x   0        0        0     4141 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm136.dat
+-rwxr-xr-x   0        0        0     1613 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm137.dat
+-rwxr-xr-x   0        0        0     1213 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm138.dat
+-rwxr-xr-x   0        0        0     5140 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm139.dat
+-rwxr-xr-x   0        0        0     1373 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm14.dat
+-rwxr-xr-x   0        0        0     2090 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm140.dat
+-rwxr-xr-x   0        0        0     9580 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm141.dat
+-rwxr-xr-x   0        0        0     3499 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm142.dat
+-rwxr-xr-x   0        0        0    14726 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm143.dat
+-rwxr-xr-x   0        0        0     7109 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm144.dat
+-rwxr-xr-x   0        0        0     1604 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm145.dat
+-rwxr-xr-x   0        0        0     2719 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm146.dat
+-rwxr-xr-x   0        0        0     2211 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm147.dat
+-rwxr-xr-x   0        0        0     2434 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm148.dat
+-rwxr-xr-x   0        0        0     9444 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm149.dat
+-rwxr-xr-x   0        0        0     3253 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm15.dat
+-rwxr-xr-x   0        0        0     3079 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm150.dat
+-rwxr-xr-x   0        0        0     1851 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm151.dat
+-rwxr-xr-x   0        0        0     2218 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm152.dat
+-rwxr-xr-x   0        0        0     3525 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm153.dat
+-rwxr-xr-x   0        0        0     1304 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm154.dat
+-rwxr-xr-x   0        0        0     2623 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm155.dat
+-rwxr-xr-x   0        0        0     2111 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm156.dat
+-rwxr-xr-x   0        0        0     2361 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm157.dat
+-rwxr-xr-x   0        0        0     1738 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm158.dat
+-rwxr-xr-x   0        0        0     1782 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm159.dat
+-rwxr-xr-x   0        0        0     3798 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm16.dat
+-rwxr-xr-x   0        0        0     1996 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm160.dat
+-rwxr-xr-x   0        0        0     1330 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm161.dat
+-rwxr-xr-x   0        0        0     1296 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm162.dat
+-rwxr-xr-x   0        0        0     1864 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm163.dat
+-rwxr-xr-x   0        0        0     1334 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm164.dat
+-rwxr-xr-x   0        0        0     2675 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm165.dat
+-rwxr-xr-x   0        0        0     5313 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm166.dat
+-rwxr-xr-x   0        0        0     6989 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm167.dat
+-rwxr-xr-x   0        0        0     3254 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm168.dat
+-rwxr-xr-x   0        0        0     3067 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm169.dat
+-rwxr-xr-x   0        0        0     4418 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm17.dat
+-rwxr-xr-x   0        0        0     1871 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm170.dat
+-rwxr-xr-x   0        0        0     6145 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm171.dat
+-rwxr-xr-x   0        0        0     3494 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm172.dat
+-rwxr-xr-x   0        0        0     2335 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm173.dat
+-rwxr-xr-x   0        0        0     3230 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm174.dat
+-rwxr-xr-x   0        0        0     7199 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm175.dat
+-rwxr-xr-x   0        0        0    10669 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm176.dat
+-rwxr-xr-x   0        0        0    13041 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm177.dat
+-rwxr-xr-x   0        0        0     2406 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm178.dat
+-rwxr-xr-x   0        0        0     3603 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm179.dat
+-rwxr-xr-x   0        0        0     2570 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm18.dat
+-rwxr-xr-x   0        0        0     1741 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm180.dat
+-rwxr-xr-x   0        0        0     1315 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm181.dat
+-rwxr-xr-x   0        0        0     2478 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm182.dat
+-rwxr-xr-x   0        0        0     2117 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm183.dat
+-rwxr-xr-x   0        0        0     8768 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm184.dat
+-rwxr-xr-x   0        0        0     7867 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm185.dat
+-rwxr-xr-x   0        0        0     7761 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm186.dat
+-rwxr-xr-x   0        0        0     4075 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm187.dat
+-rwxr-xr-x   0        0        0     3640 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm188.dat
+-rwxr-xr-x   0        0        0     2788 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm189.dat
+-rwxr-xr-x   0        0        0     2363 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm19.dat
+-rwxr-xr-x   0        0        0     4207 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm190.dat
+-rwxr-xr-x   0        0        0     8521 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm191.dat
+-rwxr-xr-x   0        0        0     1997 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm192.dat
+-rwxr-xr-x   0        0        0    19768 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm193.dat
+-rwxr-xr-x   0        0        0     1806 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm194.dat
+-rwxr-xr-x   0        0        0     2059 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm195.dat
+-rwxr-xr-x   0        0        0     4882 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm196.dat
+-rwxr-xr-x   0        0        0    10456 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm197.dat
+-rwxr-xr-x   0        0        0    11449 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm198.dat
+-rwxr-xr-x   0        0        0    16406 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm199.dat
+-rwxr-xr-x   0        0        0     1628 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm2.dat
+-rwxr-xr-x   0        0        0     1695 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm20.dat
+-rwxr-xr-x   0        0        0     5739 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm200.dat
+-rwxr-xr-x   0        0        0     6398 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm201.dat
+-rwxr-xr-x   0        0        0     2541 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm202.dat
+-rwxr-xr-x   0        0        0     2650 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm203.dat
+-rwxr-xr-x   0        0        0     3666 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm204.dat
+-rwxr-xr-x   0        0        0     4965 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm205.dat
+-rwxr-xr-x   0        0        0     2601 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm206.dat
+-rwxr-xr-x   0        0        0     3280 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm207.dat
+-rwxr-xr-x   0        0        0     1940 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm208.dat
+-rwxr-xr-x   0        0        0    12271 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm209.dat
+-rwxr-xr-x   0        0        0     2721 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm21.dat
+-rwxr-xr-x   0        0        0     9391 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm210.dat
+-rwxr-xr-x   0        0        0    10266 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm211.dat
+-rwxr-xr-x   0        0        0     6116 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm212.dat
+-rwxr-xr-x   0        0        0     7793 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm213.dat
+-rwxr-xr-x   0        0        0     2080 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm214.dat
+-rwxr-xr-x   0        0        0     1755 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm215.dat
+-rwxr-xr-x   0        0        0     2988 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm216.dat
+-rwxr-xr-x   0        0        0     2041 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm217.dat
+-rwxr-xr-x   0        0        0    11642 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm218.dat
+-rwxr-xr-x   0        0        0     3857 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm219.dat
+-rwxr-xr-x   0        0        0     1133 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm22.dat
+-rwxr-xr-x   0        0        0     5191 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm220.dat
+-rwxr-xr-x   0        0        0     2040 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm221.dat
+-rwxr-xr-x   0        0        0     2660 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm222.dat
+-rwxr-xr-x   0        0        0     5776 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm223.dat
+-rwxr-xr-x   0        0        0     3557 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm224.dat
+-rwxr-xr-x   0        0        0     3076 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm225.dat
+-rwxr-xr-x   0        0        0     3045 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm226.dat
+-rwxr-xr-x   0        0        0     2644 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm227.dat
+-rwxr-xr-x   0        0        0     6215 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm228.dat
+-rwxr-xr-x   0        0        0     6354 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm229.dat
+-rwxr-xr-x   0        0        0     6500 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm23.dat
+-rwxr-xr-x   0        0        0    13140 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm230.dat
+-rwxr-xr-x   0        0        0     7508 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm231.dat
+-rwxr-xr-x   0        0        0    12245 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm232.dat
+-rwxr-xr-x   0        0        0     3641 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm233.dat
+-rwxr-xr-x   0        0        0     2512 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm234.dat
+-rwxr-xr-x   0        0        0     3682 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm235.dat
+-rwxr-xr-x   0        0        0     5976 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm236.dat
+-rwxr-xr-x   0        0        0     6546 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm237.dat
+-rwxr-xr-x   0        0        0     3577 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm238.dat
+-rwxr-xr-x   0        0        0     7798 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm239.dat
+-rwxr-xr-x   0        0        0     1321 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm24.dat
+-rwxr-xr-x   0        0        0     2365 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm240.dat
+-rwxr-xr-x   0        0        0     8657 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm241.dat
+-rwxr-xr-x   0        0        0     3161 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm242.dat
+-rwxr-xr-x   0        0        0     2539 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm243.dat
+-rwxr-xr-x   0        0        0     2902 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm244.dat
+-rwxr-xr-x   0        0        0     3393 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm245.dat
+-rwxr-xr-x   0        0        0     6795 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm246.dat
+-rwxr-xr-x   0        0        0     7914 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm247.dat
+-rwxr-xr-x   0        0        0    21905 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm248.dat
+-rwxr-xr-x   0        0        0     7788 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm249.dat
+-rwxr-xr-x   0        0        0     3963 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm25.dat
+-rwxr-xr-x   0        0        0     7596 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm250.dat
+-rwxr-xr-x   0        0        0     8087 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm251.dat
+-rwxr-xr-x   0        0        0     4136 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm252.dat
+-rwxr-xr-x   0        0        0     3729 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm253.dat
+-rwxr-xr-x   0        0        0     8515 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm254.dat
+-rwxr-xr-x   0        0        0     4234 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm255.dat
+-rwxr-xr-x   0        0        0    13336 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm256.dat
+-rwxr-xr-x   0        0        0     8703 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm257.dat
+-rwxr-xr-x   0        0        0     7160 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm258.dat
+-rwxr-xr-x   0        0        0    20687 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm259.dat
+-rwxr-xr-x   0        0        0     5148 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm26.dat
+-rwxr-xr-x   0        0        0     8199 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm260.dat
+-rwxr-xr-x   0        0        0     5024 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm261.dat
+-rwxr-xr-x   0        0        0     3065 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm262.dat
+-rwxr-xr-x   0        0        0    26501 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm263.dat
+-rwxr-xr-x   0        0        0     7906 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm264.dat
+-rwxr-xr-x   0        0        0     5972 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm265.dat
+-rwxr-xr-x   0        0        0    10185 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm266.dat
+-rwxr-xr-x   0        0        0     5657 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm267.dat
+-rwxr-xr-x   0        0        0     3299 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm268.dat
+-rwxr-xr-x   0        0        0     2805 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm269.dat
+-rwxr-xr-x   0        0        0     1755 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm27.dat
+-rwxr-xr-x   0        0        0     4557 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm270.dat
+-rwxr-xr-x   0        0        0    15604 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm271.dat
+-rwxr-xr-x   0        0        0    20113 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm272.dat
+-rwxr-xr-x   0        0        0     5455 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm273.dat
+-rwxr-xr-x   0        0        0     3861 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm274.dat
+-rwxr-xr-x   0        0        0     8112 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm275.dat
+-rwxr-xr-x   0        0        0     3493 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm276.dat
+-rwxr-xr-x   0        0        0     2927 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm277.dat
+-rwxr-xr-x   0        0        0     3941 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm278.dat
+-rwxr-xr-x   0        0        0     8873 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm279.dat
+-rwxr-xr-x   0        0        0     2146 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm28.dat
+-rwxr-xr-x   0        0        0     5670 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm280.dat
+-rwxr-xr-x   0        0        0    11199 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm281.dat
+-rwxr-xr-x   0        0        0     5507 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm282.dat
+-rwxr-xr-x   0        0        0     4643 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm283.dat
+-rw-r--r--   0        0        0     8968 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm284.dat
+-rw-r--r--   0        0        0     3246 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm285.dat
+-rw-r--r--   0        0        0     6386 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm286.dat
+-rw-r--r--   0        0        0     4820 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm287.dat
+-rw-r--r--   0        0        0     6538 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm288.dat
+-rw-r--r--   0        0        0     4181 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm289.dat
+-rwxr-xr-x   0        0        0     4831 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm29.dat
+-rw-r--r--   0        0        0     3166 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm290.dat
+-rw-r--r--   0        0        0    10932 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm291.dat
+-rw-r--r--   0        0        0     3336 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm292.dat
+-rw-r--r--   0        0        0     4870 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm293.dat
+-rw-r--r--   0        0        0     9804 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm294.dat
+-rw-r--r--   0        0        0     4039 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm295.dat
+-rw-r--r--   0        0        0    13015 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm296.dat
+-rw-r--r--   0        0        0     3945 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm297.dat
+-rw-r--r--   0        0        0     7921 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm298.dat
+-rw-r--r--   0        0        0     2525 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm299.dat
+-rwxr-xr-x   0        0        0     1686 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm3.dat
+-rwxr-xr-x   0        0        0     2541 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm30.dat
+-rw-r--r--   0        0        0     2728 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm300.dat
+-rw-r--r--   0        0        0     3680 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm301.dat
+-rw-r--r--   0        0        0    14358 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm302.dat
+-rw-r--r--   0        0        0     7826 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm303.dat
+-rw-r--r--   0        0        0     3600 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm304.dat
+-rw-r--r--   0        0        0     2644 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm305.dat
+-rw-r--r--   0        0        0     2156 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm306.dat
+-rw-r--r--   0        0        0     1561 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm307.dat
+-rw-r--r--   0        0        0     3832 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm308.dat
+-rw-r--r--   0        0        0     2255 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm309.dat
+-rwxr-xr-x   0        0        0     3036 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm31.dat
+-rw-r--r--   0        0        0     7310 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm310.dat
+-rw-r--r--   0        0        0     8882 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm311.dat
+-rw-r--r--   0        0        0     8654 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm312.dat
+-rw-r--r--   0        0        0     4303 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm313.dat
+-rw-r--r--   0        0        0     2738 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm314.dat
+-rw-r--r--   0        0        0     4253 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm315.dat
+-rw-r--r--   0        0        0     9789 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm316.dat
+-rw-r--r--   0        0        0     6697 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm317.dat
+-rw-r--r--   0        0        0     3273 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm318.dat
+-rwxr-xr-x   0        0        0     2889 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm32.dat
+-rwxr-xr-x   0        0        0     5950 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm33.dat
+-rwxr-xr-x   0        0        0     6416 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm34.dat
+-rwxr-xr-x   0        0        0     2157 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm35.dat
+-rwxr-xr-x   0        0        0     4291 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm36.dat
+-rwxr-xr-x   0        0        0     3955 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm37.dat
+-rwxr-xr-x   0        0        0     4674 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm38.dat
+-rwxr-xr-x   0        0        0     5136 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm39.dat
+-rwxr-xr-x   0        0        0     1464 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm4.dat
+-rwxr-xr-x   0        0        0     2954 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm40.dat
+-rwxr-xr-x   0        0        0     5122 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm41.dat
+-rwxr-xr-x   0        0        0     3012 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm42.dat
+-rwxr-xr-x   0        0        0     2779 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm43.dat
+-rwxr-xr-x   0        0        0     2891 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm44.dat
+-rwxr-xr-x   0        0        0     1052 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm45.dat
+-rwxr-xr-x   0        0        0     3393 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm46.dat
+-rwxr-xr-x   0        0        0     1498 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm47.dat
+-rwxr-xr-x   0        0        0     1543 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm48.dat
+-rwxr-xr-x   0        0        0     3279 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm49.dat
+-rwxr-xr-x   0        0        0     2882 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm5.dat
+-rwxr-xr-x   0        0        0     1463 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm50.dat
+-rwxr-xr-x   0        0        0    13711 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm51.dat
+-rwxr-xr-x   0        0        0     1871 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm52.dat
+-rwxr-xr-x   0        0        0     2275 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm53.dat
+-rwxr-xr-x   0        0        0     5974 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm54.dat
+-rwxr-xr-x   0        0        0     1747 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm55.dat
+-rwxr-xr-x   0        0        0     5942 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm56.dat
+-rwxr-xr-x   0        0        0     5808 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm57.dat
+-rwxr-xr-x   0        0        0     1876 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm58.dat
+-rwxr-xr-x   0        0        0     2136 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm59.dat
+-rwxr-xr-x   0        0        0     2369 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm6.dat
+-rwxr-xr-x   0        0        0     1679 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm60.dat
+-rwxr-xr-x   0        0        0     1312 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm61.dat
+-rwxr-xr-x   0        0        0     4605 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm62.dat
+-rwxr-xr-x   0        0        0     3642 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm63.dat
+-rwxr-xr-x   0        0        0     1708 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm64.dat
+-rwxr-xr-x   0        0        0     3090 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm65.dat
+-rwxr-xr-x   0        0        0     4459 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm66.dat
+-rwxr-xr-x   0        0        0     1560 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm67.dat
+-rwxr-xr-x   0        0        0     2510 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm68.dat
+-rwxr-xr-x   0        0        0     1823 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm69.dat
+-rwxr-xr-x   0        0        0     6368 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm7.dat
+-rwxr-xr-x   0        0        0     2172 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm70.dat
+-rwxr-xr-x   0        0        0     2366 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm71.dat
+-rwxr-xr-x   0        0        0     2805 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm72.dat
+-rwxr-xr-x   0        0        0     2047 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm73.dat
+-rwxr-xr-x   0        0        0     2647 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm74.dat
+-rwxr-xr-x   0        0        0     2391 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm75.dat
+-rwxr-xr-x   0        0        0     2401 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm76.dat
+-rwxr-xr-x   0        0        0     2703 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm77.dat
+-rwxr-xr-x   0        0        0     2157 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm78.dat
+-rwxr-xr-x   0        0        0     2369 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm79.dat
+-rwxr-xr-x   0        0        0     3521 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm8.dat
+-rwxr-xr-x   0        0        0     2436 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm80.dat
+-rwxr-xr-x   0        0        0     4016 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm81.dat
+-rwxr-xr-x   0        0        0    10303 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm82.dat
+-rwxr-xr-x   0        0        0     2368 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm83.dat
+-rwxr-xr-x   0        0        0     2250 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm84.dat
+-rwxr-xr-x   0        0        0     2867 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm85.dat
+-rwxr-xr-x   0        0        0     1441 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm86.dat
+-rwxr-xr-x   0        0        0     1568 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm87.dat
+-rwxr-xr-x   0        0        0     1627 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm88.dat
+-rwxr-xr-x   0        0        0     2123 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm89.dat
+-rwxr-xr-x   0        0        0     2471 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm9.dat
+-rwxr-xr-x   0        0        0     2604 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm90.dat
+-rwxr-xr-x   0        0        0     2837 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm91.dat
+-rwxr-xr-x   0        0        0     1402 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm92.dat
+-rwxr-xr-x   0        0        0     1115 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm93.dat
+-rwxr-xr-x   0        0        0     1549 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm94.dat
+-rwxr-xr-x   0        0        0     3501 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm95.dat
+-rwxr-xr-x   0        0        0     3033 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm96.dat
+-rwxr-xr-x   0        0        0     2585 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm97.dat
+-rwxr-xr-x   0        0        0     2041 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm98.dat
+-rwxr-xr-x   0        0        0     1614 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm99.dat
+-rwxr-xr-x   0        0        0    11868 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc1.dat
+-rwxr-xr-x   0        0        0     9617 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc2.dat
+-rwxr-xr-x   0        0        0     4766 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc3.dat
+-rwxr-xr-x   0        0        0     6787 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc4.dat
+-rwxr-xr-x   0        0        0     5775 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc5.dat
+-rwxr-xr-x   0        0        0     6120 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc6.dat
+-rwxr-xr-x   0        0        0     4152 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc7.dat
+-rwxr-xr-x   0        0        0     4320 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc8.dat
+-rwxr-xr-x   0        0        0    11304 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd1.dat
+-rwxr-xr-x   0        0        0     4372 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd2.dat
+-rwxr-xr-x   0        0        0    11914 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd3.dat
+-rwxr-xr-x   0        0        0     2600 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme1.dat
+-rwxr-xr-x   0        0        0     1771 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme2.dat
+-rwxr-xr-x   0        0        0     3360 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme3.dat
+-rwxr-xr-x   0        0        0     3447 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme4.dat
+-rwxr-xr-x   0        0        0     2452 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme5.dat
+-rwxr-xr-x   0        0        0     3670 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme6.dat
+-rwxr-xr-x   0        0        0      639 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif_files.py
+-rw-r--r--   0        0        0     1455 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/wing.dat
+-rw-r--r--   0        0        0       70 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/__init__.py
+-rw-r--r--   0        0        0    20036 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/component_queries.py
+-rw-r--r--   0        0        0     2523 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/connectivity_queries.py
+-rw-r--r--   0        0        0     2973 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/core.py
+-rw-r--r--   0        0        0     5878 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/geometry_queries.py
+-rw-r--r--   0        0        0     4495 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/inline_functions.py
+-rw-r--r--   0        0        0     7220 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/line_queries.py
+-rw-r--r--   0        0        0     3021 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/nearest_queries.py
+-rw-r--r--   0        0        0     7010 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/normals_queries.py
+-rw-r--r--   0        0        0     4285 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/scalar_queries.py
+-rw-r--r--   0        0        0    16111 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/selection_queries.py
+-rw-r--r--   0        0        0     3999 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/jupyter.py
+-rw-r--r--   0        0        0    25522 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/krylov.py
+-rw-r--r--   0        0        0    61926 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/launcher.py
+-rw-r--r--   0        0        0    17789 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/licensing.py
+-rw-r--r--   0        0        0    20215 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/logging.py
+-rw-r--r--   0        0        0   149074 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl.py
+-rw-r--r--   0        0        0     7620 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_console.py
+-rw-r--r--   0        0        0    13258 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_corba.py
+-rw-r--r--   0        0        0    28656 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_geometry.py
+-rw-r--r--   0        0        0   107281 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_grpc.py
+-rw-r--r--   0        0        0      258 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_types.py
+-rwxr-xr-x   0        0        0    61110 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/math.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh/__init__.py
+-rw-r--r--   0        0        0     7707 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh/mesh.py
+-rw-r--r--   0        0        0    24709 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh_grpc.py
+-rw-r--r--   0        0        0    39484 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/misc.py
+-rw-r--r--   0        0        0    24772 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/parameters.py
+-rw-r--r--   0        0        0    37509 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/plotting.py
+-rwxr-xr-x   0        0        0    20586 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/pool.py
+-rw-r--r--   0        0        0   130584 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/post.py
+-rw-r--r--   0        0        0     8039 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/solution.py
+-rw-r--r--   0        0        0     1267 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/theme.py
+-rw-r--r--   0        0        0    16086 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/xpl.py
+-rw-r--r--   0        0        0    14064 1970-01-01 00:00:00.000000 ansys_mapdl_core-0.65.0/PKG-INFO
```

### Comparing `ansys-mapdl-core-0.64.1/LICENSE` & `ansys_mapdl_core-0.65.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/README.rst` & `ansys_mapdl_core-0.65.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 (either locally the LAN or through the internet), first ensure you
 have MAPDL started in gRPC server mode.  This example assumes that you
 are launching an instance locally from Windows, but it can be easily
 adapted to run from Linux, or the LAN provided the necessary ports are
 open. This example specifies the port with ``-port 50052``, but this
 option can be left out if you plan on using the default port 50052.
 
-.. code:: pwsh
+.. code:: pwsh-session
 
     start "MAPDL" "%ANSYS211_DIR%\bin\winx64\ANSYS211.exe" -port 50052 -grpc
 
 Next, connect to the instance of MAPDL from python with:
 
 .. code:: pycon
```

### Comparing `ansys-mapdl-core-0.64.1/pyproject.toml` & `ansys_mapdl_core-0.65.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mapdl-core"
-version = "0.64.1"
+version = "0.65.0"
 description = "A Python wrapper for Ansys MAPDL."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ansys, Inc.", email = "pyansys.maintainers@ansys.com"},
 ]
@@ -18,27 +18,29 @@
 ]
 dependencies = [
     "ansys-api-mapdl==0.5.1",  # supports at least 2020R2 - 2022R1
     "ansys-corba; python_version < '3.9'",
     "ansys-mapdl-reader>=0.51.7",
     "ansys-platform-instancemanagement~=1.0",
     "appdirs>=1.4.0",
+    "click>=8.1.3", # for CLI interface
     "grpcio>=1.30.0",  # tested up to grpcio==1.35
     "importlib-metadata>=4.0",
     "matplotlib>=3.0.0",  # for colormaps for pyvista
     "numpy>=1.14.0",
     "pexpect>=4.8.0 ; platform_system=='Linux'",
     "protobuf>=3.12.2",  # minimum required based on latest ansys-grpc-mapdl
-    "pyiges>=0.1.4",
+    "psutil>=5.9.4",
     "pyansys-tools-versioning>=0.3.3",
+    "ansys-tools-path>=0.2.4",
+    "pyiges>=0.1.4",
     "pyvista>=0.33.0",
     "scipy>=1.3.0",  # for sparse (consider optional?)
     "tqdm>=4.45.0",
-    "click>=8.1.3", # for CLI interface
-    "psutil>=5.9.4",
+    "vtk>=9.0.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
@@ -49,60 +51,59 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "ansys-dpf-core==0.8.0",
+    "ansys-dpf-core==0.8.1",
     "autopep8==2.0.2",
     "matplotlib==3.7.1",
     "scipy==1.10.1",
-    "pandas==2.0.0",
-    "pytest==7.2.2",
-    "pytest-cov==4.0.0",
-    "pyvista==0.38.5",
+    "pandas==2.0.1",
+    "pytest==7.3.1",
+    "pytest-cov==4.1.0",
+    "pyvista==0.39.1",
     "pyansys-tools-report==0.5.0",
     "vtk==9.2.6",
     "pytest-rerunfailures==11.1.2",
 ]
 doc = [
-    "sphinx==5.3.0",
-    "ansys-dpf-core==0.8.0",
-    "ansys-mapdl-reader==0.52.11",
-    "ansys-sphinx-theme==0.9.6",
+    "sphinx==6.2.1",
+    "ansys-dpf-core==0.8.1",
+    "ansys-mapdl-reader==0.52.13",
+    "ansys-sphinx-theme==0.9.9",
     "grpcio==1.51.1",
     "imageio-ffmpeg==0.4.8",
-    "imageio==2.27.0",
+    "imageio==2.30.0",
     "jupyter_sphinx==0.4.0",
     "jupyterlab>=3.2.8",
     "matplotlib==3.7.1",
     "numpydoc==1.5.0",
-    "pandas==2.0.0",
-    "plotly==5.14.0",
+    "pandas==2.0.1",
+    "plotly==5.14.1",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pythreejs==2.4.2",
-    "pyvista==0.38.5",
+    "pyvista==0.39.1",
     "sphinx-autobuild==2021.3.14",
-    "sphinx-autodoc-typehints==1.22",
-    "sphinx-copybutton==0.5.1",
-    
-    "sphinx-gallery==0.12.2",
+    "sphinx-autodoc-typehints==1.23.0",
+    "sphinx-copybutton==0.5.2",
+    "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "sphinxemoji==0.2.0",
     "vtk==9.2.6",
 ]
 
 [tool.flit.module]
 name = "ansys.mapdl.core"
 
 [project.urls]
-Source = "https://github.com/pyansys/pymapdl"
+Source = "https://github.com/ansys/pymapdl"
 
 [project.scripts]
 pymapdl_convert_script = "ansys.mapdl.core.convert:cli"
 
 [tool.pytest.ini_options]
 junit_family = "legacy"
 filterwarnings = [
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/__init__.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # Importing logging
 import logging
 import os
 
 import appdirs
 
+# Setup data directory
+USER_DATA_PATH = appdirs.user_data_dir(appname="ansys_mapdl_core", appauthor="Ansys")
+if not os.path.exists(USER_DATA_PATH):  # pragma: no cover
+    os.makedirs(USER_DATA_PATH)
+
+EXAMPLES_PATH = os.path.join(USER_DATA_PATH, "examples")
+if not os.path.exists(EXAMPLES_PATH):  # pragma: no cover
+    os.makedirs(EXAMPLES_PATH)
+
+
 from ansys.mapdl.core.logging import Logger
 
 LOG = Logger(level=logging.ERROR, to_file=False, to_stdout=True)
 LOG.debug("Loaded logging module as LOG")
 
 _LOCAL_PORTS = []
 
-LINUX_DEFAULT_DIRS = [["/", "usr", "ansys_inc"], ["/", "ansys_inc"]]
-LINUX_DEFAULT_DIRS = [os.path.join(*each) for each in LINUX_DEFAULT_DIRS]
 
 # Per contract with Sphinx-Gallery, this method must be available at top level
 try:
     from pyvista.utilities.sphinx_gallery import _get_sg_image_scraper
 
     _HAS_PYVISTA = True
 except ModuleNotFoundError:  # pragma: no cover
@@ -26,52 +34,41 @@
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:  # pragma: no cover
     import importlib_metadata
 
 __version__ = importlib_metadata.version(__name__.replace(".", "-"))
 
-from ansys.mapdl.core import examples
-from ansys.mapdl.core._version import SUPPORTED_ANSYS_VERSIONS
-from ansys.mapdl.core.convert import convert_apdl_block, convert_script
-from ansys.mapdl.core.launcher import (
+
+from ansys.tools.path.path import (
     change_default_ansys_path,
-    close_all_local_instances,
     find_ansys,
     get_ansys_path,
     get_available_ansys_installations,
     save_ansys_path,
 )
 
+from ansys.mapdl.core import examples
+from ansys.mapdl.core._version import SUPPORTED_ANSYS_VERSIONS
+from ansys.mapdl.core.convert import convert_apdl_block, convert_script
+from ansys.mapdl.core.launcher import close_all_local_instances
+
 # override default launcher when on pyansys.com
 if "ANSJUPHUB_VER" in os.environ:  # pragma: no cover
     from ansys.mapdl.core.jupyter import launch_mapdl_on_cluster as launch_mapdl
 else:
     from ansys.mapdl.core.launcher import launch_mapdl
 
 from ansys.mapdl.core.mapdl_grpc import MapdlGrpc as Mapdl
 from ansys.mapdl.core.misc import Information, Report, _check_has_ansys
 from ansys.mapdl.core.pool import LocalMapdlPool
 from ansys.mapdl.core.theme import MapdlTheme
 
 _HAS_ANSYS = _check_has_ansys()
 
-# Setup data directory
-try:
-    USER_DATA_PATH = appdirs.user_data_dir("ansys_mapdl_core")
-    if not os.path.exists(USER_DATA_PATH):  # pragma: no cover
-        os.makedirs(USER_DATA_PATH)
-
-    EXAMPLES_PATH = os.path.join(USER_DATA_PATH, "examples")
-    if not os.path.exists(EXAMPLES_PATH):  # pragma: no cover
-        os.makedirs(EXAMPLES_PATH)
-
-except:  # pragma: no cover
-    pass
-
 BUILDING_GALLERY = False
 RUNNING_TESTS = False
 
 VERSION_MAP = {
     (0, 0, 0): "2020R2",
     (0, 3, 0): "2021R1",
     (0, 4, 0): "2021R2",
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/abbreviations.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/abbreviations.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/array_param.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/array_param.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/macro_files.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/macro_files.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/matrix_op.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/matrix_op.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/parameter_definition.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/apdl/process_controls.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/process_controls.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux12_/general_radiation.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/general_radiation.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux12_/radiation_mat.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/radiation_mat.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux12_/radiosity_solver.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/radiosity_solver.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux15_.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux15_.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux2_/bin_dump.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/bin_dump.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux2_/bin_manip.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/bin_manip.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/aux3_.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux3_.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/conn.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/conn.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/components.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/components.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/coord_sys.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/coord_sys.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/picking.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/picking.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/selecting.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/selecting.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/setup.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/database/working_plane.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/working_plane.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/display_/setup.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/display_/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/annotation.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/annotation.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/graphs.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/graphs.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/labeling.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/labeling.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/scaling.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/scaling.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/setup.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/style.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/style.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/graphics_/views.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/views.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/hidden.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/hidden.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/inq_func.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/inq_func.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/map_cmd.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/map_cmd.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/misc/misc.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/misc/misc.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/parse.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/parse.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/animation.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/animation.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/controls.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/controls.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/element_table.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/element_table.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/failure_criteria.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/failure_criteria.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/listing.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/listing.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/load_case.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/load_case.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/magnetics_calc.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/magnetics_calc.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/path_operations.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/path_operations.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/results.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/results.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/setup.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/special.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/special.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/status.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/status.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/surface_operations.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/surface_operations.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post1_/trace_points.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/trace_points.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/controls.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/controls.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/display.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/display.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/listing.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/listing.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/operations.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/operations.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/setup.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/special.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/special.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/post26_/status.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/status.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/areas.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/areas.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/artificially_matched_layers.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/artificially_matched_layers.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/booleans.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/booleans.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/constraint_equations.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/constraint_equations.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/coupled_dof.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/coupled_dof.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/database.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/database.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/digitizing.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/digitizing.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/element_type.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/element_type.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/elements.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/elements.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/explicit_dynamics.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/explicit_dynamics.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/hard_points.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/hard_points.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/keypoints.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/keypoints.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/lines.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/lines.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/material_data_tables.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/material_data_tables.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/materials.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/materials.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/meshing.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/meshing.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/morphing.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/morphing.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/nodes.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/nodes.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/primitives.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/primitives.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/real_constants.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/real_constants.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/sections.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/sections.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/special_purpose.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/special_purpose.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/status.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/status.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/superelements.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/superelements.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/preproc/volumes.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/volumes.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/generation.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/generation.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/preparation.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/preparation.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/setup.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/reduced/use_pass.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/use_pass.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/files.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/files.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/list_controls.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/list_controls.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/processor_entry.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/processor_entry.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/session/run_controls.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/run_controls.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/__init__.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/analysis_options.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/analysis_options.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/birth_and_death.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/birth_and_death.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/dynamic_options.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/dynamic_options.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/fe_body_loads.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_body_loads.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/fe_constraints.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_constraints.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/fe_forces.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_forces.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/fe_surface_loads.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_surface_loads.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/gap_conditions.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/gap_conditions.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/inertia.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/inertia.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/load_step_operations.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/load_step_operations.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/load_step_options.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/load_step_options.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/master_dof.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/master_dof.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/miscellaneous_loads.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/miscellaneous_loads.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_convergence_controls.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_convergence_controls.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_definition_commands.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_definition_commands.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_global_controls.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_global_controls.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_interface_mapping.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_interface_mapping.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_load_transfer.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_load_transfer.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_time_controls.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_time_controls.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/nonlinear_options.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/nonlinear_options.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/ocean.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/ocean.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/radiosity.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/radiosity.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/rezoning.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/rezoning.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solid_body_loads.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_body_loads.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solid_constraints.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_constraints.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solid_forces.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_forces.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solid_surface_loads.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_surface_loads.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/solution_status.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solution_status.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/spectrum_options.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/spectrum_options.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_commands/solution/twod_to_3d_analysis.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/twod_to_3d_analysis.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/_version.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/commands.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,18 @@
 str
     Str object with the command console output.
 
     This object also has the extra methods:
     :meth:`to_list() <ansys.mapdl.core.commands.CommandListingOutput.to_list>`,
     :meth:`to_array() <ansys.mapdl.core.commands.CommandListingOutput.to_array>` (only on listing commands) and
     :meth:`to_dataframe() <ansys.mapdl.core.commands.CommandListingOutput.to_dataframe>` (only if Pandas is installed).
-
+    |bl|
+    **NOTE**: If you use these methods, you might
+    obtain a lower precision than using :class:`Mesh <ansys.mapdl.core.mesh_grpc.MeshGrpc>` methods.
+    |bl|
     For more information visit :ref:`user_guide_postprocessing`.
 
 """
 
 XSEL_DOCSTRING_INJECTION = r"""
 Returns
 -------
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/common_grpc.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/common_grpc.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/convert.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/convert.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/database/database.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from functools import wraps
 import os
 import time
 from warnings import warn
 import weakref
 
 from ansys.api.mapdl.v0 import mapdl_db_pb2_grpc
+from ansys.tools.versioning import server_meets_version
 import grpc
 
 from ansys.mapdl.core.errors import MapdlConnectionError
 
 from ..mapdl_grpc import MapdlGrpc
 
-VALID_MAPDL_VERSIONS = [21.1, 21.2, 22.1, 22.2]
+MINIMUM_MAPDL_VERSION = "21.1"
 
 
 class WithinBeginLevel:
 
     """Context manager to run MAPDL within the being level."""
 
     def __init__(self, mapdl):
@@ -213,15 +214,17 @@
             raise ImportError(
                 "Please upgrade the 'ansys.api.mapdl' package to at least v0.5.1."
                 "You can use 'pip install ansys-api-mapdl --upgrade"
             )
 
         ## Checking MAPDL versions
         mapdl_version = self._mapdl.version
-        if mapdl_version not in VALID_MAPDL_VERSIONS:  # pragma: no cover
+        if not server_meets_version(
+            str(mapdl_version), MINIMUM_MAPDL_VERSION
+        ):  # pragma: no cover
             from ansys.mapdl.core.errors import MapdlVersionError
 
             raise MapdlVersionError(
                 f"This MAPDL version ({mapdl_version}) is not compatible with the Database module."
                 "Please check the online documentation regarding Database Module at 'mapdl.docs.pyansys.com'."
             )
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/database/elems.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/elems.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/database/nodes.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/nodes.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/errors.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/downloads.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/examples.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/examples.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm1.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm1.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM1
 /PREP7
 /TITLE, VM1, STATICALLY INDETERMINATE REACTION FORCE ANALYSIS
 C***      STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 26, PROB.10
 ANTYPE,STATIC                  ! STATIC ANALYSIS
 ET,1,LINK180
 SECTYPE,1,LINK
@@ -14,24 +14,28 @@
 N,4,,10
 E,1,2                          ! DEFINE ELEMENTS
 EGEN,3,1,1
 D,1,ALL,,,4,3                  ! BOUNDARY CONDITIONS AND LOADING
 F,2,FY,-500
 F,3,FY,-1000
 FINISH
+/OUT,SCRATCH
 /SOLU    
 OUTPR,BASIC,1
 OUTPR,NLOAD,1
 SOLVE
 FINISH
+/OUT
 /POST1
 NSEL,S,LOC,Y,10
+ESLN
 FSUM
 *GET,REAC_1,FSUM,,ITEM,FY
 NSEL,S,LOC,Y,0
+ESLN
 FSUM
 *GET,REAC_2,FSUM,,ITEM,FY
 
 *DIM,LABEL,CHAR,2
 *DIM,VALUE,,2,3
 LABEL(1) = 'R1, lb','R2, lb '
 *VFILL,VALUE(1,1),DATA,900.0,600.0
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm10.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm10.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM10
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM10, BENDING OF A TEE SHAPED BEAM
 C***    MECHANICS OF SOLIDS, CRANDALL AND DAHL, 1959, PAGE 294, EX. 7.2
 ANTYPE,STATIC
 ET,1,BEAM188,,,3
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm100.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm100.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /SHOW,JPEG
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /VERIFY,VM100
 /PREP7      
 /TITLE, VM100, HEAT CONDUCTION ACROSS A CHIMNEY SECTION
 C***       PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 102, EX. 3-4
 ANTYPE,STATIC                ! THERMAL ANALYSIS
@@ -22,16 +22,18 @@
 OUTPR,VENG,NONE
 NSEL,S,LOC,X
 SF,ALL,CONV,12,100           ! INNER CONVECTION SURFACE
 NSEL,S,LOC,X,1
 SF,ALL,CONV,3,0              ! OUTER CONVECTION SURFACE
 NSEL,ALL
 FINISH
-/SOLU    
+/SOLU
+/OUT,vm100_SCRATCH    
 SOLVE
+/OUT
 FINISH
 /POST1
 PRNSOL,TEMP                  ! PRINT NODAL TEMPERATURES
 ESEL,S,ELEM,,1,3,2           ! SELECT ELEMENTS 1 AND 3
 FSUM                         ! PERFORM FORCE AND MOMENT SUMMATIONS
 *GET,HT13,FSUM,,ITEM,HEAT    ! ADD HEAT FLOW RATES OF ELEMENTS 1 AND 3
 HEAT=HT13*8                  ! COMPUTE TOTAL HEAT FLOW RATE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm101.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm101.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM101
 /PREP7
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM101, TEMPERATURE DISTRIBUTION IN A SHORT SOLID CYLINDER
 C***    CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 134, FIG. 6-7
 ANTYPE,STATIC
@@ -22,16 +22,18 @@
 EGEN,4,10,1,4
 OUTPR,,1
 D,1,TEMP,,,10               ! APPLY TEMPERATURES
 D,15,TEMP,,,40,5
 D,41,TEMP,40,,50
 NUMMRG,NODE                 ! MERGE COINCIDENT NODE NUMBERS
 FINISH
-/SOLU    
+/SOLU
+/OUT,vm101_SCRATCH    
 SOLVE
+/OUT
 FINISH
 /POST1
 /VIEW,,,-1
 !/DEVICE,VECTOR,ON
 PLNSOL,TEMP
 CSYS,1
 NSEL,S,LOC,X,0
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm102.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm102.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM102
 /PREP7
 /TITLE, VM102, CYLINDER WITH TEMPERATURE DEPENDENT CONDUCTIVITY
 C***    CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 166, ART. 7-9
 ANTYPE,STATIC
 ET,1,PLANE55,,,1                   ! AXISYMMETRIC OPTION
 MP,KXX,1,50                        ! CONSTANT CONDUCTIVITY
@@ -13,16 +13,18 @@
 E,1,2,12,11
 EGEN,5,1,1
 OUTPR,,1
 KBC,1                              ! STEP BOUNDARY CONDITIONS
 D,1,TEMP,100,,11,10
 D,6,TEMP,,,16,10
 FINISH
-/SOLU    
+/SOLU 
+/OUT,vm102_SCRATCH   
 SOLVE
+/OUT
 FINISH
 /POST1
 SET,1
 NSEL,S,LOC,Y
 PRNSOL,TEMP                        ! RADIAL TEMPERATURES FOR CONSTANT K
 *GET,TN2,NODE,2,TEMP
 *GET,TN3,NODE,3,TEMP
@@ -38,15 +40,17 @@
 NSEL,ALL
 FINISH
 
 /PREP7
 MP,KXX,1,50,0.5                    ! TEMPERATURE-DEPENDENT CONDUCTIVITY
 FINISH
 /SOLU
+/OUT,vm102_SCRATCH,,,APPEND  
 SOLVE
+/OUT
 FINISH
 /POST1
 SET,1
 NSEL,S,LOC,Y
 PRNSOL,TEMP                        ! RADIAL TEMPERATURES FOR K(T)
 *GET,TN2,NODE,2,TEMP
 *GET,TN3,NODE,3,TEMP
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm103.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm103.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM103
 /PREP7
 /TITLE, VM103, THIN PLATE WITH CENTRAL HEAT SOURCE
 C*** CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 173, ART. 8-1
 C*** USING SHELL131 ELEMENTS
 ANTYPE,STATIC              ! THERMAL ANALYSIS
 ET,1,SHELL131,,,2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm104.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm104.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM104  
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 SMRT,OFF
 /TITLE, VM104, LIQUID-SOLID PHASE CHANGE
 C***    DANTZIG,J.A., IJNME, VOL 28, 1989, PAGE 1773-1775.
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm105.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm105.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM105
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 /TITLE, VM105, HEAT GENERATING COIL WITH TEMP. DEPENDENT CONDUCTIVITY
 C***    CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 193, ART. 8-8
 ANTYPE,STATIC
@@ -17,16 +17,18 @@
 EGEN,9,1,1
 OUTPR,BASIC,1
 KBC,1                        ! STEP LOAD
 D,1,TEMP,0,,11,10            ! INNER WALL TEMPERATURE
 D,10,TEMP,0,,20,10           ! OUTER WALL TEMPERATURE
 BFE,ALL,HGEN,,1E6            ! APPLY HEAT GENERATION RATES
 FINISH
-/SOLU    
+/SOLU
+/OUT,vm105_SCRATCH    
 SOLVE
+/OUT
 FINISH
 /POST1
 CSYS,1
 NSEL,S,LOC,Y,-5              ! SELECT NODES ALONG RADIUS AT THETA=-5
 PRNSOL,TEMP                  ! PRINT TEMPERATURE DISTRIBUTION
 NSEL,S,NODE,,ALL
 PATH,TPATH,2,,48             ! DEFINE PATH WITH NAME = "TPATH"
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm106.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm106.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM106
 /PREP7
 /TITLE, VM106, RADIANT ENERGY EMISSION
 C***   PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 22, PROB. 1-8(B)
 ANTYPE,STATIC                   ! THERMAL ANALYSIS
 ET,1,LINK31
 R,1,144,1,1
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm107.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm107.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM107
 /PREP7
 /TITLE, VM107, THERMOCOUPLE RADIATION
 C***    HEAT TRANSFER, CHAPMAN, 1ST. PRINTING, PAGE 396, ART. 13.5
 ANTYPE,STATIC         ! STATIC ANALYSIS
 ET,1,LINK34
 ET,2,LINK31
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm108.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm108.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM108
 /PREP7
 /TITLE, VM108, TEMPERATURE GRADIENT ACROSS A SOLID CYLINDER
 C***    HILDEBRAND, ADVANCED CALCULUS, PAGE 447, EQUATIONS 38-44
 ANTYPE,STATIC
 ET,1,PLANE75            ! AXISYMMETRIC HARMONIC THERMAL SOLID
 MP,KXX,1,1
@@ -12,16 +12,18 @@
 NGEN,2,5,1,5,1,,5       ! AXIAL LENGTH IS ARBITRARY
 E,1,2,7,6               ! FOUR ELEMENTS ALONG RADIUS AT THETA=0
 EGEN,4,1,1
 OUTPR,BASIC,1
 MODE,1,1                ! ANTISYMMETRIC MODE (ISYM=1)
 D,5,TEMP,80,,10,5       ! DEFINE PEAK TEMPERATURE
 FINISH
-/SOLU    
+/SOLU
+/OUT,vm108_SCRATCH    
 SOLVE
+/OUT
 FINISH
 /POST1
 *GET,TN1,NODE,1,TEMP
 *GET,TN2,NODE,2,TEMP
 *GET,TN3,NODE,3,TEMP
 *GET,TN4,NODE,4,TEMP
 *DIM,VALUE,,4,3
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm109.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm109.dat`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM109
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 /TITLE, VM109, TEMPERATURE RESPONSE OF A SUDDENLY COOLED WIRE
 C***    PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 120, EX. 4-1
 ANTYPE,TRANS            ! THERMAL ANALYSIS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm11.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm11.dat`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM11
 /PREP7
 /TITLE, VM11, RESIDUAL STRESS PROBLEM
 C***           MECHANICS OF SOLIDS, CRANDALL AND DAHL, 1959, PAGE 234, PROB 5.31
 ANTYPE,STATIC
 ET,1,LINK180
 SECTYPE,1,LINK   
 SECDATA,1
 MP,EX,1,30E6
-TB,BKIN                           ! TABLE FOR BILINEAR KINEMATIC HARDENING
+TB,PLAS,1,,,BKIN                  ! TABLE FOR BILINEAR KINEMATIC HARDENING
 TBTEMP,100                        
 TBDATA,1,30000                    ! YIELD STRESS
 C*** DEFINE MODEL GEOMETRY USING PARAMETRIC EXPRESSIONS
 L=100
 *AFUN,DEG                         ! SET ANGULAR FUNCTION ARGUMENTS AND
                                   ! RESULTS TO DEGREES
 THETA=30
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm110.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm110.dat`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM110
 /PREP7
 /TITLE, VM110, TRANSIENT TEMPERATURE DISTRIBUTION IN A SLAB
 C***    PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 140, EX. 4-4
 ANTYPE,TRANS              ! TRANSIENT ANALYSIS
 ET,1,LINK33               ! HEAT CONDUCTING BAR
 ET,2,LINK34               ! CONVECTION LINK
@@ -26,15 +26,17 @@
 NSUBST,80
 BFUNIF,TEMP,100
 D,12,TEMP,1600
 KBC,1                     ! STEP BOUNDARY CONDITION
 AUTOTS,ON
 OUTPR,BASIC,LAST
 TINTPAR,,,,0.5             ! USE CENTRAL DIFFERENCE
+/OUT,vm110_SCRATCH
 SOLVE
+/OUT
 FINISH
 /POST26
 ESOL,2,11,,SMISC,1,HEAT   ! HEAT RATE FOR ELEMENT 11
 INT1,3,2,1,,TOTAL_HT      ! INTEGRATE HEAT RATE OVER TIME SPAN
 PRVAR,2,3
 *GET,QTOT,VARI,3,RTIME,14.5
 FINISH
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm111.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm111.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM111
 /PREP7
 /TITLE, VM111, COOLING OF A SPHERICAL BODY
 !       PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 143, EX. 4-5
 !       USING PLANE55 ELEMENTS (QUAD. ELEMENTS)
 ANTYPE,TRANS
 ET,1,PLANE55,,,1      ! AXISYMMETRIC ELEMENTS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm112.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm112.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM112
 /PREP7
 /TITLE, VM112, COOLING OF A SPHERICAL BODY
 C***       PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 143, EX. 4-5
 C***       USING PLANE77 ELEMENTS (MULTI-NODE ELEMENTS)
 ANTYPE,TRANS                    ! THERMAL ANALYSIS
 ET,1,PLANE77,,,1                ! AXISYMMETRIC ELEMENTS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm113.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm113.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM113
 /PREP7
 smrt,off
 /TITLE, VM113, TRANSIENT TEMP. DISTRIBUTION IN AN ORTHOTROPIC METAL BAR
 C***    CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 261, EX. 10-7
 ANTYPE,TRANS
 ET,1,PLANE55               ! THERMAL SOLID
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm114.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm114.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM114
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 /TITLE, VM114, TEMPERATURE RESPONSE TO A LINEARLY RISING SURFACE TEMPERATURE
 C***    CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 274, ART 11-2
 ANTYPE,TRANS
@@ -14,22 +14,25 @@
 K,1
 K,2,.3              ! LENGTH OF MODEL FROM SURFACE
 L,1,2
 LESIZE,1,,,8,3      ! NON-UNIFORM MESH WITH 8 DIVISIONS
 LMESH,1
 FINISH
 /SOLU    
-SOLCONTROL,0
 AUTOTS,ON
 OUTPR,,LAST 
 OUTRES,,ALL
 TIME,(2/60)         ! TIME PERIOD OF 2 MIN. CONVERTED TO HR.
-NSUBST,20
+NSUBST,20,20,1
 DK,1,TEMP,120       ! TEMPERATURE SPECIFICATION AT KEY POINT 1
+KBC,0
+TINTP,,,,0.5,0.5,0.2,,,
+/OUT,vm114_SCRATCH
 SOLVE
+/OUT
 FINISH
 /POST26
 NSOL,2,1,TEMP       ! TEMPERATURE HISTORY AT NODES NEAR SURFACE
 NSOL,3,3,TEMP
 NSOL,4,4,TEMP
 NSOL,5,5,TEMP
 NSOL,6,6,TEMP
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm115.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm115.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM115
 /PREP7
 /TITLE, VM115, THERMAL RESPONSE OF A HEAT GENERATING SLAB
 C***    CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 283, EQN 11-21
 ANTYPE,TRANS
 ET,1,LINK33        ! HEAT CONDUCTING BAR
 R,1,1
@@ -19,16 +19,19 @@
 TIME,(12/60)       ! CONVERT 12 MIN TO HRS
 DELTIM,0.01
 BFUNIF,TEMP,60     ! INITIAL UNIFORM TEMPERATURE
 KBC,1              ! APPLY STEP LOADS
 DK,1,TEMP,32       ! SURFACE TEMPERATURE APPLIED TO KEYPOINT 1
 BFK,ALL,HGEN,4E4   ! HEAT GENERATION SPECIFIED AT KEYPOINTS 1 & 2
 FINISH
+/OUT,SCRATCH
 /SOLU    
 SOLVE
+FINI
+/OUT
 /POST1
 *GET,TN1,NODE,1,TEMP
 *GET,TN3,NODE,3,TEMP
 *GET,TN4,NODE,4,TEMP
 *GET,TN5,NODE,5,TEMP
 *GET,TN6,NODE,6,TEMP
 *GET,TN2,NODE,2,TEMP
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm116.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm116.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM116
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7 
 /TITLE, VM116, HEAT CONDUCTING PLATE WITH SUDDEN COOLING
 C***    PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 161, EX. 4-11
 ANTYPE,TRANS
@@ -25,23 +25,27 @@
 /SOLU    
 D,2,TEMP,500       ! INITIAL SURFACE TEMPERATURES
 D,10,TEMP,100
 OUTPR,,LAST 
 OUTRES,,ALL
 TIMINT,OFF         ! TURN OFF TIME INTEGRATION FOR
 TIME,0.001         !  INITIAL STEADY-STATE CONDITION
+/OUT,vm116_SCRATCH
 SOLVE
+/OUT
 TIMINT,ON          ! TURN ON TIME INTEGRATION ON FOR
 TIME,7             !  TRANSIENT OVER 7 HRS
 DDELE,2,TEMP       ! DELETE NODAL TEMPERATURE
 D,1,TEMP,100       ! ENVIRONMENT TEMPERATURE IS DECREASED
 KBC,1              !  SUDDENLY
 AUTOTS,ON
 NSUBST,20
+/OUT,vm116_SCRATCH,,,APPEND
 SOLVE
+/OUT
 FINISH
 
 /POST26
 NSOL,2,2,TEMP
 PRVAR,2            ! PRINT TEMPERATURE HISTORY AT NODE 2
 /AXLAB,Y,TEMP
 /GRID,1
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm117.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm117.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM117
 /PREP7
 /TITLE, VM117, ELECTRIC CURRENT FLOWING IN A NETWORK
 C*** BASIC ELECTRICAL ENGR, FITZGERALD AND HIGGIN BOTHAM, 2ND ED, P. 22, EX. 1-11
 ANTYPE,STATIC
 ET,1,LINK68              ! THERMAL-ELECTRICAL LINE ELEMENT
 MP,RSVX,1,1              ! UNIT RESISTIVITY
@@ -26,17 +26,19 @@
 KBC,1                    ! STEP BOUNDARY CONDITIONS
 D,4,VOLT,100             ! NODAL VOLTAGE
 D,1,VOLT,0               ! GROUND NODE
 OUTPR,ALL,1 
 OUTPR,VENG,NONE
 FINISH
 /SOLU    
+/OUT,SCRATCH
 SOLVE
 FINISH
 /POST1
+/OUT,
 ETABLE,CUR,NMISC,5
 PRETAB,CUR               ! PRINT CURRENT FOR ALL BRANCHES
 *GET,I42,ELEM,4,ETAB,CUR ! CURRENT IN BRANCH 4-2
 *GET,I43,ELEM,5,ETAB,CUR ! CURRENT IN BRANCH 4-3
 I14=I42+I43              ! CURRENT THROUGH BATTERY (BRANCH 1-4)
 *GET,I21,ELEM,1,ETAB,CUR
 *GET,I31,ELEM,2,ETAB,CUR
@@ -87,17 +89,19 @@
 E,4,1,5
 KBC,1                    ! STEP BOUNDARY CONDITIONS
 D,1,VOLT,0               ! GROUND NODE
 OUTPR,ALL,1 
 OUTPR,VENG,NONE
 FINISH
 /SOLU    
+/OUT,SCRATCH
 SOLVE
 FINISH
 /POST1
+/OUT,
 ETABLE,CUR,SMISC,2
 PRETAB,CUR               ! PRINT CURRENT FOR ALL BRANCHES
 *GET,I42,ELEM,4,ETAB,CUR ! CURRENT IN BRANCH 4-2
 *GET,I43,ELEM,5,ETAB,CUR ! CURRENT IN BRANCH 4-3
 I14=I42+I43              ! CURRENT THROUGH BATTERY (BRANCH 1-4)
 *GET,I21,ELEM,1,ETAB,CUR
 *GET,I31,ELEM,2,ETAB,CUR
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm118.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm118.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM118
 /PREP7
 /TITLE, VM118, CENTERLINE TEMP. OF A HEAT GENERATING WIRE
 C***      HEAT, MASS AND MOMENTUM TRANS., ROHSENOW AND CHOI, 2ND. PR., PAGE 106,
 C***      EX. 6.5, USING PLANE55 ELEMENTS (PLANE ELEMENTS)
 ANTYPE,STATIC                 ! THERMAL ANALYSIS
 ET,1,PLANE55
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm119.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm119.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM119
 /PREP7
 /TITLE, VM119, CENTERLINE TEMP. OF AN ELECTRICAL WIRE
 C***      HEAT, MASS AND MOMENTUM TRANS., ROHSENOW AND CHOI, 2ND. PR., PAGE 106,
 C***      USING PLANE223 ELEMENTS (PLANE ELEMENTS)
 !
 ANTYPE,STATIC                 ! THERMAL (ELECTRICAL) ANALYSIS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm12.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm12.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM12
 /PREP7
 /SHOW,JPEG
 /TITLE, VM12, COMBINED BENDING AND TORSION
 C***      USING PIPE16     STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 299, PROB. 2
 
 ANTYPE,STATIC
@@ -15,69 +15,66 @@
 E,1,2
 D,1,ALL
 F,2,MZ,9000
 F,2,FX,-250
 FINISH
 /SOLU    
 OUTPR,BASIC,1
+/OUT,SCRATCH
 SOLVE
 FINISH
 /POST1
 ETABLE,P_STRS,NMISC,86
 ETABLE,SHR,NMISC,88
+/OUT,
 *GET,P_STRESS,ELEM,1,ETAB,P_STRS
 *GET,SHEAR,ELEM,1,ETAB,SHR
-
 *DIM,LABEL,CHAR,2,2
 *DIM,VALUE,,2,3
 LABEL(1,1) = 'MAX PRIN','MAX SH S'
 LABEL(1,2) = 'STRS psi','TRS psi '
 *VFILL,VALUE(1,1),DATA,7527,3777
 *VFILL,VALUE(1,2),DATA,P_STRESS,(SHEAR/2)
 *VFILL,VALUE(1,3),DATA,ABS(P_STRESS/7527 ) ,ABS((SHEAR/2)/3777 )
 SAVE,TABLE_1
 FINI
 /CLEAR,NOSTART
 
-
-!*********************************************************************
-
-
 /PREP7
 /SHOW,JPEG
 C***     USING PIPE288       
-
 ANTYPE,STATIC
-ET,1,PIPE288
+ET,1,PIPE288,,,,2
 SECTYPE,1,PIPE
 SECDATA,4.67017,2.33508
 KEYOPT,1,3,3			!CUBIC SHAPE FUNCTION
 MP,EX,1,30E6
 MP,NUXY,1,.3
 N,1
 N,2,,,300
 E,1,2
 D,1,ALL
 F,2,MZ,9000
 F,2,FX,-250
 FINISH
 /SOLU    
 OUTPR,BASIC,1
+/OUT,SCRATCH
 SOLVE
 FINISH
 /POST1
 SET,LAST
 /GRAPHICS,POWER
 /ESHAPE,1
 /VIEW,1,1,1,1
 PLESOL,S,1
+/OUT,
 *GET,P_STRESS,PLNSOL,0,MAX
 PLESOL,S,INT
 *GET,SHEAR,PLNSOL,0,MAX
-
 *DIM,LABEL,CHAR,2,2
 *DIM,VALUE,,2,3
 LABEL(1,1) = 'MAX PRIN','MAX SH S'
 LABEL(1,2) = 'STRS psi','TRS psi '
 *VFILL,VALUE(1,1),DATA,7527,3777
 *VFILL,VALUE(1,2),DATA,P_STRESS,(SHEAR/2)
 *VFILL,VALUE(1,3),DATA,ABS(P_STRESS/7527 ) ,ABS((SHEAR/2)/3777 )
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm120.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm120.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM120
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 SMRT,OFF
 /TITLE, VM120,  MICROSTRIP TRANSMISSION LINE ANALYSIS
 ! BEREN AND KAIRES (REF. 56)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm121.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm121.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM121
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE,VM121,VOLTAGE FORCED COIL (1/8 SYMMETRY)
 /VIEW,1,1,1,1
 /VUP,1,Z
 /COM,   REFERENCE (BENCHMARK DESCRIPTION AND EXPECTED RESULTS):
@@ -128,21 +128,20 @@
 
 C*** POST PROCESS
 /POST1
 SET,FIRST
 PLVE,B,,,,VECT,,ON
 VSEL,S,MAT,,2
 ALLS,BELO,VOLU
-/OUT
 PLVE,JT,,,,VECT,,ON
 VSEL,S,MAT,,3
 ALLS,BELO,VOLU
 PLVE,JT,,,,VECT,,ON
 FINI
-/OUT,SCRATCH
+
 /POST26
 *DIM,VALUE,,2,3
 *DIM,VALUE4,,2,3
 *DIM,VALUE7,,2,3
 *DIM,LABEL,CHAR,2		! PARAMETERS FOR POSTPROCESSING
 LABEL(1) = 'C_PLATE'
 LABEL(2) = 'C_FREE'
@@ -180,47 +179,40 @@
 VALUE7(2,1)=1.61
 VALUE(1,3)=VALUE(1,2)/VALUE(1,1)
 VALUE(2,3)=VALUE(2,2)/VALUE(2,1)
 VALUE4(1,3)=VALUE4(1,2)/VALUE4(1,1)
 VALUE4(2,3)=VALUE4(2,2)/VALUE4(2,1)
 VALUE7(1,3)=VALUE7(1,2)/VALUE7(1,1)
 VALUE7(2,3)=VALUE7(2,2)/VALUE7(2,1)
-/OUT
 *VLEN,2
-/OUT,VM121_1,vrt
+/OUT,vm121,vrt
 /COM
 /COM,----------- VM121 RESULTS COMPARISON at Time=1e-2 Sec -------------
 /COM,
 /COM,          |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,'    ',F7.3,'     ',F10.3,'       ',1F15.3)
 /COM,------------------------------------------------------------------
-/OUT,VM121_4,vrt
 /COM
 /COM,----------- VM121 RESULTS COMPARISON at Time=4e-2 Sec -------------
 /COM,
 /COM,          |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1),VALUE4(1,1),VALUE4(1,2),VALUE4(1,3)
 (1X,A8,'    ',F7.3,'     ',F10.3,'       ',1F15.3)
 /COM,------------------------------------------------------------------
-/OUT,VM121_7,vrt
 /COM
 /COM,----------- VM121 RESULTS COMPARISON at Time=7e-2 Sec -------------
 /COM,
 /COM,          |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1),VALUE7(1,1),VALUE7(1,2),VALUE7(1,3)
 (1X,A8,'    ',F7.3,'     ',F10.3,'       ',1F15.3)
 /COM,------------------------------------------------------------------
 /OUT
 /AXL,X,TIME (S)
 /AXL,Y,COIL CURRENT (A)
 PLVAR,2,3
 PRVAR,2,3
-*LIST,VM121_1,vrt
-*LIST,VM121_4,vrt
-*LIST,VM121_7,vrt
+*LIST,vm121,vrt
 FINISH
-
-
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm122.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm122.dat`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM122
 /PREP7
 /TITLE, VM122, PRESSURE DROP IN A FLOWING FLUID
 C***    FLUID MECHANICS, BINDER, 3RD. ED., PAGE 118, ART. 8-6
 ET,1,FLUID116,2             ! Use only pressure degrees of freedom
 keyo,1,7,1
 R,1,6                       ! DIAMETER
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm123.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm123.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM123
 /PREP7
 /TITLE, VM123, LAMINAR FLOW IN A PIPING SYSTEM
 C***    FLOW OF FLUIDS, CRANE TECH. PAPER NO. 410, PAGE 4-5, EX. 4-9
 ET,1,FLUID116,2     ! THERMAL-FLOW PIPE
 R,1,.4206           ! PIPE DIAMETER
 rmore
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm124.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm124.dat`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM124
 /PREP7
 /TITLE, VM124, DISCHARGE OF WATER FROM A RESERVOIR
 C***    ELEMENTARY THEORETICAL FLUID MECHANICS, BRENKERT, PAGE 224, PROB. 4
 ET,1,FLUID116,2      ! FLOW PIPE WITH LOSS COEFFICIENTS
 KEYO,1,7,3
 KEYO,1,8,1
@@ -39,16 +39,18 @@
 EGEN,4,1,-1,,,,,1    ! INCREMENT REAL CONSTANTS
 ACEL,,ACELY          ! GRAVITY LOAD
 D,1,PRES,,,5,4       ! WATER SURFACE AND PIPE OUTLET AT ZERO PRESSURE
 CNVTOL,FLOW,1,.0001  ! SET CONVERGENCE VALUE FOR FLUID FLOW WITH 
                      !  TOLERANCE LIMIT
 OUTPR,,1             ! PRINT BASIC SOLUTION QUANTITIES OF SUBSTEP 1
 FINISH
-/SOLU    
+/SOLU
+/OUT,vm124_SCRATCH    
 SOLVE
+/OUT
 FINISH
 /POST1
 ETABLE,R,NMISC,2
 ESORT,R
 *GET,RE,SORT,,MAX
 ETABLE,FL,NMISC,3
 ESORT,FL
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm125.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm125.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM125
 /PREP7
 /TITLE, VM125, RADIATION HEAT TRANSFER BETWEEN CONCENTRIC CYLINDERS
 C*** PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND PRINTING, PAGE 260
 ANTYPE,STATIC
 ET,1,LINK33,,,,,,,1    ! HEAT CONDUCTING BAR; SUPPRESS SOLUTION OUTPUT
 R,1,1                  ! UNIT CROSS-SECTIONAL AREA (ARBITRARY)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm126.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm126.dat`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM126
 /PREP7
 /TITLE, VM126, HEAT TRANSFERRED TO A FLOWING FLUID
 C***    HEAT, MASS AND MOMENTUM TRANS, ROHSENOW AND CHOI, PAGE 168, EX 7.5
 ET,1,FLUID116,1,4,,1                    ! THERMAL-FLOW PIPE ELEMENT
 ET,2,FLUID116,1
 R,1,(1/12),.00545415                    ! DIAMETER
@@ -26,15 +26,17 @@
 D,2,TEMP,200,,18,2                      ! WALL TEMPERATURE
 SFE,ALL,,HFLUX,,1.1321e-8               ! FLOW RATE INPUT  lbf-hr/ft
 OUTPR,,LAST                             ! PRINT FINAL CONVERGED ITERATION
 OUTPR,NLOAD,1
 FINISH
 /SOLU    
 EQSLV,JCG
+/OUT,vm126_SCRATCH
 SOLVE
+/OUT
 FINISH
 /POST1
 ETABLE,HEAT,NMISC,5                     ! STORE HEAT TRANSPORT RATE
 PRETAB,HEAT                             ! PRINT HEAT TRANSPORT RATES PER ELEMENT
 NSEL,S,NODE,,1,19,2                     ! SELECT PIPE NODES
 PRNSOL,TEMP                             ! PRINT TEMPERATURES ALONG PIPE LENGTH
 *GET,TO,NODE,17,TEMP
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm127.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm127.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM127
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM127, BUCKLING OF A BAR WITH HINGED SOLVES (LINE ELEMENTS)
 C***    STR. OF MATL., TIMOSHENKO, PART 2, 3RD ED., PAGE 148
 ET,1,BEAM188              ! BEAM ELEMENT
 KEYOPT,1,3,3
@@ -27,15 +27,15 @@
 F,11,FY,-1                      ! UNIT LOAD AT FREE END
 SOLVE
 FINISH
 
 /SOLU 
 ANTYPE,BUCKLE                   ! BUCKLING ANALYSIS
 BUCOPT,LANB,1                   ! USE BLOCK LANCZOS EIGENVALUE EXTRACTION METHOD
-MXPAND,1
+MXPAND,1,,,YES
 SOLVE
 *GET,FCR1,MODE,1,FREQ
 *status,parm
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
 LABEL(1,1) = 'Fcr '
 LABEL(1,2) = 'lb '
@@ -61,15 +61,15 @@
 SOLVE
 FINISH
 /SOLU 
 ANTYPE,STATIC,RESTART,,,PERTURB ! PERFORM A PERTURBATION ANALYSIS
 PERTURB,BUCKLE,,,ALLKEEP        ! PERTURBED BUCKLING SOLVE 
 SOLVE,ELFORM                    ! REFORM ELEMENT MATRICES
 BUCOPT,LANB,1,,,RANGE           ! USE BLOCK LANCZOS EIGENVALUE EXTRACTION METHOD, EXTRACT 1 MODE
-MXPAND,1                        ! EXPAND 1 MODE SHAPE
+MXPAND,1,,,YES                  ! EXPAND 1 MODE SHAPE
 SOLVE
 *GET,FCR2,MODE,1,FREQ
 *status,parm
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
 LABEL(1,1) = 'Fcr '
 LABEL(1,2) = 'lb '
@@ -101,7 +101,8 @@
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',F12.3,'   ',1F15.3)
 /COM,
 /COM,----------------------------------------------------------
 /OUT
 *LIST,vm127,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm128.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm128.dat`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM128
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM128, BUCKLING OF A BAR WITH HINGED SOLVES (AREA ELEMENTS)
 C***    STR. OF MATL., TIMOSHENKO, PART 2, 3RD ED., PAGE 148
 ET,1,PLANE182,2,,3               ! 2-D SOLID
 R,1,.5                           ! THICKNESS (SQUARE CROSS-SECTION)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm129.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm129.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM129
 /TITLE, VM129, NUMERICAL DIFFERENTIATION AND INTEGRATION USING APDL COMMAND
 C***    REFERENCE - ANY BASIC CALCULUS BOOK
 *DIM,A,,145                ! DEFINE ARRAYS WITH DIMENSION    
 *DIM,B,,145
 *DIM,C,,145
 *DIM,D,,145
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm13.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm13.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM13
 /PREP7
 /TITLE, VM13, CYLINDRICAL SHELL UNDER PRESSURE
 C***   STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 45, ART. 11
 C***   AND UGURAL AND FENSTER, ADV. STRENGTH AND APPL. ELAS., 1981
 ANTYPE,STATIC
 ET,1,SHELL208
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm130.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm130.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM130
 /TITLE, VM130, FOURIER SERIES GENERATION FOR A SAW TOOTH WAVE
 /COM    VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 102, PROB. 2
 *DIM,COEFF,,24
 *DIM,MODE,TABLE,24
 *DIM,ISYM,TABLE,24
 *DIM,THETA,TABLE,121
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm131.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm131.dat`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM131
 /PREP7
 /TITLE, VM131, ACCELERATION OF A ROTATING CRANE BOOM
 C***    VECTOR MECHANICS FOR ENGINEERS, BEER & JOHNSTON, P 616, PROB. 15.13
 ANTYPE,STATIC
 ET,1,MASS21,,,2      ! GENERALIZED MASS WITHOUT ROTARY INERTIA
 R,1,1                ! UNIT MASS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm132.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm132.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM132
 /PREP7
 /TITLE, VM132, STRESS RELAXATION OF A BOLT DUE TO CREEP
 C***    STR. OF MATL., TIMOSHENKO, PART 2, 3RD ED., PAGE 531
 ANTYPE,STATIC
 ET,1,LINK180             ! SPAR ELEMENT
 SECTYPE,1,LINK   
@@ -17,20 +17,22 @@
 INIS,DEFI,1,ALL,ALL,ALL,1/30000
 BFUNIF,TEMP,900        ! UNIFORM TEMPERATURE
 TIME,1000
 KBC,1
 D,ALL,ALL              ! FIX ALL DOFS
 FINISH
 /SOLU    
-SOLCONTROL,0
-NSUBST,100
+NSUBST,100,100,100
 RATE,ON,ON
 OUTPR,BASIC,10         ! PRINT BASIC SOLUTION FOR EVERY 10TH SUBSTEP
 OUTRES,ESOL,1          ! STORE ELEMENT SOLUTION FOR EVERY SUBSTEP
 /OUT,SCRATCH
+AUTOTS,OFF
+NEQIT,25
+TINTP,,,,0.5,,0.2
 SOLVE
 FINISH
 /POST26
 ESOL,2,1,,LS,1,SIG     ! STORE AXIAL STRESS
 /OUT,
 PRVAR,2                ! PRINT AXIAL STRESS VS TIME
 *GET,T190,VARI,2,RTIME,190
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm133.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm133.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM133
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM133, MOTION OF A ROD DUE TO IRRADIATION INDUCED CREEP
 C***    REFERENCE - ANY BASIC CALCULUS BOOK
 ANTYPE,STATIC
 ET,1,BEAM188
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm134.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm134.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM134
 /PREP7
 /TITLE, VM134, PLASTIC BENDING OF A CLAMPED I-BEAM
 C***    THE ANALYSIS OF STRUCTURES, N.J. HOFF, 1964, P. 388
 ET,1,BEAM188,,,3
 MP,EX  ,1,29E6
 MP,PRXY,1,0.3
-TB,BKIN,1,1                   ! BILINEAR KINEMATIC HARDENING BEHAVIOR
+EX=29E6
+ET=5.8E6
+EP=EX*ET/(EX-ET)
+TB,PLAS,1,1,,BKIN             ! BILINEAR KINEMATIC HARDENING BEHAVIOR
 TBTEMP,0.0
-TBDATA,1,38000,5.8E6          ! YIELD STRESSES AND TANGENT MODULUS
+TBDATA,1,38000,EP             ! YIELD STRESSES AND PLASTIC TANGENT MODULUS
 SECTYPE,1,BEAM,I
-SECDATA,95.95,95.95,10.6,0.1,0.1,0.0001
+SECDATA,19.80,19.80,10.6,0.504,0.504,0.001
 SECCONTROL,1E15               ! OVERRIDE THE PROGRAM-CALCULATED TRANSVERSE SHEAR STIFFNESS
 N,1
 N,10,72
 FILL
 N,100,,,1
 E,1,2,100
 *REPEAT,9,1,1
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm135.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm135.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM135
 /TITLE, VM135, BENDING OF A BEAM ON AN ELASTIC FOUNDATION
 C***    STR. OF MATL., TIMOSHENKO, PART 2, 3RD ED., PAGE 12
 /PREP7
 ET,1,BEAM189             ! BEAM     
 SECTYPE,1,BEAM,RECT
 SECDATA,5,4.224
 MP,EX  ,1,30E6
 MP,PRXY,1,0.3
-ET,2,153                 ! SURFACE EFFECT ELEMENT
-R,2,,,,1515.15           ! FUNDATION STIFFNESS
+ET,2,156,,,,,1            ! SURFACE EFFECT ELEMENT; NO ORIENTATION NODE
+R,2,1515.15               ! FOUNDATION STIFFNESS
+
 TYPE,1
+REAL,1
 N,1
 N,27,286
 FILL
 *DO,i,1,25,2
  E,i,i+2,i+1
 *ENDDO
 TYPE,2
@@ -47,11 +49,11 @@
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.5,'  ',F12.5,'   ',1F15.3)
 /COM,----------------------------------------------------------
 /OUT
-
+/NOPR
 FINISH
 *LIST,vm135,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm136.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm136.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM136
 /PREP7                    
 MP,PRXY,,0.3
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM136, LARGE DEFLECTIONS OF A BUCKLED BAR (THE ELASTICA)
 C***    THEORY OF ELASTIC STABILITY, TIMOSHENKO AND GERE, 2ND ED., PAGE 78
@@ -17,15 +17,14 @@
 N,11,,100
 FILL
 E,1,2
 EGEN,10,1,1
 D,ALL,UZ,,,,,ROTX,ROTY
 FINISH
 /SOLU    
-SOLCONTROL,0
 NEQIT,150                 ! PERFORM MAXIMUM 150 EQUILIBRIUM ITERATIONS
 OUTPR,BASIC,LAST          ! PRINT BASIC SOLUTION AT THE END OF EACH LOAD STEP
 D,1,ALL
 FCR=-38.553               ! SET CRITICAL LOAD PARAMETER
 PI=3.14159265359
 F,11,FY,FCR*1.015         ! VERTICAL LOAD
 F,11,FX,.5                ! SMALL HORIZONTAL LOAD
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm137.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm137.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM137
 /PREP7
 /TITLE, VM137, LARGE DEFLECTION OF A CIRCULAR MEMBRANE
 C***    THEORY OF PLATES AND SHELLS, TIMOSHENKO, P. 404, EQ. 236
 ET,1,SHELL208,,,2
 SECTYPE,1,SHELL
 SECDATA,0.0001
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm138.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm138.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM138
 /PREP7
 /TITLE, VM138, LARGE DEFLECTION BENDING OF A CIRCULAR PLATE
 C***    THEORY OF PLATES AND SHELLS, TIMOSHENKO, P. 401, EQ. 232
 ANTYPE,STATIC
 NLGEOM,ON                ! LARGE DEFLECTION OPTION
 ET,1,SHELL208,,,2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm139.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm139.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM139
 /PREP7
 /TITLE, VM139, BENDING OF A LONG UNIFORMLY LOADED RECTANGULAR PLATE
 C***            STR. OF MATL., TIMOSHENKO, PART 2, 3RD ED., PAGE 80
 C***            USING SHELL181 ELEMENTS
 ANTYPE,STATIC
 ET,1,SHELL181,,,2
@@ -31,40 +31,38 @@
 /SOLU    
 SFE,ALL,2,PRES,0,10 
 OUTPR,BASIC,LAST
 /OUT,SCRATCH
 SOLVE                    ! ANALYSIS 1 : SMALL DEFLECTION SOLUTION
 FINISH
 /POST1
-/OUT,
 SET,1                    ! ANALYSIS 1 : SMALL DEFLECTION SOLUTION
 NSEL,S,LOC,Y,0
 SHELL,BOT                ! BOTTOM STRESSES ALONG LENGTH
 PRNSOL,S,COMP
 *GET,S2,NODE,2,S,X
 PRNSOL,S,PRIN
 NSEL,ALL
 FINISH
 /SOLU    
 NLGEOM,ON                ! LARGE DEFLECTION OPTION
-/OUT,SCRATCH
 SOLVE                    ! ANALYSIS 2 : LARGE DEFLECTION SOLUTION
 FINISH
 /POST1
-/OUT,
 SET,1                    ! ANALYSIS 2 : CONVERGED LARGE DEFLECTION SOLUTION
 NSEL,S,LOC,Y,0
 SHELL,MID                ! MIDDLE STRESSES ALONG LENGTH
 PRNSOL,S,COMP
 *GET,S3,NODE,1,S,X
 PRNSOL,S,PRIN
 SHELL,BOT                ! BOTTOM STRESSES ALONG LENGTH
 PRNSOL,S,COMP
 *GET,S4,NODE,2,S,X
 PRNSOL,S,PRIN
+/OUT,
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
 LABEL(1,1) = 'BOT PRS '
 LABEL(1,2) = 'psi'
 *VFILL,VALUE(1,1),DATA,108000
 *VFILL,VALUE(1,2),DATA,S2
 *VFILL,VALUE(1,3),DATA,ABS(S2/108000)
@@ -110,15 +108,14 @@
 ESLN,S
 SFE,ALL,6,PRES,0,10 
 ALLSEL,ALL
 /OUT,SCRATCH
 SOLVE                    ! ANALYSIS 1 : SMALL DEFLECTION SOLUTION
 FINISH
 /POST1
-/OUT,
 SET,1                    ! ANALYSIS 1 : SMALL DEFLECTION SOLUTION
 NSEL,S,LOC,Z,-0.375/2    ! MID STRESSES ALONG LENGTH
 NSEL,R,LOC,Y,0
 NSEL,R,LOC,X,22.5
 *GET,ND1,NODE,0,NUM,MAX  ! NODE AT SHELL-MID   X = 0.0, Y = 0.0, Z = -0.375/2
 NSEL,S,LOC,Z,-0.375
 NSEL,R,LOC,Y,0
@@ -129,30 +126,29 @@
 PRNSOL,S,COMP
 *GET,S2,NODE,ND2,S,X
 PRNSOL,S,PRIN
 NSEL,ALL
 FINISH
 /SOLU    
 NLGEOM,ON                ! LARGE DEFLECTION OPTION
-/OUT,SCRATCH
 SOLVE                    ! ANALYSIS 2 : LARGE DEFLECTION SOLUTION
 FINISH
 /POST1
-/OUT,
 SET,1                    ! ANALYSIS 2 : CONVERGED LARGE DEFLECTION SOLUTION
 NSEL,S,LOC,Z,-0.375/2    ! MIDDLE STRESSES ALONG LENGTH
 NSEL,R,LOC,Y,0
 PRNSOL,S,COMP
 *GET,S3,NODE,ND1,S,X
 PRNSOL,S,PRIN
 NSEL,S,LOC,Z,-0.375      ! BOTTOM STRESSES ALONG LENGTH
 NSEL,S,LOC,Y,0
 PRNSOL,S,COMP
 *GET,S4,NODE,ND2,S,X
 PRNSOL,S,PRIN
+/OUT,
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
 LABEL(1,1) = 'BOT PRS '
 LABEL(1,2) = 'PSI'
 *VFILL,VALUE(1,1),DATA,108000
 *VFILL,VALUE(1,2),DATA,S2
 *VFILL,VALUE(1,3),DATA,ABS(S2/108000)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm14.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm14.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM14
 /PREP7
 /TITLE, VM14, LARGE DEFLECTION ECCENTRIC COMPRESSION OF SLENDER COLUMN
 C***      STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PG. 263, PROB. 1
 ET,1,BEAM188,,,3
 SECTYPE,1,BEAM,CHAN
 SECDATA,2.26,2.26,8,0.39,0.39,0.22
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm140.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm140.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM140
 /PREP7
 /TITLE, VM140, STRETCHING, TWISTING AND BENDING OF A LONG SOLID SHAFT
 C***    STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 296
 ET,1,PLANE83,,,,2,,1
 MP,EX,1,30E6
 MP,NUXY,1,0                ! ZERO POISSONS RATIO
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm141.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm141.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM141
 /SHOW
 /PREP7
 smrt,off
 /DEVICE,VECTOR,ON
 /TITLE, VM141, DIAMETRAL COMPRESSION OF A DISK
 /COM,               THEORY OF ELASTICITY, TIMOSHENKO AND GOODIER, 2ND ED., PG 107
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm142.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm142.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM142
 /FILNAM,vm142         ! DEFINE JOBNAME FOR THE COARSE MODEL 
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /GRAPH,POWER
 /PREP7
 smrt,off
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm143.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm143.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM143
+/TITLE, VM143, FRACTURE MECHANICS STRESS INTENSITY FOR CRACK IN A FINITE WIDTH PLATE
 *CREATE,FRACT,MAC
 !  MACRO TO CREATE 3D SOLID95 CRACK TIP ELEMENTS FROM 3D SOLID45 ELEMENTS
 !     MAKE A COMPONENT CONTAINING THE CRACK TIP NODES (CRACKTIP)
 !     THE CRACK TIP IS BETWEEN NODES K AND O 
 !     SET ELEMENT TYPE TO POINT TO SOLID95
 !     SET ARG1 TO  N  (THE TYPE OF THE ELEMENTS AROUND THE CRACK TIP)
 !
@@ -70,15 +71,14 @@
 NSEL,ALL                             ! SELECT ALL ELEMENTS
 ESEL,ALL                             ! SELECT ALL ELEMENTS
 /GOPR
 *END
 
 /PREP7
 SMRT,OFF
-/TITLE, VM143, FRACTURE MECHANICS STRESS INTENSITY  - CRACK IN A FINITE WIDTH PLATE
 C***    BROWN AND SRAWLEY, ASTM SPECIAL TECHNICAL PUBLICATION NO. 410.
 /COM,     ****** CRACK IN 3-DIMENSIONS USING SOLID45 AND SOLID95
 ANTYPE,STATIC                ! STATIC ANALYSIS
 ET,1,SOLID45
 ET,2,SOLID45                 ! ELEMENTS AROUND THE CRACK TIP
 ET,3,SOLID95                 ! CRACK TIP ELEMENTS CREATED USING MACRO FRACT
 MP,EX,1,3E7
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm144.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm144.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM144
 /PREP7
 /TITLE, VM144, BENDING OF A COMPOSITE BEAM
 C***    FORMULAS FOR STRESS AND STRAIN, ROARK, 5TH ED.
 C***    USING LAYERED SOLID ELEMENTS (SOLID185)
 ANTYPE,STATIC
 ET,1,SOLID185               ! LAYERED SOLID ELEMENT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm145.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm145.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM145
 /PREP7
 /TITLE, VM145, STRETCHING OF AN ORTHOTROPIC SOLID
 C***    MECHANICS OF SOLIDS, CRANDALL AND DAHL, 1959, PAGE 225
 ANTYPE,STATIC              ! STATIC ANALYSIS
 ET,1,SOLID185              ! ANISOTROPIC SOLID
 MP,EX,2,10E6               ! LABELED MATERIAL PROPERTY INPUT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm146.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm146.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM146
 /PREP7
 /TITLE, VM146, BENDING OF A REINFORCED CONCRETE BEAM
 C***   STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 221
  
 ANTYPE,STATIC
 ET,1,SOLID65,,,,,2           ! REINFORCED CONCRETE SOLID ELEMENT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm147.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm147.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM147
 /PREP7
 /TITLE, VM147, GRAY-BODY RADIATION WITHIN A FRUSTRUM OF A CONE
 !       REF:  SIEGEL, R., HOWELL J.R., "THERMAL RADIATION HEAT TRANSFER"
 !             2ND EDITION, HEMISPHERE PUBLISHING CORPORATION, 1981.
 ET,1,LINK33           ! HEAT CONDUCTING BAR
 N,1
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm148.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm148.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM148
 /PREP7
 /TITLE, VM148, BENDING OF A PARABOLIC BEAM 
 C***    STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 210
 C***    USING 3-D SOLID95
 ANTYPE,STATIC
 ET,1,SOLID95                   ! 20 NODE SOLID ELEMENT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm149.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm149.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /verify,vm149
 /title,vm149,Residual Vector in Mode Superposition Harmonic Analysis
 /com,
 /com, Verification manual to verify the effect of residual
 /com, vector to improve the solution accuracy in modal
 /com, response analysis
 /com,
@@ -409,10 +409,11 @@
 /NOPR,
 /com,
 /com, 
 /com, --------------------------------------------------------------------------------
 /out,
 *list,vm149,vrt
 finish
+/exit,nosave
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm15.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm15.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM15
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7   
 /TITLE, VM15, BENDING OF A CIRCULAR PLATE USING AXISYMMETRIC SHELL ELEMENTS
 C***  CASE 1 - STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 96, ART. 19
 C***  CASE 2 - STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 103, ART. 21
@@ -10,38 +10,37 @@
 ANTYPE,STATIC
 ET,1,SHELL208,,,2
 SECTYPE,1,SHELL
 SECDATA,1,1
 SECNUM,1
 MP,EX,1,30E6
 MP,NUXY,1,.3
-K,1
-K,2,40
-K,3,20
-L,1,3
-L,3,2
-LESIZE,1,,,5,20             ! BIAS THE MESH TO ALLOW STRESS RECOVERY NEAR
-LESIZE,2,,,5,.05            ! THE CENTERLINE AND EDGE CONSTRAINTS
-LMESH,ALL                   ! MESH LINE SEGMENTS
+N,1
+N,11,40
+N,6,20
+FILL,1,6,4,,,,,20           ! BIAS THE MESH TO ALLOW STRESS RECOVERY NEAR
+FILL,6,11,4,,,,,0.05        ! THE CENTERLINE AND EDGE CONSTRAINTS
+E,1,2
+EGEN,10,1,-1
 FINISH
 C***  CASE 1 - UNIFORM LOADING - CLAMPED EDGE
 /SOLU    
 OUTPR,,1
-DK,1,UX,,,,ROTZ
-DK,2,ALL
+D,1,UX,,,,ROTZ
+D,11,ALL
 SFE,ALL,1,PRES,,6           ! PRESSURE LOAD = 6 PSI ON ALL LINE SEGMENTS
 /OUT,SCRATCH
 SOLVE
 C***  CASE 2 - CONCENTRATED CENTER LOADING - CLAMPED EDGE
-FK,1,FY,-7539.82
+F,1,FY,-7539.82
 SFE,ALL,1,PRES,,0           ! REMOVE PRESSURE
 SOLVE
 C***  CASE 3 - UNIFORM LOADING - SIMPLY SUPPORTED EDGE
-DKDELE,2,ROTZ               ! DELETE CLAMPED BOUNDARY CONDITION CONSTRAINT
-FK,1,FY                     ! REMOVE CENTERLINE POINT LOAD
+DDELE,11,ROTZ               ! DELETE CLAMPED BOUNDARY CONDITION CONSTRAINT
+F,1,FY                      ! REMOVE CENTERLINE POINT LOAD
 SFE,ALL,1,PRES,,1.5
 SOLVE
 FINISH
 /POST1
 /DSCALE,1,35                ! EXAGGERATE DISPLACEMENT SCALING FOR CLARITY
 /WINDOW,1,-1,1,-1,-.333
 /OUT,
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm150.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm150.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /verify,vm150
 /title,vm150,Diffusion in a Plane Sheet
 /com,
 /com,
 /com, Reference: Crank,J. The Mathematics of Diffusion.
 /com, 2nd printing, Bristol: Oxford University Press
 /com, 1975, pg 47-48
@@ -47,14 +47,15 @@
 
 /SOLU
 ANTYPE,TRANS
 OUTRES,ALL,ALL
 KBC,1
 NSUB,SUB
 TIME,T
+AUTOTS,OFF
 SOLVE
 FINISH
 
 /POST1
 *DIM,CONCENTRATION_,TABLE,SUB,2
 *DIM,MASS_,TABLE,SUB,2
 *DO,II,1,SUB
@@ -121,7 +122,8 @@
 *VWRITE,MASS_(25,0),MASS_(25,2),MASS_(25,1),MASS_RATIO(25,1)
 (,F15.0,'         ',G14.5,'          ',G14.5,'          ',F8.3)
 /COM
 /COM ------------------------------------------------------------------------
 /OUT,
 *list,vm150,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm151.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm151.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM151
 /PREP7  
 MP,PRXY,,0.3
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM151, NONAXISYMMETRIC VIBRATION OF A CIRCULAR PLATE
 C***          FORMULAS FOR NATURAL FREQUENCY AND MODE SHAPE, BLEVINS, PAGE 240
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm152.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm152.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM152
 /PREP7
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM152, NONAXISYM. VIBR. OF A STRETCHED CIRCULAR MEMBRANE (HARMONIC ELS)
 C***          VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., ART. 69, PAGE 438
 ET,1,SHELL61
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm153.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm37.dat`

 * *Files 24% similar despite different names*

```diff
@@ -1,166 +1,143 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM153
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM37
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/FILNAM,PRSMEMB
 /PREP7
-/TITLE, VM153, NONAXISYM. VIBR. OF A STRETCHED CIRCULAR MEMBRANE (STATIC)
-C***           VIBRATION PROBS. IN ENGR., TIMOSHENKO, PAGE 439, ARTICLE 69
-C*** USING SHELL41 MEMBRANE SHELL
-ANTYPE,STATIC            ! STATIC ANALYSIS
-ET,1,SHELL41,,1
-R,1,.00005               ! PLATE THICKNESS
-MP,EX,1,30E6
-MP,ALPX,1,1E-5
-MP,DENS,1,.00073
-MP,NUXY,1,0
-CSYS,1
-N,1,.001
-N,10,3
-FILL
-NGEN,4,10,1,10,1,,10
-NROTAT,ALL               ! ROTATE ALL NODES INTO CYLINDRICAL SYSTEM
-E,1,2,12,11
-EGEN,3,10,-1
-EGEN,9,1,-3
-NSEL,S,LOC,Y,0           ! DEFINE EDGE COMPONENTS FOR CYCLIC SYMM. MACRO
-CM,RIGHT,NODE            ! RIGHT EDGE OF THE SECTOR MODEL
-NSEL,S,LOC,Y,30
-CM,LEFT,NODE             ! LEFT EDGE OF THE SECTOR MODEL
-NSEL,ALL
-/NOPR
-CYCLIC              
-/GOPR
-D,ALL,ALL,0              ! FIX ALL DISPLACEMENTS TO APPLY PRESTRESS
-TREF,0                   ! REFERENCE TEMPERATURE
-BFUNIF,TEMP,-6.66666     ! COOL DOWN TO INDUCE PRESTRESS
-FINISH
-*CREATE,SOLVIT,MAC
-/SOLU                    ! SOLVE FOR STATIC SOLUTION
-/OUTPUT,SCRATCH
+smrt,off
+/TITLE, VM37, ELONGATION OF A SOLID BAR
+/COM    INTROD. TO STRESS ANALYSIS, HARRIS, 1ST PRINTING, PAGE 237, PROB. 4
+/COM    USING 3-D STRUCTURAL SOLID45 ELEMENTS
 ANTYPE,STATIC
-PSTRES,ON                ! PRESTRESS KEY ON
-CYCOPT,HINDX,0,0
-SOLVE
-FINISH
-/PREP7
-/TITLE, VM153, NONAXISYM. VIBR. OF A STRETCHED CIRCULAR MEMBRANE (MODAL)
-CYCLIC,UNDOUBLE
-DDEL,ALL,ALL             ! RELEASE ALL DISPLACEMENTS AND THEN
-NSEL,S,LOC,Y,0           ! DEFINE BOUNDARY CONDITIONS
-NSEL,A,LOC,Y,30
-D,ALL,UX,,,,,UY
-NSEL,S,LOC,X,3
-D,ALL,ALL,0
+ET,1,SOLID45
+MP,EX,1,10.4E6
+MP,NUXY,1,.3
+K,1,1,,1               ! DEFINE KEYPOINTS
+K,2,-1,,1
+K,3,-1,,-1
+K,4,1,,-1
+K,5,.5,10,.5 
+K,6,-.5,10,.5
+K,7,-.5,10,-.5
+K,8,.5,10,-.5
+V,1,2,3,4,5,6,7,8      ! DEFINE VOLUME
+LSEL,S,LINE,,5,11,2    ! SELECT LINES
+LESIZE,ALL,,,7         ! DEVIDE SELECTED LINES BY 7 DIVISIONS
+LSEL,ALL               ! SELECT ALL LINES
+ESIZE,,1               ! USE 1 ELEMENT PER LINE DIVISION
+/OUT,SCRATCH
+VMESH,1                ! MESH THE VOLUME 
+/OUT
+OUTPR,BASIC,ALL
+NSEL,S,LOC,Y,0         ! APPLY BOUNDARY CONDITIONS AT THE BASE OF THE MODEL
+D,ALL,ALL              ! FIX ALL DEGREES OF FREEDOM AT SELECTED NODE SET
+NSEL,ALL
+NSEL,S,LOC,Y,10        ! APPLY LOAD ON FREE END OF THE MODEL 
+SF,,PRES,-10000
 NSEL,ALL
-CYCLIC
+SAVE
 FINISH
-/SOLUTION
-ANTYPE,MODAL             ! DEFINE MODAL ANALYSIS OPTIONS
-MODOPT,LANB,4,1,1000     ! USE BLOCK LANCZOS ITER, EXTRACT 4 MODES IN 1 TO 1000 HZ
-MXPAND,4                 ! EXPAND 4 MODES
-PSTRES,ON
-CYCOPT,HINDX,0,1         ! NODAL DIAMETER 0 TO 1, WITH 30 DEG. SECTORS
+/SOLU 
+/OUT,SCRATCH
 SOLVE
+/OUT,
 FINISH
+*CREATE,RES3D,MAC      ! CREATE MACRO TO RETRIEVE RESULTS
 /POST1
-/OUTPUT
-SET,1,1
-*GET,F01_1,ACTIVE,,SET,FREQ   ! NATURAL FREQ. FOR 1ST MODE, 0 MODAL DIAM.
-SET,1,2
-*GET,F02_1,ACTIVE,,SET,FREQ   ! NATURAL FREQ. FOR 2ND MODE, 0 MODAL DIAM.
-SET,2,1
-*GET,F11_1,ACTIVE,,SET,FREQ   ! NATURAL FREQ. FOR 1ST MODE, 1 MODAL DIAM.
-SET,2,2
-*GET,F11_2,ACTIVE,,SET,FREQ   ! REPEATED FREQ. FOR 1ST MODE,1 MODAL DIAM.
-SET,2,3
-*GET,F12_1,ACTIVE,,SET,FREQ   ! NATURAL FREQ. FOR 2ND MODE, 1 MODAL DIAM.
-SET,2,4
-*GET,F12_2,ACTIVE,,SET,FREQ   ! REPEATED FREQ. FOR 2ND MODE,1 MODAL DIAM.
-FINISH
+ETABLE,SIGY,S,Y        ! RETRIEVE CENTROIDAL SY
+/VIEW,1,1              ! CHANGE VIEW TO LOOKING DOWN X-AXIS
+/VUP,1,-Y              ! REORIENT MODEL ON SCREEN
+!/CLABEL,1,1            ! LABEL CONTOUR LINES
+!/CVAL,1,2700,3500,4300,5100,5900,6700,7500,8300  ! USER DEFINED CONTOURS
+NSLE,S                 ! SELECT NODES ATTACHED TO ELEMENTS
+PLNSOL,S,Y             ! DISPLAY AXIAL STRESS
+ESEL,S,ELEM,,4         ! SELECT MID-LENGTH ELEMENT
+PRETAB,SIGY            ! PRINT OUT STORED STRESS ITEM
+PRNSOL,S,COMP          ! PRINT NODAL STRESSES
+ESEL,ALL               ! SELECT ALL ELEMENTS
+NSEL,S,LOC,Y,10        ! SELECT ALL NODES AT Y=10 (FREE END OF MODEL)
+PRNSOL,DOF             ! PRINT OUT DISPLACEMENTS OF NODES
+NSEL,ALL
 /NOPR
-/POST1
-EXPAND,12                ! EXPAND RESULTS FOR THE FULL 12 SECTOR MODEL
-/VIEW,,1,1,1
-/VUP,1,Z
-/GLINE,,-1               ! NO ELEMENT OUTLINE
-/TRIAD,OFF
-SET,1,2
-/TITLE, VM153, STRETCHED CIRCULAR MEMBRANE - NODAL DIAM 0, MODE 2
-PLNSOL,U,Z
-SET,2,2
-/TITLE, VM153, STRETCHED CIRCULAR MEMBRANE - NODAL DIAM 1, MODE 2
-PLNSOL,U,Z
-FINISH
-*DIM,LABEL,CHAR,4,2
-*DIM,VALUE,,4,3
-LABEL(1,1) = 'F(0,1) ','F(0,2) ','F(1,1) ','F(1,2) '
-LABEL(1,2) = 'Hz ','Hz ','Hz ','Hz '
-*VFILL,VALUE(1,1),DATA,211.1,484.7,336.5,616.1
-*VFILL,VALUE(1,2),DATA,F01_1,F02_1,F11_1,F12_1
-*VFILL,VALUE(1,3),DATA,ABS(F01_1/211.1),ABS(F02_1/484.7),ABS(F11_1/336.5),ABS(F12_1/616.1)
+MID_NODE = NODE(0,5,0)
+MID_ELM = ENEARN(MID_NODE)
+BOT_NODE = NODE (0,10,0)
+*GET,DEF,NODE,BOT_NODE,U,Y
+*GET,STRSS,ELEM,MID_ELM,ETAB,SIGY
+*DIM,LABEL,CHAR,2,2
+*DIM,VALUE_C1,,2,3
+LABEL(1,1) = 'MAX DEF ','SIGY MID'
+LABEL(1,2) = '(in)    ','_ELM psi'
+*VFILL,VALUE_C1(1,1),DATA,.0048077,4444
+*VFILL,VALUE_C1(1,2),DATA,DEF,STRSS
+*VFILL,VALUE_C1(1,3),DATA,ABS(DEF/.0048077) ,ABS(STRSS/4444)
+/GOPR
 FINISH
 *END
-SOLVIT
+RES3D                  ! EXECUTE MACRO TO RETRIEVE RESULTS
 SAVE,TABLE_1
-/CLEAR,NOSTART
-/TITLE, VM153, NONAXISYM. VIBR. OF A STRETCHED CIRCULAR MEMBRANE (STATIC)
-C*** USING SHELL181 MEMBRANE SHELL OPTION
-/FILNAM,PRSMEMB
+
+/CLEAR, NOSTART        ! CLEAR DATABASE FOR SECOND SOLUTION
+/TITLE, VM37, ELONGATION OF A SOLID BAR
+/COM    USING 3-D STRUCTURAL SOLID185 ELEMENTS
 /PREP7
-ANTYPE,STATIC            ! STATIC ANALYSIS
-ET,1,SHELL181,1          ! MEMBRANE STIFFNESS ONLY
-SECT,1,SHELL
-SECD,.00005,1            ! PLATE THICKNESS
-MP,EX,1,30E6
-MP,ALPX,1,1E-5
-MP,DENS,1,.00073
-MP,NUXY,1,0
-CSYS,1
-N,1,.001
-N,10,3
-FILL
-NGEN,4,10,1,10,1,,10
-NROTAT,ALL               ! ROTATE ALL NODES INTO CYLINDRICAL SYSTEM
-E,1,2,12,11
-EGEN,3,10,-1
-EGEN,9,1,-3
-NSEL,S,LOC,Y,0           ! DEFINE EDGE COMPONENTS FOR CYCLIC SYMM. MACRO
-CM,RIGHT,NODE            ! RIGHT EDGE OF THE SECTOR MODEL
-NSEL,S,LOC,Y,30
-CM,LEFT,NODE             ! LEFT EDGE OF THE SECTOR MODEL
-NSEL,ALL
-/NOPR
-CYCLIC              
-/GOPR
-D,ALL,ALL,0              ! FIX ALL DISPLACEMENTS TO APPLY PRESTRESS
-TREF,0                   ! REFERENCE TEMPERATURE
-BFUNIF,TEMP,-6.66666     ! COOL DOWN TO INDUCE PRESTRESS
-FINISH
-SOLVIT
+RESUME
+ET,1,SOLID185, ,2      ! ANALYZE AGAIN USING 3-D SOLID185      
+FINISH             
+/SOLU			
+/OUT,SCRATCH
+SOLVE			
+FINISH  		
+/OUT,
+RES3D                  ! EXECUTE MACRO TO RETRIEVE RESULTS
 SAVE,TABLE_2
+
+/CLEAR, NOSTART        ! CLEAR DATABASE FOR THIRD SOLUTION
+/TITLE, VM37, ELONGATION OF A SOLID BAR
+/COM    USING 3-D STRUCTURAL SOLSH190 ELEMENTS
+/PREP7
+RESUME
+ET,1,SOLSH190          ! ANALYZE AGAIN USING 3-D SOLSH190      
+FINISH             
+/SOLU			
+/OUT,SCRATCH
+SOLVE			
+FINISH  		
+/OUT,
+RES3D                  ! EXECUTE MACRO TO RETRIEVE RESULTS
+SAVE,TABLE_3
+
 /NOPR
 RESUME,TABLE_1
+/GOPR
 /COM
-/OUT,vm153,vrt
-/COM,------------------- VM153 RESULTS COMPARISON -------------
+/OUT,vm37,vrt
+/COM,------------------- VM37 RESULTS COMPARISON ---------------
 /COM,
-/COM,                 |    TARGET   |    Mechanical APDL   |    RATIO
+/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
+/COM,RESULTS FOR SOLID45:
 /COM,
-/COM, SHELL41
-/COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.1,'  ',F16.1,'   ',1F16.3)
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE_C1(1,1),VALUE_C1(1,2),VALUE_C1(1,3)
+(1X,A8,A8,'   ',F12.7,'  ',F16.7,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_2
 /GOPR
 /COM,
-/COM, SHELL181
+/COM,RESULTS FOR SOLID185:
 /COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.1,'  ',F16.1,'   ',1F16.3)
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE_C1(1,1),VALUE_C1(1,2),VALUE_C1(1,3)
+(1X,A8,A8,'   ',F12.7,'  ',F16.7,'   ',1F15.3)
 /NOPR
-/COM,----------------------------------------------------------
+RESUME,TABLE_3
+/GOPR
+/COM,
+/COM,RESULTS FOR SOLSH190:
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE_C1(1,1),VALUE_C1(1,2),VALUE_C1(1,3)
+(1X,A8,A8,'   ',F12.7,'  ',F16.7,'   ',1F15.3)
+/COM,-----------------------------------------------------------
 /OUT
-*LIST,vm153,vrt
+FINISH
+*LIST,vm37,vrt
+/DELETE,RES3D,MAC
+FINISH
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm154.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm154.dat`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM154
 /PREP7
 /TITLE, VM154, VIBRATION OF A FLUID COUPLING
 C***            FRITZ, ASME J. OF ENG. FOR INDUST., VOL. 94, 1972, PP 167-173.
 C***            USING FLUID COUPLING ELEMENTS (FLUID38)
 ANTYPE,MODAL          ! MODE-FREQUENCY ANALYSIS
 ET,1,FLUID38
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm155.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm155.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM155
 /TITLE,VM155,VERIFY CHABOCHE RATE-DEPENDENT PLASTICITY MATERIAL MODEL
 /COM, REFERENCE:"R.C.Lin,ET AL.,MODELING OF FINITE STRAIN VISCOPLASTICITY BASED
 /COM,            ON THE LOGARITHMIC COROTATIONAL DESCRIPTION
 /COM,            ARCH APPL MECH, 2006(75),PG: 693-708
 /COM,
 /OUT,SCRATCH
@@ -10,15 +10,15 @@
 ET,1,PLANE182                    ! 2D 8 NODE ELEMENT
 KEYOPT,1,3,0                     ! PLANE STRESS
 
 MP,EX,1,149650e6
 MP,NUXY,1,0.33
 TB,CHAB,1,,1                     ! DEFINE CHABOCHE MATERIAL DATA
 TBDATA,1,1.53e8,62511e6,1.1/311e6*62511e6
-TB,RATE,1,,6,CHABOCHE            ! DEFINE RATE DEPENDENT MATERIAL DATA
+TB,RATE,1,,6,EVH                ! DEFINE RATE DEPENDENT MATERIAL DATA
 TBDATA,1,1.53e8,0,-1.53e8,317,1/7.7,1150e6
 
 N, 1, 0.0, 0.0, 0.0    
 N, 2, 0.0, 1.0, 0.0     
 N, 3, 1.0, 0.0, 0.0   
 N, 4, 1.0, 1.0, 0.0
 E,1,3,4,2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm156.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm156.dat`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM156
 /PREP7
 /TITLE, VM156, NATURAL FREQUENCY OF NONLINEAR SPRING-MASS SYSTEM
 C***            VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 141
 C***             USING NONLINEAR SPRING ELEMENT (COMBIN39)
 ANTYPE,TRANS                 ! NONLINEAR TRANSIENT DYNAMIC ANALYSIS
 ET,1,COMBIN39,,,2            ! ELEMENT WITH DISPLACEMENT ALONG NODAL Y-AXIS
@@ -22,24 +22,26 @@
 D,2,UX
 IC,2,UY,-1                   ! INITIAL DISPLACEMENT AND VELOCITY
 KBC,1                        ! STEP LOADING
 SAVE
 FINISH
 /SOLU    
 TRNOPT, , , , , ,HHT
-SOLCONTROL,0
 CNVTOL,F,1,1E-4              ! FORCE CONVERGENCE CRITERIA
 OUTRES,NSOL,1
-NSUBST,5
+NSUBST,5,5,1
 OUTPR,BASIC,NONE
 TIME,.0002                   ! TIME TO ALLOW INITIAL CHANGE IN ACCELERATION
+KBC,0
+AUTOTS,OFF
 LSWRITE                      ! WRITE LOAD STEP FILE 1
-NSUBST,40
+NSUBST,40,40,1
 OUTPR,BASIC,LAST
 TIME,0.18                    ! TIME ARBITRARILY SELECTED
+KBC,0
 LSWRITE                      ! WRITE LOAD STEP FILE 2
 /OUT,SCRATCH
 LSSOLVE,1,2,1                ! READ IN 2 LOAD STEPS AND SOLVE
 FINISH
 /POST26
 TIMERANGE,.003,.18
 NSOL,2,2,U,Y,2UY
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm157.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm157.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM157
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE,VM157, MODAL ANALYSIS OF GAS WITH SUDDEN TEMPERATURE CHANGE
 /COM, REFERENCE: OBERG, C.L., RYAN, N.W., BAER, A.D.
 /COM, A STUDY OF T-BURNER BEHAVIOR, AIAA VOL. 6 NO. 6
 /COM, PP 1131-1137 (1968)
@@ -50,19 +50,19 @@
 
 /SOLU
 ANTYPE,MODAL
 MODOPT,LANB,5,,,,ON                 ! LANCZOS EIGENSOLVER
 MXPAND,5
 VSEL,S,VOLUME,,1,,,1
 BFE,ALL,TEMP,,TMP_COLD
-BF,ALL,CHRGD,REF_PRESSURE
+BF,ALL,SPRE,REF_PRESSURE
 ALLSEL,ALL
 VSEL,S,VOLUME,,3,,,1
 BFE,ALL,TEMP,,TMP_HOT
-BF,ALL,CHRGD,REF_PRESSURE
+BF,ALL,SPRE,REF_PRESSURE
 ALLSEL,ALL
 /OUT,SCRATCH
 SOLVE
 FINISH
 
 /POST1
 /OUT,
@@ -91,7 +91,8 @@
 *VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A3,' ',F10.3,' ',F13.3,' ',F15.3)
 /COM,
 /COM,-------------------------------------------------------------------------
 /OUTPUT
 *LIST,vm157,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm158.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm158.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM158
 /PREP7   
 MP,PRXY,,0.3
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM158, MOTION OF A BOBBING BUOY
 C***            ELEMENTARY THEORETICAL FLUID MECHANICS, BRENKERT, PAGE 37
 ANTYPE,TRANS
 NLGEOM,ON                     ! LARGE DISPLACEMENTS
-ET,1,PIPE288
+ET,1,PIPE288,,,,2
 SECTYPE,1,PIPE
 SECDATA,1,.03                  ! DIAMETER, WALL THICKNESS
 MP,EX,1,21E10
 MP,DENS,1,8000
 MP,PRXY,1,0.3
 MP,DENS,2,1000
 N,1,,,-9
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm159.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm159.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM159
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 /TITLE, VM159, TEMPERATURE CONTROLLED HEATER
 C***            REFERENCE - SELF-CHECKING (RESPONSE FOLLOWS INPUT REQUEST)
 ANTYPE,TRANS
@@ -29,25 +29,25 @@
 REAL,5
 E,4,1,2                    ! CONTROL
 TYPE,2
 REAL,4
 E,2,3                      ! CONVECTION LINK
 FINISH
 /SOLU    
-SOLCONTROL,0
 TIME,.2
 IC,1,TEMP,70               ! UNIFORM STARTING TEMPERATURE
 IC,2,TEMP,70
 KBC,1
 D,3,TEMP,70
 D,4,TEMP,0
 AUTOTS,ON
 OUTPR,,10
 OUTRES,,ALL
-DELTIM,0.001
+TINTP,,,,0.5,0.5,0.2
+DELTIM,0.10000E-02,0.10000E-02,0.20000
 /OUT,SCRATCH
 SOLVE
 FINISH
 /POST26
 NSOL,2,1,TEMP
 NSOL,3,2,TEMP
 ESOL,4,4,,NMISC,1,STAT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm16.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm16.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM16
 /SHOW,JPEG
 /PREP7
 /TITLE, VM16, BENDING OF A SOLID BEAM (PLANE ELEMENTS)
 C***           FORMULAS FOR STRESS AND STRAIN, ROARK, 4TH ED.,PG. 104,106
 C***           USING PLANE42 ELEMENTS
 ANTYPE,STATIC
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm160.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm160.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM160
 /PREP7
 /TITLE, VM160, SOLID CYLINDER WITH HARMONIC TEMPERATURE LOAD
 C***    HILDEBRAND, ADVANCED CALCULUS FOR APPLICATIONS, PAGE 447
 ET,1,PLANE78               ! AXISYMMETRIC THERMAL SOLID
 MP,KXX,1,1
 N,1
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm161.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm161.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM161
 /PREP7
 /TITLE, VM161, HEAT FLOW FROM AN INSULATED PIPE
 C***  PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 36, EX. 2-7
 ANTYPE,STATIC
 ET,1,SOLID90
 MP,KXX,1,25
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm162.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm162.dat`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM162
 /PREP7
 /TITLE, VM162, CIRCULAR COOLING FIN OF RECTANGULAR PROFILE
 C***     CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 82, ART. 4-10
 ANTYPE,STATIC
 ET,1,SOLID90
 MP,KXX,1,15
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm163.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm163.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM163
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 SMRT,OFF
-/TITLE, VM163 GROUNDWATER SEEPAGE
+/TITLE, VM163, GROUNDWATER SEEPAGE
 C***          A SIMPLE GUIDE TO FINITE ELEMENTS, R.J.OWEN AND E. HINTON, P.89
 ANTYPE,STATIC             ! THERMAL ANALYSIS           
 ET,1,PLANE55,,,1,,,,1     ! AXISYMMETRIC, SUPRESS ALL PRINTOUT
 MP,KXX,1,0.864            ! PERMEABILITY
 K,1
 *REPEAT,3,1,,3.5
 KGEN,2,1,3,1,8.0
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm164.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm164.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM164
 /PREP7
 /TITLE, VM164, DRYING OF A THICK WOODEN SLAB (DIFFUSION)
 C***     HEAT, MASS AND MOMENTUM TRANS., ROHSENOW AND CHOI, 2ND. PR., PAGE 392
 ANTYPE,TRANS
 ET,1,LINK33
 R,1,1                   ! ARBITRARY AREA
@@ -14,15 +14,14 @@
 FILL
 E,1,2
 EGEN,10,1,1
 TUNIF,30                ! INITIAL MOISTURE CONCENTRATION (THAT OF WOOD)
 D,11,TEMP,5             ! FINAL MOISTURE CONCENTRATION (AMBIENT)
 FINISH
 /SOLU    
-SOLCONTROL,0
 AUTOTS,ON
 OUTPR,,LAST
 DELTIM,0.434
 TIME,127                ! TIME AT END OF LOAD STEP
 KBC,1                   ! STEP BOUNDARY CONDITIONS
 /OUT,SCRATCH
 SOLVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm165.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm39.dat`

 * *Files 25% similar despite different names*

```diff
@@ -1,191 +1,154 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM165
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM39
+/PREP7    
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/PREP7
-SMRT,OFF
-/TITLE, VM165, CURRENT CARRYING FERROMAGNETIC CONDUCTOR
-C***           PRINCIPLES OF ELECTRIC AND MAGNETIC FIELDS, BOAST, PAGE 225
-ET,1,PLANE13           ! 2-D COUPLED FIELD SOLID
-ET,2,INFIN9            ! 2-D INFINITE BOUNDARY ELEMENT
-EMUNIT,MKS             ! MKS UNITS
-MP,MURX,1,1            ! SET RELATIVE PERMEABILITY FOR AIR TO 1
-TB,BH,2                ! B-H CURVE FOR MATERIAL 2
-TBPT,,150,.21          ! H AND B RESPECTIVELY
-TBPT,,300,.55
-TBPT,,460,.80
-TBPT,,640,.95
-TBPT,,720,1.0
-TBPT,,890,1.1
-TBPT,,1020,1.15
-TBPT,,1280,1.25
-TBPT,,1900,1.40
-TBPLOT,BH,2
-TBPLOT,NB,2
-/WIND,1,TOP
-/WIND,2,BOTTOM
-/GTYPE,1,GRPH,1
-/GTYPE,2,GRPH,1
-/GCMD,1,TBPLOT,BH,2
-/GCMD,2,TBPLOT,NB,2
-GPLOT
-/WIND,2,OFF
-/WIND,1,FULL
-SF=.0254               ! SET CONVERSION (INCHES TO METERS)
-CSYS,1
-K,1
-K,2,.3,-2.5            ! INNER RADIUS OF RING
-K,3,.45,-2.5           ! OUTER RADIUS OF RING
-K,4,.75,-2.5           ! OUTER RADIUS OF SURROUNDING AIR
-KPSCALE,ALL,,,SF,,,,,1 ! MOVE ORIGINAL KEYPOINTS TO NEW POSITION
-CSYS,0
-L,1,2
-LESIZE,1,,,5
-L,2,3
-LESIZE,2,,,6
-L,3,4
-LSYMM,2,ALL
-NUMMRG,KP              ! MERGE KEYPOINTS
-L,4,8                  ! DEFINE OUTER RADIUS LINE SEGMENT
-LESIZE,7,,,1
-TYPE,2
-ESIZE,,,1
-LMESH,7                ! MESH LINE SEGMENT (WITH BOUNDARY ELEMENT)
-A,2,6,1,1
-A,2,3,7,6
-A,3,4,8,7
-ASEL,S,AREA,,2
-AATT,2                 ! ASSIGN MATERIAL 2 TO STEEL AREA
-ASEL,ALL
-ESIZE,,1               ! DEFAULT ELEMENT DIVISIONS=1
-TYPE,1
-AMESH,1,2
-AMESH,3
-FINISH
-/SOLU                  ! ENTER SOLVER
-BFA,2,JS,,,438559      ! APPLY CURRENT DENSITY JS(Z)	
-MAGSOLV
+/TITLE, VM39, BENDING OF A CIRCULAR PLATE WITH A CENTER HOLE
+C***          STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 111, EQNS. (E,F)
+C***          USING SHELL63 ELEMENTS
+ANTYPE,STATIC
+ET,1,SHELL63
+R,1,.25                     ! DEFINE PLATE THICKNESS = .25
+MP,EX,1,30.E6
+MP,NUXY,1,.3
+CSYS,1                      ! DEFINE CYLINDRICAL C.S.
+N,1,10                      ! BEGIN NODE DEFINITION
+N,7,30
+FILL,,,,,,,,3               ! USE 3:1 SPACING RATIO FOR FILLING IN NODES 
+NGEN,2,10,1,7,1,,10
+NROTAT,1,17,1
+E,1,2,12,11                 ! DEFINE FIRST ELEMENT
+EGEN,6,1,1                  ! GENERATE NEXT 5 ELEMENTS 
+D,1,ALL,,,11,10             ! CONSTRAIN INNER EDGE IN ALL D.O.F.
+D,2,UY,,,7,,ROTX,ROTZ       ! CONSTRAIN LOWER EDGE AGAINST ROTATIONS IN X & Z
+D,12,UY,,,17,,ROTX,ROTZ     ! CONSTRAIN UPPER EDGE AGAINST ROTATIONS IN X & Z
+F,7,MY,-26.18,,17,10        ! APPLY MOMENT LOAD AT OUTER EDGE
+OUTPR,BASIC,1
+FINISH
+*CREATE,SOLVIT,MAC
+/SOLU    
+/OUT,SCRATCH
+SOLVE
 FINISH
 /POST1
-CSYS,1
-NSEL,S,LOC,X,.325*SF
-NSEL,A,LOC,X,.375*SF
-NSEL,A,LOC,X,.425*SF
-RSYS,1                 ! SET RESULTS C.S. TO CYLINDRICAL
-PRNSOL,B,COMP          ! PRINT NODAL FLUX DENSITY
-*GET,B1,NODE,21,B,SUM
-*GET,B2,NODE,23,B,SUM
-*GET,B3,NODE,25,B,SUM
-*DIM,LABEL,CHAR,3,2
-*DIM,VALUE,,3,3
-LABEL(1,1) = '@ R=','@ R=','@ R='
-LABEL(1,2) = '.325','.375','.425'
-*VFILL,VALUE(1,1),DATA,.48,1.03,1.22
-*VFILL,VALUE(1,2),DATA,B1,B2,B3
-*VFILL,VALUE(1,3),DATA,ABS(B1/.48),ABS(B2/1.03),ABS(B3/1.22)
+/WINDOW,1,TOP               ! SET UP WINDOW 1 FOR DISPLACEMENT CONTOUR DISPLAY
+/PLOPTS,MINM,OFF	    ! TURN OFF MN AND MX DUE TO INSTABILITY
+PLNSOL,U,Z                  ! DISPLAY PERPENDICULAR DISPLACEMENTS AS CONTOURS
+/WINDOW,1,OFF               ! TURN OFF WINDOW 1
+/NOERASE                    ! TURN OFF AUTOMATIC ERASE BETWEEN DISPLAYS
+/WINDOW,2,BOT               ! SET UP WINDOW 2 FOR EDGE DISPLACEMENT DISPLAY
+/VIEW,2,,-1                 ! CHANGE VIEW FOR WINDOW 2
+PLDISP,1                    ! DISPLAY UNDISPLACED & DISPLACED SHAPES
+/OUT,
+SHELL,TOP
+ESEL,,,,1                   ! SELECT INNER ELEMENT(ELEM #1) 
+ETABLE,MOMX,SMISC,4         ! RETRIEVE MOMENT(X) AND SX AT TOP
+ETABLE,SIGX,S,X
+PRETAB,GRP1                 ! PRINT STORED VALUES
+*GET,M1,ETAB,1,ELEM,1
+*GET,P1,ETAB,2,ELEM,1
+ESEL,,,,6                   ! SELECT OUTER ELEMENT(ELEM#6)
+ETABLE,REFL
+PRETAB,GRP1                 ! PRINT STORED VALUES 
+*GET,M2,ETAB,1,ELEM,6
+*GET,P2,ETAB,2,ELEM,6
+ESEL,ALL                        
+RSYS,1
+PRNSOL,S,COMP               ! PRINT NODAL STRESSES
+NSEL,S,LOC,X,30             ! SELECT NODES AT R=A     
+PRNSOL,DOF                  ! PRINT DISPLACEMENTS
+*GET,DEF,NODE,7,U,Z
+*GET,ROT,NODE,7,ROT,Y
+*DIM,LABEL,CHAR,2,2
+*DIM,VALUE,,2,3
+LABEL(1,1) = 'DEFLECTI','MX_SLOPE'
+LABEL(1,2) = 'ON (in) ','(rad)   '
+*VFILL,VALUE(1,1),DATA,.049064,-.0045089
+*VFILL,VALUE(1,2),DATA,DEF,ROT
+*VFILL,VALUE(1,3),DATA,ABS(DEF/.049064 ) ,ABS( ROT/.0045089)
+*DIM,LABEL2,CHAR,2,2
+*DIM,VALUE2,,2,3
+LABEL2(1,1) = 'MOMENT ','PRESSURE'
+LABEL2(1,2) = 'in-lb/in',' psi  '
+*VFILL,VALUE2(1,1),DATA,-13.783,-1323.2
+*VFILL,VALUE2(1,2),DATA,M1,P1
+*VFILL,VALUE2(1,3),DATA,ABS(M1/13.783),ABS(P1/1323.2)
+*DIM,VALUE3,,2,3
+*VFILL,VALUE3(1,1),DATA,-10.127,-972.22
+*VFILL,VALUE3(1,2),DATA,M2,P2
+*VFILL,VALUE3(1,3),DATA,ABS(M2/10.127),ABS(P2/972.22)
+FINISH
+*END
+SOLVIT
+SAVE,TABLE_1
+/CLEAR, NOSTART                ! CLEAR DATABASE FOR SECOND SOLUTION
+/TITLE, VM39, BENDING OF A CIRCULAR PLATE WITH A CENTER HOLE
+C***          USING SHELL181 ELEMENTS
+/PREP7    
+ANTYPE,STATIC
+ET,1,SHELL181, , ,2
+SECT,1,SHELL
+SECD,.25,1                  ! DEFINE PLATE THICKNESS = .25
+MP,EX,1,30.E6
+MP,NUXY,1,.3
+CSYS,1                      ! DEFINE CYLINDRICAL C.S.
+N,1,10                      ! BEGIN NODE DEFINITION
+N,7,30
+FILL,,,,,,,,3               ! USE 3:1 SPACING RATIO FOR FILLING IN NODES 
+NGEN,2,10,1,7,1,,10
+NROTAT,1,17,1
+E,1,2,12,11                 ! DEFINE FIRST ELEMENT
+EGEN,6,1,1                  ! GENERATE NEXT 5 ELEMENTS 
+D,1,ALL,,,11,10             ! CONSTRAIN INNER EDGE IN ALL D.O.F.
+D,2,UY,,,7,,ROTX,ROTZ       ! CONSTRAIN LOWER EDGE AGAINST ROTATIONS IN X & Z
+D,12,UY,,,17,,ROTX,ROTZ     ! CONSTRAIN UPPER EDGE AGAINST ROTATIONS IN X & Z
+F,7,MY,-26.18,,17,10        ! APPLY MOMENT LOAD AT OUTER EDGE
+OUTPR,NSOL,1
+OUTPR,RSOL,1
+FINISH
+SOLVIT
+SAVE,TABLE_2
+/NOPR
+RESUME,TABLE_1
 /COM
-/OUT,vm165,vrt
-/COM,------------------- VM165 RESULTS COMPARISON --------------
+/OUT,vm39,vrt
+/COM,------------------- VM39 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
-/COM,PLANE13
+/COM,
+/COM,RESULTS USING SHELL63:
+/COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F13.2,'   ',1F15.3)
-/OUT
-FINISH
-
-/CLEAR,NOSTART
+(1X,A8,A8,'   ',F10.7,'  ',F14.7,'   ',1F15.3)
+/COM,
+/COM,X=10.81 in
+/COM,
+*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
+/COM,
+/COM,X=27.1 in
+/COM,
+*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE3(1,1),VALUE3(1,2),VALUE3(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
 /NOPR
-JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
-/SHOW,JPEG
-/PREP7
-SMRT,OFF
-/TITLE, VM165, CURRENT CARRYING FERROMAGNETIC CONDUCTOR
-ET,1,PLANE233          ! 2-D MAGNETIC SOLID
-ET,2,INFIN9            ! 2-D INFINITE BOUNDARY ELEMENT
-EMUNIT,MKS             ! MKS UNITS
-MP,MURX,1,1            ! SET RELATIVE PERMEABILITY FOR AIR TO 1
-TB,BH,2                ! B-H CURVE FOR MATERIAL 2
-TBPT,,150,.21          ! H AND B RESPECTIVELY
-TBPT,,300,.55
-TBPT,,460,.80
-TBPT,,640,.95
-TBPT,,720,1.0
-TBPT,,890,1.1
-TBPT,,1020,1.15
-TBPT,,1280,1.25
-TBPT,,1900,1.40
-TBPLOT,BH,2
-TBPLOT,NB,2
-/WIND,1,TOP
-/WIND,2,BOTTOM
-/GTYPE,1,GRPH,1
-/GTYPE,2,GRPH,1
-/GCMD,1,TBPLOT,BH,2
-/GCMD,2,TBPLOT,NB,2
-GPLOT
-/WIND,2,OFF
-/WIND,1,FULL
-SF=.0254               ! SET CONVERSION (INCHES TO METERS)
-CSYS,1
-K,1
-K,2,.3,-2.5            ! INNER RADIUS OF RING
-K,3,.45,-2.5           ! OUTER RADIUS OF RING
-K,4,.75,-2.5           ! OUTER RADIUS OF SURROUNDING AIR
-KPSCALE,ALL,,,SF,,,,,1 ! MOVE ORIGINAL KEYPOINTS TO NEW POSITION
-CSYS,0
-L,1,2
-LESIZE,1,,,5
-L,2,3
-LESIZE,2,,,6
-L,3,4
-LSYMM,2,ALL
-NUMMRG,KP              ! MERGE KEYPOINTS
-L,4,8                  ! DEFINE OUTER RADIUS LINE SEGMENT
-LESIZE,7,,,1
-TYPE,2
-ESIZE,,,1
-LMESH,7                ! MESH LINE SEGMENT (WITH BOUNDARY ELEMENT)
-A,2,6,1,1
-A,2,3,7,6
-A,3,4,8,7
-ASEL,S,AREA,,2
-AATT,2                 ! ASSIGN MATERIAL 2 TO STEEL AREA
-ASEL,ALL
-ESIZE,,1               ! DEFAULT ELEMENT DIVISIONS=1
-TYPE,1
-AMESH,1,2
-AMESH,3
-FINISH
-
-/SOLU                  ! ENTER SOLVER
-BFA,2,JS,,,438559      ! APPLY CURRENT DENSITY JS(Z)	
-SOLVE
-FINISH
-
-/POST1
-CSYS,1
-NSEL,S,LOC,X,.325*SF
-NSEL,A,LOC,X,.375*SF
-NSEL,A,LOC,X,.425*SF
-RSYS,1                 ! SET RESULTS C.S. TO CYLINDRICAL
-PRNSOL,B,COMP          ! PRINT NODAL FLUX DENSITY
-*GET,B1,NODE,44,B,SUM
-*GET,B2,NODE,48,B,SUM
-*GET,B3,NODE,52,B,SUM
-*DIM,LABEL,CHAR,3,2
-*DIM,VALUE,,3,3
-LABEL(1,1) = '@ R=','@ R=','@ R='
-LABEL(1,2) = '.325','.375','.425'
-*VFILL,VALUE(1,1),DATA,.48,1.03,1.22
-*VFILL,VALUE(1,2),DATA,B1,B2,B3
-*VFILL,VALUE(1,3),DATA,ABS(B1/.48),ABS(B2/1.03),ABS(B3/1.22)
-/COM
-/OUT,vm165,vrt,,APPEND
-/COM,PLANE233
+RESUME,TABLE_2
+/GOPR
+/COM,
+/COM,RESULTS USING SHELL181:
+/COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F13.2,'   ',1F15.3)
-/COM,-----------------------------------------------------------
+(1X,A8,A8,'   ',F10.7,'  ',F14.7,'   ',1F15.3)
+/COM,
+/COM,X=10.81 in
+/COM,
+*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
+/COM,
+/COM,X=27.1 in
+/COM,
+*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE3(1,1),VALUE3(1,2),VALUE3(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
+/COM,----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm165,vrt
+*LIST,vm39,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm166.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm166.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM166
 /PREP7
 SMRT,OFF
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM166, LONG CYLINDER IN A SINUSOIDAL MAGNETIC FIELD
 /COM,   ELECTROMAGNETIC WORKSHOP, RAL-86-049, EMSON, PAGE 39
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm167.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm167.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM167
 /PREP7
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM167, TRANSIENT EDDY CURRENTS IN A SEMI-INFINITE SOLID
 /COM,   HOLMAN, J.P., 'HEAT TRANSFER', 4TH EDITION, MCGRAW HILL,
 /COM,   INC., 1976, PAGE 104, EQN. 4-14 (ANALOGOUS FIELD SOLUTION)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm168.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm168.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM168
 /PREP7
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM168, MAGNETIC FIELD IN A NONFERROUS SOLENOID
 /COM,   PRINCIPLES OF ELECTRIC AND MAGNETIC FIELDS, BOAST, PG.243
 ANTYPE,STATIC
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm169.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm169.dat`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM169
+/OUT,SCRATCH
+_GEOMGEN_1=0                    ! SET THIS TO 1 TO UPDATE CDB FILE 
+_EXIT1=0                       ! SET THIS TO 1 TO EXIT WITHOUT SOLVING
+*IF,_GEOMGEN_1,EQ,1,THEN 
 /PREP7
 smrt,off
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM169, PERMANENT MAGNET CIRCUIT WITH AN AIR GAP
-/stitle,1,Reason COMPARE differences are acceptable:
-/stitle,2,  mesher accuracy - number of nodes, elements, numbering; near-zero values
 !                MAGNETO-SOLID MECHANICS, MOON, PG. 275
 !                USING TETRAHEDRAL SOLID ELEMENTS (SOLID98)
 ET,1,SOLID98,10             ! TETRAHEDRAL COUPLED-FIELD SOLID
 EMUNIT,MKS                  ! MKS UNITS
 MP,MURX,1,1
 MP,MURX,2,1E5               ! IRON RELATIVE PERMEABILITY
 MP,MURX,3,5.30504           ! PERMANENT MAGNET RELATIVE PERMEABILITY
@@ -46,18 +48,29 @@
 MSHA,1,3D                 ! USING TETS 
 VMESH,ALL
 VSEL,ALL
 VMESH,6                     ! MESH AIR GAP 
 NSEL,,LOC,X,0
 D,ALL,MAG,0                 ! SET FLUX-NORMAL BOUNDARY CONDITION
 NSEL,ALL
-WSORT,Y                     ! REORDER WAVEFRONT
+
+CDWRITE,db,vm169,cdb
+FINISH
+*IF,_EXIT1,EQ,1,THEN
+/EXIT,NOSAVE
+*ENDIF
+
+*ELSE
+CDREAD,db,vm169,cdb
+*ENDIF
 FINISH
 /SOLU    
+/OUT
 MAGSOLV,2                   ! RSP METHOD
+/OUT,SCRATCH
 FINISH
 /POST1
 RSYS,11
 /VIEW,,6E-2,5E-2,6E-2
 /EDGE,1,1
 /DEVICE,VECTOR,1	    ! TURN ON WIREFRAME MODE
 PLVECT,B                    ! DISPLAY B VECTOR
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm17.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm17.dat`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,71 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM17
 JPGPRF,500,100,1         ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
-smrt,off
 /TITLE, VM17, SNAP-THROUGH BUCKLING OF A HINGED SHELL
-:COM    CHANG, C.C.,"PERIODICALLY RESTARTED QUASI-NEWTON UPDATES IN
-:COM    IN CONSTANT ARC-LENGTH METHOD", COMPUTERS AND STRUCTURES,
-:COM    VOL. 41, NO. 5, PP. 963-972, 1991.
-C***    USING SHELL63 ELEMENTS
+!    CHANG, C.C.,"PERIODICALLY RESTARTED QUASI-NEWTON UPDATES IN
+!    IN CONSTANT ARC-LENGTH METHOD", COMPUTERS AND STRUCTURES,
+!    VOL. 41, NO. 5, PP. 963-972, 1991.
+/TITLE, VM17, SNAP-THROUGH BUCKLING OF A HINGED SHELL
+C***    USING SHELL181 ELEMENTS
+/PREP7
 ANTYPE,STATIC            ! STATIC ANALYSIS
-ET,1,SHELL63,,1
-R,1,6.350                ! SHELL THICKNESS
+ET,1,SHELL181
+SECT,1,SHELL
+SECD,6.350,1             ! SHELL THICKNESS
 MP,EX,1,3102.75
 MP,NUXY,1,0.3
-:COM  CREATE FINITE ELEMENT MODEL
+!  CREATE FINITE ELEMENT MODEL
 R1 = 2540                ! SHELL MID-SURFACE RADIUS
 L  = 254                 ! HALF THE LENGTH
 PI = 4*ATAN(1)           ! VALUE OF PI COMPUTED
 THETA = 0.1*180/PI       ! 0.1 RADIANS CONVERTED TO DEGREES
 CSYS,1                   ! CYLINDRICAL CO-ORDINATE SYSTEM
 N,1,R1,90                ! NODES 1 AND 2 ARE CREATED AT POINTS
 N,2,R1,90,L              ! A AND B RESPECTIVELY.
-K,1,R1,90
-K,2,R1,(90-THETA)
-K,3,R1,90,L
-K,4,R1,(90-THETA),L
-ESIZE,,2                 ! TWO DIVISION ALONG THE REGION BOUNDARY
-A,1,3,4,2
-AMESH,1
-NUMMRG,NODE           
+N,3,R1,(90-THETA)
+N,4,R1,(90-THETA),L
+FILL,1,2,1,5,1
+FILL,2,4,1,6,1
+FILL,4,3,1,7,1
+FILL,3,1,1,8,1
+FILL,8,6,1,9,1          
+E,3,8,9,7
+E,7,9,6,4
+E,8,1,5,9
+E,9,5,2,6
 FINISH
 *CREATE,SOLVIT,MAC
 /PREP7
-:COM  APPLY BOUNDARY CONDITIONS
+!  APPLY BOUNDARY CONDITIONS
 NSEL,S,LOC,Z,0
 DSYM,SYMM,Z
 NSEL,S,LOC,Y,90
 DSYM,SYMM,X
 NSEL,S,LOC,Y,(90-THETA)
 D,ALL,UX,,,,,UY,UZ
 NSEL,ALL
 FINISH
-:COM   SOLUTION PHASE
-:COM SINCE THE SOLUTION OUTPUT IS SUBSTANTIAL IT IS DIVERTED TO A 
-:COM  SCRATCH FILE
+!   SOLUTION PHASE
+! SINCE THE SOLUTION OUTPUT IS SUBSTANTIAL IT IS DIVERTED TO A SCRATCH FILE
 /OUTPUT,SCRATCH
 /SOLUTION
 NLGEOM,ON                ! LARGE DEFLECTION TURNED ON
 OUTRES,,1                ! WRITE SOLUTION ON RESULTS FILE FOR EVERY SUBSTEP 
 F,1,FY,-250              ! 1/4 TH OF THE TOTAL LOAD APPLIED DUE TO SYMMETRY
 NSUBST,30                ! BEGIN WITH 30 SUBSTEPS
 ARCLEN,ON,5              ! ARC-LENGTH SOLUTION TECHNIQUE TURNED ON WITH
                          !  MAX. ARC-LENGTH KEPT AT 5 TO COMPUTE AND STORE
 			 !  SUFFICIENT INTERMEDIATE SOLUTION INFORMATION
 SOLVE
 FINISH
 /OUTPUT
-:COM   POSTPROCESSING PHASE
+!   POSTPROCESSING PHASE
 /POST26
 NSOL,2,1,U,Y             ! STORE UY DISPLACEMENT OF NODE 1
 NSOL,3,2,U,Y             ! STORE UY DISPLACEMENT OF NODE 2
 PROD,4,1,,,LOAD,,,4*250  ! TOTAL LOAD IS 4*250 DUE TO QUARTER SYMMETRY
 PROD,5,2,,,,,,-1         ! CHANGE SIGNS OF THE DISPLACEMENT VALUES
 PROD,6,3,,,,,,-1
 *GET,UY1,VARI,2,EXTREM,VMIN
@@ -84,104 +88,68 @@
 LABEL(1,2) = 'mm ','mm '
 *VFILL,VALUE(1,1),DATA,-30,-26 
 *VFILL,VALUE(1,2),DATA,UY1,UY2
 *VFILL,VALUE(1,3),DATA,ABS(UY1/30) ,ABS(UY2/26 )
 FINISH
 *END
 SOLVIT
-SAVE,TABLE_1
-/CLEAR, NOSTART          ! CLEAR DATABASE FOR NEXT SOLUTION
-/TITLE, VM17, SNAP-THROUGH BUCKLING OF A HINGED SHELL
-C***    USING SHELL181 ELEMENTS
-/PREP7
-SMRT,OFF
-ANTYPE,STATIC            ! STATIC ANALYSIS
-ET,1,SHELL181
-SECT,1,SHELL
-SECD,6.350,1             ! SHELL THICKNESS
-MP,EX,1,3102.75
-MP,NUXY,1,0.3
-:COM  CREATE FINITE ELEMENT MODEL
-R1 = 2540                ! SHELL MID-SURFACE RADIUS
-L  = 254                 ! HALF THE LENGTH
-PI = 4*ATAN(1)           ! VALUE OF PI COMPUTED
-THETA = 0.1*180/PI       ! 0.1 RADIANS CONVERTED TO DEGREES
-CSYS,1                   ! CYLINDRICAL CO-ORDINATE SYSTEM
-N,1,R1,90                ! NODES 1 AND 2 ARE CREATED AT POINTS
-N,2,R1,90,L              ! A AND B RESPECTIVELY.
-K,1,R1,90
-K,2,R1,(90-THETA)
-K,3,R1,90,L
-K,4,R1,(90-THETA),L
-ESIZE,,2                 ! TWO DIVISION ALONG THE REGION BOUNDARY
-A,1,3,4,2
-AMESH,1
-NUMMRG,NODE           
-FINISH
-SOLVIT
-SAVE,TABLE_2
+SAVE,TABLE_1              
 /CLEAR, NOSTART          ! CLEAR DATABASE FOR NEXT SOLUTION
 /TITLE, VM17, SNAP-THROUGH BUCKLING OF A HINGED SHELL
 C***    USING SHELL281 ELEMENTS
 /PREP7
-SMRT,OFF
 ANTYPE,STATIC            ! STATIC ANALYSIS
 ET,1,SHELL281
 SECT,1,SHELL
 SECD,6.350,1             ! SHELL THICKNESS
 MP,EX,1,3102.75
 MP,NUXY,1,0.3
-:COM  CREATE FINITE ELEMENT MODEL
+!  CREATE FINITE ELEMENT MODEL
 R1 = 2540                ! SHELL MID-SURFACE RADIUS
 L  = 254                 ! HALF THE LENGTH
 PI = 4*ATAN(1)           ! VALUE OF PI COMPUTED
 THETA = 0.1*180/PI       ! 0.1 RADIANS CONVERTED TO DEGREES
 CSYS,1                   ! CYLINDRICAL CO-ORDINATE SYSTEM
 N,1,R1,90                ! NODES 1 AND 2 ARE CREATED AT POINTS
 N,2,R1,90,L              ! A AND B RESPECTIVELY.
-K,1,R1,90
-K,2,R1,(90-THETA)
-K,3,R1,90,L
-K,4,R1,(90-THETA),L
-ESIZE,,2                 ! TWO DIVISION ALONG THE REGION BOUNDARY
-A,1,3,4,2
-AMESH,1
-NUMMRG,NODE           
+N,3,R1,(90-THETA)
+N,4,R1,(90-THETA),L
+FILL,1,2,3,5,1
+FILL,2,4,3,8,1
+FILL,4,3,3,11,1
+FILL,3,1,3,14,1
+FILL,6,12,3,17,1  
+FILL,9,15,3,20,1
+NUMMRG,NODE
+E,3,12,18,15,13,19,22,14  
+E,12,4,9,18,11,10,20,19
+E,15,18,6,1,22,17,5,16
+E,18,9,2,6,20,8,7,17 
 FINISH
 SOLVIT
-SAVE,TABLE_3
+SAVE,TABLE_2
 /NOPR
 RESUME,TABLE_1
 /COM
 /OUT,vm17,vrt
 /COM,------------------- VM17 RESULTS COMPARISON ---------------------
-/COM,
-/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
-/COM,
-/COM,SHELL63
-/COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
-/NOPR
-RESUME,TABLE_2
 /GOPR
 /COM,
 /COM,SHELL181
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
 /NOPR
-RESUME,TABLE_3
+RESUME,TABLE_2
 /GOPR
 /COM,
 /COM,SHELL281
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
 /COM,-------------------------------------------------------------
 /OUT
 FINISH
 *LIST,vm17,vrt
 /DELETE,TABLE_1
 /DELETE,TABLE_2
-/DELETE,TABLE_3
 /DELETE,SOLVIT,MAC
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm170.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm170.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM170
 /PREP7
 /TITLE, VM170, MAGNETIC FIELD FROM A SQUARE CURRENT LOOP
 /COM,   REF. BOAST, "PRINCIPLES OF ELECTRIC AND MAGNETIC FIELDS"
 /COM,   PG. 200
 ET,1,LINK68               ! LINK68 ELEMENT
 R,1,1                     ! ARBITRARY AREA
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm171.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm171.dat`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM171
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/PREP7
 /TITLE, VM171, PERMANENT MAGNET CIRCUIT WITH AN ELASTIC KEEPER
 /COM,   MAGNETO-SOLID MECHANICS, MOON, PG. 275
+
+/COM,   USING PLANE13 - 2-D COUPLED-FIELD SOLID
+/PREP7
 ET,1,PLANE13,4                  ! 2-D COUPLED-FIELD SOLID (UX,UY,AZ DOF'S)
 ET,2,COMBIN14,,,2
 R,1,1.6534E5                    ! SPRING CONSTANT
 MP,EX,1,1E2                     
 MP,EX,2,10E10
 MP,EX,3,10E10
 MP,EX,4,10E10
@@ -91,19 +93,129 @@
 *DIM,LABEL,CHAR,2,2
 *DIM,VALUE,,2,3
 LABEL(1,1) = 'DEFL ','MFLUX '
 LABEL(1,2) = 'm','T'
 *VFILL,VALUE(1,1),DATA,1.5E-3,.2496
 *VFILL,VALUE(1,2),DATA,Y,B
 *VFILL,VALUE(1,3),DATA,ABS(Y/1.5E-3),ABS(B/.2495)
+SAVE,TABLE1
+FINI
+/CLEAR,NOSTART
+
+/COM,   USING PLANE223 - 2-D 8-NODE COUPLED-FIELD SOLID
+/PREP7
+ET,1,PLANE223,10001             ! elastic air
+keyop,1,4,1
+ET,2,COMBIN14,,,2
+ET,3,PLANE223,10001             ! ferromagnetic core, PM
+keyop,3,4,0
+ET,4,PLANE223,10001             ! keeper
+keyop,4,4,0
+R,1,1.6534E5                    ! SPRING CONSTANT
+MP,EX,1,1E2                     
+MP,EX,2,10E10
+MP,EX,3,10E10
+MP,EX,4,10E10
+MP,NUXY,1,0.0
+*REP,4,,1
+MP,KXX,1,1                      ! APPLY DUMMY KXX TO PREVENT WARNING MSGS.
+*REP,4,,1
+EMUNIT,MKS                      ! MKS UNITS
+MP,MURX,1,1                     ! AIR RELATIVE PERMEABILITY
+MP,MURX,2,1E5                   ! IRON RELATIVE PERMEABILITY
+MP,MURX,3,5.30504               ! PERMANENT MAGNET RELATIVE PERMEABILITY
+MP,MGXX,3,149990.0              ! COERCIVE FORCE (X-DIRECTION)
+MP,MURX,4,1E5                   ! KEEPER RELATIVE PERMEABILITY
+N,1
+N,6,5E-2
+FILL
+NGEN,6,6,1,6,1E-2,,1E-2
+N,37,0,6E-2
+N,38,5E-2,6E-2
+type,3
+MAT,3
+E,2,3,9,8
+EGEN,3,1,-1
+MAT,2
+E,1,2,8,7
+EGEN,3,6,-1
+E,5,6,12,11
+EGEN,3,6,-1
+type,4
+MAT,4
+E,25,26,32,31
+EGEN,5,1,-1
+type,1
+MAT,1
+E,19,20,26,25
+E,23,24,30,29
+TYPE,2                          ! SPRINGS
+E,37,31
+E,38,36
+D,37,ALL,0,,38                  ! CONSTRAIN SPRING
+ESEL,S,MAT,,2,3
+NSLE
+D,ALL,UX,0,,,,UY                ! CONSTRAIN PERMANENT MAGNET STRUCTURE
+ESEL,ALL
+NSEL,S,LOC,X,0
+NSEL,A,LOC,X,5E-2
+NSEL,A,LOC,Y,0
+NSEL,A,LOC,Y,5E-2
+D,ALL,AZ,0                      ! SET EXTERIOR FLUX-PARALLEL BOUNDARY
+NSEL,ALL
+CP,1,AZ,8,9,10,11,14            ! COUPLE INTERNAL NODES
+CP,1,AZ,17,20,23,26
+CP,1,AZ,27,28,29
+NSLE                            ! SELECT ONLY NODES USED IN MODEL
+D,ALL,UX,0                      ! CONSTRAIN ALL HORIZONTAL DISPLACEMENTS
+FINISH
+/SOLU    
+NLGEOM,ON                       ! ACTIVATE LARGE DEFLECTION
+CNVTOL,F                        ! SET FORCE CONVERGENCE (USE DEFAULTS)
+CNVTOL,CSG                      ! SET CSG CONVERGENCE (.001% OF DEFAULT)
+SOLVE
+FINISH
+/POST1
+NSEL,S,LOC,Y,4e-2
+PRNSOL,U,COMP                   ! PRINT NODAL DISPLACEMENTS
+*GET,Y1,NODE,25,U,Y
+*SET,Y,ABS(Y1)
+ESEL,S,MAT,,3
+NSLE
+PRNSOL,B,COMP                   ! PRINT NODAL FLUX DENSITY IN PERMANENT MAGNET
+*GET,B,NODE,2,B,X
+NSEL,ALL
+ESEL,S,MAT,,2,4                 ! SELECT ONLY ELEMENTS OF IRONAND KEEPER
+/EDGE,1,1
+/DSCALE,1,1                     ! TRUE SCALING OPTION
+PLDISP,1                        ! DISPLAY DEFLECTED AND UNDEFLECTED SHAPE
+*DIM,LABEL,CHAR,2,2
+*DIM,VALUE,,2,3
+LABEL(1,1) = 'DEFL ','MFLUX '
+LABEL(1,2) = 'm','T'
+*VFILL,VALUE(1,1),DATA,1.5E-3,.2496
+*VFILL,VALUE(1,2),DATA,Y,B
+*VFILL,VALUE(1,3),DATA,ABS(Y/1.5E-3),ABS(B/.2495)
+SAVE,TABLE2
+FINI
+
+/NOPR
 /COM
 /OUT,vm171,vrt
 /COM,------------------- VM171 RESULTS COMPARISON -------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
+/COM,PLANE13:
+RESUME,TABLE1
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
+(1X,A8,A8,'  ',E11.5,'  ',E14.5,' ',1F16.4)
+/COM,
+/COM,PLANE223:
+RESUME,TABLE2
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'  ',E11.5,'  ',E14.5,' ',1F16.4)
+/COM,
 /COM,----------------------------------------------------------
 /OUT
 FINISH
 *LIST,vm171,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm172.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm172.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM172
+/NOPR
 /PREP7
 smrt,off
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM172, STRESS ANALYSIS OF A LONG, THICK, ISOTROPIC SOLENOID
 /COM,   MAGNETO-SOLID MECHANICS, MOON, PG. 275, 2D ANALYSIS
 ANTYPE,STATIC                       ! COUPLED FIELD ANALYSIS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm173.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm173.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM173
 /PREP7
 /TITLE, VM173, CENTERLINE TEMPERATURE OF AN ELECTRICAL WIRE
 C***      HEAT, MASS AND MOMENTUM TRANS., ROHSENOW AND CHOI, 2ND. PR., PAGE 106,
 C***      EX. 6.5, USING SOLID5 ELEMENTS
 ET,1,SOLID5,1                    ! SOLID5, TEMP,VOLT,MAG DOF OPTION
 MP,KXX,1,13                      ! THERMAL CONDUCTIVITY
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm174.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm174.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM174
 /PREP7
 MP,PRXY,,0.3
 MP,PRXY,,0.3
 SMRT,OFF
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
@@ -119,8 +119,9 @@
 /COM
 /OUT,vm174,vrt,,APPEND
 /COM,PLANE223
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
 /COM,----------------------------------------------------------
 /OUT
+FINISH
 *LIST,vm174,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm175.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm175.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM175
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 SMRT,OFF
 /TITLE, VM175, NATURAL FREQUENCY OF A PIEZOELECTRIC TRANSDUCER
 /COM,         COMPUTATION OF THE VIBRATIONAL MODES FOR PIEZOELECTRIC
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm176.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm176.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM176
 /PREP7
 SMRT,OFF
 /TITLE, VM176, FREQUENCY RESPONSE OF ELECTRICAL INPUT ADMITTANCE FOR A
 /COM           PIEZOELECTRIC TRANSDUCER
 /COM    KAGAWA AND YAMABUCHI, FINITE ELEMENT SIMULATION OF A COMPOSITE
 /COM    PIEZOELECTRIC ULTRASONIC TRANSDUCER, IEEE TRANS. SONICS AND
 /COM    ULTRASONICS, VOL. SU-26, NO.2, MARCH 1979
+/out,scratch
 ET,1,SOLID5,0                    ! 3-D COUPLED-FIELD SOLID
 MP,DENS,3,7730                   ! NEPEC DENSITY
 MP,EX,2,7.03E10                  ! ALUMINUM MODULUS OF ELASTICITY
 MP,NUXY,2,.345                   ! ALUMINUM POISSON RATIO
 MP,DENS,2,2690                   ! ALUMINUM DENSITY
 MP,EX,4,10E9                     ! ADHESIVE MODULUS OF ELASTICITY
 MP,DENS,4,1700                   ! ADHESIVE DENSITY
@@ -101,15 +102,14 @@
 EQSLV,ICCG                       ! ICCG SOLVER
 SOLVE
 HARFRQ,39000,45000               ! SOLVE FOR FREQ=42KHZ AND 45KHZ
 SOLVE
 HARFRQ,46000,54000               ! SOLVE FOR FREQ=50KHZ AND 54KHZ
 SOLVE
 FINISH
-/out
 /POST26
 RFORCE,2,N1,AMPS                 ! STORE CHARGES ON ELECTRODE
 PI2=(3.14159*2.)
 PROD,3,2,1,,MHOS,,,PI2           ! CALCULATE ADMITTANCE (10 DEG. SLICE)
 PROD,4,3,,,MMHO,,,36000          ! CALCULATE TOTAL ADMITTANCE (MMHOS)
 PRVAR,4                          ! PRINT ELECTRICAL ADMITTANCE VS. FREQUENCY
 *GET,F1,VARI,4,RTIME,20000
@@ -135,14 +135,15 @@
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /OUT
 
 FINISH
 
 /CLEAR,NOSTART
+/out,scratch
 /PREP7
 SMRT,OFF
 ET,1,SOLID186,,1                 ! 3-D STRUCTURAL SOLID
 MP,DENS,3,7730                   ! NEPEC DENSITY
 MP,EX,2,7.03E10                  ! ALUMINUM MODULUS OF ELASTICITY
 MP,NUXY,2,.345                   ! ALUMINUM POISSON RATIO
 MP,DENS,2,2690                   ! ALUMINUM DENSITY
@@ -222,28 +223,28 @@
 CP,1,VOLT,ALL                    ! COUPLE VOLT DOF ON ELECTRODE
 *GET,N1,NODE,,NUM,MIN            ! GET NODE ON ELECTRODE
 D,N1,VOLT,-0.5                   ! APPLY -0.5 VOLT TO TOP ELECTRODE
 NSEL,S,LOC,Z,0                   ! SELECT NODES AT SYMMETRY PLANE
 D,ALL,VOLT,0.0                   ! SET VOLT TO ZERO AT SYMMETRY PLANE
 NSEL,ALL
 FINISH
-/out,scratch
-/SOLU
+
+/SOLUTION
 ANTYPE,HARMIC                    ! PERFORM HARMONIC ANALYSIS
 OUTRES,ALL,ALL                   ! STORE EVERY SUBSTEP
 HARFRQ,5000,35000                ! SOLVE FOR FREQ=20KHZ AND 35KHZ
 NSUBST,2
 KBC,1                            ! STEP BOUNDARY CONDITIONS  
 SOLVE
 HARFRQ,39000,45000               ! SOLVE FOR FREQ=42KHZ AND 45KHZ
 SOLVE
 HARFRQ,46000,54000               ! SOLVE FOR FREQ=50KHZ AND 54KHZ
 SOLVE
 FINISH
-/out
+
 /POST26
 RFORCE,2,N1,CHRG                 ! STORE CHARGE ON ELECTRODE
 PI2=(3.14159*2.)
 PROD,3,2,1,,MHOS,,,PI2           ! CALCULATE ADMITTANCE (10 DEG. SLICE)
 PROD,4,3,,,MMHO,,,36000          ! CALCULATE TOTAL ADMITTANCE (MMHOS)
 PRVAR,4                          ! PRINT ELECTRICAL ADMITTANCE VS. FREQUENCY
 *GET,F1,VARI,4,RTIME,20000
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm177.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm177.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM177
 /PREP7  
 JPGPRF,500,100,1               ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM177, NATURAL FREQUENCY OF SUBMERGED RING
 /COM, REF. "FINITE ELEMENT SOLUTION OF FLUID STRUCTURE
 /COM, INTERACTION PROBLEMS"  SCHROEDER & MARCUS
@@ -92,16 +92,16 @@
 SOLVE
 FINISH
 
 /POST26
 NSOL,2,1,U,X
 NSOL,3,41,U,X
 NSOL,4,81,U,Y
-/OUT,
 PRVAR,2,3,4                    	! PRINT DISPLACEMENTS OF RING VS. FREQUENCY
+/OUT,
 /COM,
 /COM, GETTING THE FREQUENCY AT WHICH RESONANCE OCCURS
 /COM, EXPECT THE FREQUENCY TO BE SAME FOR ALL 3 VARIABLES
 /COM,
 *GET,MAXFRQ1,VARI,2,EXTREM,TMAX
 *GET,MAXFRQ2,VARI,3,EXTREM,TMAX
 *GET,MAXFRQ3,VARI,4,EXTREM,TMIN
@@ -299,16 +299,16 @@
 SOLVE
 FINISH
 
 /POST26
 NSOL,2,1,U,X
 NSOL,3,41,U,X
 NSOL,4,81,U,Y
-/OUT,
 PRVAR,2,3,4                    	! PRINT DISPLACEMENTS OF RING VS. FREQUENCY
+/OUT,
 /COM,
 /COM, GETTING THE FREQUENCY AT WHICH RESONANCE OCCURS
 /COM, EXPECT THE FREQUENCY TO BE SAME FOR ALL 3 VARIABLES
 /COM,
 *GET,MAXFRQ1,VARI,2,EXTREM,TMAX
 *GET,MAXFRQ2,VARI,3,EXTREM,TMAX
 *GET,MAXFRQ3,VARI,4,EXTREM,TMIN
@@ -439,16 +439,16 @@
 SOLVE
 FINISH
 
 /POST26
 NSOL,2,203,U,X
 NSOL,3,211,U,X
 NSOL,4,191,U,Y
-/OUT,
 PRVAR,2,3,4                    	! PRINT DISPLACEMENTS OF RING VS. FREQUENCY
+/OUT,
 /COM,
 /COM, GETTING THE FREQUENCY AT WHICH RESONANCE OCCURS
 /COM, EXPECT THE FREQUENCY TO BE SAME FOR ALL 3 VARIABLES
 /COM,
 *GET,MAXFRQ1,VARI,2,EXTREM,TMAX
 *GET,MAXFRQ2,VARI,3,EXTREM,TMAX
 *GET,MAXFRQ3,VARI,4,EXTREM,TMIN
@@ -578,16 +578,16 @@
 SOLVE
 FINISH
 
 /POST26
 NSOL,2,423,U,X
 NSOL,3,433,U,X
 NSOL,4,407,U,Y
-/OUT,
 PRVAR,2,3,4                    	! PRINT DISPLACEMENTS OF RING VS. FREQUENCY
+/OUT,
 /COM,
 /COM, GETTING THE FREQUENCY AT WHICH RESONANCE OCCURS
 /COM, EXPECT THE FREQUENCY TO BE SAME FOR ALL 3 VARIABLES
 /COM,
 *GET,MAXFRQ1,VARI,2,EXTREM,TMAX
 *GET,MAXFRQ2,VARI,3,EXTREM,TMAX
 *GET,MAXFRQ3,VARI,4,EXTREM,TMIN
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm178.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm178.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM178
 /TITLE, VM178, TWO DIMENSIONAL DOUBLE CANTILEVER BEAM PROBLEM
 /COM, REFERENCE:" J.F.MANDELL, ET AL., PREDICTION OF DELAMINATION IN 
 /COM,             WIND TURBINE BLADE STRUCTURAL DETAILS
 /COM,             JOURNAL OF SOLAR ENERGY ENGINEERING, VOL. 25, 2003, PG: 522-530
 /COM,
 /OUT,SCRATCH
@@ -12,15 +12,15 @@
 PP=10                       ! LOADING
 A=DL*0.3                    ! CRACK LENGTH
 ET,1,PLANE182               ! 2D 4-NODE STRUCTURAL SOLID ELEMENT
 KEYOPT,1,3,2                ! PLANE STRAIN
 
 !MATERIAL PROPERTIES
 YOUNG = 210000              ! YOUNG'S MODULUS
-NU = 0.3                    ! POISSION'S RATIO
+NU = 0.3                    ! POISSON'S RATIO
 MP,EX,1,YOUNG               !MPa
 MP,PRXY,1,NU
 
 RECTNG,0,DL,DH/2            !DEFINE AREAS
 RECTNG,0,DL,0,-DH/2
 LSEL,S,LINE,,2,8,2          !DEFINE LINE DIVISION
 LESIZE,ALL,DH/4
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm179.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm179.dat`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM179
 /PREP7
 /TITLE, VM179, DYNAMIC DOUBLE ROTATION OF A JOINTED BEAM
 C***   REFERENCE -- ANY BASIC MECHANICS TEXT
 ANTYPE,TRANS                ! FULL TRANSIENT DYNAMIC ANALYSIS
 NLGEOM,ON                   ! LARGE DEFLECTION
 TRNOPT,FULL,,,,,HHT         ! USE HHT METHOD
@@ -35,18 +35,23 @@
 SECLOCK,4,-0.08727,0.08727  ! JOINT LOCK-UP WHEN STOP ENGAGED
 TYPE,1
 SECN,1
 E,2,3                       ! JOINT ELEMENT
 D,1,UX,0,,,,UY,UZ,ROTX,ROTY ! ALLOW ONLY Z-ROTATION AT PINNED END
 KBC,1
 FINISH
-/OUTPUT,SCRATCH             ! SEND SUBSEQUENT OUTPUT TO SCRATCH FILE
-/SOLU    
+/OUT,vm179_SCRATCH          ! SEND SUBSEQUENT OUTPUT TO SCRATCH FILE
+/SOLU
+DMPOPT,RNNN,YES    
+SOLCONT,ON
 PRED,ON
 CNVTOL,M
+CNVTOL,F,-1
+CNVTOL,U,-1
+CNVTOL,ROT,-1
 NSUBST,100,1000,10
 F,1,MZ,.7854                ! BEGIN ROTZ WITH NON-ZERO ACCELERATION
 TIME,.05
 SOLVE
 NSUBST,60
 TIME,1               ! DELTA THETA-Z = 45 DEG. ( AT 1 SEC )
 SOLVE
@@ -74,26 +79,20 @@
 *GET,DY2,NODE,4,U,Y
 *GET,RZ2,NODE,4,ROT,Z
 ESEL,S,TYPE,,1
 ETABLE,REFL
 ESEL,ALL
 PRETAB,ROTATE,ROT_STAT
 FINISH
+
 PARSAV
-/COPY,,rdb,,rest,rdb          ! SAVE THE FILES NEEDED FOR RESTART (NOT NEEDED
-/COPY,,ldhi,,rest,ldhi        ! FOR STRAIGHT-THRU RUN)
-/COPY,,r001,,rest,r001
-/COPY,,rst,,rest,rst          ! NEEDED FOR CONTINUITY OF THE RESULTS FILE
 /CLEAR,NOSTART                ! CLEAR THE DATABASE (TO SIMULATE RESTART)
 /COM,    
 /COM,        -----     RESTART  ANALYSIS    -----
-/COPY,rest,rdb,,file,rdb      ! COPY THE FILES NEEDED FOR RESTART (NOT NEEDED
-/COPY,rest,ldhi,,file,ldhi    ! FOR STRAIGHT-THRU RUN)
-/COPY,rest,r001,,file,r001
-/COPY,rest,rst,,file,rst
+
 /SOLU    
 ANTYPE,,REST         ! USE RESTART ANALYSIS TO DEFINE MORE LOADSTEPS
 F,1,MZ,0             ! REMOVE M1, ALLOW ROTZ MOTION TO STABILIZE
 TIME,2.05
 SOLVE
 NSUBST,60
 FJ,5,MX,-0.5         ! DELTA THETA-X = 5 DEG., THEN STOP ( AT 3 SEC )
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm18.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm18.dat`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM18
 /PREP7
 /TITLE, VM18, OUT-OF-PLANE BENDING OF A CURVED BAR
 !    USING PIPE18    STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 412, EQN. 241
 ANTYPE,STATIC
 ET,1,PIPE18,,,,,,2   ! KEYOPT(6)=2 PRINTS MEMBER FORCES
 MP,EX,1,30E6
@@ -40,48 +40,46 @@
 FINI
 /CLEAR,NOSTART
 
 !**********************************************
 
 /SHOW,JPEG
 /PREP7
-!     USING ELBOW290   
+!     USING PIPE289  
 ANTYPE,STATIC
-ET,1,ELBOW290
+ET,1,PIPE289,,, ,2
 MP,EX,1,30E6
 MP,NUXY,1,.3
 SECTYPE,1,PIPE
-SECDATA,2,1,8	     ! OD = 2, WALL THICKNESS = 1
-
-K,1,100              ! DEFINE NODES
-K,2,,100
-K,3,70.710,70.710
-LARC,1,2,3
-LESIZE,1,,,9
-LMESH,ALL
-
-DK,1,ALL              ! BOUNDARY CONDITIONS + LOAD
-FK,2,FZ,-50
+SECDATA,2,1,16	     ! OD = 2, WALL THICKNESS = 1
+CSYS,1
+N,1,100              ! DEFINE NODES
+NGEN,19,1,1,,,,5
+E,1,3,2
+EGEN,9,2,-1
+CSYS,0
+D,1,ALL              ! BOUNDARY CONDITIONS + LOAD
+F,19,FZ,-50
 FINISH
 /SOLU    
 OUTPR,BASIC,1
 /OUT,SCRATCH
 SOLVE
 FINISH 
 /POST1
 SET,LAST
 /GRAPHICS,POWER
 /ESHAPE,1
 /VIEW,1,1,1,1
 /OUT,
-*GET,DEF,NODE,2,U,Z
-ETABLE,STRS_BEN,SMISC,12
+*GET,DEF,NODE,19,U,Z
+ETABLE,STRS_BEN,SMISC,35
 *GET,STRSS_B,ELEM,1,ETAB,STRS_BEN
-PLESOL,S,YZ
-*GET,SHEAR,PLNSOL,0,MAX
+PLESOL,S,XY
+*GET,SHEAR,PLNSOL,0,MIN
 *DIM,LABEL,CHAR,3,2
 *DIM,VALUE,,3,3
 LABEL(1,1) = 'DEFLECTI','STRSS BE','STRSS SH'
 LABEL(1,2) = 'ON (in) ','ND   psi','EAR  psi'
 *VFILL,VALUE(1,1),DATA,-2.648,6366,-3183
 *VFILL,VALUE(1,2),DATA,DEF,ABS(STRSS_B) ,SHEAR 
 *VFILL,VALUE(1,3),DATA,ABS(DEF/2.648) ,ABS(STRSS_B /6366 ),ABS(SHEAR /3183 )
@@ -97,15 +95,15 @@
 /COM,
 RESUME,TABLE_1
 /COM,USING PIPE18
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
 /COM,
 RESUME,TABLE_2 
-/COM,USING ELBOW290
+/COM,USING PIPE289
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
 /COM,
 /COM,-----------------------------------------------------------------
 /OUT
 
 FINISH
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm180.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm180.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM180
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 smrt,off
 /TITLE, VM180, BENDING OF A CURVED BEAM
 C***    THEORY OF ELASTICITY, TIMOSHENKO & GOODIER, 3RD ED., P. 78
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm181.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm181.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM181
 /PREP7
 SMRT,OFF
 /TITLE, VM181, NATURAL FREQUENCY OF A FLAT CIRCULAR PLATE WITH A CLAMPED EDGE
 C***          FORMULAS FOR NATURAL FREQUENCY AND MODE SHAPE, BLEVINS, PAGE 241
 ET,1,PLANE183,,,1       ! AXISYMMETRIC ELEMENTS
 MP,EX,1,3E7
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm182.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm182.dat`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM182
 /PREP7   
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/TITLE, VM182; TRANSIENT RESPONSE OF A SPRING-MASS SYSTEM
+/TITLE, VM182, TRANSIENT RESPONSE OF A SPRING-MASS SYSTEM
 C***               R. K. VIERCK, "VIBRATION ANALYSIS", 2ND EDITION, SEC.5-8
 ANTYPE,MODAL          ! MODE-FREQUENCY ANALYSIS
 MODOPT,LANB,2,,,      ! PRINT TWO REDUCED MODE SHAPES
 ET,1,COMBIN40,,,2     ! UY DOF
 R,1,6,,2              ! K1=6 N/M     M1=2 KG
 R,2,16,,2             ! K2=16 N/M    M2=2 KG
 N,1
@@ -16,32 +16,40 @@
 REAL,1
 E,1,2
 REAL,2
 E,2,3
 D,3,ALL
 OUTPR,,ALL
 FINISH
-/SOLU    
+/SOLU
+/OUT,vm182_SCRATCH    
 SOLVE
+/OUT
 FINISH
 /SOLU    
 ANTYPE,TRANS          ! TRANSIENT DYNAMIC ANALYSIS
 TRNOPT,MSUP,2         ! MODE SUPERPOSITION, BOTH MODES
 DELTIM,0.01           ! INTEGRATION TIME STEP = .01
 OUTPR,,NONE
 OUTRES,,1
 KBC,1                 ! STEP BOUNDARY CONDITIONS
 F,1,FY,0              ! FORCE = 0 AT TIME = 0 (INIT. CONDITIONS)
+/OUT,vm182_SCRATCH,,,APPEND    
 SOLVE
+/OUT
 TIME,1.8
 F,1,FY,50             ! FORCE = 50N FROM TIME = 0 TO 1.8 SEC
+/OUT,vm182_SCRATCH,,,APPEND    
 SOLVE
+/OUT
 TIME,2.4
 F,1,FY,0              ! FORCE = 0 FROM TIME = 1.8 TO 2.4 SEC
+/OUT,vm182_SCRATCH,,,APPEND    
 SOLVE
+/OUT
 FINISH
 /POST26
 FILE,,rdsp            ! REDUCED DISPLACEMENTS FILE
 NSOL,2,1,U,Y,UY1
 NSOL,3,2,U,Y,UY2
 /GRID,1
 /AXLAB,Y,DISP
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm183.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm183.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM183
 /PREP7  
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM183,  HARMONIC RESPONSE OF A SPRING-MASS SYSTEM
 C***  R.K. VIERCK, "VIBRATION ANALYSIS", 2ND EDITION, SECTION 4-2
 ANTYPE,MODAL         ! MODE - FREQUENCY ANALYSIS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm184.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm184.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM184
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 smrt,off
 /TITLE, VM184, STRAIGHT CANTILEVER BEAM
 C***  ANY BASIC MECHANICS OF MATERIALS TEXT
 C***  USING SOLID5 HEXAHEDRONS
+/OUT,SCRATCH
 ANTYPE,STATIC         ! STATIC ANALYSIS
 ET,1,SOLID5,2         ! MULTI-FIELD SOLID5
 MP,EX,1,1E7
 MP,NUXY,1,0.3
 K,1
 K,2,6
 KGEN,2,1,2,1,,.2
@@ -21,15 +22,14 @@
 V,1,2,4,3,5,6,8,7
 VMESH,1
 NSEL,S,LOC,X,0
 D,ALL,ALL              ! CONSTRAIN LEFT END
 NSEL,ALL
 FK,2,FX,0.25           ! APPLY AXIAL FORCES
 *REPEAT,4,2
-NOORDER
 FINISH
 /SOLU    
 SOLVE
 FKDELE,ALL,FX          ! DELETE AXIAL FORCES
 FK,2,FY,0.25           ! APPLY IN-PLANE LOADS
 *REPEAT,4,2
 SOLVE
@@ -349,39 +349,39 @@
 /OUT,vm184,vrt
 /COM,------------------- VM184 RESULTS COMPARISON ------------
 /COM,
 /COM,                      TARGET   |    Mechanical APDL   |    RATIO
 /COM, SOLID5
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.6,'  ',F15.6,'   ',1F16.3)
+(1X,A8,A8,'   ',F11.3,'  ',F15.3,'   ',1F16.2)
 /NOPR
 RESUME,TABLE_2
 /GOPR
 /COM,
 /COM, SOLID92
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.6,'  ',F15.6,'   ',1F16.3)
+(1X,A8,A8,'   ',F11.3,'  ',F15.3,'   ',1F16.2)
 /NOPR
 RESUME,TABLE_3
 /GOPR
 /COM,
 /COM, SOLID98
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.6,'  ',F15.6,'   ',1F16.3)
+(1X,A8,A8,'   ',F11.3,'  ',F15.3,'   ',1F16.2)
 /NOPR
 RESUME,TABLE_4
 /GOPR
 /COM,
 /COM, SOLID187
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.6,'  ',F15.6,'   ',1F16.3)
+(1X,A8,A8,'   ',F11.3,'  ',F15.3,'   ',1F16.2)
 /COM,---------------------------------------------------------
 /OUT
 FINISH
 /DELETE,MAC
 /DELETE,TABLE_1
 /DELETE,TABLE_2
 /DELETE,TABLE_3
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm185.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm185.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM185
 /PREP7
 SMRT,OFF
 /TITLE, VM185, AC ANALYSIS OF A SLOT EMBEDDED CONDUCTOR
 C***    KONRAD, A., "INTEGRODIFFERENTIAL FINITE ELEMENT FORMULATION
 C***    OF TWO-DIMENSIONAL STEADY-STATE SKIN EFFECT PROBLEMS",
 C***    IEEE TRANS. MAGNETICS, VOL. MAG-18, NO. 1, JAN. 1982
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm186.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm186.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM186
 /PREP7  
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM186, TRANSIENT ANALYSIS OF A SLOT EMBEDDED CONDUCTOR
 C***            KONRAD, IEEE TRANS., MAGNETICS, VOL. MAG-18, NO. 1, JAN. 1982
 /NOPR
+/OUT,vm186_SCRATCH
+/OUT
 ANTYPE,TRANS                  ! NONLINEAR TRANSIENT DYNAMIC ANALYSIS
 ET,1,PLANE13                  ! PLANE13, AZ DOF, (FOR AIR)
 ET,2,PLANE13,6                ! PLANE13, AZ VOLT DOF, (FOR CONDUCTOR)
 EMUNIT,MUZRO,1                ! SET MUZERO=1
 MP,MURX,1,1                   ! RELATIVE PERMEABILITY
 MP,MURX,2,1                   ! RELATIVE PERMEABILITY (CONDUCTOR)
 MP,RSVX,2,1                   ! RESISTIVITY (CONDUCTOR)
@@ -53,15 +55,17 @@
 *IF,C,EQ,((N*.75)+1),THEN     ! SET FOR PRINTOUT AT DESIRED TIME POINTS
  OUTPR,,1
 *ELSEIF,C,EQ,(N+1),THEN
  OUTPR,,1
 *ELSE
  OUTPR,,0
 *ENDIF
+/OUT,vm186_SCRATCH,,,APPEND
 SOLVE
+/OUT
 *END
 *DO,I,1,81                    ! REPEAT MACRO EXECUTION
  *USE,LOAD                    ! EXECUTE MACRO
 *ENDDO
 FINISH
 /POST26
 NUMVAR,12                     ! INCREASE STORAGE ARRAY SIZE
@@ -187,15 +191,17 @@
 *IF,C,EQ,((N*.75)+1),THEN     ! SET FOR PRINTOUT AT DESIRED TIME POINTS
  OUTPR,,1
 *ELSEIF,C,EQ,(N+1),THEN
  OUTPR,,1
 *ELSE
  OUTPR,,0
 *ENDIF
+/OUT,vm186_SCRATCH,,,APPEND
 SOLVE
+/OUT
 *END
 *DO,I,1,81                    ! REPEAT MACRO EXECUTION
  *USE,LOAD                    ! EXECUTE MACRO
 *ENDDO
 FINISH
 /POST26
 NUMVAR,12                     ! INCREASE STORAGE ARRAY SIZE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm187.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm187.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM187
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 smrt,off
 /TITLE, VM187, BENDING OF A CURVED BEAM
 C***  FORMULAS FOR STRESS AND STRAIN, ROARK, 4TH ED.
+/out,scratch
 ANTYPE,STATIC
 ET,1,SOLID5,2             ! USING SOLID5 HEXAHEDRONS, DISPLACEMENT DOF ONLY
 MP,EX,,1E7
 MP,NUXY,,.25
 CSYS,1
 K,1,4.12                  ! DEFINE KEYPOINTS
 K,2,4.32
@@ -21,15 +22,14 @@
 ESIZE,,1
 VMESH,1                   ! CREATE NODES AND ELEMENTS
 NSEL,S,LOC,Y,0
 D,ALL,ALL,0               ! BOUNDARY CONDITIONS AND LOADING
 NSEL,ALL
 FK,5,FY,.25               ! APPLY LOAD
 *REPEAT,4,1
-NOORDER
 FINISH
 /SOLU    
 SOLVE
 FINISH
 *CREATE,MAC               ! CREATE A MACRO TO DO POSTPROCESSING
 /POST1
 CSYS,0
@@ -140,39 +140,39 @@
 /OUT,vm187,vrt
 /COM,------------------- VM187 RESULTS COMPARISON ------------
 /COM,
 /COM,                      TARGET   |    Mechanical APDL   |    RATIO
 /COM, SOLID5
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.6,'  ',F15.6,'   ',1F16.3)
+(1X,A8,A8,'   ',F11.4,'  ',F15.4,'   ',1F16.3)
 /NOPR
 RESUME,TABLE_2
 /GOPR
 /COM,
 /COM, SOLID92
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.6,'  ',F15.6,'   ',1F16.3)
+(1X,A8,A8,'   ',F11.4,'  ',F15.4,'   ',1F16.3)
 /NOPR
 RESUME,TABLE_3
 /GOPR
 /COM,
 /COM, SOLID98
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.6,'  ',F15.6,'   ',1F16.3)
+(1X,A8,A8,'   ',F11.4,'  ',F15.4,'   ',1F16.3)
 /NOPR
 RESUME,TABLE_4
 /GOPR
 /COM,
 /COM, SOLID187
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F11.6,'  ',F15.6,'   ',1F16.3)
+(1X,A8,A8,'   ',F11.4,'  ',F15.4,'   ',1F16.3)
 /COM,---------------------------------------------------------
 /OUT
 FINISH
 /DELETE,TABLE_1
 /DELETE,TABLE_2
 /DELETE,TABLE_3
 /DELETE,TABLE_4
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm189.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm189.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM189 
 /TITLE,VM189,STRESS RELAXATION OF A CHLOROPRENE RUBBER
 /COM,
 /COM, REFERENCE:
 /COM, HUSNU DAL, MICHAEL KALISKE, "BERGSTROM-BOYCE MODEL FOR
 /COM, NONLINEAR FINITE RUBBER VISCOELASTICITY: THEORITICAL
 /COM, ASPECTS AND ALGORITHMIC TREATMENT FOR THE FE METHOD  
@@ -138,10 +138,11 @@
 /COM,
 *VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,'  ',F11.3,'   ',1F14.3,'  ',1F14.3)
 /COM, ---------------------------------------------------------------
 /OUT,
 *LIST,vm189,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm19.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm19.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM19
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 /TITLE, VM19, RANDOM VIBRATION ANALYSIS OF A DEEP SIMPLY-SUPPORTED BEAM
 /COM REFERENCE:  NAFEMS FORCED VIBRATION BENCHMARKS TEST 5R
 ET,1,BEAM188                         ! DEFINE ELEMENT TYPE
@@ -26,15 +26,14 @@
 MODOPT,LANB,9
 D,1,UX,0,0,1,1,UY,UZ,ROTX          ! APPLY CONSTRAINTS
 D,11,UY,0,0,11,1,UZ
 /OUT,SCRATCH
 SOLVE
 *GET,FREQ,MODE,1,FREQ
 FINISH
-!/COPY,,tri,,mode,tri
 
 /SOLU
 ANTYPE,SPECTR                      ! PREFORM SPECTRUM PSD ANALYSIS
 SPOPT,PSD,9,ON                     ! CALC. STRESS RESPONSE FOR FIRST 9 MODES
 PSDUNIT,1,FORCE
 DMPRAT,0.02
 F,1,FY,-0.5E6                      ! SCALE LOADS
@@ -45,15 +44,14 @@
 PFACT,1,NODE
 PSDRES,DISP,REL
 PSDCOM 
 SOLVE
 FINISH
 
 /POST26
-/OUT,
 STORE,PSD,10
 NSOL,2,6,U,Y
 RPSD,8,2,2,0,2,,,1.0e-3
 PRTIME,42.630,42.631
 PRVAR,8
 *GET,P1,VARI,8,RTIME,42.63
 PM=P1*1000000
@@ -63,14 +61,15 @@
 STORE,PSD,10
 ESOL,3,5,6,SMISC,37  
 RPSD,9,3,3,0,2,,,1.0e-3
 PRTIME,42.630,42.631
 PRVAR,9
 *GET,P2,VARI,9,RTIME,42.63
 PM2=P2/(1E12)
+/OUT,
 *DIM,LABEL,CHAR,3,2
 *DIM,VALUE,,3,3
 LABEL(1,1) = 'FREQ1','PEAK d','PSD(N/mm'
 LABEL(1,2) = ' (Hz)',' mm^2/Hz','^2)^2/Hz'
 *VFILL,VALUE(1,1),DATA,42.65,180.9,58515.6
 *VFILL,VALUE(1,2),DATA,FREQ,PM,PM2
 *VFILL,VALUE(1,3),DATA,ABS(FREQ/42.65) ,ABS(PM/180.9 ),ABS(PM2/58515.6 )
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm190.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm190.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM190
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
+/out,scratch
+/COM, CREATING CDB FILE TO STORE MESH DATA
+/COM,
+_GEOMGEN = 0            ! SET TO 1 TO WRITE CDB FILE
+*IF,_GEOMGEN,EQ,1,THEN
 /PREP7
 smrt,off
 /TITLE, VM190, FERROMAGNETIC INDUCTOR
 /COM,   CHAPMAN, "ELECTRIC MACHINERY FUNDAMENTALS", MCGRAW-HILL,
 /COM,   1985, EXAMPLE 1-1, PG. 14
 ET,1,SOLID98,10               ! 10-NODE TETRAHEDRAL, MAG OPTION
 ET,2,INFIN47                  ! INFINITE ELEMENT
@@ -39,19 +44,27 @@
 MAT,2
 VMESH,4,6                     ! MESH IRON
 MAT,1
 VMESH,2                       ! MESH AIR
 NSEL,S,LOC,Z,0
 D,ALL,MAG,0                   ! SET FLUX-NORMAL SYMMETRY CONDITION
 NSEL,ALL
+ALLSEL
+cdwrite,db,vm190,cdb
+FINISH
+*ELSE
+/PREP7
+cdread,db,vm190,cdb
+*ENDIF
 FINISH
 /SOLU
 ANTYPE,STATIC                 ! STATIC MAGNETIC FIELD ANALYSIS
 MAGSOLV,4
 FINISH
+/out,scratch
 /POST1
 PATH,IRON,7,,48               ! DEFINE PATH WITH NAME = "IRON"
 PPATH,1,,-.2,0,0             ! DEFINE PATHS POINTS BY 
 PPATH,2,,-.2,0,.20
 PPATH,3,,-.2,0,.375
 PPATH,4,,.025,0,.375
 PPATH,5,,.225,0,.375
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm191.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm191.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM191 
 /TITLE, VM191, HERTZ CONTACT BETWEEN TWO CYLINDERS
-/stitle,1,Reason COMPARE differences are acceptable:
-/stitle,2,  Contact Element Number
 /COM    "FINITE ELEMENT ANALYSIS OF HERTZ CONTACT PROBLEM"
 /COM     N. CHANDRASEKARAN, W.E. HAISLER, R.E. GOFORTH,
 /COM     FINITE ELEMENTS IN ANALYSIS AND DESIGN 3, 1987, PP 39-56.
 /COM
 /COM  2-D ANALYSIS USING PLANE182 AND CONTA175
 /COM  CONTACT ALGORITHM: AUGMENTED LAGRANGIAN - KEYOPT(2) = 0
 /COM
+/OUT,SCRATCH
 /PREP7 
 SMRT,OFF 
 ANTYPE,STATIC
 ET,1,PLANE182          ! 2-D SOLID ELEMENTS
 ET,2,TARGE169          ! 2-D TARGET ELEMENTS
 ET,3,CONTA175          ! 2-D CONTACT ELEMENTS
 MP,EX,1,30000          ! SMALLER CYLINDER PROPERTIES
@@ -80,24 +79,22 @@
 NSEL,S,LOC,Y
 D,ALL,UY
 NSEL,ALL
 FINISH
 SAVE,MODEL2D
 
 *CREATE,SOLV2D,MAC     ! CREATE SOLUTION MACRO FOR 2-D CASE
-/out,scratch
 /SOLU
 D,NC,UY,-0.005         ! APPLY SMALL DISPLACEMENT TO ENGAGE CONTACT
 SOLVE                  ! SOLVE FIRST LOAD STEP
 DDELE,NC,UY            ! DELETE IMPOSED DISPLACEMENT
 F,NC,FY,-1600          ! APPLY HALF LOAD ON (SYMMETRY) MODEL
-nsub,2,10,1
+NSUB,2,10,1
 SOLVE                  ! SOLVE SECOND LOAD STEP
 FINISH
-/out
 *END
 
 SOLV2D                 ! EXECUTE SOLUTION MACRO FOR 2-D CASE
 
 *CREATE,RES2D,MAC      ! CREATE RESULTS MACRO FOR 2-D CASE
 /POST1
 NSEL,,LOC,Y,23         ! SELECT TOP EDGE OF SMALLER CYLINDER
@@ -212,24 +209,22 @@
 NSEL,S,LOC,Z
 D,ALL,UZ
 NSEL,ALL
 FINISH
 SAVE,MODEL3D
 
 *CREATE,SOLV3D,MAC     ! CREATE SOLUTION MACRO FOR 3-D CASE
-/out,scratch
 /SOLU
 D,NC,UY,-0.001         ! APPLY SMALL DISPLACEMENT TO ENGAGE CONTACT
 SOLVE                  ! SOLVE FIRST LOAD STEP
 DDELE,NC,UY            ! DELETE IMPOSED DISPLACEMENT
 F,NC,FY,-1600          ! APPLY HALF LOAD ON (SYMMETRY) MODEL
-nsub,2,10,1
+NSUB,2,10,1
 SOLVE                  ! SOLVE SECOND LOAD STEP
 FINISH
-/out
 *END
 
 SOLV3D                 ! EXECUTE SOLUTION MACRO FOR 3-D CASE 
 
 *CREATE,RES3D,MAC      ! CREATE RESULTS MACRO FOR 3D CASE
 /POST1
 NSEL,,LOC,Y,23         ! SELECT TOP EDGE OF SMALLER CYLINDER
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm192.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm192.dat`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM192
 /PREP7
 SMRT,OFF
 /TITLE, VM192, COOLING OF A BILLET BY RADIATION
 /COM    THERMAL RADIATION HEAT TRANSFER, SIEGEL AND HOWELL, 2ND EDITION,
 /COM    PG. 229, PROBLEM NO. 21.
 ET,1,SOLID70            ! 3-D THERMAL SOLID ELEMENT
@@ -20,24 +20,25 @@
 REAL,2
 MAT,2
 N,100,5,5,5             ! EXTRA "SPACE" NODE FOR RADIATION
 ESURF,100               ! GENERATE SURF152 ELEMENTS
 FINISH
 
 /SOLU
-SOLCONTROL,0
 ANTYPE,TRANS            ! TRANSIENT ANALYSIS
 D,100,TEMP,530          ! SPECIFY SURROUNDING ABSOLUTE TEMPERATURE
 TUNIF,2000              ! INITIAL BILLET ABSOLUTE TEMPERATURE
 AUTOTS,ON               
 KBC,1                   ! STEP SURROUNDING TEMPERATURE IN FIRST TIME STEP
-DELTIM,0.005            ! INITIAL (MINIMUM) INTEGRATION TIME STEP
+DELTIM,0.005,0.005,0.005! INITIAL (MINIMUM) INTEGRATION TIME STEP
 OUTRES,,ALL
 OUTPR,NSOL,LAST
 TIME,3.7                ! TRANSIENT TIME SPAN
+CNVTOL,HEAT,,,,1.0
+TINTP,,,,0.5,,0.2
 /OUT,SCRATCH
 SOLVE
 FINISH
 
 /POST26
 /OUT,
 NSOL,2,1,TEMP,,TEMP
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm193.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm92.dat`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM193
-JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
-/SHOW,JPEG
-/NOPR
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM92
 /PREP7
-SMRT,OFF
-/TITLE, VM193, TWO DIMENSIONAL HEAT TRANSFER WITH CONVECTION
-C***    "THE STANDARD NAFEMS BENCHMARKS", TEST NO. T4,
-C***    NAFEMS, REV 3, OCTOBER 1990.
-ANTYPE,STATIC                       
-ET,1,PLANE55
-MP,KXX,1,52.0                
-K,1                          
-K,2,.6                                                                          
-K,3,.6,1.0                                                                      
-K,4,,1.0
-K,5,.6,.2
-L,1,2
-L,2,5
-L,5,3
-L,3,4
-L,4,1
-AL,ALL
-DK,1,TEMP,100,,1
-DK,2,TEMP,100,,1
-SFL,2,CONV,750.0,,0.0
-SFL,3,CONV,750.0,,0.0
-SFL,4,CONV,750.0,,0.0
+/TITLE, VM92, INSULATED WALL TEMPERATURE
+C***        PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 32, EX. 2-5
+ANTYPE,STATIC                ! THERMAL ANALYSIS
+ET,1,LINK34
+ET,2,LINK33
+R,1,1                        ! AREA = 1
+MP,KXX,1,.8
+MP,HF,1,12
+MP,KXX,2,.1
+MP,HF,2,2
+N,1
+N,2
+N,3,.75
+N,4,(14/12)                  ! 14 INCHES TO FEET
+N,5,(14/12)
+E,1,2
+TYPE,2
+E,2,3
+MAT,2
+E,3,4
+TYPE,1
+E,4,5
+D,1,TEMP,3000
+D,5,TEMP,80
+FINISH
+/SOLU    
+SOLVE
 FINISH
-ADAPT,10,,5,0.2,1            ! FINAL PERCENT ERROR NEAR 5% WITHIN 10 LOOPS
 /POST1
-PLNSOL,TEMP                  ! DISPLAY TEMP CONTOURS IN FINAL MESH
-*GET,TEPC,PRERR,,TEPC        
-KSEL,,,,5
-NSLK
-*GET,N1,NODE,,NUM,MAX
-*GET,TEMP1,NODE,N1,TEMP
-*status,parm
-*DIM,VALUE,,1,3
-*DIM,LABEL,CHAR,1,2
-LABEL(1,1) = 'TEMP '
-LABEL(1,2) = 'DEG C'
-*VFILL,VALUE(1,1),DATA,18.3
-*VFILL,VALUE(1,2),DATA,TEMP1
-*VFILL,VALUE(1,3),DATA,ABS(TEMP1/18.3)
+PRNSOL,TEMP                  ! PRINT NODAL TEMPERATURES
+PRNLD,HEAT                   ! PRINT HEAT FLOW RATES
+*GET,TI,NODE,2,TEMP
+*GET,TO,NODE,4,TEMP
+FINISH
+/POST26
+ESOL,2,4,5,HEAT,,HEAT
+STORE
+*GET,HEAT,VARI,2,EXTREM,VMAX
+*DIM,LABEL,CHAR,3,2
+*DIM,VALUE,,3,3
+LABEL(1,1) = 'Q, BTU/h','TI,     ','TO,     '
+LABEL(1,2) = 'r       ','F       ','F       '
+*VFILL,VALUE(1,1),DATA,513,2957,336
+*VFILL,VALUE(1,2),DATA,HEAT,TI,TO
+*VFILL,VALUE(1,3),DATA,ABS(HEAT/513) ,ABS(TI/2957),ABS(TO/336)
 /COM
-/OUT,vm193,vrt
-/COM,------------------- VM193 RESULTS COMPARISON --------------
-/COM,
-/COM,  LOAD STP 4      |   TARGET   |   Mechanical APDL   |   RATIO
+/OUT,vm92,vrt
+/COM,------------------- VM92 RESULTS COMPARISON --------------
 /COM,
+/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F15.1,'   ',1F18.3)
-/COM,-----------------------------------------------------------
+(1X,A8,A8,'   ',F10.0,'  ',F14.0,'   ',1F15.3)
+/COM,----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm193,vrt
+*LIST,vm92,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm194.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm194.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM194
 /PREP7  
 /TITLE, VM194, ELEMENT BIRTH/DEATH IN A FIXED BAR WITH THERMAL LOADING
 /COM    ANY STANDARD MECHANICS OF MATERIALS TEXT
 ET,1,LINK180        ! 3-D SPAR ELEMENTS
 MP,EX,1,30E6        ! BAR MATERIAL PROPERTIES
 MP,ALPX,1,.00005
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm195.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm195.dat`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM195
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM195, TOGGLE MECHANISM
 C*** KINEMATICS AND DYNAMICS OF MACHINES, MARTIN, 2ND ED., P 56, FIG 3-22 
 ET,1,MPC184,6,,,1
 ET,2,BEAM188,,,3
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm196.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm53.dat`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,75 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM196
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM53
 /PREP7
-MP,PRXY,,0.3
-SMRT,OFF
-/TITLE, VM196, COUNTER-BALANCED LOADS ON A BLOCK
-C***   ANY BASIC MECHANICS BOOK
-C***   USING 3-D SOLID45 
-ET,1,SOLID45       
-MP,EX,1,70E9          ! ALUMINUM 
-MP,DENS,1,2712
-MP,PRXY,1,0.3
-WPOFFS,,,300          ! AXIS OF ROTATION 300 M
-BLOCK,-1,1,-1,1,0,3   ! 3 M HIGH BY 2 M SQUARE
-ESIZE,1
-VMESH,ALL
-DK,1,ALL              ! CONSTRAIN 6 DOF SUCH THAT NO ROTATIONS OCCUR
-DK,4,UX
-DK,6,UY
-DK,7,UZ
-SAVE                  ! SAVE DATABASE FOR SECOND SOLUTION
+/TITLE, VM53, VIBRATION OF A STRING UNDER TENSION
+C***           VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND. PRINTING,
+C***           PAGE 264, ART. 8.2,  
+ANTYPE,STATIC              ! STATIC ANALYSIS
+ET,1,LINK180
+KEYOPT,1,3,1		   	   ! TENSION ONLY OPTION
+SECTYPE,1,LINK   
+SECDATA,306796E-8	         ! DEFINE AREA
+MP,EX,1,30E6
+MP,DENS,1,73E-5
+N,1                        ! DEFINE NODES
+N,14,100
+FILL
+E,1,2                      ! DEFINE ELEMENTS
+EGEN,13,1,1
+INIS,SET,CSYS,-2           ! ARBITRARY INITIAL STRAIN
+INIS,SET,DTYP,EPEL
+INIS,DEFINE,,,,,543248E-8
+OUTPR,BASIC,1
+D,ALL,ALL                  ! FIX ALL MOTIONS FOR STATIC STRESSES
 FINISH
-*CREATE,SOLV3D,MAC    ! CREATE MACRO TO SOLVE AND RETRIEVE RESULTS
-/SOLU
-ANTYPE,STATIC
-IRLF,1                ! INERTIA RELIEF CALCULATIONS
-FK,5,FX,-2000
-FK,5,FY,3000
-OUTPR,RSOL,1          ! PRINT REACTION SOLUTION
+/out,scratch
+/SOLU    
+RESCONTROL,LINEAR,ALL,1     ! NEEDED FOR PERTURBED ANALYSIS
 SOLVE
-IRLIST                ! LIST INERTIA RELIEF LOADS AND ACCELERATIONS
-*GET,MX,ELEM,,MMOR,X
-*GET,MY,ELEM,,MMOR,Y
-*GET,MZ,ELEM,,MMOR,Z
-*DIM,LABEL,CHAR,3,2
-*DIM,VALUE,,3,3
-LABEL(1,1) = 'MOM X ','MOM Y','MOM Z'
-LABEL(1,2) = 'N-m','N-m','N-m'
-*VFILL,VALUE(1,1),DATA,-909000,-606000,-5000
-*VFILL,VALUE(1,2),DATA,MX,MY,MZ
-*VFILL,VALUE(1,3),DATA,ABS(MX/909000),ABS(MY/606000),ABS(MZ/5000)
 FINISH
-*END
-
-SOLV3D                ! EXECUTE MACRO TO SOLVE AND RETRIEVE RESULTS
-SAVE,TABLE_1
-
-/CLEAR, NOSTART       ! CLEAR DATABASE FOR 2ND SOLUTION
-/TITLE, VM196, COUNTER-BALANCED LOADS ON A BLOCK
-C***   USING 3-D SOLID185 
-/PREP7
-SMRT,OFF
-RESUME                ! RESUME DATABASE
-ET,1,SOLID185         ! ANALYZE AGAIN USING 3-D SOLID185 
+/out
+/POST1
+ETABLE,STRS,LS,1
+*GET,STRSS,ELEM,13,ETAB,STRS
 FINISH
+/POST26
+RFORCE,2,1,F,X
+STORE
+*GET,FORCE,VARI,2,EXTREM,VMAX
+PARSAV,ALL
+/out,scratch
+/SOLU    
+ANTYPE,STATIC,RESTART,,,PERTURB   ! RESTART FROM LAST LOAD STEP AND LAST SUB STEP
+PERTURB,MODAL,,,PARKEEP           ! PERFORM PERTURBED MODAL SOLVE
+SOLVE,ELFORM                      ! REFORM ELEMENT MATRICES
 
-SOLV3D                ! EXECUTE MACRO TO SOLVE AND RETRIEVE RESULTS
-SAVE,TABLE_2
-/NOPR
-RESUME,TABLE_1
-/GOPR
+PARRES,CHANGE
+MODOPT,LANB,3              ! EXTRACT 3 MODES USING LANB EXTRACTION METHOD
+MXPAND,3                   ! EXPAND FIRST THREE MODES
+DDELE,2,UX,13              ! RELEASE INTERIOR DOFS
+DDELE,2,UY,13
+SOLVE
+/out
+*GET,FREQ1,MODE,1,FREQ
+*GET,FREQ2,MODE,2,FREQ
+*GET,FREQ3,MODE,3,FREQ
+*DIM,LABEL,CHAR,5,2
+*DIM,VALUE,,5,3
+LABEL(1,1) = '      F,','      SI','      f1','      f2','      f3'
+LABEL(1,2) = ' lb     ','GMA,psi ',', Hz    ',', Hz    ',', Hz    '
+*VFILL,VALUE(1,1),DATA,500,162974,74.708,149.42,224.12
+*VFILL,VALUE(1,2),DATA,ABS(FORCE),STRSS,FREQ1,FREQ2,FREQ3
+*VFILL,VALUE(1,3),DATA,ABS(FORCE/500),ABS(STRSS/162974),ABS(FREQ1/74.708)
+*VFILL,VALUE(4,3),DATA,ABS(FREQ2/149.42),ABS(FREQ3/224.12)
 /COM
-/OUT,vm196,vrt
-/COM,------------------- VM196 RESULTS COMPARISON --------------
+/OUT,vm53,vrt
+/COM,------------------- VM53 RESULTS COMPARISON ---------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-/COM, SOLID45
-/COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.0,'  ',F15.0,'   ',1F15.3)
-/NOPR
-RESUME,TABLE_2
-/GOPR
-/COM,
-/COM, SOLID185
-/COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.0,'  ',F15.0,'   ',1F15.3)
-/COM,-----------------------------------------------------------
-/COM,
-/COM,-----------------------------------------------------------
-/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM196  NOT CONTAINED IN
-/COM,THIS TABLE
+(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
 /COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm196,vrt
+*LIST,vm53,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm198.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm201.dat`

 * *Files 26% similar despite different names*

```diff
@@ -1,252 +1,223 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM198
-JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM201
+JPGPRF,500,100,1               ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-EL='PLANE182'
-*DIM,A,CHAR,2              ! DEFINE AND DIMENSION THE CHARACTER PARAMETER A 
-A(1)='UX','UY'             ! SET CHARACTER STRINGS AS VALUES OF CHARACTER 
-!                             PARAMETER A 
+R = 200                        ! RADIUS OF CYLINDER (mm)
 /PREP7
-/TITLE, VM198, LARGE STRAIN IN-PLANE TORSION TEST (%EL%)
-!       "SOME COMPUTATIONAL ASPECTS ....",NAGTEGAAL ET AL.
-ET,1,PLANE182,,,2		   ! 2-D 4 NODE PLANE ELEMENT
-MP,EX,1,7200
-MP,NUXY,1,0.33
-TB,BISO,1                  ! BILINEAR ISOTROPIC HARDENING
-TBDATA,1,10                ! YIELD STRESS
-TBDATA,2,40                ! TANGENT MODULUS
-SAVE                       ! SAVE DATABASE FOR LATER USE
-CSYS,1
-N,1,10
-N,11,20
-FILL
-NGEN,2,100,1,11,1,,3
-E,1,2,102,101
-EGEN,10,1,1,1
-!         APPLY BOUNDARY CONDITIONS
-NSEL,S,LOC,X,20
-D,ALL,ALL                  ! CLAMP OUTER SURFACE
+smrt,off
+/TITLE, VM201, RUBBER CYLINDER PRESSED BETWEEN TWO PLATES
+/COM    REF: T. SUSSMAN, K.J. BATHE, "A FE FORMULATION FOR NONLINEAR ..."
+/COM         COMPUTERS & STRUCTURES, VOL. 26, NOS. 1/2, 1987
+ET,1,PLANE182, , ,2            ! 2-D PLANE-STRAIN 4-NODE STRUCTURAL SOLID
+KEYOPT,1,6,1
+ET,2,CONTA175                  ! 2-D 1-NODE NODE-TO-SURFACE CONTACT ELEMENT
+R,2, , ,-2000                  ! SET SURFACE STIFFNESS
+ET,3,TARGE169                  ! 2-D TARGET ELEMENT
+C10 = 0.293
+C01 = 0.177
+NU1 = 0.49967
+DD  = (1-2*NU1)/(C10+C01)
+TB,HYPER,1,1,2,MOONEY
+TBDATA,1,C10,C01,DD
+CSYS,1                         ! SWITCH TO CYLINDRICAL C.S.
+K,1                            ! DEFINE KEYPOINTS
+K,2,R,-90
+K,3,R
+K,4,(0.5*R),-90
+K,5,(0.6*R),-45
+K,6,(0.5*R)
+K,7,R,-45
+L,2,7
+L,7,3
+CSYS,0                         ! SWITCH TO CARTESIAN C.S.
+A,2,7,5,4
+A,7,3,6,5
+A,4,5,6,1
+ESIZE,,4                       ! SET ELEMENT DIVISION SIZE
+AMESH,ALL                      ! MESH ALL AREAS
+SAVE                           ! SAVE MODEL FOR MORE ANALYSIS
+N,1001,(-2*R),-R               ! TARGET SURFACE NODES
+N,1002,(2*R) ,-R
+NSEL,S,NODE,,1001,1002
+TYPE,3
+REAL,2
+TSHAP,LINE                     ! SET TARGET SHAPE TO LINE
+E,1002,1001                    ! GENERATE RIGID TARGET
+D,ALL,ALL,0                    ! FIX TARGET
+NSEL,S,LOC,X                   ! SELECT LEFT EDGE
+D,ALL,UX                       ! CONSTRAIN LEFT EDGE IN UX
+NSEL,S,LOC,Y                   ! SELECT TOP EDGE
+CP,1,UY,ALL                    ! COUPLE TOP EDGE IN UY
+*GET,NCEN,NODE,,NUM,MIN        ! GET MINIMUM NODE NUMBER FROM SELECTED SET
 NSEL,ALL
-!         ROTATE APPROPRIATE NODES AND APPLY COUPLING
-LOCAL,11,0,,,,3          
-NROTAT,101,111
+CSYS,1                         ! SWITCH TO CYLINDRICAL C.S.
+ESEL,S,TYPE,,1
+NSLE
+NSEL,R,LOC,X,R
+TYPE,2
+REAL,2
+ESURF                          ! DEFINE CONTACT ELEMENTS
+ALLSEL,ALL
 CSYS,0
-CP,1,A(1),2,102            ! USE A(1) VALUE FOR DOF LABEL
-CP,2,A(2),2,102            ! USE A(2) VALUE FOR DOF LABEL
-CPSGEN,9,1,1,2,1
+SAVE,CONT2D                    ! SAVE 2D CONTACT MODEL FOR SECOND ANALYSIS
 FINISH
-/OUTPUT,SCRATCH            ! DIVERT VOLUMINOUS SOLUTION OUTPUT
-/SOLU
-!     CREATE SOLUTION OPTIONS AND LOADING MACRO FOR MULTIPLE USE
-*CREATE,SOLD,MAC
-   SOLCONTROL,0
-   ANTYPE,STATIC
-   NLGEOM,ON                  ! LARGE STRAIN OPTION ACTIVATED
-   NEQIT,100                  ! 100 EQUILIBRIUM ITERATIONS ALLOWED
-  CUTC,PLSLIMIT,0.5          ! RESET MAXIMUM PLASTIC INCREMENTAL STRAIN 
-  NSUBS,100,1000,10
-  D,ARG1,ARG2,,,ARG3,ARG4,ARG5
-   SOLVE
-   OUTRES,ESOL,1              ! STORE RESULTS FOR EVERY SUBSTEP
-   NSTP = 10                  ! NO. OF LOAD STEPS USED
-   T1   = 60/NSTP             ! ROTATION PER LOAD STEP
-   T2   = 3.1415927/180       ! PARAMETER FOR FURTHER CALCULATIONS
-   T33  = T1*T2               ! DEGREES TO RADIANS CONVERSION
-   *DO,I,1,NSTP               ! USE DO LOOP FOR LOADING
-       T3   = (I*T33)         ! CURRENT ANGLE
-       T4   = (10*SIN(T3))    ! UY DISPLACEMENT
-       T5   = (10*COS(T3))    
-       T5   = (T5-10)         ! UX DISPLACEMENT
-       D,ARG1,ARG2,T5,,ARG3,ARG4
-       D,ARG1,ARG5,T4,,ARG3,ARG4
-       SOLVE
-   *ENDDO
+
+*CREATE,SOLVIT,MAC             ! MACRO TO SOLVE MODEL
+ /SOLU
+ ANTYPE,STATIC
+ CNVTOL,F,,,,-1
+ NLGEOM,ON                     ! INCLUDE LARGE DEFORMATION EFFECTS
+ NSUBST,6                      ! SPECIFY NUMBER OF SUBSTEPS IN LOAD STEP
+ OUTRES,,1                     ! WRITE SOLUTION FOR EVERY SUBSTEP
+ D,NCEN,UY,-100                ! APPLY DISPLACEMENT UY = -100 TO COUPLED NODES
+ SOLVE
+ FINISH
 *END
-SOLD,1,A(1),101,100,A(2)      ! USE A(1) AND A(2) AS ARG2 AND ARG5 VALUES FOR 
-FINISH                        !  DOF LABELS  
-/OUTPUT
-!         CREATE POST PROCESSING MACRO FOR MULTIPLE USE
-*CREATE,POSP,MAC
-   !COM      PLOT THE FINAL DISPLACED GEOMETRY USING POST1
-   /POST1
-   SET,NSTP+1
-   /DSCALE,1,1
-   /DIST,1,13
-   PLDISP,1
-   /DIST,1
-   FINISH
-   !         OBTAIN MAXIMUM SHEAR STRESS USING POST26
-   /POST26
-   ESOL,2,1,1,S,1
-   ESOL,3,1,1,S,3
-   FILLDATA,5,1,,,0,6
-   ADD,4,2,3,,SHEAR,,,-1/2,1/2         ! COMPUTE MAX. SHEAR USING
-                                       !  PRINCIPAL STRESSES
-   PRVAR,4,5
-   /GRID,1
-   /XRANGE,0,60
-   /YRANGE,-60,0
-   /AXLAB,X,ROTATION (DEGREES)
-   /AXLAB,Y,SHEAR STRESS (PSI)
-   XVAR,5
-   PLVAR,4
-   *GET,P1,VARI,4,RTIME,11
-   *DIM,LABEL,CHAR,1,2
-   *DIM,VALUE,,1,3
-   LABEL(1,1) = 'PRS MAX '
-   LABEL(1,2) = 'psi'
-   *VFILL,VALUE(1,1),DATA,-48
-   *VFILL,VALUE(1,2),DATA,P1
-   *VFILL,VALUE(1,3),DATA,ABS(P1/48)
-   FINISH
+SOLVIT                         ! USE MACRO SOLVIT
+
+*CREATE,PLOTS,MAC              ! MACRO FOR POST-PROCESSING
+ /POST1
+ /DSCALE,1,1
+ PLDISP,1                      ! PLOT DISPLACED SHAPE
+ FINISH
+ /POST26
+ /AXLAB,Y,FORCE
+ /AXLAB,X,DISPLACEMENT
+ NSOL,2,NCEN,U,Y
+ RFORCE,3,NCEN,F,Y
+ PROD,2,2,,,,,,-2
+ PROD,3,3,,,,,,-2
+ XVAR,2
+ PLVAR,3                       ! PLOT DISPLACEMENT VS FORCE
+ PRVAR,2,3                     ! PRINT DISPLACEMENT, FORCE
+ *GET,F1,VARI,3,RTIME,.5
+ *GET,F2,VARI,3,RTIME,1
+ *DIM,LABEL,CHAR,2,2
+ *DIM,VALUE,,2,3
+ LABEL(1,1) = 'F (N) @ ','F (N) @ '
+ LABEL(1,2) = '.1','.2'
+ *VFILL,VALUE(1,1),DATA,250,1400
+ *VFILL,VALUE(1,2),DATA,F1,F2
+ *VFILL,VALUE(1,3),DATA,ABS(F1/250),ABS(F2/1400)
+ FINISH
 *END
-POSP
+PLOTS                          ! USE MACRO PLOTS
 SAVE,TABLE_1
-/CLEAR, NOSTART 
 
-!         ANALYZE THE SAME PROBLEM WITH ELEMENT SOLID185
-/PREP7
 RESUME
-EL='SOLID185'
-/OUT,SCRATCH
-/STATUS,TITLE              ! DISPLAY TITLE WITH NEW VALUE OF PARAMETER EL     
-/OUT,
-ET,1,SOLID185	           ! 3D 8 NODE SOLID ELEMENT
-CSYS,1
-N,1,10
-N,11,20
-FILL
-NGEN,2,100,1,11,1,,3
-NGEN,2,200,1,111,1,,,1
-E,1,2,102,101,201,202,302,301
-EGEN,10,1,1,1
-!          APPLY BOUNDARY CONDITIONS
-D,ALL,UZ
-NSEL,S,LOC,X,20
-D,ALL,ALL                  ! CLAMP OUTER SURFACE
+/PREP7
+SMRT,OFF
+ET,5,SOLID185                  ! 3-D 8-NODE STRUCTURAL SOLID
+KEYOPT,5,6,1
+ET,6,CONTA175                  ! 3-D 1-NODE NODE-TO-SURFACE CONTACT ELEMENT
+R,6, , ,-2000,-0.1,
+ET,7,TARGE170                  ! 3-D TARGET ELEMENT
+ET,8,MESH200,6                 ! 2-D 4-NODED QUAD
+R,8,0.05
+ALLSEL
+TYPE,5
+ESIZE,,1
+VEXT,ALL,,,,,1
+N,1001,,-R                     ! CREATE TARGET PLANE OF NODES
+N,1002,2*R,-R
+N,1003,2*R,-R,8*R
+N,1004,,-R,8*R
+TYPE,8
+REAL,8
+E,1002,1001,1004,1003
+NSEL,S,NODE,,1001,1004
+TYPE,7
+REAL,6
+ESURF                          ! GENERATE TARGET ELEMENTS
+D,ALL,ALL,0
+CSYS,1                         ! SWITCH TO CYLINDRICAL C.S.
+ESEL,S,TYPE,,5
+NSLE
+NSEL,R,LOC,X,R
+ESEL,S,TYPE,,5,7
+TYPE,6
+REAL,6
+ESURF
+CSYS,0                         ! SWITCH TO CARTESIAN C.S.
 NSEL,ALL
-!          ROTATE APPROPRIATE NODES AND APPLY COUPLING
-LOCAL,11,0,,,,3
-NROTAT,101,111
-NROTAT,301,311
-CSYS,0
-CP,1,A(1),2,102,202,302
-CP,2,A(2),2,102,202,302
-CPSGEN,9,1,1,2,1
+D,ALL,UZ                       ! CONSTRAIN ALL NODES IN Z (PLANE STRAIN)
+NSEL,S,LOC,X
+D,ALL,UX
+NSEL,S,LOC,Y
+CP,1,UY,ALL                    ! COUPLE TOP NODES IN Y
+*GET,NCEN,NODE,,NUM,MIN
+ESEL,S,TYPE,,5,7
+NSLE
+SAVE,CONT3D                    ! SAVE 3D CONTACT MODEL FOR SECOND ANALYSIS
 FINISH
-/OUTPUT,SCRATCH            ! DIVERT VOLUMINOUS SOLUTION OUTPUT
-/SOLU
-SOLD,1,A(1),301,100,A(2)
-FINISH
-/OUTPUT
-POSP                       ! POSTPROCESS RESULTS USING POSP MACRO
+/OUT,SCRATCH
+SOLVIT                         ! USE MACRO TO OBTAIN SOLUTION
+PLOTS                          ! USE MACRO TO POSTPROCESS
 SAVE,TABLE_2
 
-!         ANALYZE THE SAME PROBLEM WITH ELEMENT PLANE183 
+RESUME,CONT2D                  ! RESUME CONT175 -2D MODEL
+/OUT,
 /PREP7
-RESUME
-EL='PLANE183'
+R,2                            ! CONTACT STIFFNESS IS NOT REQUIRED
+KEYOPT,2,2,3                   ! LAGRANGE MULTIPLIER ON CONTACT NORMAL AND PENALTY ON TANGENT
+FINISH
 /OUT,SCRATCH
-/STATUS,TITLE              ! DISPLAY TITLE WITH NEW VALUE OF PARAMETER EL     
+SOLVIT                         ! USE MACRO TO OBTAIN SOLUTION
+PLOTS                          ! USE MACRO TO POSTPROCESS
+SAVE,TABLE_3
+
+/clear,nostart
+RESUME,CONT3D                  ! RESUME CONT175 -3D MODEL
 /OUT,
-et,1,PLANE183,,,2
-N,1,10
-N,21,20
-FILL
-CSYS,1
-NGEN,3,30,1,21,1,,1.5
-E,1,3,63,61,2,33,62,31
-EGEN,10,2,1,1,1
-NSLE 
-NSEL,INVE
-NDELE,ALL
-!         APPLY BOUNDARY CONDITIONS
-NSEL,S,LOC,X,20
-D,ALL,ALL
-!         ROTATE APPROPRIATE NODES AND APPLY COUPLING
-NSEL,S,NODE,,61,81
-LOCAL,11,0,,,,3
-NROTAT,ALL
-NSEL,S,NODE,,31,51,2
-LOCAL,12,0,,,,1.5
-NROTAT,ALL
-NSEL,ALL
-CSYS,0
-CP,1,A(1),3,33,63
-CP,2,A(2),3,33,63
-CPSGEN,9,2,1,2,1
-CP,21,A(1),2,62
-CP,22,A(2),2,62
-CPSGEN,10,2,21,22,1
+/PREP7
+R,6                            ! CONTACT STIFFNESS IS NOT REQUIRED
+KEYOPT,6,2,4                   ! PURE LAGRANGE MULTIPLIER ON CONTACT NORMAL AND TANGENT
 FINISH
-
 /OUT,SCRATCH
-/SOLU
-!     CREATE SOLUTION OPTIONS AND LOADING MACRO FOR MULTIPLE USE
-*CREATE,SOLD1,MAC
-   SOLCONTROL,0
-   ANTYPE,STATIC
-   NLGEOM,ON                  ! LARGE STRAIN OPTION ACTIVATED
-   NEQIT,100                  ! 100 EQUILIBRIUM ITERATIONS ALLOWED
-   CUTC,PLSLIMIT,0.5          ! RESET MAXIMUM PLASTIC INCREMENTAL STRAIN 
-   NSUBS,500,10000,100
-   cnvtol,f,1,1.0e-3
-   D,ARG1,ARG2,,,ARG3,ARG4,ARG5
-   SOLVE
-   OUTRES,ESOL,1              ! STORE RESULTS FOR EVERY SUBSTEP
-   NSTP = 10                  ! NO. OF LOAD STEPS USED
-   T1   = 60/NSTP             ! ROTATION PER LOAD STEP
-   T2   = 3.1415927/180       ! PARAMETER FOR FURTHER CALCULATIONS
-   T33  = T1*T2               ! DEGREES TO RADIANS CONVERSION
-   *DO,I,1,NSTP               ! USE DO LOOP FOR LOADING
-       T3   = (I*T33)         ! CURRENT ANGLE
-       T4   = (10*SIN(T3))    ! UY DISPLACEMENT
-       T5   = (10*COS(T3))    
-       T5   = (T5-10)         ! UX DISPLACEMENT
-       D,ARG1,ARG2,T5,,ARG3,ARG4
-       D,ARG1,ARG5,T4,,ARG3,ARG4
-       SOLVE
-   *ENDDO
-*END
-SOLD1,1,A(1),61,30,A(2)      ! USE A(1) AND A(2) AS ARG2 AND ARG5 VALUES FOR 
-FINISH  
+SOLVIT                         ! USE MACRO TO OBTAIN SOLUTION
+PLOTS                          ! USE MACRO TO POSTPROCESS
+SAVE,TABLE_4
 
-/OUTPUT
-POSP                       ! POSTPROCESS RESULTS USING POSP MACRO
-SAVE,TABLE_3
 RESUME,TABLE_1
+/OUT,
 /COM
-/OUT,vm198,vrt
-/COM,------------------- VM198 RESULTS COMPARISON --------------
+/OUT,vm201,vrt
+/COM,------------------- VM201 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-/COM,RESULTS USING PLANE182
+/COM,RESULTS USING PLANE182 AND 2D-CONTA175:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F15.1,'   ',1F15.3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_2
 /GOPR
 /COM,
-/COM,RESULTS USING SOLID185
+/COM,RESULTS USING SOLID185 AND 3D-CONTA175:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F15.1,'   ',1F15.3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_3
 /GOPR
 /COM,
-/COM,RESULTS USING PLANE183
+/COM,RESULTS USING PLANE182 AND 2D-CONTA175 WITH K(2)=3:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F15.1,'   ',1F15.3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
+/NOPR
+RESUME,TABLE_4
+/GOPR
+/COM,
+/COM,RESULTS USING SOLID185 AND 3D-CONTA175 WITH K(2)=4:
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /COM,-----------------------------------------------------------
+/COM,
 /OUT
 FINISH
-/NOPR
-/DELETE,POSP,MAC
-/DELETE,SOLD,MAC
-/DELETE,SOLD1,MAC
+*LIST,vm201,vrt
+/DELETE,PLOTS,MAC
+/DELETE,SOLVIT,MAC
 /DELETE,TABLE_1
 /DELETE,TABLE_2
 /DELETE,TABLE_3
-FINISH
-*LIST,vm198,vrt
+/DELETE,TABLE_4
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm199.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm36.dat`

 * *Files 25% similar despite different names*

```diff
@@ -1,192 +1,163 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM199
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM36
 /PREP7
-/TITLE, VM199, VISCOPLASTIC ANALYSIS OF A BODY UNDERGOING SHEAR DEFORMATION
-!              " AN IMPLICIT STRESS UPDATE ....", LWO ET AL.
-!           PLANE182 ELEMENT
-ET,1,182	  	                ! 2-D, 4-NODE ELEMENT
-KEYOPT,1,3,2					! PLANE STRAIN
-MP,EX,1,60.6E9
-MP,NUXY,1,0.4999
-TB,RATE,1,,9,ANAND              ! VISCOPLASTIC MODEL BY ANAND
-TBDATA,1,29.7E6
-TBDATA,2,21.08999E3
-TBDATA,3,1.91E7
-TBDATA,4,7.0
-TBDATA,5,0.23348
-TBDATA,6,1115.6E6
-TBDATA,7,18.92E6
-TBDATA,8,0.07049
-TBDATA,9,1.3
-SAVE                            ! SAVE DATABASE FOR LATER USE
-N,1
-N,2,1E-2
-N,3,1E-2,1E-2
-N,4,,1E-2
-E,1,2,3,4
-D,1,ALL,,,2
+/TITLE, VM36, LIMIT MOMENT ANALYSIS
+!           MECHANICS OF SOLIDS, CRANDALL AND DAHL, 1959, PAGE 389, EX. 8.9
+ANTYPE,STATIC
+ET,1,BEAM188,,,3
+ET,2,COMBIN40,,,5,             ! ROTY D.O.F. SPRING
+SECT,1,BEAM,RECT
+SECD,3.93597,3.93597
+R,2,1E12,,,,27777.8           ! DEFINE REAL CONSTANTS FOR COMBIN ELEMENTS
+R,3,1,,,,1E6
+MP,EX,1,30E6                  ! DEFINE MATERIAL PROPERTIES
+MP,NUXY,1,.3
+N,1                           ! BEGIN NODES DEFINITION
+N,2,100
+N,3,100
+N,4,150
+N,5,150
+E,1,2                         ! DEFINE BEAM ELEMENTS
+E,3,4
+TYPE,2                        ! DEFINE BREAKAWAY HINGE ELEMENTS
+REAL,2  
+E,2,3  
+E,4,5
+REAL,3  
+E,2,3  
+E,4,5                         ! EXTRA ELEMENTS FOR SOLUTION STABILITY
+OUTPR,ALL,ALL                 
+CNVTOL,M,27778,.001
+CP,1,UX,2,3                   ! COUPLE TRANSLATIONS ACROSS PLASTIC HINGE
+CPLGEN,1,UZ                   ! GENERATE 2ND SET IN DIRECTION UZ W/ SAME NODES
+CPSGEN,2,2,1,2,1              ! GENERATE TWO ADDITIONAL SETS W/ DIFFERENT NODES
+DSYM,SYMM,Y                   ! CONSTRAIN MODEL SYMMETRICALLY IN Y DIRECTION
+D,1,UZ                        ! CONSTRAIN SIMPLY SUPPORTED END AGAINST DISP.
+D,4,UZ,,,,,UX                 ! CONSTRAIN RIGID END AGAINST TWO DIRECTIONAL DISP
+D,5,ROTY                      ! CONSTRAIN RIGID END AGAINST ROTATIONAL MOVEMENT
+F,2,FZ,-1000                  ! APPLY ELASTIC FORCE AT HINGE B
+FINISH
+/SOLU    
+/OUT,SCRATCH
+SOLVE                         ! WRITE LOAD STEP
 FINISH
-/OUTPUT,SCRATCH                 ! DIVERT VOLUMINOUS SOLUTION OUTPUT
-/SOLU
-SOLCONTROL,0
-ANTYPE,STATIC                   
-NLGEOM,ON                       ! LARGE DEFORMATION ACTIVATED
-OUTRES,RSOL,ALL                 ! STORE REACTION RESULTS FOR ALL SUBSTEPS
-BFUNIF,TEMP,673                 ! UNIFORM TEMPERATURE OF 673 K
-D,3,ALL,0.0,,4
-TIME,0.000001                   ! NEAR ZERO TIME FOR FIRST LOAD STEP
-SOLVE
-NSUBST,20
-D,3,UX,0.2E-2,,4
-TIME,20
-SOLVE
-FINISH
-/OUTPUT
+
 /POST26
-RFORCE,2,3,F,X
-RFORCE,3,4,F,X
-ADD,4,2,3,,LOAD,,,(1/100),(1/100)    
-!         THE FX FORCE IS DIVIDED BY 100 BECAUSE THE DEFAULT OUT-
-!          OF-PLANE THICKNESS IS 1 METER WHILE PROBLEM CONSIDERED 
-!          HAS OUT-OF-PLANE THICKNESS OF 0.01 METER WHICH IS 100 
-!          TIMES LESS THAN 1 METER.
-PRVAR,4
-*GET,F1,VARI,4,RTIME,20
-*DIM,LABEL,CHAR,1,2
-*DIM,VALUE,,1,3
-LABEL(1,1) = 'Fx '
-LABEL(1,2) = 'N'
-*VFILL,VALUE(1,1),DATA,845
-*VFILL,VALUE(1,2),DATA,F1
-*VFILL,VALUE(1,3),DATA,ABS(F1/845)
-SAVE,TABLE1
+/OUT,
+RFORCE,2,1,F,Z
+RFORCE,3,5,M,Y
+STORE
+*GET,RA,VARI,2,EXTREM,VMAX 
+*GET,MC,VARI,3,EXTREM,VMAX 
+*GET,UB,NODE,2,U,Z
+*DIM,LABEL1,CHAR,3,2
+*DIM,VALUE1,,3,3
+LABEL1(1,1) = 'DEFLECTI','REACTION','MOMENT_C'
+LABEL1(1,2) = 'ON (in) ','_A (lb) ',' (ib-lb)'
+*VFILL,VALUE1(1,1),DATA,-.02829,148.15,27778
+*VFILL,VALUE1(1,2),DATA,UB,RA,MC
+*VFILL,VALUE1(1,3),DATA,ABS(UB/.02829) ,ABS(RA/148.15 ),ABS(MC/27778)
+SAVE,TABLE_1
 FINISH
-/CLEAR, NOSTART 
-!         PLANE183 ELEMENT TYPE
-/PREP7
-RESUME
-ET,1,183	                   ! 2-D, 8-NODE  ELEMENT
-KEYOPT,1,3,2					! PLANE STRAIN
-N,1
-N,2,1E-2
-N,3,1E-2,1E-2
-N,4,,1E-2
-N,5,0.5E-2
-N,6,1E-2,0.5E-2
-N,7,0.5E-2,1E-2
-N,8,,0.5E-2
-E,1,2,3,4,5,6,7,8
-D,1,ALL
-D,2,ALL
-D,5,ALL
-FINISH
-/OUTPUT,SCRATCH                 ! DIVERT VOLUMINOUS SOLUTION OUTPUT
-/SOLU
-SOLCONTROL,0
-NLGEOM,ON                       ! LARGE DEFORMATION ACTIVATED
-OUTRES,RSOL,ALL                 ! STORE REACTION RESULTS FOR ALL SUBSTEPS
-BFUNIF,TEMP,673                 ! UNIFORM TEMPERATURE OF 673 K
-D,3,ALL,0.0,,8
-TIME,0.000001                   ! NEAR ZERO TIME FOR FIRST LOAD STEP
-SOLVE
-NSUBST,20
-D,3,UX,0.2E-2,,4
-D,7,UX,0.2E-2
-D,6,UX,0.1E-2,,8,2
-TIME,20
+
+/SOLUTION
+
+NSUBST,3                      ! USE CONVERGENCE CRITERIA,3 SUBSTEPS MAX
+OUTPR,ALL,LAST                ! PRINT LAST ITERATION.
+F,2,FZ,-1388.8                ! APPLY VALUE SLIGHTLY SMALLER THAN PL TO HINGE B
+/OUT,SCRATCH
 SOLVE
-FINISH
-/OUTPUT
-/POST26
-RFORCE,2,3,F,X
-RFORCE,3,4,F,X
-RFORCE,4,7,F,X
-ADD,5,2,3,4,LOAD,,,(1/100),(1/100),(1/100)    
-PRVAR,5
-*GET,F1,VARI,5,RTIME,20
-*DIM,LABEL,CHAR,1,2
-*DIM,VALUE,,1,3
-LABEL(1,1) = 'Fx '
-LABEL(1,2) = 'N'
-*VFILL,VALUE(1,1),DATA,845
-*VFILL,VALUE(1,2),DATA,F1
-*VFILL,VALUE(1,3),DATA,ABS(F1/845)
-SAVE,TABLE2
-FINISH
+FINI
+
+/POST1
+/OUT,
+ESEL,S,ELEM,,3,4
+ETABLE,ELEM_STAT,NMISC,1	    !RETRIEVE THE STATUS(COMBIN40)
+ESEL,ALL
+PRETAB,
+
+/GRAPHICS,POWER
+/ESHAPE,1
+/VIEW,1,1,1,1
+/SHOW
+
+PLETAB,ELEM_STAT                    !PLOT ELEMENT TABLE(COMBIN40 STATUS)
+*GET,PLETAB_MAX1,PLNSOL,0,MAX
+*GET,PLETAB_MIN1,PLNSOL,0,MIN
+
+*DIM,LABEL2,CHAR,2,2
+*DIM,VALUE2,,2,3
+LABEL2(1,1) = 'HINGE','HINGE'
+LABEL2(1,2) = '@B','@C'
+*VFILL,VALUE2(1,1),DATA,1.0,2.0
+*VFILL,VALUE2(1,2),DATA,PLETAB_MIN1,PLETAB_MAX1
+*VFILL,VALUE2(1,3),DATA,ABS(PLETAB_MIN1/1.0) ,ABS(PLETAB_MAX1/2)
+SAVE,TABLE_2
+
+FINI
 
-/CLEAR, NOSTART 
-!         SOLID185 ELEMENT
-/PREP7
-RESUME
-ET,1,SOLID185    		        !3-D, 8-NODE VISCOPLASTIC ELEMENT
-N,1
-N,2,1E-2
-N,3,1E-2,1E-2
-N,4,,1E-2
-NGEN,2,4,1,4,1,,,1E-2
-E,1,2,3,4,5,6,7,8
-D,1,ALL,,,2
-D,5,ALL,,,6
-FINISH
-/OUTPUT,SCRATCH                 ! DIVERT VOLUMINOUS SOLUTION OUTPUT
 /SOLU
-SOLCONTROL,0
-NLGEOM,ON                       ! LARGE DEFORMATION ACTIVATED
-OUTRES,RSOL,ALL                 ! STORE REACTION RESULTS FOR ALL SUBSTEPS
-BFUNIF,TEMP,673                 ! UNIFORM TEMPERATURE OF 673 K
-D,3,ALL,0.0,,8
-TIME,0.000001                   ! NEAR ZERO TIME FOR FIRST LOAD STEP
-SOLVE
-NSUBST,20
-D,3,UX,0.2E-2,,4
-D,7,UX,0.2E-2,,8
-TIME,20
+
+F,2,FZ,-1390                  ! APPLY VALUE SLIGHTLY LARGER THAN PL TO HINGE B
+!                               LARGE DISPLACEMENT VALUES INDICATE COLLAPSE
+!                               AND PLASTIC DEFORMATION
+/OUT,SCRATCH
 SOLVE
+
 FINISH
-/OUTPUT
-/POST26
-RFORCE,2,3,F,X
-RFORCE,3,4,F,X
-RFORCE,4,7,F,X
-RFORCE,5,8,F,X
-ADD,6,2,3,4
-ADD,7,6,5,,LOAD
-PRVAR,7
-*GET,F1,VARI,7,RTIME,20
-*DIM,LABEL,CHAR,1,2
-*DIM,VALUE,,1,3
-LABEL(1,1) = 'Fx '
-LABEL(1,2) = 'N'
-*VFILL,VALUE(1,1),DATA,845
-*VFILL,VALUE(1,2),DATA,F1
-*VFILL,VALUE(1,3),DATA,ABS(F1/845)
+
+/POST1
+/OUT,
+ESEL,S,ELEM,,3,4
+ETABLE,ELEM_STAT,NMISC,1		!RETRIEVE THE STATUS(COMBIN40)
+ESEL,ALL
+PRETAB,
+
+PLETAB,ELEM_STAT			!PLOT ELEMENT TABLE(COMBIN40 STATUS)
+
+*GET,PLETAB_MAX2,PLNSOL,0,MAX
+*GET,PLETAB_MIN2,PLNSOL,0,MIN
+
+*DIM,LABEL3,CHAR,2,2
+*DIM,VALUE3,,2,3
+LABEL3(1,1) = 'HINGE','HINGE'
+LABEL3(1,2) = '@B','@C'
+*VFILL,VALUE3(1,1),DATA,-2.0,2.0
+*VFILL,VALUE3(1,2),DATA,PLETAB_MIN2,PLETAB_MAX2
+*VFILL,VALUE3(1,3),DATA,ABS(ABS(PLETAB_MIN2)/2.0) ,ABS(PLETAB_MAX2/2.0)
+SAVE,TABLE_3
+FINI
+
+RESUME,TABLE_1
 /COM
-/OUT,vm199,vrt
-/COM,------------------- VM199 RESULTS COMPARISON --------------
+/OUT,vm36,vrt
+/COM,------------------- VM36 RESULTS COMPARISON ---------------
 /COM,
-/COM,                  |   TARGET   |   Mechanical APDL   |   RATIO
+/COM,                 |   TARGET   |   ANSYS   |   RATIO
 /COM,
-/COM,PLANE182 RESULTS:
+/COM,RESULTS FOR P=1000 LBS (ELASTIC):
 /COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F15.2,'   ',1F18.3)
-/NOPR
-RESUME,TABLE1
-/GOPR
+*VWRITE,LABEL1(1,1),LABEL1(1,2),VALUE1(1,1),VALUE1(1,2),VALUE1(1,3)
+(1X,A8,A8,'   ',F11.5,'  ',F11.5,'   ',1F5.3)
 /COM,
-/COM,PLANE183 RESULTS:
 /COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F15.2,'   ',1F18.3)
 /NOPR
-RESUME,TABLE2
-/GOPR
+/COM,RESULTS FOR P=1388.8 LBS:
+/COM
+RESUME,TABLE_2
+*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
+(1X,A8,A8,'   ',F11.5,'  ',F11.5,'   ',1F5.3)
+/NOPR
+/COM,
+/COM,RESULTS FOR P=1390 LBS :
+/COM
+RESUME,TABLE_3
+*VWRITE,LABEL3(1,1),LABEL3(1,2),VALUE3(1,1),VALUE3(1,2),VALUE3(1,3)
+(1X,A8,A8,'   ',F11.5,'  ',F11.5,'   ',1F5.3)
 /COM,
-/COM,SOLID185 RESULTS:
+/COM,-----------------------------------------------------------
 /COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F15.2,'   ',1F18.3)
-/COM,----------------------------------------------------------
+
 /OUT
 FINISH
-*LIST,vm199,vrt
+*LIST,vm36,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm2.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm2.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM2
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM2, BEAM STRESSES AND DEFLECTIONS
 C***        STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 98, PROB. 4
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm20.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm20.dat`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,11 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM20
-/PREP7
 /TITLE, VM20, CYLINDRICAL MEMBRANE UNDER PRESSURE
 C*** STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 121, ART. 25
-C*** USING SHELL141 - MEMBRANE SHELL
-ANTYPE,STATIC
-ET,1,SHELL41
-MP,EX,1,30E6
-MP,NUXY,1,0.3
-R,1,1                   ! THICKNESS = 1
-CSYS,1                  ! CYLINDRICAL C.S.
-N,1,60                  ! DEFINE NODES
-N,2,60,,10
-NGEN,2,2,1,2,1,,10
-NROTAT,ALL              ! ROTATE NODAL C.S. TO CYLINDRICAL C.S.
-E,1,2,4,3               ! DEFINE ELEMENT
-CP,1,UX,1,2,3,4         ! COUPLE RADIAL DISPLACEMENTS
-CP,2,UZ,2,4             ! COUPLE UZ DISPLACEMENTS
-D,1,UZ,,,3,2
-D,ALL,UY
-SFE,1,4,PRES,,-15000    ! AXIAL TRACTION 
-SFE,1,1,PRES,,-500      ! INTERNAL PRESSURE 
-FINISH
-/SOLU    
-OUTPR,,1
-/OUT,SCRATCH
-SOLVE
-FINISH
-/POST1
-/OUT,
-*GET,STRS_HOP,NODE,1,S,2
-*GET,STRS_AX,NODE,1,S,1
-*DIM,LABEL,CHAR,2,2
-*DIM,VALUE,,2,3
-LABEL(1,1) = 'AXIAL ST','HOOP STR'
-LABEL(1,2) = 'RSS psi ','SS  psi '
-*VFILL,VALUE(1,1),DATA,15000,29749
-*VFILL,VALUE(1,2),DATA,STRS_HOP,STRS_AX
-*VFILL,VALUE(1,3),DATA,ABS(STRS_HOP/15000),ABS(STRS_AX/29749)
-SAVE,TABLE_1
-FINISH
-/CLEAR,NOSTART
-/TITLE, VM20, CYLINDRICAL MEMBRANE UNDER PRESSURE
 C*** USING SHELL181 - FINITE STRAIN MEMBRANE
 /PREP7
 ANTYPE,STATIC
 ET,1,SHELL181
 KEYOPT,1,1,1            ! MEMBRANE STIFFNESS ONLY
 KEYOPT,1,3,2            ! FULL INTEGRATION
 MP,EX,1,30E6
@@ -78,33 +38,24 @@
 *DIM,LABEL,CHAR,2,2
 *DIM,VALUE,,2,3
 LABEL(1,1) = 'AXIAL ST','HOOP STR'
 LABEL(1,2) = 'RSS psi ','SS  psi '
 *VFILL,VALUE(1,1),DATA,15000,29749
 *VFILL,VALUE(1,2),DATA,STRS_HOP,STRS_AX
 *VFILL,VALUE(1,3),DATA,ABS(STRS_HOP/15000),ABS(STRS_AX/29749)
-SAVE,TABLE_2
-RESUME,TABLE_1
+SAVE,TABLE_1
 /COM
 /OUT,vm20,vrt
 /COM,------------------- VM20 RESULTS COMPARISON ---------------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-/COM, SHELL41
-/COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.0,'  ',F14.0,'   ',1F15.3)
-/NOPR
-RESUME,TABLE_2
-/GOPR
 /COM,
 /COM, SHELL181
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.0,'  ',F14.0,'   ',1F15.3)
 /COM,-----------------------------------------------------------------
 /OUT
 FINISH
 *LIST,vm20,vrt
 /DELETE,TABLE_1
-/DELETE,TABLE_2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm200.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm200.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM200
 JPGPRF,500,100,1
 /SHOW,JPEG
 /PREP7
 /TITLE, VM200, VISCOELASTIC SANDWICH SEAL ANALYSIS
 /COM,    ----- 2-D ANALYSIS -----
 /COM,    "FE CALCULATIONS OF RESIDUAL STRESSES ....",SOULES ET AL.
@@ -65,26 +65,29 @@
 CPSGEN,2,2,2,3,1
 FINISH
 /COM    SINCE THE SOLUTION OUTPUT IS VOLUMINOUS IT IS DIVERTED TO A
 /COM     SCRATCH FILE
 /OUTPUT,SCRATCH
 *CREATE,MAC2                   ! CREATE MACRO FOR ANALYSIS TYPE AND LOADING
 /SOLU
-SOLCONTROL,0
 ANTYPE,STATIC
 /COM,    TEMPERATURE SET UP
 TREF,618
 TOFFST,273
 TUNIF,618
 TIME,1E-5
 CNVTOL,F,,,,.001             ! VERY SMALL MINIMUM ENFORCED
                                !  FOR CONVERGENCE
+CNVTOL,U,-1
+NEQIT,25
+AUTOTS,OFF
+KBC,0
 SOLVE
 OUTRES,ESOL,1                  ! STORE RESULTS FOR EVERY SUBSTEP
-NSUBST,200
+NSUBST,200,200,1
 TUNIF,460                      ! COOLING
 TIME,3160
 SOLVE
 TIME,(14400+3160)              ! ISOTHERMAL HOLD
 SOLVE
 TUNIF,18                       ! FURTHER COOLING
 TIME,(14400+12000)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm202.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm202.dat`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,131 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM202
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 /TITLE, VM202, TRANSVERSE VIBRATIONS OF A SHEAR BEAM
 /COM, REF:  R. BLEVINS, FORMULAS FOR NATURAL FREQUENCY AND MODE SHAPE, 1979.
-ANTYPE,MODAL
-ET,1,SHELL28
-R,1,0.1                 ! DEFINE REAL CONSTANT SET 1; THICKNESS OF SHELL
+ET,1,SHELL281           ! SHELL281 ELEMENT
+KEYOPT,1,1,1            ! MEMBRANE STIFFNESS ONLY
+SECTYPE,1,SHELL
+SECDATA,0.1             ! DEFINE THICKNESS OF SHELL
 MP,EX,  1,200E9
 MP,NUXY,1,0.27
 MP,DENS,1,7860.0 
-N,1                     ! DEFINE NODES
+
+N,1                     ! DEFINE NODES  
+N,5,5
 N,2,10
+N,6,10,5
 N,3,10,10
-N,4,  ,10
-NGEN,9,4,1,4,1,,,3.75
-E,1,2,6,5               ! DEFINE ELEMENTS
+N,7,5,10
+N,4,0,10
+N,8,0,5
+NGEN,17,8,1,8,1,,,3.75/2
+
+E,1,2,18,17,5,10,21,9   ! DEFINE ELEMENTS
+
 EGEN,3,1,-1
-E,4,1,5,8
-EGEN,8,4,-4
+
+E,1,17,20,4,9,24,12,8
+
+EGEN,15,8,1,8,1
+
 D,ALL,UZ                ! DEFINE BOUNDARY CONDITIONS
-D,1,UX,,,4,1,UY
-NSEL,S,LOC,Z,3.75       ! SELECT NODES AT COMMON Z LOCATION
-CP,1,UX,ALL             ! COUPLE NODES IN X AND Y DOF
+NSEL,S,LOC,Z,0
+D,ALL,UX,0
+D,ALL,UY,0
+NSEL,ALL
+
+NSEL,S,LOC,Z,1.8750
+CP,1,UX,ALL             ! COUPLE NODES IN X AND Y DOF 
 CP,2,UY,ALL
-NSEL,S,LOC,Z,7.5
-CP,3,UX,ALL
+
+NSEL,S,LOC,Z,3.75       
+CP,3,UX,ALL             
 CP,4,UY,ALL
-NSEL,S,LOC,Z,11.25
+
+NSEL,S,LOC,Z,5.625
 CP,5,UX,ALL
 CP,6,UY,ALL
-NSEL,S,LOC,Z,15
+
+NSEL,S,LOC,Z,7.5
 CP,7,UX,ALL
 CP,8,UY,ALL
-NSEL,S,LOC,Z,18.75
+
+NSEL,S,LOC,Z,9.375
 CP,9,UX,ALL
 CP,10,UY,ALL
-NSEL,S,LOC,Z,22.5
+
+NSEL,S,LOC,Z,11.25
 CP,11,UX,ALL
 CP,12,UY,ALL
-NSEL,S,LOC,Z,26.25
+
+NSEL,S,LOC,Z,13.125
 CP,13,UX,ALL
 CP,14,UY,ALL
-NSEL,S,LOC,Z,30
+
+
+NSEL,S,LOC,Z,15
 CP,15,UX,ALL
 CP,16,UY,ALL
+
+NSEL,S,LOC,Z,16.875
+CP,17,UX,ALL
+CP,18,UY,ALL
+
+NSEL,S,LOC,Z,18.75
+CP,19,UX,ALL
+CP,20,UY,ALL
+
+NSEL,S,LOC,Z,20.625
+CP,21,UX,ALL
+CP,22,UY,ALL
+
+NSEL,S,LOC,Z,22.5
+CP,23,UX,ALL
+CP,24,UY,ALL
+
+NSEL,S,LOC,Z,24.375
+CP,25,UX,ALL
+CP,26,UY,ALL
+
+NSEL,S,LOC,Z,26.25
+CP,27,UX,ALL
+CP,28,UY,ALL
+
+NSEL,S,LOC,Z,28.125
+CP,29,UX,ALL
+CP,30,UY,ALL
+
+NSEL,S,LOC,Z,30
+CP,31,UX,ALL
+CP,32,UY,ALL
 NSEL,ALL
+
 FINISH
-/out,scratch
+/OUT,SCRATCH
 /SOLU
-MXPAND,4                ! EXPAND FIRST TWO REPEATED MODES
-MODOPT,LANB,8
+ANTYPE,MODAL
+MODOPT,LANB,4
+MXPAND,4,,,YES          ! EXPAND THE 1ST 2 REPEATED MODES
 SOLVE
 *GET,F1,MODE,1,FREQ
 *GET,F2,MODE,3,FREQ
 FINISH
-/out
+
+/OUT,
 /POST1
 SET,1,1
 /VUP,,Z
 /VIEW,,,1
 PLDISP,1                ! DISPLAY DISPLACEMENTS (FIRST MODE)
 SET,1,3
 PLDISP,1                ! DISPLAY DISPLACEMENTS (SECOND MODE)
-*status,parm
 *DIM,VALUE,,2,3
 *DIM,LABEL,CHAR,2,2
 LABEL(1,1) = 'F1 ','F2 '
 LABEL(1,2) = 'Hz ','Hz '
 *VFILL,VALUE(1,1),DATA,17.375,52.176
 *VFILL,VALUE(1,2),DATA,F1,F2
 *VFILL,VALUE(1,3),DATA,ABS(F1/17.375),ABS(F2/52.176)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm203.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm203.dat`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM203   
 /SHOW,JPEG
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /PREP7
 /TITLE, VM203, DYNAMIC LOAD EFFECT ON SIMPLY-SUPPORTED THICK SQUARE PLATE
 /COM REFERENCE: NAFEMS FORCED VIBRATION BENCHMARKS, TEST 21R
 C***          USING SHELL281 ELEMENTS
@@ -21,39 +21,35 @@
 N,29,1.25,10,0
 FILL,21,29,3
 NGEN,4,40,21,29,2,2.5
 EN,1,1,41,43,3,21,42,23,2
 EGEN,4,2,1
 EGEN,4,40,1,4
 FINISH
-SAVE,MODEL
-*CREATE,SOLVIT,MAC
-/out,scratch
 /SOLU
 ANTYPE,MODAL                 ! DEFINE ANALYSIS TYPE AS MODAL VIBRATION
-MODOPT,LANPCG,16
-MXPAND,16,,,YES
+MODOPT,LANPCG,2
+MXPAND,2,,,YES
 SFE,ALL,,PRES,,-1E6          ! PRESS LOAD OF 1000,000 N/M**2
 D,ALL,UX,0,,,,UY,ROTZ        ! APPLY CONSTRAINTS
 D,1,UZ,0,0,9,1,ROTX
 D,161,UZ,0,0,169,1,ROTX
 D,1,UZ,0,0,161,20,ROTY
 D,9,UZ,0,0,169,20,ROTY
 SOLVE
 *GET,F,MODE,1,FREQ
-/out
 FINISH
 /SOLU
 /TITLE, VM203, RANDOM VIBRATION , RESPONSE TO UNIFORM PSD FORCE
 ANTYPE,SPECTR                 ! DEFINE ANALYSIS TYPE
 SPOPT,PSD,2,ON                ! USE FIRST 2 MODES, CALC ELEM. STRESSES
 PSDUNIT,1,PRES                ! DEFINE TYPE OF PSD AS A PRESSURE SPECTRUM 
 DMPRAT,0.02
 PSDFRQ,1,1,1.0,80.0
-PSDVAL,1,1.0,1.0              ! IN N**2/HZ
+PSDVAL,1,1.0,1.0              ! IN (N/m**2)**2/HZ
 SFEDELE,ALL,,PRES,,
 LVSCALE,1                     ! USE AND SCALE THE LOAD VECTOR GENERATED AT MODAL ANALYSIS
 PFACT,1,NODE
 PSDRES,DISP,REL
 PSDCOM
 SOLVE
 FINISH
@@ -64,50 +60,38 @@
 PRNSOL,U,Z
 L2=NODE(2,8,0)  
 *GET,SIGEL2,NODE,L2,S,EQV   
 NSEL,,NODE,,L2
 PRNSOL,S,COMP
 NSEL,ALL
 FINISH
-/SOLUTION
-ANTYPE,HARMIC                ! REDEFINE ANALYSIS TYPE AND SOLVE AGAIN 
-HROPT,MSUP                   ! USING MODE SUPERPOSITION HARMONIC ANALYSIS
-HROUT,OFF,ON                 ! PRINT AMPLITUDE & PHASE, CLUSTER FREQUENCIES
-KBC,1
-HARFRQ,1,80
-DMPRAT,0.02
-NSUBSTEP,10
-SOLVE
-FINISH
 /POST26
-FILE,,rfrq
-PRCPLX,1
+STORE,PSD,2
 NSOL,2,85,U,Z
-PSDDAT,6,1,1.0,80,1.0
-PSDTYP,2
-PSDCAL,7,2
-PSDPRT
-PRVAR,2,7
-*GET,P,VARI,7,EXTREM,VMAX
-*STATUS,PARM
-/AXLAB,Y,PSD  (M^2/HZ)
-PLVAR,7
+RPSD,3,2,,1,2,RPSD_UZ
+PRVAR,2,3
+EXTREM,2,3
+*GET,P,VARI,3,EXTREM,VMAX
+/AXLAB,Y,RPSD  (M^2/HZ)
+/XRANGE,0,80
+/GRID,OFF
+/SHOW,,PNG
+PLVAR,3
+/SHOW,CLOSE
+FINISH
 *DIM,LABEL,CHAR,2,2
 *DIM,VALUE,,2,3
-LABEL(1,1) = 'f ','PSD '
-LABEL(1,2) = 'Hz','SQmmS/Hz'
+LABEL(1,1) = 'f ','RPSD '
+LABEL(1,2) = 'Hz','m^2/Hz'
 *VFILL,VALUE(1,1),DATA,45.9,3.4018E-3
 *VFILL,VALUE(1,2),DATA,F,P
 *VFILL,VALUE(1,3),DATA,ABS(F/45.9),ABS(P/(3.4018E-3))
 FINISH
-*END
-SOLVIT
 SAVE,TABLE_1
 /NOPR
-RESUME,TABLE_1
 /COM
 /OUT,vm203,vrt
 /COM,------------------- VM203 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 /COM, SHELL281
@@ -117,10 +101,8 @@
 /COM,
 /COM,
 /COM,-----------------------------------------------------------
 /COM,
 /OUT
 FINISH
 *LIST,vm203,vrt
-/DELETE,MODEL
-/DELETE,SOLVIT,MAC
 /DELETE,TABLE_1
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm204.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm204.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM204
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /UNITS,BIN
 /PREP7 
 /TITLE, VM204, SOLID MODEL OF AN AXIAL BEARING 
 /COM    ANY BASIC GEOMETRY TEXT
@@ -60,14 +60,15 @@
 VDELE,1,,,1
 VGLUE,ALL                                       ! GLUE VOLUMES - CONTINUITY
 /TYPE,1,4
 /VIEW,1,1,2,3                                   ! VIEWING ANGLE
 /AUTO,1
 /TRIAD,OFF 
 VPLOT                                           ! DISPLAY VOLUMES
+/OUT,SCRATCH
 VSUM                                            ! CALCULATE TOTAL VOLUME
 *GET,TVOL,VOLU,,VOLU
 *status,parm
 *DIM,VALUE,,1,3
 *DIM,LABEL,CHAR,1,2
 LABEL(1,1) = 'VOLUME '
 LABEL(1,2) = 'NO UNTS '
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm205.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm5.dat`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,97 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM205
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM5
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
-SMRT,OFF
-/TITLE, VM205, ELLIPTIC MEMBRANE UNDER A UNIFORMLY-DISTRIBUTED LOAD
-/COM,   NAFEMS (REF.58), TEST NO. LE1 (MODIFIED)
-/COM,   USING 2-D STRUCTURAL SOLID, PLANE182
-ANTYPE,STATIC   
-ET,1,PLANE182,3,,3          ! DEFINE ELEMENT AS PLANE182 FOR PLANE STRESS 
-                            !  WITH THICKNESS
-MP,EX,1,210E9               ! DEFINE MATERIAL PROPERTIES
-MP,NUXY,1,.3
-R,1,0.1                     ! SET THICKNESS
-LOCAL,11,1,,,,,,,0.5        ! DEFINE ELLIPTICAL COORD. SYSTEM
-K,1,2,90                    ! CREATE MODEL GEOMETRY
-K,2,2,0                     ! DEFINE KEYPOINTS
-L,1,2                       ! DEFINE LINE SEGMENTS
-LOCAL,12,1,,,,,,,0.8461585
-K,3,3.25,90
-K,4,3.25,0.0
-L,3,4
-CSYS,0
-L,2,4
-L,1,3
-AL,2,4,1,3                  ! DEFINE AREA
-DL,4,1,SYMM                 ! APPLY BOUNDARY CONDITIONS 
-DL,3,1,SYMM
-SFL,2,PRES,-10E6            ! APPLY LINE PRESSURE LOAD
-MSHK,2                    ! MAPPED AREA MESH IF POSSIBLE
-MSHA,0,2D                 ! USING QUADS
-SAVE                        ! SAVE DATABASE
-FINISH
-ADAPT,4,7,,,1               ! USE Mechanical APDL PREDEFINED MACRO FOR ADAPTIVE MESHING
-                            !  AND SOLUTION WITH NSOLN=3, STARGT=7, AND FACMX=1
-*CREATE,MAC                 ! CREATE MACRO FOR POST PROCESSING 
-/POST1
-EPLOT                       ! PLOT ELEMENTS
-PRERR                       ! PRINT THE ENERGY NORM PERCENT ERROR (SEPC)
-NSEL,S,LOC,Y,0.0
-NSEL,R,LOC,X,2.0
-*GET,MNODE,NODE,,NUM,MAX
-*GET,SY_D,NODE,MNODE,S,Y    ! GET DESIRED STRESS SY VALUE
+/TITLE, VM5, LATERALLY LOADED TAPERED SUPPORT STRUCTURE (QUAD. ELEMENTS)
+C***     MECHANICS OF SOLIDS, CRANDALL AND DAHL, 1959, PAGE 342, PROB. 7.18
+C***          USING PLANE42 ELEMENTS
+ANTYPE,STATIC
+ET,1,PLANE182,2,,3      
+R,1,2
+MP,EX,1,30E6
+MP,NUXY,1,0.0            ! POISSON'S RATIO SET TO 0.0 TO AGREE WITH BEAM THEORY
+N,1,25
+N,7,75 
+FILL
+N,8,25,-3 
+N,14,75,-9
+FILL     
+E,2,1,8,9 
+EGEN,6,1,1   
+NSEL,S,LOC,X,75   
+D,ALL,ALL                ! CONSTRAIN NODES AT FIXED END
 NSEL,ALL
-ESEL,ALL
-*status,parm                     ! SHOW STATUS OF PARAMETERS
-*END
-*USE,MAC                    ! USE POST PROCESSING MACRO
-*DIM,LABEL,CHAR,1,2
-*DIM,VALUE,,1,3
-LABEL(1,1) = 'TAN STR '
-LABEL(1,2) = 'MPa'
-*VFILL,VALUE(1,1),DATA,92.70
-*VFILL,VALUE(1,2),DATA,(SY_D/1000000)
-*VFILL,VALUE(1,3),DATA,ABS((SY_D/1000000)/92.7)
-SAVE,TABLE1
+F,1,FY,-4000
+FINISH
+/SOLU    
+OUTPR,,1
+/OUT,SCRATCH
+SOLVE
+FINISH
+/POST1
+/OUT,
+END_NODE = NODE (75,0,0)
+*GET,STS_E_182,NODE,END_NODE,S,X       ! STRESS AT FIXED END (END NODE )
+PLDISP,2
+MID_NODE = NODE (50,0,0)
+*GET,STS_M_182,NODE,MID_NODE,S,EQV 
 FINISH
-/CLEAR, NOSTART ! CLEAR DATABASE BEFORE STARTING PART 2
-/COM,        USING 2-D 8-NODE STRUCTURAL SOLID, PLANE82 
 /PREP7
-SMRT,OFF
-RESUME                      ! RESUME DATABASE
-ET,1,PLANE183,,,3            ! DEFINE ELEMENT AS PLANE82 FOR PLANE STRESS 
-                            !  WITH THICKNESS
-FINISH
-ADAPT,2,5,,,1               ! USE Mechanical APDL PREDEFINED MACRO FOR ADAPTIVE MESHING
-                            !  AND SOLUTION WITH NSOLN=2, STARGT=5, AND FACMX=1
-*USE,MAC                    ! USE POST PROCESSING MACRO
-*DIM,VALUE,,1,3
-*DIM,LABEL,CHAR,1,2
-LABEL(1,1) = 'TAN STR '
-LABEL(1,2) = 'MPa'
-*VFILL,VALUE(1,1),DATA,92.70
-*VFILL,VALUE(1,2),DATA,(SY_D/1000000)
-*VFILL,VALUE(1,3),DATA,ABS((SY_D/1000000)/92.7)
-SAVE,TABLE2
-RESUME,TABLE1
-/COM
-/OUT,vm205,vrt
-/COM,------------------- VM205 RESULTS COMPARISON --------------
+/TITLE, VM5, LATERALLY LOADED TAPERED SUPPORT STRUCTURE (QUAD. ELEMENTS)
+C***          MECHANICS OF SOLIDS, CRANDALL AND DAHL, 1959, PAGE 342, PROB. 7.18
+C***          USING PLANE183 ELEMENTS
+C***                      ! CHANGE ELEMENT TYPE TO HIGHER ORDER PLANE82
+ET,1,PLANE183,,,3
+EMID                      ! ADD MIDSIDE NODES TO PLANE183 ELEMENTS
+NSEL,R,LOC,X,75  
+NSEL,R,LOC,Y,-4.5         ! SELECT MIDSIDE NODE AT FIXED END
+D,ALL,ALL                 ! CONSTRAIN  MIDSIDE NODE AT FIXED END
+NSEL,ALL
+FINISH
+/SOLU    
+/OUT,SCRATCH
+SOLVE
+FINISH
+/POST1
+/OUT,
+END_NODE = NODE (75,0,0) 
+*GET,STS_E_183,NODE,END_NODE,S,X       ! STRESS AT FIXED END (END NODE )
+MID_NODE = NODE (50,0,0)   
+*GET,STS_M_183,NODE,MID_NODE,S,EQV  
+
+*DIM,LABEL,CHAR,2,2
+*DIM,VALUEI,,2,3
+*DIM,VALUEII,,2,3
+LABEL(1,1) = 'MID_STRS','END-STRS'
+LABEL(1,2) = ' (psi)  ',' (psi)  '
+*VFILL,VALUEI(1,1),DATA,8333,7407
+*VFILL,VALUEI(1,2),DATA,STS_M_182,STS_E_182
+*VFILL,VALUEI(1,3),DATA,(STS_M_182/8333),(STS_E_182/7407)
+*VFILL,VALUEII(1,1),DATA,8333,7407
+*VFILL,VALUEII(1,2),DATA,STS_M_183,STS_E_183
+*VFILL,VALUEII(1,3),DATA,(STS_M_183/8333),(STS_E_183/7407)
+/COM,STS_M_42 = STRESS AT MID-LENGTH USING ELEMENT 42
+/COM,STS_E_42 = STRESS AT FIXED END USING ELEMENT 42
+/COM,STS_M_183 = STRESS AT MID-LENGTH USING ELEMENT 183
+/COM,STS_E_183 = STRESS AT FIXED END USING ELEMENT 183
 /COM,
-/COM,                  |   TARGET   |   Mechanical APDL   |   RATIO
+/OUT,vm5,vrt
+/COM,------------------- VM5 RESULTS COMPARISON ---------------------
 /COM,
-/COM,PLANE182 RESULTS:
+/COM,RESULTS FOR PLANE182:
 /COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F18.3)
-/NOPR
-RESUME,TABLE2
-/GOPR
+/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUEI(1,1),VALUEI(1,2),VALUEI(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
 /COM,
-/COM,PLANE183 RESULTS:
+/COM,RESULTS FOR PLANE183:
 /COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F18.3)
-/COM,----------------------------------------------------------
+/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUEII(1,1),VALUEII(1,2),VALUEII(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
+/COM,----------------------------------------------------------------
 /OUT
+
 FINISH
-*LIST,vm205,vrt
+*LIST,vm5,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm207.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm286.dat`

 * *Files 26% similar despite different names*

```diff
@@ -1,270 +1,312 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM207
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM286
+/TITLE,VM286,WEAR OF BLOCK UNDER UNIFORM COMPRESSION
+/COM, 2D MODEL WITH CONTACT ELEMENT 172
 /PREP7 
-JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
-/SHOW,JPEG
-SMRT,OFF
-/TITLE,VM207,  STRANDED COIL MODEL, CIRCUIT-FED OPTION
-/COM,   REF: BOAST "ELECTRIC AND MAGNETIC FIELDS", PG. 247, EQN. 12.18
-ET,1,53,,,1         ! AIR
-ET,2,53,3,,1        ! CIRCUIT-COUPLED STRANDED COIL
-ET,3,110,,,1        ! FAR-FIELD
-ET,4,124,0          ! EXTERNAL RESISTOR
-ET,5,124,4,4        ! INDEPENDENT VOLTAGE SOURCE, PIECEWISE LINEAR LOAD
-ET,6,124,5          ! STRANDED COIL (TO FEA DOMAIN)
-R,2,2               ! 2 OHM RESISTOR
-R,3,1               ! SYMMETRY FACTOR FOR COIL
-EMUNIT,MKS
-MP,MURX,1,1
-MP,MURX,2,1
-MP,RSVX,2,3.04878E-8  ! RESISTIVITY OF COIL
-S=.02
-N=500
-R=3*S/2
-N,1                   ! CREATE NODES FOR CIRCUIT ELEMENTS
-*REPEAT,4,1
-RECTNG,S,2*S,0,S/2
-PCIRC,0,6*S,0,90
-PCIRC,0,12*S,0,90
-AOVLAP,ALL
-ASEL,S,AREA,,1
-AATT,2,1,2
-ASUM
-*GET,A,AREA,,AREA        ! AREA OF 1/2 COIL CROSS-SECTION
-ASEL,S,AREA,,5
-AATT,1,1,1
-ASEL,S,AREA,,4
-AATT,1,1,3
-ASEL,ALL
-CSYS,1
-LSEL,S,LOC,X,9*S
-LESIZE,ALL,,,1  
-ESIZE,,8
-AMESH,4   
-*GET,A,AREA,,AREA        ! AREA OF 1/2 COIL CROSS-SECTION
-R,1,2*A,500,,1,.9
-ASEL,S,AREA,,1
-LSLA,S  
-LESIZE,ALL,,,5  
-LSEL,ALL
-ASEL,ALL
-CSYS,0
-KSEL,S,LOC,X,0
-KSEL,R,LOC,Y,0
-KESIZE,ALL,S/5
-AMESH,ALL
-N1=NODE(S,0,0)           ! GET A NODE ON THE COIL
-TYPE,5                   ! VOLTAGE SOURCE
-R,4,0,12,.01,12,.010001,0 ! PIECEWISE LINEAR LOAD
-REAL,4
-E,2,1,4                  ! VOLTAGE SOURCE ELEMENT
-TYPE,4                   ! RESISTOR
+LEN=10
+! ELEMENTS TYPES
+ET,1,PLANE182
+ET,2,TARGE169
+ET,3,CONTA172
+KEYOPT,3,2,0            ! AUGMENTED LAGRANGIAN CONTACT FORMULATION
+KEYOPT,3,4,2            ! NODAL DETECTION-NORMAL TO TARGET
+KEYOPT,3,10,1           ! USE CONSTANT CONTACT STIFFNESS
+
+!MATERIAL PROPETIES
+MP,EX,1,100E3           ! YOUNG'S MODULUS
+MP,NUXY,1,0.3           ! POISSON'S RATIO
+
+! WEAR PROPERTIES
+KARCD=0.0001            ! WEAR COEFFICIENT
+TB,WEAR,2,,,ARCD        ! WEAR MATERIAL MODEL
+TBFIELD,TIME,0
+TBDATA,1,0.00000,1,1,1  ! NO WEAR IN FIRST LOAD STEP  
+TBFIELD,TIME,1
+TBDATA,1,0.00000,1,1,1 
+TBFIELD,TIME,1.0001
+TBDATA,1,KARCD,1,1,1    ! START WEAR IN 2ND LOAD STEP
+TBFIELD,TIME,10
+TBDATA,1,KARCD,1,1,1 
+
+! GEOMETRY AND MESH
+RECTNG,,LEN,,LEN
+LESIZE,ALL,,,2
+TYPE,1
+REAL,1
+MAT,1
+AMESH,1
+
+! GENERATE CONTACT ELEMENTS
+TYPE,3
+REAL,2
+MAT,2
+NSEL,S,LOC,Y
+ESURF
+ALLSEL,ALL,
+
+! GENERATE TARGET ELEMENTS
+TYPE,2
 REAL,2
-E,2,3                    ! EXTERNAL RESISTOR ELEMENT
-TYPE,6                   ! STRANDED COIL (TO FEA DOMAIN)
-REAL,3
-E,3,1,N1                 ! STRANDED COIL "ELEMENT"
-ESEL,S,MAT,,2            ! GET COIL ELEMENTS
-NSLE,S
-CP,1,CURR,ALL            ! COUPLE CURR DOF IN COIL
-CP,2,EMF,ALL             ! COUPLE EMF DOF IN COIL 
-*GET,ELM,ELEM,,NUM,MIN   ! GET AN ELEMENT NUMBER IN THE COIL REGION
+MAT,2
+N,1001,-5*LEN
+N,1002,5*LEN
+E,1002,1001
+TSHAP,PILOT
+E,1001
+NSEL,S,NODE,,1001
+CM,PILOTNODE,NODES
 NSEL,ALL
-ESEL,ALL
-FINISH
-/SOLU
-ANTYPE,STATIC
-TIME,1E-9
-CSYS,1
-NSEL,S,LOC,X,12*S
-SF,ALL,INF               ! APPLY INFINITE SURFACE FLAG
-CSYS,0
-NSEL,S,LOC,X,0
-D,ALL,AZ,0
+
+! APPLY BC
+NSEL,S,LOC,X
+NSEL,R,LOC,Y,LEN
+CM,UXFIX,NODES
+D,UXFIX,UX,0
 NSEL,ALL
-D,1,VOLT,0               ! GROUND
-SOLVE
+NSEL,S,LOC,Y,LEN
+CM,UYFIX,NODES
+D,UYFIX,UY,-0.01*LEN
+ALLSEL,ALL,ALL
 FINISH
-/POST1
-SET,LAST
-ESEL,S,MAT,,2            ! SELECT COIL ELEMENTS
-ETABLE,RES,NMISC,8       ! STORE ELEMENT RESISTANCE
-ETABLE,IND,NMISC,9       ! STORE ELEMENT INDUCTANCE
-SSUM
-*GET,CRES,SSUM,,ITEM,RES ! GET COIL RESISTANCE
-*GET,CIND,SSUM,,ITEM,IND ! GET COIL INDUCTANCE
- CRES=2*CRES
- CIND=2*CIND
-ESEL,ALL
-FINISH
-/SOLU
-ANTYPE,TRANS
-OUTRES,ALL,ALL           ! STORE EVERY SUBSTEP
-DELTIM,.0004
-TIME,.01
-SOLVE
+
+/SOLUTION
+ANTYPE,STATIC           ! STATIC ANALYSIS
+NLGEOM,ON               ! NON-LINEAR ANALYSIS
+OUTRES,ALL,ALL
+AUTOTS,ON               ! AUTO TIME STEPPING
+! LOAD STEP 1, PUSH DOWN THE BLOCK ON THE RIGID PLATE
+TIME,1                  ! END TIME
+DELTIM,1,1E-3,1         ! TIME INCREMENT
+/OUT,SCRATCH
+SOLVE                   ! 1ST LOAD STEP
+
+! LOAD STEP 2, START WEAR BY SLIDING THE RIGID PLATE
+D,PILOTNODE,UX,1
+TIME,2                  ! END TIME
+DELTIM,0.01,1E-4,0.01   ! TIME INCREMENT
+SOLVE                   ! 2ND LOAD STEP
 FINISH
-/POST26
-NSOL,2,N1,CURR           ! GET CURRENT IN COIL
-RES=CRES+2
-I01=(12/RES)*(1-(EXP(-RES*.01/CIND)))
-PRVAR,2  
-*GET,ICUR,VARI,2,RTIME,.01                
-/AXLAB,X,TIME
-/AXLAB,Y,CURRENT IN COIL (AMPS)
-/SHOW
-PLVAR,2                  ! PLOT COIL CURRENT VS TIME.
-*DIM,LABEL,CHAR,3,2
-*DIM,VALUE,,3,3
-LABEL(1,1) = 'INDUCTAN','RESISTAN','CURRENT,'
-LABEL(1,2) = 'CE,HENRY','CE, OHM ',' AMPS   '
-*VFILL,VALUE(1,1),DATA,.01274,3.9908,1.9849
-*VFILL,VALUE(1,2),DATA,CIND,CRES,ICUR
-*VFILL,VALUE(1,3),DATA,ABS(CIND/.01274),ABS(CRES/3.9908),ABS(ICUR/1.9849)
-/COM
-/OUT,vm207,vrt
-/COM,------------------- VM207 RESULTS COMPARISON -------------
-/COM,
-/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
-/COM,PLANE53
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
-/OUT
+
+/POST1
+! CALCULATE THE REFERENCE SOLUTION
+EX_MODULI=100e3
+LEN=10
+U_APPLIED=0.01*LEN
+TIME=1
+DTIME=0.01
+NSUBTOT=TIME/DTIME +1
+KWEAR=1e-4
+*DIM,WEAR,ARRAY,NSUBTOT
+*VFILL,WEAR,RAMP,0,0
+*DIM,STRAIN_,ARRAY,NSUBTOT
+*VFILL,STRAIN_,RAMP,0,0
+*DIM,STRESS_,ARRAY,NSUBTOT
+*VFILL,STRESS_,RAMP,0,0
+*DO,I,1,NSUBTOT
+STRAIN_(I)=((U_APPLIED-WEAR(I))/LEN)+ 0.5*((U_APPLIED-WEAR(I))/LEN)**2
+STRESS_(I)=EX_MODULI*STRAIN_(I)
+*IF,I,LT,NSUBTOT,THEN
+WEAR(I+1)=WEAR(I)+(KWEAR*STRESS_(I)*DTIME)
+*ENDIF
+*ENDDO
+*DIM,LABEL1,CHAR,8
+LABEL1(1)='WEAR-Y'
+*DIM,LABEL2,CHAR,8
+LABEL2(1)='CON-PRES'
+! POSTPROCESS MAPDL RESULTS
+SET,2
+ESEL,S,TYPE,,3
+EL1_=ELNEXT(0)
+*GET,ANSWEAR,ELEM,EL1_,NMISC,88
+*GET,ANSPRES,ELEM,EL1_,SMISC,5
+/OUT,vm286,vrt
+/COM,----------------- VM286 RESULTS COMPARISON -------------------
+/COM,
+/COM,
+/COM,2D    WEAR    |  TARGET   |  Mechanical APDL  |   RATIO
+/COM,
+*VWRITE,LABEL1(1),WEAR(NSUBTOT),ANSWEAR,ANSWEAR/WEAR(NSUBTOT)
+(2X,A12,6X,,F6.4,6X,,F6.4,12X,,F5.3)
+/COM,
+/COM,
+/COM,
+/COM,2D    PRES      |  TARGET   |  Mechanical APDL  |   RATIO
+/COM,
+*VWRITE,LABEL2(1),STRESS_(NSUBTOT),ANSPRES,ANSPRES/STRESS_(NSUBTOT)
+(2X,A12,4X,,F12.4,4X,,F12.3,8X,,F5.3)
+/COM,
+/COM,
+/COM,----------------- VM286 RESULTS COMPARISON -------------------
 FINISH
 
+
 /CLEAR,NOSTART
-/NOPR
-/PREP7
-JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
-/SHOW,JPEG
-SMRT,OFF
-/TITLE,VM207,  STRANDED COIL MODEL, CIRCUIT-FED OPTION
-ET,1,233,,,1        ! AIR
-ET,2,233,2,,1       ! STRANDED COIL
-ET,3,110,,,1        ! FAR-FIELD
-ET,4,124,0          ! EXTERNAL RESISTOR
-ET,5,124,4,4        ! INDEPENDENT VOLTAGE SOURCE, PIECEWISE LINEAR LOAD
-R,2,2               ! 2 OHM RESISTOR
-R,4,0,12,.01,12,.010001,0 ! PIECEWISE LINEAR LOAD
-
-EMUNIT,MKS
-MP,MURX,1,1
-MP,MURX,2,1
-
-S=.02		    ! COIL WIDTH AND HEIGHT
-SC=S**2             ! COIL CROSS-SECTIONAL AREA
-N=500		    ! NUMBER OF TURNS
-RMID=3*S/2	    ! BROOKS COIL MIDSPAN RADIUS
-R=3.991             ! COIL RESISTANCE
-
-N,1                 ! CREATE NODES FOR CIRCUIT ELEMENTS
-*REPEAT,3,1
-
-R,3,1.0,SC,N,RMID,1,R
-RMORE,2
-
-RECTNG,S,2*S,0,S/2
-PCIRC,0,6*S,0,90
-PCIRC,0,12*S,0,90
-AOVLAP,ALL
-ASEL,S,AREA,,1
-AATT,2,3,2
-ASUM
-*GET,A,AREA,,AREA        ! AREA OF 1/2 COIL CROSS-SECTION
-ASEL,S,AREA,,5
-AATT,1,1,1
-ASEL,S,AREA,,4
-AATT,1,1,3
-ASEL,ALL
-CSYS,1
-LSEL,S,LOC,X,9*S
-LESIZE,ALL,,,1  
-ESIZE,,8
-AMESH,4   
-
-ASEL,S,AREA,,1
-LSLA,S  
-LESIZE,ALL,,,5  
-LSEL,ALL
-ASEL,ALL
-CSYS,0
-KSEL,S,LOC,X,0
-KSEL,R,LOC,Y,0
-KESIZE,ALL,S/5
-AMESH,ALL
 
-NSEL,ALL
+/OUT,
+/COM, 3D MODEL WITH  CONTACT ELEMENT 174
+/PREP7 
+LEN=10
+! ELEMENTS TYPES
+ET,1,SOLID185
+ET,2,TARGE170
+ET,3,CONTA174
+KEYOPT,3,2,3            ! PURE LAGRANGIAN CONTACT FORMULATION
+KEYOPT,3,4,2            ! NODAL DETECTION-NORMAL TO TARGET
+KEYOPT,3,10,1           ! USE CONSTANT CONTACT STIFFNESS
+
+!MATERIAL PROPETIES
+MP,EX,1,100E3           ! ELASTIC PROP
+MP,NUXY,1,0.3
+
+! WEAR PROPERTIES
+KARCD=0.0001            ! WEAR COEFFICIENT
+TB,WEAR,2,,,ARCD        ! WEAR MATERIAL MODEL
+TBFIELD,TIME,0
+TBDATA,1,0.00000,1,1,1  ! NO WEAR IN FIRST LOAD STEP  
+TBFIELD,TIME,1
+TBDATA,1,0.00000,1,1,1 
+TBFIELD,TIME,1.0001
+TBDATA,1,KARCD,1,1,1    ! START WEAR IN 2ND LOAD STEP
+TBFIELD,TIME,10
+TBDATA,1,KARCD,1,1,1 
+
+! GEOMETRY AND MESH
+BLOCK,,LEN,,LEN,,LEN
+LESIZE,ALL,,,2
+TYPE,1
+REAL,1
+MAT,1
+VMESH,1
+! GENERATE CONTACT ELEMENTS
 
-N1=NODE(S,0,0)           ! GET A NODE ON THE COIL
+TYPE,3
+REAL,2
+MAT,2
+NSEL,S,LOC,Z
+ESURF
+ALLSEL,ALL,ALL
 
-TYPE,5                   ! VOLTAGE SOURCE
-REAL,4
-E,2,1,3                  ! VOLTAGE SOURCE ELEMENT
-TYPE,4                   ! RESISTOR
+! GENERATE TARGET ELEMENTS
+TYPE,2
 REAL,2
-E,2,N1                   ! EXTERNAL RESISTOR ELEMENT, DIRECTLY CONNECTED TO THE COIL
+MAT,2
+N,1001,-5*LEN,-5*LEN
+N,1002,5*LEN,-5*LEN
+N,1003,5*LEN,5*LEN
+N,1004,-5*LEN,5*LEN
+E,1001,1002,1003,1004
+TSHAP,PILOT
+E,1001
+NSEL,S,NODE,,1001
+CM,PILOTNODE,NODES
+NSEL,ALL
+
+! APPLY BC
+NSEL,S,LOC,X
+NSEL,R,LOC,Y
+NSEL,R,LOC,Z,LEN
+CM,ALLFIX,NODES
+D,ALLFIX,UX,0
+D,ALLFIX,UY,0
 
-ESEL,S,MAT,,2            ! GET COIL ELEMENTS
-NSLE,S
-CP,1,VOLT,ALL            ! COUPLE VOLT DOF IN COIL
-CP,2,EMF,ALL             ! COUPLE EMF DOF IN COIL
-*GET,ELM,ELEM,,NUM,MIN   ! GET AN ELEMENT NUMBER IN THE COIL REGION
 NSEL,ALL
-ESEL,ALL
-CSYS,1
-NSEL,S,LOC,X,12*S
-SF,ALL,INF
-CSYS,0
-NSEL,S,LOC,X,0
-D,ALL,AZ,0
+NSEL,S,LOC,Z,LEN
+NSEL,R,LOC,X,LEN
+NSEL,R,LOC,Y
+CM,UYFIX,NODES
+D,UYFIX,UY,0
+
 NSEL,ALL
+NSEL,S,LOC,Z,LEN
+NSEL,R,LOC,Y,LEN
+NSEL,R,LOC,X
+CM,UXFIX,NODES
+D,UXFIX,UX,0
+
+NSEL,S,LOC,Z,LEN
+CM,BCNODES,NODES
+D,BCNODES,UZ,-0.01*LEN
+ALLSEL,ALL,ALL
 FINISH
 
 /SOLU
-ANTYPE,STATIC
-TIME,1E-9
-D,1,VOLT,0               ! GROUND
-SOLVE
+ANTYPE,STATIC           ! STATIC ANALYSIS
+NLGEOM,ON               ! NON-LINEAR ANALYSIS
+OUTRES,ALL,ALL
+AUTOTS,ON               ! AUTO TIME STEPPING
+! LOAD STEP 1, PUSH DOWN THE BLOCK ON THE RIGID PLATE
+TIME,1                  ! END TIME
+DELTIM,1,1E-3,1         ! TIME INCREMENT
+/OUT,SCRATCH
+SOLVE                   ! PERFORM 1ST LOAD STEP
+
+! LOAD STEP 2, START WEAR BY SLIDING THE RIGID PLATE
+D,PILOTNODE,UX,1
+TIME,2                  ! END TIME
+DELTIM,0.01,1E-4,0.01   ! TIME INCREMENT
+SOLVE                   ! PERFORM 2ND LOAD STEP
 FINISH
 
 /POST1
-*GET,IC,NODE,1,RF,AMPS   ! GET COIL CURRENT
-ETABLE,_SENE,SENE        ! SUM UP MAGNETIC ENERGY STORED
-SSUM
-*GET,W,SSUM,,ITEM,_SENE
-W=2*W                    ! SYMMETRY FACTOR
-LCOIL=2*W/IC**2          ! CALCULATE INDUCTANCE VIA MAGNETIC ENERGY
-FINISH
-
-/SOLU
-ANTYPE,TRANS
-OUTRES,ALL,ALL           ! STORE EVERY SUBSTEP
-DELTIM,.0004
-TIME,.01
-SOLVE
-FINISH
+! CALCULATE THE REFERENCE SOLUTION
+EX_MODULI=100e3
+LEN=10
+U_APPLIED=0.01*LEN
+TIME=1
+DTIME=0.01
+NSUBTOT=TIME/DTIME +1
+KWEAR=1e-4
+*DIM,WEAR,ARRAY,NSUBTOT
+*VFILL,WEAR,RAMP,0,0
+*DIM,STRAIN_,ARRAY,NSUBTOT
+*VFILL,STRAIN_,RAMP,0,0
+*DIM,STRESS_,ARRAY,NSUBTOT
+*VFILL,STRESS_,RAMP,0,0
+*DO,I,1,NSUBTOT
+STRAIN_(I)=((U_APPLIED-WEAR(I))/LEN)+ 0.5*((U_APPLIED-WEAR(I))/LEN)**2
+STRESS_(I)=EX_MODULI*STRAIN_(I)
+*IF,I,LT,NSUBTOT,THEN
+WEAR(I+1)=WEAR(I)+ (KWEAR*STRESS_(I)*DTIME)
+*ENDIF
+*ENDDO
+*DIM,LABEL1,CHAR,8
+LABEL1(1)='WEAR-Z'
+*DIM,LABEL2,CHAR,8
+LABEL2(1)='CON-PRES'
+! POSTPROCESS ANSYS RESULTS
+SET,2
+ESEL,S,TYPE,,3
+EL1_=ELNEXT(0)
+*GET,ANSWEAR,ELEM,EL1_,NMISC,181
+*GET,ANSPRES,ELEM,EL1_,SMISC,13
 
-/POST26
-RFOR,2,1,AMPS           ! GET CURRENT IN COIL
-/AXLAB,X,TIME
-/AXLAB,Y,CURRENT IN COIL (AMPS)
-/YRANGE,0,2,.2
-/SHOW
-PLVAR,2                  ! PLOT COIL CURRENT VS TIME.
-PRVAR,2                  ! PRINT COIL CURRENT VS TIME.
-*DIM,LABEL,CHAR,2,2
-*DIM,VALUE,,2,3
-LABEL(1,1) = 'INDUCTAN','CURRENT,'
-LABEL(1,2) = 'CE,HENRY',' AMPS   '
-*VFILL,VALUE(1,1),DATA,.01274,1.9849
-*VFILL,VALUE(1,2),DATA,LCOIL,IC
-*VFILL,VALUE(1,3),DATA,ABS(LCOIL/.01274),ABS(IC/1.9849)
-/COM
-/OUT,vm207,vrt,,APPEND            
-/COM,PLANE233
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
-/COM,----------------------------------------------------------
+/OUT,vm286,vrt,,append
+/COM,----------------- VM286 RESULTS COMPARISON -------------------
+/COM,
+/COM,
+/COM,3D    WEAR    |  TARGET   |  Mechanical APDL  |   RATIO
+/COM,
+*VWRITE,LABEL1(1),WEAR(NSUBTOT),ANSWEAR,ANSWEAR/WEAR(NSUBTOT)
+(2X,A12,6X,,F6.4,6X,,F6.4,12X,,F5.3)
+/COM,
+/COM,
+/COM,
+/COM,
+/COM,3D    PRES      |  TARGET   |  Mechanical APDL  |   RATIO
+/COM,
+*VWRITE,LABEL2(1),STRESS_(NSUBTOT),ANSPRES,ANSPRES/STRESS_(NSUBTOT)
+(2X,A12,4X,,F12.4,4X,,F12.3,8X,,F5.3)
+/COM,
+/COM,
+/COM,----------------- VM286 RESULTS COMPARISON -------------------
 /OUT
-FINISH
-*LIST,vm207,vrt
+*LIST,vm286,vrt
+FINI
+/EXIT,NOSAVE
+
+
+
+
+
+
+
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm208.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm208.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM208
 /PREP7
 /TITLE, VM208, TEST CIRCUIT COMPONENT CCCS IN HARMONIC ANALYSIS
 /COM  REV.5.2  SDS-98
 /COM,   SEE SCHAUMS OUTLINE "BASIC CIRCUIT ANALYSIS", 2ND ED, 1992,
 /COM,   PROBLEM 14.23, FIGURE 14-25.
 /NOPR
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm209.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm209.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM209
 /TITLE,VM209,DOUBLE BELLOWS AIR SPRING
 /COM, REFERENCE: BERRY,DALE T. AND YANG,HENRY T.Y.,"FORMULATION AND EXPERIMENTAL
 /COM, VERIFICATION OF A PNEUMATIC FINITE ELEMENT" - IJNME, VOL. 39, PG:1097-1114 (1996)
 /COM, 
 /PREP7
 ET,1,208				!AXISYMMETRIC SHELL
@@ -126,21 +126,21 @@
 RFOR,5,14,F,Y,FY14
 ADD,6,4,5,,RFOR,,,-1,-1			!SWITCH THE SIGNS OF RFOR RESULTS
 
 /OUT
 /RESET
 AA=
 *DIM,AA,TABLE,7,6
-AA(1,0) = 10,9,8,7,6,5			!VALUES FOR DISPLACEMENT
-AA(0,1) = 0,990,1231,1692,2230,2769,3384,4230
-AA(0,2) = 0,869.659,1226.55,1609.8,2050.35,2581.33,3246.09,4109.82
-AA(0,3) = 0, 1850,2640,3350,4050,5000,6000,7333
-AA(0,4) = 0,1750.69,2405.88,3089.12,3849.41,4738.9,5825.32,7209.64
-AA(0,5) = 0,2667,3875,4650,6000,7200,8750
-AA(0,6) = 0,2644.49,3596.3,4578.78,5658.43,6906.07,8413.2
+AA(1,0) = 5,6,7,8,9,10			!VALUES FOR DISPLACEMENT
+AA(0,1) = 2769,   2230,   1692,   1231,   990    ,0.0
+AA(0,2) = 2581.33,2050.35,1609.8, 1226.55,869.659,0.0 
+AA(0,3) = 5000,   4050,   3350,   2640,   1850   ,0.0
+AA(0,4) = 4738.9, 3849.41,3089.12,2405.88,1750.69,0.0
+AA(0,5) = 7200,   6000,   4650,   3875,   2667   ,0.0 
+AA(0,6) = 6906.07,5658.43,4578.78,3596.3, 2644.49,0.0
 /TITLE,ANALYSIS OF DOUBLE BELLOWS AIR SPRING
 /GCOLUMN,1,EXP 20 PSI			!ASSIGNS AA(0,1) AS EXPERIMENTAL DATA AT 20 PSI
 /GMARKER,1,1
 /GCOLUMN,2,ANS 20 PSI			!ASSIGNS AA(0,2) AS Mechanical APDL DATA AT 20 PSI (GAS)
 /GMARKER,2,2
 /GCOLUMN,3,EXP 40 PSI			!ASSIGNS AA(0,3) AS EXPERIMENTAL DATA AT 40 PSI
 /GMARKER,3,1
@@ -353,21 +353,21 @@
 RFOR,5,14,F,Y,FY14  
 ADD,6,4,5,,RFOR,,,-1,-1			!SWITCH THE SIGNS OF RFOR RESULTS 
     
 /OUT
 /RESET
 AA=
 *DIM,AA,TABLE,7,6
-AA(1,0) = 10,9,8,7,6,5			!VALUES FOR DISPLACEMENT
-AA(0,1) = 0,990,1231,1692,2230,2769,3384,4230
-AA(0,2) = 0,869.659,1249.79,1650.75,2077.76,2613.12,3263.09,4238.18
-AA(0,3) = 0, 1850,2640,3350,4050,5000,6000,7333
-AA(0,4) = 0,1750.69,2455.05,3185.58,3950.18,4742.42,5923.76,7251.99
-AA(0,5) = 0,2667,3875,4650,6000,7200,8750
-AA(0,6) = 0,2644.49,3613.49,4580.66,5674.34,6922.04,8780.85
+AA(1,0) = 5,6,7,8,9,10			!VALUES FOR DISPLACEMENT
+AA(0,1) = 2769.0, 2230.0, 1692.0, 1231.0, 990.0,  0.0
+AA(0,2) = 2613.12,2077.76,1650.75,1249.79,869.659,0.0
+AA(0,3) = 5000.0, 4050.0, 3350.0, 2640.0, 1850.0, 0.0
+AA(0,4) = 4742.42,3950.18,3185.58,2455.0, 1750.69,0.0
+AA(0,5) = 7200.0, 6000.0, 4650.0, 3875.0, 2667.0, 0.0
+AA(0,6) = 6922.04,5674.34,4580.66,3613.49,2644.49,0.0
 /TITLE,ANALYSIS OF DOUBLE BELLOWS AIR SPRING
 /GCOLUMN,1,EXP 20 PSI			!ASSIGNS AA(0,1) AS EXPERIMENTAL DATA AT 20 PSI
 /GMARKER,1,1
 /GCOLUMN,2,ANS 20 PSI			!ASSIGNS AA(0,2) AS Mechanical APDL DATA AT 20 PSI (PVDATA)
 /GMARKER,2,2
 /GCOLUMN,3,EXP 40 PSI			!ASSIGNS AA(0,3) AS EXPERIMENTAL DATA AT 40 PSI
 /GMARKER,3,1
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm21.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm21.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM21
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM21, TIE ROD WITH LATERAL LOADING, NO STREES STIFFENING 
 C***   STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 42, ART. 6
 ANTYPE,STATIC
 ET,1,BEAM188
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm210.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm210.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM210
 /TITLE,VM210, BENDING OF HEX-TO-TET INTERFACE, FORMATION OF PYRAMIDS
 /COM,   ****** USING 3-D SOLID95 ******
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
+/OUT,SCRATCH
 /PREP7 
 SMRT,OFF
 ET,1,95                                  ! ELEMENT TYPE SOLID95
 ET,2,95                                  ! ELEMENT TYPE SOLID95
 
 *CREATE,MSHGEN3D,MAC                     ! CREATE MACRO TO GENERATE MESH
 MP,EX,1,30E6                             ! ELASTIC MODULUS
@@ -101,15 +102,14 @@
 *END
 
 SOLV3D                                     ! READ MACRO TO PERFORM SOLUTION
 
 *CREATE,RES3D,MAC
 /POST1
 SET,LAST
-/OUT,
 PRRSOL                                     ! PRINT REACTION SOLUTIONS
 /GRA,OFF
 /VIEW,1,1,0,0
 /GLINE,1,0
 /DEV,VECT,ON
 PLNSOL,S,Z                                 ! Z-STRESS CONTOUR 
 /NUM,0
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm211.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm211.dat`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM211
-/config,nproc,1
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 R = 200                        ! RADIUS OF CYLINDER (mm)
 /PREP7
 SMRT,OFF
 /TITLE, VM211, RUBBER CYLINDER PRESSED BETWEEN TWO PLATES
-/stitle,1,Reason COMPARE differences are acceptable:
-/stitle,2,  mesher accuracy - number of nodes, elements, dof, iterations; affects solution
 /COM    REF: T. SUSSMAN, K.J. BATHE, "A FE FORMULATION FOR NONLINEAR ..."
 /COM         COMPUTERS & STRUCTURES, VOL. 26, NOS. 1/2, 1987
 ET,1,PLANE182, , ,2            ! 2-D PLANE-STRAIN 4-NODE STRUCTURAL SOLID
 KEYOPT,1,6,1                   ! Mixed U-P FORMULATION
 ET,2,TARGE169                  ! 2-D TARGET ELEMENT
-ET,3,CONTA171                  ! 2-D CONTACT ELEMENT
+ET,3,CONTA172                  ! 2-D 3-NODE CONTACT ELEMENT WITH DROPPED MIDSIDE NODES
 KEYOPT,3,5,4
-KEYOPT,3,10,2
+KEYOPT,3,10,0
 C10 = 0.293
 C01 = 0.177
 NU1 = 0.49967
 DD  = (1-2*NU1)/(C10+C01)
 TB,HYPER,1,1,2,MOONEY
 TBDATA,1,C10,C01,DD
 CSYS,1                         ! SWITCH TO CYLINDRICAL C.S.
@@ -46,33 +43,30 @@
 AMESH,ALL                         ! MESH ALL AREAS
 REAL,2
 TYPE,2
 LMESH,10
 LSEL,S,LINE,,1,2,1
 TYPE,3
 LMESH,ALL
-save,cont171,db
+save,plane182,db
 FINI
 
 *CREATE,SOLV2D,MAC             ! MACRO TO SOLVE MODEL
 /SOLU
-!SOLCONTROL,0
 ANTYPE,STATIC
 NSEL,S,LOC,X
 D,ALL,UX
 NSEL,S,LOC,Y
 CP,1,UY,ALL
 *GET,NCEN,NODE,,NUM,MIN
 ALLSEL
-!CNVTOL,F,,,,-1
 NLGEOM,ON                     ! INCLUDE LARGE DEFORMATION EFFECTS
 NSUBST,20,1000,10             ! SPECIFY NUMBER OF SUBSTEPS IN LOAD STEP
 OUTRES,,1                     ! WRITE SOLUTION FOR EVERY SUBSTEP
 D,NCEN,UY,-100                ! APPLY DISPLACEMENT UY = -100 TO COUPLED NODES
-!NROPT,FULL,,OFF
 SOLVE
 FINISH
 *END
 /OUT,SCRATCH
 SOLV2D                         ! USE MACRO SOLVE2D
 /OUT,
 *CREATE,PLOTS,MAC              ! MACRO FOR POST-PROCESSING
@@ -107,40 +101,41 @@
 
 RESUME,temp,db
 /PREP7
 ALLSEL
 ET,1,PLANE183, , ,2            ! 2-D PLANE-STRAIN 8-NODE STRUCTURAL SOLID
 KEYOPT,1,6,1                   ! Mixed U-P FORMULATION
 ET,2,TARGE169                  ! 2-D TARGET ELEMENT
-ET,3,CONTA172                  ! 2-D CONTACT ELEMENT
+ET,3,CONTA172                  ! 2-D 3-NODE CONTACT ELEMENT
 KEYOPT,3,5,4
-KEYOPT,3,10,2
+KEYOPT,3,10,0
 TYPE,1
 AMESH,ALL
 REAL,2
 TYPE,2
 LMESH,10
 LSEL,S,LINE,,1,2,1
 TYPE,3
 LMESH,ALL
-save,cont172,db
+save,plane183,db
 FINISH
 /OUT,SCRATCH
 SOLV2D                         ! USE MACRO TO OBTAIN SOLUTION
 PLOTS                          ! USE MACRO TO POSTPROCESS
 /OUT,
 SAVE,TABLE_2
-
+fini
+/clear,nostart
 /PREP7
 RESUME,temp,db
 ET,5,SOLID185                  ! 3-D 8-NODE STRUCTURAL SOLID
 KEYOPT,5,6,1                   ! Mixed U-P FORMULATION
 ET,2,TARGE170
-ET,3,CONTA173                  ! 3-D 4 NODE CONTACT ELEMENT
-KEYOPT,3,10,2
+ET,3,CONTA174                  ! 3-D 8 NODE CONTACT ELEMENT WITH DROPPED MIDSIDE NODES 
+KEYOPT,3,10,0
 KEYOPT,3,5,4
 ET,4,200,6                     ! 2-D 4 NODED MESH200
 LDELETE,10,,,1
 ALLSEL
 CSYS,0
 K,1001,-.1*R,-R,-.1*R
 K,1002,2*R,-R,-.1*R
@@ -164,31 +159,29 @@
 ASEL,S,LOC,X,R
 TYPE,3
 REAL,2
 AMESH,ALL
 LSEL,ALL
 NSEL,ALL
 CSYS,0
-save,cont173,db
+save,solid185,db
 FINISH
 
 *CREATE,SOLV3D,MAC            ! MACRO TO SOLVE MODEL
 /SOLUTION
 ANTYPE,STATIC
 D,ALL,UZ                      ! CONSTRAIN ALL IN Z (PLANE STRAIN)
 NSEL,S,LOC,X
 D,ALL,UX
 NSEL,S,LOC,Y
 CP,1,UY,ALL
 *GET,NCEN,NODE,,NUM,MIN
 NSEL,ALL
-!CNVTOL,F,1
 NLGEOM,ON                     ! INCLUDE LARGE DEFORMATION EFFECTS
 NSUBST,20,1000,10             ! SPECIFY NUMBER OF SUBSTEPS IN LOAD STEP
-!NROPT,FULL,,OFF
 OUTRES,,1                     ! WRITE SOLUTION FOR EVERY SUBSTEP
 D,NCEN,UY,-100                ! APPLY DISPLACEMENT UY = -100 TO COUPLED NODES
 SOLVE
 FINISH
 *END
 /OUT,SCRATCH
 SOLV3D                         ! USE MACRO TO OBTAIN SOLUTION
@@ -197,16 +190,16 @@
 SAVE,TABLE_3
 
 /PREP7
 RESUME,temp3d,db
 ET,1,SOLID186                  ! 3-D 20-NODE STRUCTURAL SOLID
 KEYOPT,1,6,1                   ! Mixed U-P FORMULATION
 ET,2,TARGE170
-ET,3,CONTA174
-KEYOPT,3,10,2
+ET,3,CONTA174                  ! 3-D 8-NODE CONTACT ELEMENT
+KEYOPT,3,10,0
 KEYOPT,3,5,4
 KEYOPT,3,7,1
 VEXT,1,3,1,,,1
 TYPE,1
 VMESH,ALL
 REAL,2
 TYPE,3
@@ -215,124 +208,193 @@
 AMESH,ALL
 ESIZE,,1
 TYPE,2
 ASEL,ALL
 AMESH,4
 ALLSEL
 CSYS,0
-save,cont174,db
+save,solid186,db
 FINI
 /OUT,SCRATCH
 SOLV3D
 /OUT,
 PLOTS
 SAVE,TABLE_4
 
 !* THE INPUT BELOW IS SAME AS INPUT ABOVE BUT WITH K(2)=3 OF CONTAC171-174 ELEMENTS...
-RESUME,cont171,db
+RESUME,plane182,db
 /PREP7
 KEYOPT,3,4,2                   ! ON NODAL POINT - NORMAL TO TARGET SURFACE
 KEYOPT,3,2,3                   ! LAGRANGE MULTIPLIER ON CONTACT NORMAL AND PENALTY ON TANGENT
 FINISH
 /OUT,SCRATCH
 SOLV2D                         ! USE MACRO TO OBTAIN SOLUTION
 /OUT,
 PLOTS                          ! USE MACRO TO POSTPROCESS
 SAVE,TABLE_5
 
-RESUME,cont172,db
+RESUME,plane183,db
 /PREP7
 KEYOPT,3,4,2                   ! ON NODAL POINT - NORMAL TO TARGET SURFACE
 KEYOPT,3,2,3                   ! LAGRANGE MULTIPLIER ON CONTACT NORMAL AND PENALTY ON TANGENT
 FINISH
 /OUT,SCRATCH
 SOLV2D                         ! USE MACRO TO OBTAIN SOLUTION
 /OUT,
 PLOTS                          ! USE MACRO TO POSTPROCESS
 SAVE,TABLE_6
 
-RESUME,cont173,db
+RESUME,solid185,db
 /PREP7
 KEYOPT,3,4,2                   ! ON NODAL POINT - NORMAL TO TARGET SURFACE
 KEYOPT,3,2,3                   ! LAGRANGE MULTIPLIER ON CONTACT NORMAL AND PENALTY ON TANGENT
 FINISH
 /OUT,SCRATCH
 SOLV3D                         ! USE MACRO TO OBTAIN SOLUTION
 /OUT,
 PLOTS                          ! USE MACRO TO POSTPROCESS
 SAVE,TABLE_7
 
-RESUME,cont174,db
+RESUME,solid186,db
 /PREP7
 KEYOPT,3,4,2                   ! ON NODAL POINT - NORMAL TO TARGET SURFACE
 KEYOPT,3,2,3                   ! LAGRANGE MULTIPLIER ON CONTACT NORMAL AND PENALTY ON TANGENT
 FINISH
 /OUT,SCRATCH
 SOLV3D
 /OUT,
 PLOTS
 SAVE,TABLE_8
 
+!* THE INPUT BELOW IS SAME AS INPUT ABOVE BUT WITH K(6)=3 OF CONTAC171-174 ELEMENTS...
+RESUME,plane182,db
+/PREP7
+KEYOPT,3,6,3                   ! USE AN EXPONENTIAL PRESSURE-PENETRATION RELATIONSHIP
+FINISH
+/OUT,SCRATCH
+SOLV2D                         ! USE MACRO TO OBTAIN SOLUTION
+/OUT,
+PLOTS                          ! USE MACRO TO POSTPROCESS
+SAVE,TABLE_9
+
+RESUME,plane183,db
+/PREP7
+KEYOPT,3,6,3                   ! USE AN EXPONENTIAL PRESSURE-PENETRATION RELATIONSHIP
+FINISH
+/OUT,SCRATCH
+SOLV2D                         ! USE MACRO TO OBTAIN SOLUTION
+/OUT,
+PLOTS                          ! USE MACRO TO POSTPROCESS
+SAVE,TABLE_10
+
+RESUME,solid185,db
+/PREP7
+KEYOPT,3,6,3                   ! USE AN EXPONENTIAL PRESSURE-PENETRATION RELATIONSHIP
+FINISH
+/OUT,SCRATCH
+SOLV3D                         ! USE MACRO TO OBTAIN SOLUTION
+/OUT,
+PLOTS                          ! USE MACRO TO POSTPROCESS
+SAVE,TABLE_11
+
+RESUME,solid186,db
+/PREP7
+KEYOPT,3,6,3                   ! USE AN EXPONENTIAL PRESSURE-PENETRATION RELATIONSHIP
+FINISH
+/OUT,SCRATCH
+SOLV3D
+/OUT,
+PLOTS
+SAVE,TABLE_12
+
 /COM
 /OUT,vm211,vrt
 RESUME,TABLE_1
 /COM,------------------- VM211 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-/COM,RESULTS USING PLANE182:
+/COM,PLANE182:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_2
 /GOPR
 /COM,
-/COM,RESULTS USING PLANE183:
+/COM,PLANE183:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_3
 /GOPR
 /COM,
-/COM,RESULTS USING SOLID185:
+/COM,SOLID185:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_4
 /GOPR
 /COM,
-/COM,RESULTS USING SOLID186:
+/COM,SOLID186:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_5
 /GOPR
 /COM,
-/COM,RESULTS USING PLANE182 WITH KEYOPT(2)=3 OF CONTAC171:
+/COM,PLANE182 WITH KEYOPT(2)=3 OF CONTAC172(DROPPED MIDSIDE NODES):
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_6
 /GOPR
 /COM,
-/COM,RESULTS USING PLANE183 WITH KEYOPT(2)=3 OF CONTAC172:
+/COM,PLANE183 WITH KEYOPT(2)=3 OF CONTAC172:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_7
 /GOPR
 /COM,
-/COM,RESULTS USING SOLID185 WITH KEYOPT(2)=3 OF CONTAC173:
+/COM,SOLID185 WITH KEYOPT(2)=3 OF CONTAC174(DROPPED MIDSIDE NODES):
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_8
 /GOPR
 /COM,
-/COM,RESULTS USING SOLID186 WITH KEYOPT(2)=3 OF CONTAC174:
+/COM,SOLID186 WITH KEYOPT(2)=3 OF CONTAC174:
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
+/NOPR
+RESUME,TABLE_9
+/GOPR
+/COM,
+/COM,PLANE182 WITH KEYOPT(6)=3 OF CONTAC172(DROPPED MIDSIDE NODES):
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
+/NOPR
+RESUME,TABLE_10
+/GOPR
+/COM,
+/COM,PLANE183 WITH KEYOPT(6)=3 OF CONTAC172:
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
+/NOPR
+RESUME,TABLE_11
+/GOPR
+/COM,
+/COM,SOLID185 WITH KEYOPT(6)=3 OF CONTAC174(DROPPED MIDSIDE NODES):
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
+/NOPR
+RESUME,TABLE_12
+/GOPR
+/COM,
+/COM,SOLID186 WITH KEYOPT(6)=3 OF CONTAC174:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /COM,-----------------------------------------------------------
 /COM,
 /OUT
 FINISH
 *LIST,vm211,vrt
@@ -343,13 +405,17 @@
 /DELETE,TABLE_2
 /DELETE,TABLE_3
 /DELETE,TABLE_4
 /DELETE,TABLE_5
 /DELETE,TABLE_6
 /DELETE,TABLE_7
 /DELETE,TABLE_8
+/DELETE,TABLE_9
+/DELETE,TABLE_10
+/DELETE,TABLE_11
+/DELETE,TABLE_12
 /DELETE,temp,db
 /DELETE,temp3d,db
-/DELETE,cont171,db
-/DELETE,cont172,db
-/DELETE,cont173,db
-/DELETE,cont174,db
+/DELETE,plane182,db
+/DELETE,plane183,db
+/DELETE,solid185,db
+/DELETE,solid186,db
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm212.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm212.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM212
 /TITLE,VM212,DDAM ANALYSIS OF FOUNDATION SYSTEM (2-DOF SYSTEM)
 /COM, --------------------------------------------------------------------
 /COM  REFERENCE:
 /COM, INTERIM DESIGN VALUES FOR SHOCK DESIGN OF SHIPBOARD EQUIPMENT
 /COM  NRL MEMORANDUM REPORT 1396, G. J. O'HARA, FEBRUARY 1963, P10.
 /COM, --------------------------------------------------------------------
@@ -179,23 +179,23 @@
 *VFILL,VALUE(1,3),DATA,FREQ_1/46.3,FREQ_2/114
 
 *DIM,LAB1,CHAR,5,2
 *DIM,VALUE1,,5,3
 LAB1(1,1) = 'DEF.(20), ','DEF.(30)  ','MCOEF  ','PFACT ','SHOCK,D1  ' 
 LAB1(1,2) = '  INCH','  INCH','','','  IN/S^2'
 *VFILL,VALUE1(1,1),DATA,0.1629,0.1099,0.1931,7.0659,2316
-*VFILL,VALUE1(1,2),DATA,UZ1_20,UZ1_30,MODC_1,PFAC_1,DA_1
+*VFILL,VALUE1(1,2),DATA,ABS(UZ1_20),ABS(UZ1_30),ABS(MODC_1),ABS(PFAC_1),ABS(DA_1)
 *VFILL,VALUE1(1,3),DATA,ABS(UZ1_20)/0.1629,ABS(UZ1_30)/0.1099,ABS(MODC_1)/0.1932,ABS(PFAC_1)/7.060,ABS(DA_1)/2316
 
 *DIM,LAB2,CHAR,5,2
 *DIM,VALUE2,,5,3
 LAB2(1,1) = 'DEF.(20), ','DEF.(30)  ','MCOEF  ','PFACT ','SHOCK,D2  ' 
 LAB2(1,2) = '  INCH','  INCH','','','  IN/S^2'
-*VFILL,VALUE2(1,1),DATA,-0.1099,0.1629,0.2175E-01,1.373,8133
-*VFILL,VALUE2(1,2),DATA,UZ2_20,UZ2_30,MODC_2,PFAC_2,DA_2
+*VFILL,VALUE2(1,1),DATA,0.1099,0.1629,0.2175E-01,1.373,8133
+*VFILL,VALUE2(1,2),DATA,ABS(UZ2_20),ABS(UZ2_30),ABS(MODC_2),ABS(PFAC_2),ABS(DA_2)
 *VFILL,VALUE2(1,3),DATA,ABS(UZ2_20)/0.1099,ABS(UZ2_30)/0.1629,ABS(MODC_2)/0.2176E-01,ABS(PFAC_2)/1.373,ABS(DA_2)/8133
 /COM
 /OUT,vm212,vrt
 /COM,------------------- VM212 RESULTS COMPARISON --------------
 /COM,
 /COM,                   |   TARGET   |   Mechanical APDL   			|   RATIO
 /COM,
@@ -211,7 +211,8 @@
 /COM,
 *VWRITE,LAB2(1,1),LAB2(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
 (1X,A8,A8,'   ',F12.4,'  ',F16.4,'   ',1F15.3)
 /COM,----------------------------------------------------------
 /OUT,
 *LIST,vm212,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm213.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm213.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM213
 /TITLE,VM213, DIFFERENTIAL INDUCTANCE OF A TRANSFORMER
 /NOPR
 /COM
 /COM  REFERENCE:
 /COM  M.GYIMESI,D.OSTERGAARD,"INDUCTANCE COMPUTATION BY
 /COM  INCREMENTAL FINITE ELEMENT ANALYSIS", IEEE
@@ -294,7 +294,8 @@
 /COM,
 *VWRITE,LABEL(1),VALUE(1,1),RESULTS(1,1),VALUE(1,2)
 (1X,A10,'     ',F10.4,'    ',F10.4,'     ',1F13.3)
 /COM,-------------------------------------------------------------------
 /OUT,
 *LIST,vm213,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm214.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm214.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM214
 /TITLE, VM214, ROD ROTATING IN UNIFORM MAGNETIC FIELD
 /com,
 /com,  Problem description:
 /com,  A conducting rod of length L and radius R is rotating in a uniform
 /com,  magnetic field Bz with angular velocity OMEGAZ. Determine the EMF
 /com,  induced in the rod.
 /com,  
 /com,  Reference: Any basic electromagnetic text book
 /com,
 
 JPGPRF,500,100,1
+/OUT,SCRATCH
 /PREP7
 
 PI=ACOS(-1)
 
 L_ROD=0.06		    ! LENGTH OF ROD
 R_ROD=L_ROD/10		! RADIUS OF ROD
 
@@ -41,15 +42,14 @@
 ET,2,SOLID236,1
 MP,MURX,2,1
 MP,RSVX,2,1
 
 VSEL,S,MAT,,2
 VSWE,ALL
 VSEL,S,MAT,,1
-/OUT,SCRATCH
 MSHA,1
 MSHMID,1              ! STRAIGHT EDGES
 VMES,ALL
 
 BF,ALL,VELO,,,,,,OMG_ROD ! OMEGAZ (RAD/S)
 
 DFLX,ALL,,,BZ_EXT     ! UNIFORM MAGNETIC FIELD
@@ -57,15 +57,15 @@
 VSEL,S,MAT,,2
 ALLS,BELO,VOLU
 NSEL,R,LOC,X
 D,ALL,VOLT            ! ELECTRICALLY GROUND ONE END
 ALLSEL,ALL
 FINISH
 
-/SOLU
+/SOLUTION
 ANTYPE,STATIC         ! ELECTROMAGNETIC STATIC ANALYSIS
 TIME,1.0
 SOLVE
 FINISH
 
 /POST1
 SET,LAST
@@ -93,7 +93,8 @@
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F9.5,'  ',F13.5,'   ',1F15.3)
 /COM,
 /COM,-----------------------------------------------------------
 /OUT
 FINISH
 *LIST,vm214,vrt
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm215.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm215.dat`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM215
 /PREP7
 /TITLE,VM215, CONDUCTING SPHERE
 ET,1,157              
 R,1,0.2               ! THICKNESS = 0.2
 MP,RSVX,,7            ! DEFINE ELECTRICAL RESISTIVITIES PROPERTY 
 MP,KXX,,3             ! DEFINE THERMAL CONDUCTIVITIES PROPERTY
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm216.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm216.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM216
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM216, LATERAL BUCKLING OF RIGHT-ANGLE FRAME
 !  J.C. SIMO, L. VU-QUOC, "THREE-DIMENSIONAL FINITE-STRAIN ROD
 !  MODEL",PART II CMAME, VOL 58, 1986, PP 79-116
 
@@ -36,15 +36,15 @@
 F,41,FZ,1.0E-3		!APPLY PERTURBATION FORCE
 /OUT,SCRATCH,		!SUPPRESS SOLUTION DATA
 SOLVE
 OUTRES,ALL,ALL
 ARCLEN,ON
 ARCTRM,U,60,41,UZ
 F,41,FX,1.485		!APPLY END FORCE
-NSUBST,10
+NSUBST,20
 SOLVE
 FINISH
 
 /POST26
 /AXLAB,X,TIP DISPLACEMENT
 /AXLAB,Y,END FORCE
 NSOL,2,41,U,Z,DISP
@@ -104,15 +104,15 @@
 F,41,FZ,1.0E-3
 /OUT,SCRATCH,,,APPEND
 SOLVE
 OUTRES,ALL,ALL
 ARCLEN,ON
 ARCTRM,U,60,41,UZ
 F,41,FX,1.485
-NSUBST,10
+NSUBST,20
 SOLVE
 FINISH
 
 /POST26
 /AXLAB,X,TIP DISPLACEMENT
 /AXLAB,Y,END FORCE
 NSOL,2,41,U,Z,DISP
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm217.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm217.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM217
 /TITLE,VM217, PORTAL FRAME UNDER SYMMETRIC LOADING
 ! N. J. HOFF, THE ANALYSIS OF STRUCTURES, PG 115
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 W=-500
 A=400
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm218.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm218.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM218
 /TITLE,VM218, HYPERELASTICITY TEST: BALLOON/CIRCULAR PLATE PROBLEM
 /COM          USING SHELL181 ELEMENTS
 /GRAPHICS,POWER
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
@@ -44,15 +44,14 @@
 OUTRES, ALL, ALL,
 SF,ALL,PRES,50.0
 NEQITR,20 
 FINISH
 /SOLUTION
 /OUT,SCRATCH
 SOLVE
-/OUT
 FINISH
 /POST1
 /NOPR		   !SUPPRESS GRAPHING DATA
 /VIEW,1,,-1
 /ANG,1
 /USER
 /FOCUS,1,4,,8,0	   !SET UP CENTER OF GRAPHICS SCREEN FOR DISPLACEMENT PLOT
@@ -140,16 +139,18 @@
 /NOERASE
 NSOL,2,1,U,Z,UZ_1
 PROD,7,1, , ,SH.181 , , ,50,0,0,!MULTIPLY SOLUTION BY 50
 /COLOR,CURVE,MRED
 XVAR,2  		        !SPECIFY X VARIABLE TO BE DISPLAYED
 PLVAR,7 		        !DISPLAY SOLUTION IN GRPH FILE
 /ERASE
+/OUT,
 PRVAR,7,2		        !LIST VARIABLE 7 VERSUS VARIABLE 2
 FINISH
+/OUT,SCRATCH
 /POST1
 /NOPR
 SET,NEAR,,,,0.08		!SELECT UZ VALUE FOR NODE 1 AT T=0.08
 *GET,VR1,NODE,1,U,Z
 SET,NEAR,,,,0.48		!UZ VALUE FOR NODE 1 AT T=0.48
 *GET,VR2,NODE,1,U,Z
 SET,NEAR,,,,0.76		!UZ VALUE FOR NODE 1 AT T=0.76
@@ -221,15 +222,14 @@
 /ANG,1
 /ESHAPE,1
 EPLOT
 FINISH
 /SOLUTION
 /OUT,SCRATCH
 SOLVE
-/OUT
 FINISH
 *END
 SOLVEIT
 *CREATE,PLOTS,MAC
 /POST1
 /NOPR		   !SUPPRESS GRAPHING DATA
 /VIEW,1,,,1
@@ -320,15 +320,17 @@
 /NOERASE
 NSOL,2,1,U,Y,UY_1
 PROD,7,1, , ,SH.%ET1%, , ,50,0,0,!MULTIPLY SOLUTION BY 50
 /COLOR,CURVE,MRED
 XVAR,2  		         !SPECIFY X VARIABLE TO BE DISPLAYED
 PLVAR,7 		         !DISPLAY SOLUTION IN GRPH FILE
 /ERASE
+/OUT,
 PRVAR,7,2		         !LIST VARIABLE 7 VERSUS VARIABLE 2
+/OUT,SCRATCH
 FINISH
 /POST1
 /NOPR
 SET,NEAR,,,,0.08		 !SELECT UZ VALUE FOR NODE 1 AT T=0.08
 *GET,VR1,NODE,1,U,Y
 SET,NEAR,,,,0.48		 !UZ VALUE FOR NODE 1 AT T=0.48
 *GET,VR2,NODE,1,U,Y
@@ -375,14 +377,15 @@
 E,    4,       5
 E,    5,       6
 E,    6,       7
 E,    7,       8
 E,    8,       9
 E,    9,      10
 E,   10,      11
+/OUT,SCRATCH
 EMID,ADD  ! ADD MIDSIDE NODES FOR SHELL209
 FINISH
 SOLVEIT
 PLOTS
 SAVE,TABLE_3
 /CLEAR,NOSTART
 /TITLE,VM218, HYPERELASTICITY TEST: BALLOON/CIRCULAR PLATE PROBLEM
@@ -424,15 +427,14 @@
 OUTRES, ALL, ALL,
 SF,ALL,PRES,50.0
 NEQITR,20
 FINISH
 /SOLUTION
 /OUT,SCRATCH
 SOLVE
-/OUT
 FINISH
 /POST1
 /NOPR		   !SUPPRESS GRAPHING DATA
 /VIEW,1,,-1
 /ANG,1
 /USER
 /FOCUS,1,4,,8,0	   !SET UP CENTER OF GRAPHICS SCREEN FOR DISPLACEMENT PLOT
@@ -520,16 +522,18 @@
 /NOERASE
 NSOL,2,1,U,Z,UZ_1
 PROD,7,1, , ,SH.281 , , ,50,0,0,!MULTIPLY SOLUTION BY 50
 /COLOR,CURVE,MRED
 XVAR,2  		        !SPECIFY X VARIABLE TO BE DISPLAYED
 PLVAR,7 		        !DISPLAY SOLUTION IN GRPH FILE
 /ERASE
+/OUT,
 PRVAR,7,2		        !LIST VARIABLE 7 VERSUS VARIABLE 2
 FINISH
+/OUT,SCRATCH
 /POST1
 /NOPR
 SET,NEAR,,,,0.08		!SELECT UZ VALUE FOR NODE 1 AT T=0.08
 *GET,VR1,NODE,1,U,Z
 SET,NEAR,,,,0.48		!UZ VALUE FOR NODE 1 AT T=0.48
 *GET,VR2,NODE,1,U,Z
 SET,NEAR,,,,0.76		!UZ VALUE FOR NODE 1 AT T=0.76
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm219.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm219.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM219
 /PREP7
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM219, FREQUENCY RESPONSE OF A PRE-STRESSED BEAM USING *EIGEN
 /COM,
 /COM, REFERENCE: " FORMULAS FOR NATURAL FREQUENCY AND MODE SHAPES"
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm22.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm22.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM22
 /PREP7
 /TITLE, VM22, SMALL DEFLECTION OF A BELLEVILLE SPRING
 C*** STR. OF MATL., TIMOSHENKO, PART 2, 3RD ED., PAGE 143, PROB. 2
 ANTYPE,STATIC
 ET,1,SHELL208,,,2
 SECTYPE,1,SHELL
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm221.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm221.dat`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM221
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE,VM221, SIMULATION OF SHAPE MEMORY ALLOY EFFECT
 /COM,   REF: ANGELA C.SOUZA, EDGAR N.MAMIYA, NESTOR ZOUAIN,
 /COM,   "THREE-DIMENSIONAL MODEL FOR SOLIDS UNDERGOING
 /COM,   STRESS-INDUCED PHASE TRANSFORMATIONS"
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm222.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm222.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,vm222
 /TITLE,vm222, Warping Torsion Bar
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 !
 /PREP7
 !
@@ -108,15 +108,16 @@
 SOLVE
 FINISH
 /POST1
 /OUT,
 PRNSOL,DOF
 NSORT,ROT,X 
 *GET,ROTX2,SORT, ,MAX		!GET VERIFIED RESULTS FOR PART 2
-PRRSOL
+PRRSOL,MX
+PRRSOL,BMOM
 PRES,SMISC,4
 PRES,SMISC,17
 PRES,SMISC,27
 T1=ROTX1
 T2=ROTX2
 !
 !SET UP AND FILL VM RATIO TABLE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm223.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm223.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM223
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM223, ELECTRO-THERMAL-COMPLIANT MICROACTUATOR
-/stitle,1,Reason COMPARE differences are acceptable:
-/stitle,2,Convergence Difference
 /COM,
 /COM, REFERENCE:
 /COM, N.D. MANKAME AND G.K. ANANTHASURESH, "COMPREHENSIVE THERMAL MODELLING
 /COM, AND CHARACTERIZATION OF AN ELECTRO-THERMAL-COMPLIANT MICROACTUATOR,"
 /COM, J. MICROMECH. MICROENG., V.11 (2001), PP. 452-462
 /COM,
 /NOPR
@@ -111,14 +109,15 @@
 D,N_VLT,VOLT,VLT
 NSEL,ALL
 
 /COM, === RADIOSITY BOUNDARY CONDITIONS
 SF,ALL,RDSF,0.7,1    ! SURFACE-TO-SURFACE RADIATION LOAD
 SPCTEMP,1,TBLK       ! AMBIENT TEMPERATURE
 STEF,5.6704E-8       ! STEFAN-BOLTZMAN RADIATION CONSTANT, J/(K)4(M)2(S)
+TOFFST,0.            ! OFFSET TEMPERATURE, K
 
 /COM, === TEMPERATURE DEPENDENT CONVECTION BOUNDARY CONDITIONS
 MPTEMP               ! INITIALIZE TEMPERATURE TABLE
 /COM, TEMPERATURE TABLE FOR THERMAL LOADING
 MPTEMP,1,300,500,700,900,1100,1300
 MPTEMP,7,1500
 /COM, === UPPER FACE
@@ -182,19 +181,18 @@
 ASEL,ALL
 MPDATA,HF,8,1,929,1193,1397,1597,1791,1982
 MPDATA,HF,8,7,2176
 FINISH
 
 /SOLU
 ANTYPE,STATIC
-CNVTOL,F,1,1.E-4     ! DEFINE CONVERGENCE TOLERANCES
-CNVTOL,HEAT,1,1.E-5
-CNVTOL,AMPS,1,1.E-5
+CNVTOL,HEAT,1,1.E-6
 NLGEOM,ON            ! LARGE DEFLECTION ANALYSIS
 /OUT,SCRATCH
+NSUB,2
 SOLVE
 FINISH
 
 /POST1
 /DSCALE,1,10
 PLNSOL,U,SUM         ! PLOT DISPLACEMENT VECTOR SUM
 PLNSOL,TEMP          ! PLOT TEMPERATURE
@@ -220,7 +218,9 @@
 /COM,
 *VWRITE,LABEL(1),UYANALYT,UYANSYS,RATIO
 (1X,A10,'     ',E10.4,'    ',E14.4,'     ',1F15.3)
 /COM,-------------------------------------------------------------------
 /OUT
 FINISH
 *LIST,vm223,vrt
+qaend,10
+/exit,nosave
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm224.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm224.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,vm224
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM224, Implicit Creep Under Biaxial Load
 /COM, NAFEMS Fundamental Tests of Creep Behavior, Becker and Hyde
 /NOPR
 /COM,
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm225.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm225.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM225
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM225, BEAM WITH PRETENSION LOAD
-C***    USING 3-D SOLID45
+C***    USING 3-D SOLID185
 /COM,  
 /PREP7					!ENTER PREPROCESSOR
 MP,PRXY,,0.3
 BLOCK,,12,,1,,.5			!CREATE BLOCK
 /VIEW,1,1,2,3				!CHANGE VIEW
-ET,1,SOLID45				!SET ELEMENT TYPE
+ET,1,SOLID185				!SET ELEMENT TYPE
 MP,EX,1,30E6, 				!DEFINE YOUNG'S MODULUS
-MP,PRXY,1,0.3                           !DEFINE POISSON'S RATIO
+MP,PRXY,1,0.3               !DEFINE POISSON'S RATIO
 MP,DENS,1,.283,				!DEFINE DENSITY
-DA,2,SYMM				!DEFINE SYMMETRY BC ON AREA
-DA,3,SYMM				!DEFINE SYMMETRY BC ON AREA
-DA,5,UX					!DEFINE DOF ON AREA
-DA,6,UX					!DEFINE DOF ON AREA
-VMESH,ALL				!MESH VOLUME
+DA,2,SYMM				    !DEFINE SYMMETRY BC ON AREA
+DA,3,SYMM				    !DEFINE SYMMETRY BC ON AREA
+DA,5,UX					    !DEFINE DOF ON AREA
+DA,6,UX				    	!DEFINE DOF ON AREA
+VMESH,ALL			    	!MESH VOLUME
 PSMESH, , ,1000,ALL,,0,X,6,,,,EEE,NNN   !APPLY LOAD VIA PRE-TENSION ELEMENT
 SLOAD,1,PL01,LOCK,FORC,125,1,2
 EPLOT
 SAVE                                    !SAVE DATABASE FOR SECOND SOLUTION                                 
-FINISH					!EXIT PREP7
+FINISH					    !EXIT PREP7
 /out,scratch
-/SOLU					!ENTER SOLVER
-SOLVE					!SOLVE
-FINISH  				!EXIT SOLVER
+/SOLUTION					!ENTER SOLVER
+SOLVE		    			!SOLVE
+FINISH  		    		!EXIT SOLVER
 /out
-*CREATE,RES3D,MAC                       !CREATE MACRO TO RETRIEVE RESULTS
-/POST1 					!ENTER POST PROCESSOR
+*CREATE,RES3D,MAC           !CREATE MACRO TO RETRIEVE RESULTS
+/POST1 				    	!ENTER POST PROCESSOR
 NSORT,S,INT,1,0,,			!SORT STRESS RESULTS
-*GET,MAXNFEA2,SORT,,IMAX		!GET NODE VALUE
+*GET,MAXNFEA2,SORT,,IMAX	!GET NODE VALUE
 *GET,SIGFEA2,NODE,MAXNFEA2,S,INT	!GET MAXIMUM VON MISSES STRESS
-NSORT,U,X,SUM,1,0,,,			!SORT DEFLECTION RESULTS
-*GET,MAXNFEA2,SORT,,IMAX		!GET NODE VALUE
+NSORT,U,X,SUM,1,0,,,		!SORT DEFLECTION RESULTS
+*GET,MAXNFEA2,SORT,,IMAX	!GET NODE VALUE
 *GET,UXFEA2,NODE,MAXNFEA2,U,X,SUM	!GET MAXIMUM UX VALUE
 *STAT,UXFEA2				!LIST PARAMETER VALUE
 *STAT,SIGFEA2				!LIST PARAMETER VALUE
 /COM,**********************************
 /COM,*** CLASSICAL ANALYSIS RESULTS ***
 /COM,**********************************
 SIGCA = 250
@@ -52,45 +52,45 @@
 FINISH
 *END
 RES3D                                   !EXECUTE MACRO TO RETRIEVE RESULTS
 SAVE,TABLE_1
 
 /CLEAR, NOSTART                         !CLEAR DATABASE FOR SECOND SOLUTION
 /TITLE, VM225, BEAM WITH PRETENSION LOAD
-C***    USING 3-D SOLID185 
+C***    USING 3-D SOLID186 
 /PREP7
 RESUME                                  !RESUME DATABASE
-ET,1,SOLID185                           !ANALYZE AGAIN USING 3-D SOLID185 
+ET,1,SOLID186                           !ANALYZE AGAIN USING 3-D SOLID186 
 FINISH                                  !EXIT PREP7
 /out,scratch
-/SOLU					!ENTER SOLVER
-SOLVE					!SOLVE
-FINISH  				!EXIT SOLVER
+/SOLUTION           					!ENTER SOLVER
+SOLVE					                !SOLVE
+FINISH  				                !EXIT SOLVER
 /out
 RES3D                                   !EXECUTE MACRO TO RETRIEVE RESULTS
 SAVE,TABLE_2
 
 /NOPR
 RESUME,TABLE_1
 /GOPR
 /OUT,vm225,vrt
 /COM
 /COM,------------------- VM225 RESULTS COMPARISON ---------------------
 /COM,
 /COM,          |   TARGET   |    Mechanical APDL    |    RATIO
 /COM,
-/COM, SOLID45
+/COM, SOLID185
 /COM,
 *VWRITE,LABEL(1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,'   ',F10.5,'   ',F14.5,'     ',1F15.3)
 /NOPR
 RESUME,TABLE_2
 /GOPR
 /COM,
-/COM, SOLID185
+/COM, SOLID186
 /COM,
 *VWRITE,LABEL(1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,'   ',F10.5,'   ',F14.5,'     ',1F15.3)
 /COM,----------------------------------------------------------------
 /OUT
 FINISH
 *LIST,vm225,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm226.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm294.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,vm226
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,vm294
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/TITLE,VM226, FOURIER SERIES ANALYSIS OF A DIODE RECTIFIED CIRCUIT
+/TITLE,VM294, FOURIER SERIES ANALYSIS OF A DIODE RECTIFIED CIRCUIT
 /COM, REF: SEDRA/SMITH "MICROELECTRONIC CIRCUITS 4TH ED." SEC. 3.7
 /COM,
 /COM   FIRST PART: NO CAPACITANCE
 /COM
 PI = 4*ATAN(1)
 R1=2500                         ! RESISTOR VALUE
 OMEGA=2*PI*60
@@ -47,16 +47,16 @@
 TYPE,2
 REAL,2
 MAT,1
 E,4,5                         !CREATE 2500 OHM RESISTOR
 !
 ! THE FOLLOWING COMMANDS ARE USED TO SET UP THE IDEAL DIODE
 !
-ET,3,125,
-R,3
+ET,3,125
+R,3,,,,1.e-6,,1.e+8
 TYPE,3
 REAL,3
 E,1,4
 !
 ! APPLY GROUND TO CIRCUIT
 !
 D,2,VOLT,0
@@ -72,28 +72,29 @@
 /SOLU
 ANTYPE,TRANS
 OUTRES,ALL,ALL,
 TIME,0.025
 AUTOTS,-1
 DELTIM,0.0001, , ,1
 CNVTOL,VOLT,,0.0001,2,1.0E-6    !CONVERGANCE CRITERIA
+CNVTOL,AMPS,1,1.E-2   		!CONVERGANCE CRITERIA
 /OUT,SCRATCH
 SOLVE
 /OUT
 FINISH
 
 
 /POST26
 NSOL,2,4,VOLT,,
 
 /COLOR,CURVE,BLUE,1
-/TITLE,VM226, LOAD VOLTAGE WAVEFORM WITH NO CAPACITANCE
+/TITLE,VM294, LOAD VOLTAGE WAVEFORM WITH NO CAPACITANCE
 /AXLAB,Y,OUTPUT POTENTIAL (VOLT)
 PLVAR,2,
-/TITLE,VM226, FOURIER SERIES ANALYSIS OF A DIODE RECTIFIED CIRCUIT
+/TITLE,VM294, FOURIER SERIES ANALYSIS OF A DIODE RECTIFIED CIRCUIT
 !
 ! SET UP TABLE ARRAYS TO DISPLAY OUTPUT RESULTS
 !
 *DIM,VOLTG,TABLE,251
 *DIM,TARGET,ARRAY,251
 *DO,INC,1,251,1
   T = INC*0.0001
@@ -225,33 +226,34 @@
 /SOLU
 ANTYPE,TRANS
 OUTRES,ALL,ALL,
 TIME,0.025
 AUTOTS,-1
 DELTIM,0.0001, , ,1
 CNVTOL,VOLT,,0.0001,2,1.0E-6    !CONVERGANCE CRITERIA
+CNVTOL,AMPS,1,1.E-1    !CONVERGANCE CRITERIA
 /OUT,SCRATCH
 SOLVE
 /OUT
 FINISH
 /POST26
 NSOL,2,4,VOLT,,
 /COLOR,CURVE,BLUE,1
 *IF,CAP,EQ,1,THEN
-/TITLE,VM226, VLOAD WITH CAPACITANCE OF 1E-6F
+/TITLE,VM294, VLOAD WITH CAPACITANCE OF 1E-6F
 *ENDIF
 *IF,CAP,EQ,2,THEN
-/TITLE,VM226, VLOAD WITH CAPACITANCE OF 10E-6F
+/TITLE,VM294, VLOAD WITH CAPACITANCE OF 10E-6F
 *ENDIF
 *IF,CAP,EQ,3,THEN
-/TITLE,VM226, VLOAD WITH CAPACITANCE OF 1E-3F
+/TITLE,VM294, VLOAD WITH CAPACITANCE OF 1E-3F
 *ENDIF
 /AXLAB,Y,OUTPUT POTENTIAL (VOLT)
 PLVAR,2,
-/TITLE,VM226, FOURIER SERIES ANALYSIS OF A DIODE RECTIFIED CIRCUIT
+/TITLE,VM294, FOURIER SERIES ANALYSIS OF A DIODE RECTIFIED CIRCUIT
 !
 ! DETERMINE T0
 !
 T0=1/OMEGA*ATAN(1/(OMEGA*TAU))
 !
 ! DETERMINE T0' : MACRO TO DO A BISECTION BETWEEN THE TWO CURVES
 !
@@ -402,17 +404,17 @@
 RESUL(I,3*CAP+1)=COEFF(I)
 RESUL(I,3*CAP+3)=RESUL(I,3*CAP+2)/RESUL(I,3*CAP+1)
 *ENDDO
 *ENDDO
 !
 ! DISPLAY RESULTS
 !
-/OUT,vm226,vrt
+/OUT,vm294,vrt
 /COM
-/COM,------------------- VM226 RESULTS COMPARISON -------------------------
+/COM,------------------- VM294 RESULTS COMPARISON -------------------------
 /COM
 *VWRITE,TAUARR(1,1)
 ('                   TAU=0                       TAU=',F8.4)
 /COM
 /COM     Mechanical APDL    TARGET     RATIO  |  Mechanical APDL    TARGET    RATIO
 /COM     ----------------------------------------------------------------------------
 *VWRITE,COEFFOU(1),RESUL(1,1),RESUL(1,2),RESUL(1,3),RESUL(1,4),RESUL(1,5),RESUL(1,6)
@@ -427,10 +429,8 @@
 /COM     ------------------------------------------------------------------
 *VWRITE,COEFFOU(1),RESUL(1,7),RESUL(1,8),RESUL(1,9)
 (A5,'| ',3F11.4,' |',3F13.4)
 /COM
 /COM,------------------------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm226,vrt
-
-
+*LIST,vm294,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm227.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm227.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM227
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM227, Radiation Between Finite Coaxial Cylinders
 /COM,* EXPECTED RESULTS:
 ! RESULTS DERIVED FROM MODEST, RADIATIVE HEAT TRANSFER, P.791
 ! VIEW FACTOR EVALUATIONS 44, 45
@@ -26,15 +26,15 @@
 SFL,2,RDSF,1, ,1,
 SFL,8,RDSF,1, ,1,
 FINISH  
 /AUX12    
 STEF,0.119E-10                      !SET STEFAN-BOLTZMAN CONSTANT FOR MODEL
 hemiopt,,,,,,,,,,,,,,,,,,,0
 TOFFST,100                          !SET TEMPERATURE OFFSET
-RADOPT,0.1,0.1,2,1000,0.1,0.1  !SET RADIOSITY OPTIONS
+RADOPT,,0.1,2,1000,0.1,0.1  !SET RADIOSITY OPTIONS
 SPCTEMP,1,0.E+00                    !SET TEMPERATURE FOR RADIATION TO SPACE
                                     !(NO RADIATION WILL APPEAR IN THIS MODEL)
 HEMIOPT,1000,0.01  !SET HEMICUBE OPTIONS
 V2DOPT,1,NDIV,0.E+00,200            !SET 2D CALCULATIONS TO AXISYMMETRIC
 VFOPT,NEW   
 !VFCALC   !CALCULATE RADIOSITY VIEW FACTORS
 ASEL,S, , ,       1 
@@ -70,11 +70,7 @@
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F8.3,'  ',F14.3,'   ',1F17.2)
 /COM,-----------------------------------------------------------
 /OUT
 FINISH
 *LIST,vm227,vrt
 
-
-
-
-
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm229.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm229.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM229
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM229, FRICTION HEATING OF A SLIDING BLOCK
 /COM, REF: WRIGGER AND MIEHE, COMP METH APPL ENGR 113, PP301-319
+/OUT,SCRATCH
 /PREP7
 ET,1,PLANE13,4							! 2-D COUPLED-FIELD SOLID
 RECT,,5,,1.25
 RECT,,1.25,1.25,2.5
 LESIZE,ALL,0.25, , ,1,1
 AMESH,ALL
 UIMP,1,EX, , ,70000,
 UIMP,1,DENS, , ,2.7E-9,
 UIMP,1,ALPX, , ,23.86E-6,
 UIMP,1,NUXY, , ,0.3,
 UIMP,1,MU, , ,0.2,
 UIMP,1,KXX, , ,150,
 UIMP,1,C, , ,9E8,
-TOFFSET,460
-TUNIF = 0.00
+TOFFST,460
+TUNIF,0.00
 ET,2,TARGE169						! 2-D TARGET SEGMENT
-ET,3,CONTA171						! 2-D SURFACE-TO-SURFACE CONTACT
+ET,3,CONTA172						! 2-D 3-NODE SURFACE-TO-SURFACE CONTACT
 KEYOPT,3,1,1
 ASEL,S,,,1
 NSLA,S,1
 NSEL,R,LOC,Y,1.25
 R,1
 TYPE,2
 ESURF
@@ -78,39 +79,41 @@
 /POST1
 ALLSEL
 PLNSOL,TEMP
 /COM  *****************************************************************
 /COM   TEST FROM COMP. METH. APPL. MECH. ENG. VOL.113,P301,1994
 /COM   SOLUTION TEMPERATURE = 1.235
 /COM  *****************************************************************
-ESEL,S,ENAME,,CONTA171
+ESEL,S,ENAME,,CONTA172
 NSLE
 PRNSOL,TEMP
 *GET,TEMP1,NODE,130,TEMP
 /COM  *****************************************************************
 /COM   SOLUTION TEMPERATURE = 0.309
 /COM  *****************************************************************
 ESEL,S,ENAME,,TARGE169
 NSLE
 PRNSOL,TEMP
+/OUT,
 *GET,TEMP2,NODE,40,TEMP
 *DIM,LABEL,CHAR,2
 *DIM,VALUE,,2,3
 LABEL(1) = 'TEMP1','TEMP2 '
 *VFILL,VALUE(1,1),DATA,1.235,0.309
 *VFILL,VALUE(1,2),DATA,TEMP1,TEMP2
 *VFILL,VALUE(1,3),DATA,ABS(TEMP1 / 1.235) ,ABS(TEMP2 / 0.309)
 SAVE,TABLE_1
 FINISH
 
-!* SOLVE USING K(2)=3 OF CONTA171
+!* SOLVE USING K(2)=3 OF CONTA172
+/OUT,SCRATCH
 RESUME
 /PREP7
 KEYOPT,3,4,2						! ON NODAL POINT - NORMAL TO TARGET SURFACE
-KEYOPT,3,2,4						! PURE LAGRANGE MULTIPLIER ON CONTACT NORMAL AND TANGENT
+KEYOPT,3,2,3						! PURE LAGRANGE MULTIPLIER ON CONTACT NORMAL AND PENALTY ON TANGENT
 FINISH
 /SOLU
 NSUB,1
 ASEL,S,,,2
 NSLA,S,1
 NSEL,R,LOC,X,1.25
 D,ALL,UX,3.75
@@ -142,55 +145,58 @@
 /POST1
 ALLSEL
 PLNSOL,TEMP
 /COM  *****************************************************************
 /COM   TEST FROM COMP. METH. APPL. MECH. ENG. VOL.113,P301,1994
 /COM   SOLUTION TEMPERATURE = 1.235
 /COM  *****************************************************************
-ESEL,S,ENAME,,CONTA171
+ESEL,S,ENAME,,CONTA172
 NSLE
 PRNSOL,TEMP
 *GET,TEMP1,NODE,130,TEMP
 /COM  *****************************************************************
 /COM   SOLUTION TEMPERATURE = 0.309
 /COM  *****************************************************************
 ESEL,S,ENAME,,TARGE169
 NSLE
 PRNSOL,TEMP
+/OUT,
 *GET,TEMP2,NODE,40,TEMP
 *DIM,LABEL,CHAR,2
 *DIM,VALUE,,2,3
 LABEL(1) = 'TEMP1','TEMP2 '
 *VFILL,VALUE(1,1),DATA,1.235,0.309
 *VFILL,VALUE(1,2),DATA,TEMP1,TEMP2
 *VFILL,VALUE(1,3),DATA,ABS(TEMP1 / 1.235) ,ABS(TEMP2 / 0.309)
 SAVE,TABLE_2
 FINI
 /COM,
 /COM, -------------------------
 /COM,  USING PLANE 223 ELEMENT
 /COM, ------------------------
 /CLEAR,NOSTART
+/OUT,SCRATCH
 /PREP7
 ET,1,PLANE223,11							! 2-D STRUCTURAL-THERMAL SOLID
+KEYOPT,1,9,1
 RECT,,5,,1.25
 RECT,,1.25,1.25,2.5
 LESIZE,ALL,0.25, , ,1,1
 AMESH,ALL
 UIMP,1,EX, , ,70000,
 UIMP,1,DENS, , ,2.7E-9,
 UIMP,1,ALPX, , ,23.86E-6,
 UIMP,1,NUXY, , ,0.3,
 UIMP,1,MU, , ,0.2,
 UIMP,1,KXX, , ,150,
 UIMP,1,C, , ,9E8,
-TOFFSET,460
-TUNIF = 0.00
+TOFFST,460
+TUNIF,0.00
 ET,2,TARGE169								! 2-D TARGET SEGMENT
-ET,3,CONTA172								! 2-D SURFACE-TO-SURFACE CONTACT
+ET,3,CONTA172								! 2-D 3-NODE SURFACE-TO-SURFACE CONTACT
 KEYOPT,3,1,1
 ASEL,S,,,1
 NSLA,S,1
 NSEL,R,LOC,Y,1.25
 R,1
 TYPE,2
 ESURF
@@ -227,15 +233,14 @@
 TIMINT,OFF,STRUC
 TINTP,,,,1.0
 NLGEOM,ON
 TIME,3.75E-3
 AUTO,ON
 NSUB,100,10000,100
 OUTRES,ALL,-10
-NROP,UNSYM
 /OUT,SCRATCH
 SOLVE
 TIME,1
 AUTO,ON
 TINTP,,,,1.0
 NSUB,100,10000,10
 OUTRES,ALL,LAST
@@ -255,14 +260,15 @@
 *GET,TEMP1,NODE,NODE(0.5,1.25,0),TEMP
 /COM  *****************************************************************
 /COM   SOLUTION TEMPERATURE = 0.309
 /COM  *****************************************************************
 ESEL,S,ENAME,,TARGE169
 NSLE
 PRNSOL,TEMP
+/OUT,
 *GET,TEMP2,NODE,NODE(1.75,1.25,0),TEMP
 *DIM,LABEL,CHAR,2
 *DIM,VALUE,,2,3
 LABEL(1) = 'TEMP1','TEMP2 '
 *VFILL,VALUE(1,1),DATA,1.235,0.309
 *VFILL,VALUE(1,2),DATA,TEMP1,TEMP2
 *VFILL,VALUE(1,3),DATA,ABS(TEMP1 / 1.235) ,ABS(TEMP2 / 0.309)
@@ -284,15 +290,15 @@
 /COM,
 /COM,
 /OUT,
 RESUME,TABLE_2
 /OUT,vm229,vrt,,APPEND
 /COM,
 /COM, ----------------------------------
-/COM,  RESULTS USING K(2)=3 OF CONTA171
+/COM,  RESULTS USING K(2)=3 OF CONTA172
 /COM, ----------------------------------
 /COM,
 *VWRITE,LABEL(1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,'  ',F7.4,'      ',F14.4,'     ',1F15.3)
 /COM,
 /COM,
 /OUT,
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm23.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm23.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM23
 /PREP7
 /TITLE, VM23, THERMAL-STRUCTURAL CONTACT OF TWO BODIES
 /COM
 /COM,  SOLVING USING PLANE13 ELEMENTS
 /COM,
 ET,1,PLANE13,4,,2        ! COUPLE-FIELD ELEMENT TYPE 
@@ -78,37 +78,38 @@
 *GET,TEMP_C2,NODE,2,TEMP
 SUBSET,3,3               ! READ LOAD STEP 3, SUBSTEP 3 DATA
 ETABLE,REFL
 PRETAB
 *GET,TEMP_C3,ELEM,4,ETAB,HEAT-FLO
 PRNSOL,TEMP
 ALLSEL,ALL
+
 *DIM,LABEL,CHAR,2,2
 *DIM,LABEL_C3,CHAR,1,2
 *DIM,VALUE_C1,,2,3
 *DIM,VALUE_C2,,2,3
 *DIM,VALUE_C3,,1,2
 LABEL(1,1) = 'TEMP AT ','HEAT FLO'
 LABEL(1,2) = 'EA2 (C) ','W (W)   '
 LABEL_C3(1,1) = 'HEAT FLO'
 LABEL_C3(1,2) = 'W (W)   '
-*VFILL,VALUE_C1(1,1),DATA,539,2439    
+*VFILL,VALUE_C1(1,1),DATA,539.02,2439.02    
 *VFILL,VALUE_C1(1,2),DATA,TEMP_C1,HEAT_C1
-*VFILL,VALUE_C1(1,3),DATA,ABS(TEMP_C1/539  ) ,ABS( HEAT_C1/2439 )
-*VFILL,VALUE_C2(1,1),DATA,636.6,8536.6
+*VFILL,VALUE_C1(1,3),DATA,ABS(TEMP_C1/539.02  ) ,ABS( HEAT_C1/2439.02 )
+*VFILL,VALUE_C2(1,1),DATA,636.59,8536.59
 *VFILL,VALUE_C2(1,2),DATA,TEMP_C2,HEAT_C2
-*VFILL,VALUE_C2(1,3),DATA,ABS(TEMP_C2/636.6 ) ,ABS( HEAT_C2/8536.6)
+*VFILL,VALUE_C2(1,3),DATA,ABS(TEMP_C2/636.59 ) ,ABS( HEAT_C2/8536.59 )
 *VFILL,VALUE_C3(1,1),DATA,0
 *VFILL,VALUE_C3(1,2),DATA,TEMP_C3
 SAVE,TABLE_1
 FINISH
 /CLEAR,NOSTART
 
 /COM, 
-/COM,  SOLVING USING PLANE233 ELEMENT WITH WEAK COUPLING BETWEEN U AND TEMP DOF
+/COM,  SOLVING USING PLANE223 ELEMENT WITH WEAK COUPLING BETWEEN U AND TEMP DOF
 /COM,
 
 /PREP7
 ET,1,PLANE223,11,1       ! COUPLE-FIELD ELEMENT TYPE, WEAK COUPLING
 ET,2,CONTA175,1          ! CONTACT ELEMENT TYPE 
 ET,3,TARGE169            ! TARGET ELEMENT TYPE
 MP,EX,1,10E6             ! YOUNG'S MODULUS
@@ -139,14 +140,15 @@
 ESURF
 ALLSEL
 !      APPLY INITIAL BOUNDARY CONDITIONS
 D,1,UY,,,4,1
 D,1,UX,,,5,4
 D,4,UX,,,8,4
 TREF,100
+ERESX,YES
 FINISH
 /SOLU
 NLGEOM,ON                ! LARGE DEFLECTION EFFECTS TURNED ON
 D,1,TEMP,500,,5,4
 D,3,TEMP,100,,4
 D,7,TEMP,100,,8
 /OUT,SCRATCH
@@ -158,15 +160,15 @@
 SOLVE                    ! SECOND LOAD STEP
 D,4,TEMP,100,,8,4
 SOLVE                    ! THIRD LOAD STEP
 FINISH
 
 /POST1
 /OUT,
-INRES,NSOL,MISC          ! RETRIEVE NODAL AND MISCELLANEOUS DATA
+INRES,NSOL,MISC,EPEL,EPTH      ! RETRIEVE NODAL, MISCELLANEOUS, AND STRAIN DATA
 SUBSET,2,2               ! READ LOAD STEP 2, SUBSTEP 2 DATA 
 ESEL,S,,,3,4
 ETABLE,HEAT-FLO,SMISC,14 ! STORE HEAT FLOWS FOR CONTACT ELEMENTS
 SSUM
 *GET,HEAT_C1B,SSUM,,ITEM,HEAT-FLO
 NSEL,S,,,2,6,4 
 PRNSOL,TEMP
@@ -180,75 +182,73 @@
 *GET,TEMP_C2B,NODE,2,TEMP
 SUBSET,3,3               ! READ LOAD STEP 3, SUBSTEP 3 DATA
 ETABLE,REFL
 PRETAB
 *GET,TEMP_C3B,ELEM,4,ETAB,HEAT-FLO
 PRNSOL,TEMP
 ALLSEL,ALL
+
 *DIM,LABEL,CHAR,2,2
 *DIM,LABEL_C3,CHAR,1,2
 *DIM,VALUE_C1,,2,3
 *DIM,VALUE_C2,,2,3
 *DIM,VALUE_C3,,1,2
 LABEL(1,1) = 'TEMP AT ','HEAT FLO'
 LABEL(1,2) = 'EA2 (C) ','W (W)   '
 LABEL_C3(1,1) = 'HEAT FLO'
 LABEL_C3(1,2) = 'W (W)   '
-*VFILL,VALUE_C1(1,1),DATA,539,2439    
+*VFILL,VALUE_C1(1,1),DATA,539.01,2450.64    
 *VFILL,VALUE_C1(1,2),DATA,TEMP_C1B,HEAT_C1B
-*VFILL,VALUE_C1(1,3),DATA,ABS(TEMP_C1B/539  ) ,ABS( HEAT_C1B/2439 )
-*VFILL,VALUE_C2(1,1),DATA,636.6,8536.6
+*VFILL,VALUE_C1(1,3),DATA,ABS(TEMP_C1B/539.01  ) ,ABS( HEAT_C1B/2450.64 )
+*VFILL,VALUE_C2(1,1),DATA,636.65,8588.71
 *VFILL,VALUE_C2(1,2),DATA,TEMP_C2B,HEAT_C2B
-*VFILL,VALUE_C2(1,3),DATA,ABS(TEMP_C2B/636.6 ) ,ABS( HEAT_C2B/8536.6)
+*VFILL,VALUE_C2(1,3),DATA,ABS(TEMP_C2B/636.65 ) ,ABS( HEAT_C2B/8588.71 )
 *VFILL,VALUE_C3(1,1),DATA,0
 *VFILL,VALUE_C3(1,2),DATA,TEMP_C3B
 SAVE,TABLE_2
 FINISH
 RESUME,TABLE_1
 /COM
+/NOPR
 /OUT,vm23,vrt
 /COM,------------------- VM23 RESULTS COMPARISON ---------------------
 /COM,
-/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
+/COM,                   |    TARGET    |   Mechanical APDL   |   RATIO
 /COM,
 /COM,
 /COM,  USING PLANE13 ELEMENTS
 /COM,
 /COM,TEMP AT EB2 = 600 C:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE_C1(1,1),VALUE_C1(1,2),VALUE_C1(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
+(1X,A8,A8,'   ',F11.2,'  ',F15.2,'   ',1F15.3)
 /COM,
 /COM,TEMP AT EB2 = 850 C:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE_C2(1,1),VALUE_C2(1,2),VALUE_C2(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
+(1X,A8,A8,'   ',F11.2,'  ',F15.2,'   ',1F15.3)
 /COM,
 /COM,TEMP AT EB2 = 100 C:
 *VWRITE,LABEL_C3(1,1),LABEL_C3(1,2),VALUE_C3(1,1),VALUE_C3(1,2)
-(1X,A8,A8,'   ',F10.1,'  ',F10.1)
+(1X,A8,A8,'   ',F11.1,'  ',F11.1)
 /COM,
-/COM,
-/NOPR
 RESUME,TABLE_2
-/GOPR,
-/COM,
-/COM,
 /COM,
-/COM, USING PLANE233 ELEMENTS
+/COM, USING PLANE223 ELEMENTS
 /COM,
 /COM,TEMP AT EB2 = 600 C:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE_C1(1,1),VALUE_C1(1,2),VALUE_C1(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
+(1X,A8,A8,'   ',F11.2,'  ',F15.2,'   ',1F15.3)
 /COM,
 /COM,TEMP AT EB2 = 850 C:
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE_C2(1,1),VALUE_C2(1,2),VALUE_C2(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
+(1X,A8,A8,'   ',F11.2,'  ',F15.2,'   ',1F15.3)
 /COM,
 /COM,TEMP AT EB2 = 100 C:
 *VWRITE,LABEL_C3(1,1),LABEL_C3(1,2),VALUE_C3(1,1),VALUE_C3(1,2)
-(1X,A8,A8,'   ',F10.1,'  ',F10.1)
+(1X,A8,A8,'   ',F11.2,'  ',F11.2)
 /COM,
 /COM,-----------------------------------------------------------------
 /OUT
 FINISH
 *LIST,vm23,vrt
 /delete,TABLE_1
 /delete,TABLE_2
+/exit,nosave
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm231.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm231.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,vm231
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE, VM231, PIEZOCERAMIC RECTANGLE UNDER PURE BENDING LOAD
 /COM,   REF: PARTON,V.Z., KUDRYAVTSEV, B.A. AND SENIK,N.A. (1989)
 /COM,   "MECHANICS OF PIEZOELECTRIC MATERIALS" IN "APPLIED MECHANICS:
 /COM,   SOVIET REVIEW.", Vol.2: ELECTROMAGNETOELASTICITY,
@@ -256,7 +256,8 @@
 /COM,
 /COM,---------------------------------------------------------------------
 /out,
 *list,vm231,vrt
 FINISH
 /delete,table_1
 /delete,table_2
+/exit,nosave
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm233.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm233.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM233
 /TITLE,VM233, STATIC FORCE COMPUTATION OF A 3D SOLENOID ACTUATOR
-/STITLE,1,Reason COMPARE differences are acceptable:
-/STITLE,2,  No of nodes/elements affect accuracy
 /COM, REFERENCE: ANALYSIS OF BENCHMARK PROBLEM TEAM20 WITH VARIOUS
 /COM,            FORMULATION, PROCEEDINGS OF TEAM WORKSHOP,COMPUMAF RIO
 /COM,		     PG 18-20,1997.
 /COM,		     IEEE TRANS. ON MAG, VOL. 34. NO. 5. PG 2481-84,1998
 /COM,		     IEEE TRANS. ON MAG, VOL. 35. NO. 3. PG 1406-84,1998
 /COM,		     ANALYSIS SOLUTIONS, VOL.1. ISSUE 2,WINTER 1997-98,PG 10-11. 
 /COM
 /PREP7
 /NOPR
 /OUT,SCRATCH
+_GEOMGEN = 0                    ! SET THIS TO 1 TO GENERATE CDB FILE
+_EXIT = 0                       ! SET THIS TO 1 TO EXIT WITHOUT SOLVING
+*IF,_GEOMGEN,EQ,1,THEN
 ET,1,SOLID98,10
 MP,MURX,1,1
 MP,MURX,4,1
 
 TB,BH,2,,40
 TBPT,,355,.7
 ,,405,.8
@@ -93,47 +94,68 @@
 
 ALLSEL,ALL
 SMRT,10
 MSHAPE,1,3D
 MSHMID,1
 MSHKEY,0
 VMESH,ALL
+ALLSEL,ALL
+CDWRITE,ALL,VM233,CDB,,VM233,IGES
+
+*IF,_EXIT,EQ,1,THEN
+/EXIT,NOSAVE
+*ENDIF
+
+*ELSE
+CDREAD,ALL,VM233,CDB,,VM233,IGES
+*ENDIF
+FINISH  
 
+/PREP7
 ESEL,S,MAT,,3      				! ARMATURE
 CM,ARM,ELEM
-FMAGBC,'ARM'
+NSLE
+BF,ALL,MVDI,1
 ALLSEL,ALL
-
 VLSCALE,ALL,,,.001,.001,.001,,0,1     	! SCALE TO METERS
-
 LOCAL,12,0,0,0,75/1000
 WPCSYS,-1
 RACE,.0285,.0285,.014,TCUR,.018,.0966     ! CREATE COIL
 SAVE
-FINISH  
-/SOLU
+
+
+/SOLUTION
 NSLE,S
 *GET,NMIN,NODE,,NUM,MIN
 D,NMIN,MAG,0
 NSEL,ALL
 EQSLV,JCG
 MAGSOLV,3,,,,,1
 FINISH
 
 /POST1
-/OUT
 *MSG,NOTE,TCUR
-%/RESULTS FOR CURRENT = %G (MULTIPLY ORCE BY 4 FOR SYMMETRY)
-FMAGSUM,'ARM'
-*GET,FVWZ,SSUM, ,ITEM,FVW_Z     		! EXTRACT VIRTUAL FORCE Z DIRECTION
-FZ = 4*FVWZ                     		! SCALE FORCE FOR SYMMETRY
+%/RESULTS FOR CURRENT = %G (MULTIPLY FORCE BY 4 FOR SYMMETRY)
+
+ESEL,S,MAT,,3
+NSLE
+ESLN
+ESEL,U,MAT,,3
+ETABLE,FVWZ,NMISC,6
+SSUM
+*GET,_FZSUM,SSUM,,ITEM,FVWZ
+ALLSEL
+
+FZ = 4*_FZSUM                     		! SCALE FORCE FOR SYMMETRY
 ESEL,S,MAT,,2,3
 NSLE,S
 NSEL,A,NODE,,1,2
-LPATH,1,2
+PATH,P1,2,,48                           ! SETUP PATH - NODES 1, 2
+PPATH,1,1
+PPATH,2,2
 PDEF,BZ,B,Z
 PRPATH,BZ
 *GET,BZPOLE,PATH,0,LAST,BZ      		! EXTRACT BZ AT POLE
 *GET,BZARM,PATH,0,MAX,BZ        		! EXTRACT BZ at ARM
 *DIM,LABEL,CHAR,3
 *DIM,VALUE,,3,3
 LABEL(1) = 'FVW(Z) ','POLE(BZ) ','ARM(BZ) '
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm234.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm234.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,vm234
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM234, CYCLIC LOADING ON RUBBER BLOCK
 /COM, REFERENCE: HOLZAPFEL, GERHARD A. " ON LARGE STRAIN VISCOELASTICITY:
 /COM,		     CONTINUUM, FORMULATION AND FINITE ELEMENT APPLICATIONS TO
 /COM,		     ELASTOMERIC STRUCTURES", INTERNATIONAL JOURNAL FOR NUMERICAL
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm235.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm235.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM235
 /PREP7
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM235, FREQUENCY RESPONSE OF A PRE-STRESSED BEAM
 /COM,
 /COM, REFERENCE: " FORMULAS FOR NATURAL FREQUENCY AND MODE SHAPES"
@@ -90,15 +90,15 @@
 /out
 /POST1
 FINISH
 
 /SOLUTION
 ANTYP,MODAL
 MODOPT,UNSYM,3   			! EXTRACT 3 MODES
-MXPAND
+MXPAND,,,,YES
 PSTRES,ON
 SOLVE
 FINISH
 /POST1
 /NOPR						! SETUP RESULTS TABLE DATA
 SET,1,1
 PLDISP,1					! PLOT MODE SHAPE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm236.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm236.dat`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM236
 /TITLE,VM236,HYSTERESIS LOOP VERIFICATION OF A CLAMPED BEAM
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /COM, ------------------------------------------------------
 /COM,          2D BEAM UNDER ELECTROSTATIC LOAD
 /COM,          --------------------------------
@@ -42,15 +42,15 @@
 !---------------------- Model ---------------
 
 /PREP7
 
 EMUNIT,EPZRO,EPS0
 
 ET,1,182,3,,2
-ET,2,223,1001,,,1  
+ET,2,223,1001,1,,1   ! force coupling 
 ET,3,178,,1
 
 MP,EX,1,169E3
 MP,NUXY,1,0.25
 MP,PERX,2,1
 MP,EX,2,1E-5
 MP,NUXY,2,0.0
@@ -68,24 +68,25 @@
 AATT,1,,1
 ASEL,INVERT
 AATT,2,1,2
 CM,AREA1,AREA
 
 ALLS
 ESIZE,ESIZE
-MSHMID,2
 
 ASEL,S,MAT,,1
-MSHAPE,0,2
+MSHAPE,0,2D
 MSHKEY,2
 AMESH,ALL
 
-ASEL,S,MAT,,2
-MSHAPE,1,2
-MSHKEY,1
+ASEL,S,MAT,,2         ! "ELASTIC AIR" 
+MSHA,0,2D
+MSHMID,2              ! MESH WITHOUT MIDSIDE NODES
+LSEL,S,,,9,10
+LESIZE,ALL,,,1        ! ONE ELEMENT THROUGH LAYER
 AMESH,ALL
 
 TYPE,3				! GAP ELEMENT MESH
 MAT,3
 REAL,2
 *GET,NOMAX,NODE,0,NUM,MAX
 KN=BL/ESIZE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm237.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm237.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM237
 /TITLE,VM237, PIEZOELECTRIC-CIRCUIT ANALYSIS 
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /COM,  ---------------------------------------------------------------
 /COM,     FINITE ELEMENT MODEL OF A PIEZOELECTRIC CIRCULAR PLATE 
 /COM,  ---------------------------------------------------------------
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm238.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm238.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM238
 /TITLE,VM238,WHEATSTONE BRIDGE CONNECTION OF PIEZORESISTORS, UMKSV SYSTEM OF UNITS
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /COM,
 /COM,  GEOMETRIC PARAMETERS:
 /COM,
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm239.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm239.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM239
 /OUT,SCRATCH
 /PREP7
 JPGPRF,500,100,1                     ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /OUT
 /COM
@@ -172,17 +172,15 @@
 ZDIST = L*SIN(ACOS(R/L))
 
 C*** DEFINING ELEMENTS, KEY OPTIONS AND MATERIAL PROPERTIES
 ET,1,BEAM188                         ! BEAM ELEMENTS
 ET,2,MPC184,7                        ! UNIVERSAL JOINT
 ET,3,MPC184,6                        ! REVOLUTE JOINT
 ET,4,MPC184,3                        ! SLIDER
-
-ET,11,TARGE170                       ! TARGET ELEMENT
-KEYOPT,11,2,1                        ! TARGET ELEMENT DEFINED AS RIGID BODY
+et,5,MPC184,1,1                      ! RIGID BEAM WITH LAGRANGE MULTIPLIER REDUCTION METHOD
 
 MP,EX,1,30E6
 MP,PRXY,1,0.33
 MP,DENS,1,10.0
 
 C*** CREATING NODES AND LINK ELEMENTS
 N,1, 0,0,0
@@ -195,46 +193,23 @@
 N,9, 2+COS(ANG),.5+SIN(ANG),0
 N,10, 2+COS(ANG),SIN(ANG),ZDIST
 N,11, 2+COS(ANG),SIN(ANG),.75
 N,12, 2+COS(ANG),SIN(ANG),2.25
 N,13, 2+COS(ANG),SIN(ANG),2.26
 
 ! DEFINE RIGID BODIES
-TYPE,11
-REAL,11
+TYPE,5
 EN,1, 1,2      ! TARGET ELEMENT FOR 1ST RIGID BODY
-REAL, 12
 EN,2, 3,4      ! TARGET ELEMENT FOR 2ND RIGID BODY
-REAL, 13
 EN,3, 6,5
 EN,4, 6,8      ! TARGET ELEMENTS FOR 3RD RIGID BODY
-REAL, 14
 EN,5, 10,9     ! TARGET ELEMENT FOR 4TH RIGID BODY
-REAL, 15
 EN,6, 11, 12   ! TARGET ELEMENT FOR 5TH RIGID BODY 
 EN,101, 12,13
 
-! PILOT NODES FOR RIGID BODIES
-TYPE,11
-REAL,11
-TSHAP,PILO
-EN,11,1       ! PILOT NODE FOR 1ST RIGID BODY
-REAL,12
-TSHAP,PILO
-EN,12,3       ! PILOT NODE FOR 2ND RIGID BODY
-REAL,13
-TSHAP,PILO
-EN,13,5       ! PILOT NODE FOR 3ND RIGID BODY
-REAL,14
-TSHAP,PILO
-EN,14,10       ! PILOT NODE FOR 4TH RIGID BODY
-REAL,15
-TSHAP,PILO
-EN,15,13      ! PILOT NODE FOR 5TH RIGID BODY
-
 ! COORDINATE SYSTEMS FOR JOINTS
 LOCAL,11,0, 0,0,0,-90.0         ! DEFINING LOCAL CSYS FOR UNIV. JOINTS
 LOCAL,12,0, 0,0,0,-45.0
 LOCAL,14,0, 0,0,0, 0,           ! DEFINING LOCAL CSYS FOR REVO. JOINTS
 LOCAL,15,0, 0,0,0, 0,
 
 C*** CREATING UNIVERSAL CONNECTIVITY ELEMENTS
@@ -272,14 +247,17 @@
 TIME, 1.0
 NSUBST, 32, 6400, 32
 D,1,UX,0,,,,UY, UZ
 D, 6, UY, 0.0
 D, 6, UZ, 0.0
 D, 13, UX, 0,,,,UY,UZ,ROTX,ROTY,ROTZ
 D,1,ROTX,2*PI
+D,1,ROTY
+D,1,ROTZ
+D,10,ROTY
 OUTRES, ALL, ALL
 LNSRCH,OFF 
 CNVTOL, F
 CNVTOL, M
 CNVTOL,U 
 CNVTOL,ROT
 SOLVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm24.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm24.dat`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM24
 /PREP7
 /TITLE, VM24, PLASTIC HINGE IN A RECTANGULAR BEAM
 C*** STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PG. 349, ART. 64
 C*** USING BILINEAR KINEMATIC HARDENING PLASTICITY BEHAVIOR TO DESCRIBE  
 C*** THE MATERIAL NONLINEARITY
 ET,1,BEAM188
 SECTYPE,1,BEAM,RECT
 SECDATA,2,1,6,1           ! 2 x 1 CROSS-SECTION USING 6 CELLS THRU THE THICKNESS
 MP,EX,1,30E6
 MP,PRXY,1,0.3
-TB,BKIN,1,1               ! BILINEAR KINEMATIC HARDENING
+TB,PLAS,1,,,BKIN          ! BILINEAR KINEMATIC HARDENING
 TBTEMP,70
 TBDATA,1,36000,0          ! YIELD POINT AND ZERO TANGENT MODULUS
 N,1                       ! DEFINE NODES
 N,2,10
 E,1,2                     ! DEFINE ELEMENT
 D,1,ALL                   ! BOUNDARY CONDITIONS
 DSYM,SYMM,Z               ! 2-DIMENSIONAL MODEL
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm240.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm240.dat`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /VERIFY,VM240
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /TITLE,VM240,THERMAL EXPANSION OF RIGID BEAMS IN A COMPOSITE BAR
 /COM J.M. GERE, S.P. TIMOSHENKO, MECHANICS OF MATERIALS, 2ND EDITION,
 /COM PWS PUBLISHERS, 1984, P. 20-21,71
 /COM
 
 /GRAPH,POWER
 /AUTO
@@ -70,15 +70,14 @@
 E,4,48
 E,5,47
 E,2,46
 
 /SOLU
 ANTYPE,STATIC
 NROPT,FULL
-SOLCON,ON
 NLGEOM,ON
 RESCON,DEFINE,NONE
 OUTRES,ALL,ALL
 AUTOTS,ON
 NSUBST,10,1000,10
 
 NSEL,S,LOC,X,0                ! APPLYING BOUNDARY CONDITIONS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm241.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm241.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 /VERIFY,VM241 
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /TITLE, VM241, TEAM20: 3-D STATIC FORCE PROBLEM
 C*** USING SOLID237
-/stitle,1,Reason COMPARE differences are acceptable:
-/stitle,2,Mesh Difference, Accuracy
 JPGPRF,500,100,1
 /SHOW,JPEG
 /COM
 /COM
 /COM REFERENCE:
 /COM  N.TAKAHASHI,T.NAKATA,H.MORISHIGE,"SUMMARY OF RESULTS FOR 
 /COM, PROBLEM 20 (3-D STATIC FORCE PROBLEM)", COMPEL, VOL.14,1995,PG:57-75
 /NOPR
 SMT=10					     ! SMART SIZING MESHING PARAMETER
 		                             ! COIL PARAMETERS
 TCUR=5000				     ! INPUT CURRENT HERE (AT)
 AREA=(18*96.6)*.001**2			     ! AREA
 CURDEN=TCUR/AREA			     ! CURRENT DENSITY
 
+/OUT,SCRATCH
+
+/COM, GENERATE CDB FILE TO STORE GEOMETRY AND MESH DATA
+
+_GEOMGEN = 0
+_EXIT = 0
+
+*IF,_GEOMGEN,EQ,1,THEN
+
 /PREP7
 ET,1,MESH200,9
 MP,RSVX,4,1E-7
 
 MP,MURX,1,1
 MP,MURX,4,1
 
@@ -100,22 +107,33 @@
 VATT,4,3,1							! COIL +Y THETA
 
 ALLSEL,ALL
 SMRT,SMT							! SMART SIZING MESHING PARAMETER
 MSHKEY,0
 VMESH,ALL
 
-ESEL,S,MAT,,3						! ARMATURE FORCE EXTRACTION
+ESEL,S,MAT,,3						! POLE FORCE EXTRACTION
 CM,ARM,ELEM
 ALLSEL,ALL
 
 VLSCALE,ALL,,,.001,.001,.001,,0,1   ! SCALE TO METERS
 CSYS,0
+ALLSEL,ALL
+cdwrite,db,vm241-1,cdb
 FINISH
 
+*IF,_EXIT,EQ,1,THEN
+/EXIT,NOSAVE
+*ENDIF
+
+*ELSE
+cdread,db,vm241-1,cdb
+*ENDIF
+finish
+
 /COM
 /COM *** CREATE CURRENT DENSITY LOADING IN THE COIL
 /PREP7
 ET,1,SOLID232						! VOLT
 ESEL,S,MAT,,4						! CONDUCTOR
 NSLE
 NSEL,R,LOC,X,0
@@ -193,52 +211,61 @@
 ND=0
 *DO,I,1,NNOD
  ND=NDNEXT(ND)
  *GET,FZ,NODE,ND,FMAG,Z
  _FZSUM=_FZSUM+FZ
 *ENDDO
                                  ! ALTERNATIVELY, ISSUE THE EMFT COMMAND
-!EMFT                            ! MACRO TO SUM UP MAGNETIC FORCES
 
 FMAGZ=_FZSUM                      
 FZ=4*FMAGZ                       ! SCALE FORCE FOR SYMMETRY
 
 ESEL,S,MAT,,2,3
 NSLE,S
 NSEL,A,NODE,,1,2
-LPATH,1,2
+PATH,P1,2,,48                    ! SETUP PATH - NODES 1, 2
+PPATH,1,1
+PPATH,2,2
 /COM
 /COM, PATH RESULTS FOR ARM AND POLE REGIONS
 /COM
 PDEF,BZ,B,Z
 PRPATH,BZ
+/OUT,
 *GET,BZPOLE,PATH,0,LAST,BZ      ! EXTRACT BZ AT POLE
 *GET,BZARM,PATH,0,MAX,BZ        ! EXTRACT BZ AT ARM
 VALUE(1,2)=ABS(FZ)
 VALUE(2,2)=ABS(BZPOLE)
 VALUE(3,2)=ABS(BZARM)
 VALUE(1,3)=ABS(FZ)/VALUE(1,1)
 VALUE(2,3)=ABS(BZPOLE)/VALUE(2,1)
 VALUE(3,3)=ABS(BZARM)/VALUE(3,1)
 *VLEN,3
 SAVE,INF1
 FINISH
 /CLEAR,NOSTART
 
-
-
-
 /TITLE, VM241, TEAM20: 3-D STATIC FORCE PROBLEM
 C*** USING SOLID236
 SMT=10					     ! SMART SIZING MESHING PARAMETER
 		                             ! COIL PARAMETERS
 TCUR=5000				     ! INPUT CURRENT HERE (AT)
 AREA=(18*96.6)*.001**2			     ! AREA
 CURDEN=TCUR/AREA			     ! CURRENT DENSITY
 
+/OUT,SCRATCH
+
+/COM, GENERATE CDB FILE TO STORE GEOMETRY AND MESH DATA
+
+_GEOMGEN = 0
+_EXIT = 0
+
+*IF,_GEOMGEN,EQ,1,THEN
+
+
 /PREP7
 ET,1,SOLID231
 MP,RSVX,4,1E-7
 
 MP,MURX,1,1
 MP,MURX,4,1
 
@@ -318,20 +345,31 @@
 
 ALLSEL,ALL
 SMRT,SMT							! SMART SIZING MESHING PARAMETER
 MSHKEY,0
 MSHAPE,1,3D
 VMESH,ALL
 
-ESEL,S,MAT,,3						! ARMATURE FORCE EXTRACTION
+ESEL,S,MAT,,3						! POLE FORCE EXTRACTION
 CM,ARM,ELEM
 ALLSEL,ALL
 
 VLSCALE,ALL,,,.001,.001,.001,,0,1   ! SCALE TO METERS
 CSYS,0
+ALLSEL,ALL
+cdwrite,db,vm241-2,cdb
+FINISH
+
+*IF,_EXIT,EQ,1,THEN
+/EXIT,NOSAVE
+*ENDIF
+
+*ELSE
+cdread,db,vm241-2,cdb
+*ENDIF
 FINISH
 
 /COM
 /COM *** CREATE CURRENT DENSITY LOADING IN THE COIL
 /PREP7
 ESEL,S,MAT,,4						! CONDUCTOR
 NSLE
@@ -418,20 +456,23 @@
 
 FMAGZ=_FZSUM                      
 FZ=4*FMAGZ                       ! SCALE FORCE FOR SYMMETRY
 
 ESEL,S,MAT,,2,3
 NSLE,S
 NSEL,A,NODE,,1,2
-LPATH,1,2
+PATH,P2,2,,48                    ! SETUP PATH - NODES 1, 2
+PPATH,1,1
+PPATH,2,2
 /COM
 /COM, PATH RESULTS FOR ARM AND POLE REGIONS
 /COM
 PDEF,BZ,B,Z
 PRPATH,BZ
+/OUT,
 *GET,BZPOLE,PATH,0,LAST,BZ      ! EXTRACT BZ AT POLE
 *GET,BZARM,PATH,0,MAX,BZ        ! EXTRACT BZ AT ARM
 VALUE(1,2)=ABS(FZ)
 VALUE(2,2)=ABS(BZPOLE)
 VALUE(3,2)=ABS(BZARM)
 VALUE(1,3)=ABS(FZ)/VALUE(1,1)
 VALUE(2,3)=ABS(BZPOLE)/VALUE(2,1)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm242.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm242.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /verify,vm242
 /title,vm242,Johnson-Champoux-Allard Equivalent Fluid Model
 /com,
 /com, Evaluation of the acoustic and non-acoustic properties
 /com, of sound absorbing materials using a three-microphone
 /com, impedance tube
 /com,
@@ -66,15 +66,16 @@
 vatt,2,2,2
 vsel,all
 esize,DIM_ESIZE
 vmesh,all
 
 asel,s,loc,y,DIM_LENGTH
 nsla,s,1
-bf,all,js,LOADING		! mass source
+!bf,all,js,LOADING		! mass source
+bf,all,mass,LOADING
 sf,all,inf			! Robin radiation boundary flag
 allsel,all
 finish
 
 /solu
 antype,harmic
 harfrq,0,FREQUENCY		
@@ -147,8 +148,9 @@
 /NOPR,
 /com,
 /com, 
 /com, --------------------------------------------------------------------------------
 /out,
 *list,vm242,vrt
 finish
+/exit,nosave
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm243.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm243.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM243
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM243,CANTILEVER BEAM WITH TRIANGULAR LOADING DEFINED BY FUNCTION
 /COM,  REFERENCE: F.P BEER AND E.J. JOHNSTON,JR, MECHANICS OF MATERIALS,
 /COM, 		MCGRAW-HILL, NEW YORK, NY, 1981, PP. 356,366,397,613
 MINLOAD=0					! MINIMUM LOAD
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm244.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm244.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,100 +1,107 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM244         
 /TITLE,VM244, MODAL ANALYSIS OF CYCLIC SYMMETRIC ANNULAR PLATES
 C*** ROBERT D BLEVINS,"FORMULAS FOR NATURAL FREQUENCY AND MODE
 C*** SHAPE", NEW YORK, NY, VAN NOSTRAND REINHOLD PUBLISHING INC
 C*** 1979, PP. 246-247, 286-287  
 _THETA1 = 0	        ! DEGREE, STARTING ANGLE FOR SECTION
 _THETA2 = 30		! DEGREE, ENDING ANGLE FOR SECTION
 _FLOWER = 23.381	! HZ, LOWER FREQUENCY LIMIT PER BLEVINS
 _FREQDIF = 2.1		! PERCENT
-_A = 500		! OUTSIDE RADIUS (MM)
-_B = 185		! INSIDE RADIUS (MM)
-_H = 5			! THICKNESS (MM)
-_E = 70000		! YOUNGS (N/MM^2)
-_V = 0.3		! POISON'S RATIO
-_D = 2.7E-9		! DENSITY AL1100 H14 (NSEC^2/MM^4)
+_A = 500		    ! OUTSIDE RADIUS (MM)
+_B = 185		    ! INSIDE RADIUS (MM)
+_H = 5			    ! THICKNESS (MM)
+_E = 70000		    ! YOUNGS (N/MM^2)
+_V = 0.3		    ! POISON'S RATIO
+_D = 2.7E-9		    ! DENSITY AL1100 H14 (NSEC^2/MM^4)
 *DIM,VALUE,ARRAY,6,3
 *DIM,LABEL,CHAR,6
 LABEL(1)='SOLID185'
 LABEL(2)='SOLID186'
 LABEL(3)='SOLID187'
 LABEL(4)='SHELL181'
 LABEL(5)='SHELL281'
 LABEL(6)='SOLSH190'
+/OUT,SCRATCH
 *DO,I,1,6,1
 *IF,LABEL(I),EQ,'SHELL181',OR,LABEL(I),EQ,'SHELL281',THEN
 C*** CYCSYM MODEL, SIMPLE SUPPORT OUTER EDGE, FREE INNER EDGE,
 C*** SHELL ELEMENT
 /PREP7
 MP,EX,1,_E
 MP,NUXY,1,_V
 MP,DENS,1,_D
 CYL4,0,0,_A,_THETA1,_B,_THETA2
-R,1,_H
+SECTYPE,1,SHELL
+SECDATA,_H,1,0,3
+SECNUM,1
+CYCLIC
 ET,1,LABEL(I)
 AMESH,ALL
+CSYS,1
 NSEL,S,LOC,X,_A
-D,ALL,UY
 NROTAT,ALL
+D,ALL,UY
 D,ALL,UZ
 NSEL,ALL
-CYCLIC
 FINISH
 *ELSE
 C*** CYCSYM MODEL, SIMPLE SUPPORT OUTER EDGE, FREE INNER EDGE
 C*** SOLID ELEMENTS
 /PREP7  
 MP,EX,1,_E
 MP,NUXY,1,_V
 MP,DENS,1,_D
-CSYS,6
-WPCSYS,6
 CYL4,0,0,_A,_THETA1,_B,_THETA2,_H
+CYCLIC
 ET,1,LABEL(I)
 *IF,LABEL(I),EQ,'SOLID185',THEN
 KEYOPT,1,2,3     ! REDUCE STIFFNESS FORMULATION TO MAKE FREQUENCIES MATCH
 *ELSEIF,LABEL(I),EQ,'SOLSH190',THEN
 VEORIENT,1,THIN
 *ENDIF
 VMESH,ALL
-CSYS,4
+CSYS,1
 NSEL,S,LOC,X,_A-.00001,_A+.00001
 NSEL,R,LOC,Z,0
-D,ALL,UY
 NROTAT,ALL
+D,ALL,UY
 D,ALL,UZ
 NSEL,ALL
-CYCLIC
 FINISH
 *ENDIF
-/SOLU
+/SOLUTION
 ANTYPE,2
 MODOPT,LANB,3
 MXPAND,3, , ,1
 MODOPT,LANB,3,1,100000, ,OFF
 CYCOPT,HINDEX,0,0
 SOLVE
 FINISH
 /POST1
+SET,LIST
 *GET,F%I%,MODE,1,FREQ
 /COM,                 FREQUENCY COMPARE FOR ELEMENT %LABEL(I)%
 *IF,(ABS((F%I% - _FLOWER)/_FLOWER))*100,LT,_FREQDIF,THEN
 C*** FREQUENCIES COMPARE WITHIN BLEVINS RESULT!!!
 *ELSE
 C*** FAILURE: FREQUENCIES OUT OF ACCAPTABLE LIMITS!!!
 FINISH
 /EXIT,NOSAVE           ! EXIT DUE TO FAILURE
 *ENDIF
 FINISH
+/PREP7
+CYCLIC,OFF
+FINISH
 PARSAV,ALL
 /CLEAR,NOSTART
 PARRES,
 *ENDDO
+/OUT,
 *VFILL,VALUE(1,1),DATA,_FLOWER,_FLOWER,_FLOWER,_FLOWER,_FLOWER,_FLOWER
 *VFILL,VALUE(1,2),DATA,F1,F2,F3,F4,F5,F6
 *VFILL,VALUE(1,3),DATA,ABS(F1/_FLOWER),ABS(F2/_FLOWER),ABS(F3/_FLOWER),ABS(F4/_FLOWER),ABS(F5/_FLOWER),ABS(F6/_FLOWER)
 /OUT,vm244,vrt
 /COM,------------------- VM244 RESULTS COMPARISON -------------
 /COM,
 /COM,                 |    TARGET   |    Mechanical APDL   |    RATIO
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm245.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm245.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM245
 /TITLE, VM245,SQUEEZE FILM DAMPING-RECTANGULAR PLATE
 /COM, REFERENCE:  COUPLED FLUID-STRUCTURAL DOMAIN SOLVER AND ROM
 /COM,		  EXTRACTION FOR MEMS, J. MEHNER, 1/31/03
 /COM,			BENCHMARK #1: RECTANGULAR PLATE
 /COM,
 /COM,	CHARACTERISTICS:
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm246.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm246.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /VERIFY,VM246         
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /TITLE,VM246, CYCLIC ANALYSIS OF AN END-LOADED HOLLOW CYLINDRICAL CANTILEVER BEAM
 /COM,*************************************************************
 /COM,* PREMISE OF TEST:   TEST UTILIZES THE FUNDAMENTAL FEATURES *
 /COM,*                    OF ANSYS TO VERIFY FEA RESULTS         *
 /COM,*                    TO CALCULATED APPROXIMATION RESULTS    *
 /COM,*************************************************************
 /COM,*************************************************************
@@ -170,13 +170,14 @@
 /COM,*************************************************
 /COM,********* ALL TEST WERE SUCCESSFUL !!! **********
 /COM,*************************************************
 /COM,*************************************************
 FINISH                                    !FINISH
 *LIST,vm246,vrt
 QAEND,23
+/EXIT,NOSAVE                              !EXIT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm247.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm247.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM247
 JPGPRF,500,100,1                                         ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/TITLE, VM247 CAMPBELL DIAGRAMS AND CRITICAL SPEEDS USING SYMMETRIC BEARINGS
+/TITLE, VM247, CAMPBELL DIAGRAMS AND CRITICAL SPEEDS USING SYMMETRIC BEARINGS
 /COM,   REF: "THE DYNAMICS OF ROTOR-BEARING SYSTEMS USING FINITE ELEMENTS"
 /COM,   JOURNAL OF ENG. FOR INDUSTRY - MAY 1976
 /COM
 JPGPRF,500,100,1
 /SHOW,JPEG
 /PREP7
 *DIM,SPIN,,4		                                    ! SPIN VELOCITY (RPM)
@@ -232,7 +232,8 @@
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,12),VALUE(12,1),VALUE(12,2),VALUE(12,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 /COM
 /OUT
 FINISH
 *LIST,vm247,vrt
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm248.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm248.dat`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM248
 /SHOW,JPEG
 JPGPRF,500,100,1           !* MACRO TO SET PREFS FOR JPEG PLOTS
 /TITLE, VM248, DELAMINATION OF DOUBLE CANTILEVER BEAM - 2D PLANE STRAIN
 C*** USING INTER202
 /COM,   REF: ALFANO, G. AND CRISFIELD, M. A.,
 /COM,   "FINITE ELEMENT INTERFACE MODELS FOR THE DELAMINATION ANALYSIS
 /COM,   OF LAMINATED COMPOSITES: MECHANICAL AND COMPUTATIONAL ISSUES"
 /COM,   INT. J. NUMER. METH. ENGNG 2001, 50:1701-1736.
 /PREP7
-ET,1,182                   !* 2D 4-NODE STRUCTURAL SOLID ELEMENT
+ET,1,PLANE182              !* 2D 4-NODE STRUCTURAL SOLID ELEMENT
 KEYOPT,1,1,2               !* ENHANCE STRAIN FORMULATION
 KEYOPT,1,3,2               !* PLANE STRAIN
-ET,2,182
+ET,2,PLANE182
 KEYOPT,2,1,2
 KEYOPT,2,3,2
-ET,3,202                   !* 2D 4-NODE COHESIVE ZONE ELEMENT
+ET,3,INTER202              !* 2D 4-NODE COHESIVE ZONE ELEMENT
 KEYOPT,3,3,2               !* PLANE STRAIN
 MP,EX,4,1.353E5            !* E11 = 135.3 GPA
 MP,EY,4,9.0E3              !* E22 =   9.0 GPA
 MP,EZ,4,9.0E3              !* E33 =   9.0 GPA
 MP,GXY,4,5.2E3             !* G12 =   5.2 GPA
 MP,PRXY,4,0.24
 MP,PRXZ,4,0.24
@@ -115,28 +115,28 @@
 *VFILL,VALUE(1,1),DATA,60.0,1.0
 *VFILL,VALUE(1,2),DATA,RF_MAX,UY_NTOP
 *VFILL,VALUE(1,3),DATA,ABS(RF_MAX/60.0),ABS(UY_NTOP/1.0)
 *VFILL,VALUE2(1,1),DATA,24,10.0
 *VFILL,VALUE2(1,2),DATA,RF_END,UY_END
 *VFILL,VALUE2(1,3),DATA,ABS(RF_END/24.0),ABS(UY_END/10.0)
 SAVE,INF1
-FINI
+FINISH
 /CLEAR,NOSTART
 /OUT,SCRATCH
 
 
 
 /TITLE, VM248, DELAMINATION OF DOUBLE CANTILEVER BEAM - 2D PLANE STRAIN
 C*** USING INTER203
 /PREP7
-ET,1,183                   !* 2D 8-NODE STRUCTURAL SOLID ELEMENT
+ET,1,PLANE183              !* 2D 8-NODE STRUCTURAL SOLID ELEMENT
 KEYOPT,1,3,2               !* PLANE STRAIN
-ET,2,183
+ET,2,PLANE183
 KEYOPT,2,3,2
-ET,3,203                   !* 2D 6-NODE COHESIVE ZONE ELEMENT
+ET,3,INTER203              !* 2D 6-NODE COHESIVE ZONE ELEMENT
 KEYOPT,3,3,2               !* PLANE STRAIN
 MP,EX,4,1.353E5            !* E11 = 135.3 GPA
 MP,EY,4,9.0E3              !* E22 =   9.0 GPA
 MP,EZ,4,9.0E3              !* E33 =   9.0 GPA
 MP,GXY,4,5.2E3             !* G12 =   5.2 GPA
 MP,PRXY,4,0.24
 MP,PRXZ,4,0.24
@@ -232,28 +232,28 @@
 *VFILL,VALUE(1,1),DATA,60.0,1.0
 *VFILL,VALUE(1,2),DATA,RF_MAX,UY_NTOP
 *VFILL,VALUE(1,3),DATA,ABS(RF_MAX/60.0),ABS(UY_NTOP/1.0)
 *VFILL,VALUE2(1,1),DATA,24,10.0
 *VFILL,VALUE2(1,2),DATA,RF_END,UY_END
 *VFILL,VALUE2(1,3),DATA,ABS(RF_END/24.0),ABS(UY_END/10.0)
 SAVE,INF2
-FINI
+FINISH
 /CLEAR,NOSTART
 /OUT,SCRATCH
 
 
 
-/TITLE, VM248, DELAMINATION OF DOUBLE CANTILEVER BEAM - 2D PLANE STRAIN
+/TITLE, VM248, DELAMINATION OF DOUBLE CANTILEVER BEAM - 3D
 C*** USING INTER205
 /PREP7
-ET,1,185		   !* 3D 8-NODE STRUCTURAL SOLID ELEMENT
+ET,1,SOLID185	           !* 3D 8-NODE STRUCTURAL SOLID ELEMENT
 KEYOPT,1,2,2               !* PLANE STRAIN
-ET,2,185
+ET,2,SOLID185
 KEYOPT,2,2,2
-ET,3,205                   !* 3D 8-NODE COHESIVE ZONE ELEMENT
+ET,3,INTER205              !* 3D 8-NODE COHESIVE ZONE ELEMENT
 MP,EX,4,1.353E5            !* E11 = 135.3 GPA
 MP,EY,4,9.0E3              !* E22 =   9.0 GPA
 MP,EZ,4,9.0E3              !* E33 =   9.0 GPA
 MP,GXY,4,5.2E3             !* G12 =   5.2 GPA
 MP,GYZ,4,5.2E3
 MP,GXZ,4,3.08E3
 MP,PRXY,4,0.24
@@ -290,15 +290,14 @@
 MAT,5
 CZMESH,,,1,Y,0,            !* GENERATE INTERFACE ELEMENTS
 ALLSEL,ALL
 NSEL,S,LOC,X,100           !* APPLY CONSTRAINTS
 D,ALL,ALL
 NSEL,ALL
 D,ALL,UZ,0
-
 FINISH
 /SOLU
 ESEL,S,TYPE,,2
 NSLE,S
 NSEL,R,LOC,X
 NSEL,R,LOC,Y,1.5           !* APPLY DISPLACEMENT LOADING ON TOP
 D,ALL,UY,10
@@ -356,20 +355,433 @@
 *VFILL,VALUE(1,1),DATA,60.0,1.0
 *VFILL,VALUE(1,2),DATA,RF_MAX,UY_NTOP
 *VFILL,VALUE(1,3),DATA,ABS(RF_MAX/60.0),ABS(UY_NTOP/1.0)
 *VFILL,VALUE2(1,1),DATA,24,10.0
 *VFILL,VALUE2(1,2),DATA,RF_END,UY_END
 *VFILL,VALUE2(1,3),DATA,ABS(RF_END/24.0),ABS(UY_END/10.0)
 SAVE,INF3
+FINISH
+/CLEAR,NOSTART
+/OUT,SCRATCH
+
+
+
+/TITLE, VM248, DELAMINATION OF DOUBLE CANTILEVER BEAM - 2D PLANE STRAIN
+C*** USING CONTA172 WITH DROPPED MIDSIDE NODES
+/PREP7
+ET,1,PLANE182              !* 2D 4-NODE STRUCTURAL SOLID ELEMENT
+KEYOPT,1,1,2               !* ENHANCE STRAIN FORMULATION
+KEYOPT,1,3,2               !* PLANE STRAIN
+ET,2,PLANE182
+KEYOPT,2,1,2
+KEYOPT,2,3,2
+! DEFINE CONTACT ELEMENTS
+ET,3,CONTA172
+ET,4,TARGE169
+KEYOPT,3,12,2
+MP,EX,4,1.353E5            !* E11 = 135.3 GPA
+MP,EY,4,9.0E3              !* E22 =   9.0 GPA
+MP,EZ,4,9.0E3              !* E33 =   9.0 GPA
+MP,GXY,4,5.2E3             !* G12 =   5.2 GPA
+MP,PRXY,4,0.24
+MP,PRXZ,4,0.24
+MP,PRYZ,4,0.46
+GMAX = 0.004
+TNMAX = 25                 !* TENSILE STRENGTH
+TB,CZM,5,,,EXPO            !* COHESIVE ZONE MATERIAL
+TBDATA,1,TNMAX,GMAX,1000.0
+RECTNG,0,100,0,1.5         !* DEFINE AREAS
+RECTNG,0,100,0,-1.5
+LSEL,S,LINE,,2,8,2         !* DEFINE LINE DIVISION
+LESIZE,ALL,0.75
+LSEL,INVE
+LESIZE,ALL, , ,200
+ALLSEL,ALL
+TYPE,1                     !* MESH AREA 2
+MAT,4
+LOCAL,11,0,0,0,0
+ESYS,11
+AMESH,2
+CSYS,0
+TYPE,2                     !* MESH AREA 1
+ESYS,11
+AMESH,1
+CSYS,0
+! GENERATE CONTACT ELEMENTS
+ESEL,S,TYPE,,1
+NSLE
+NSEL,R,LOC,Y
+NSEL,R,LOC,X,30,100
+TYPE,3
+REAL,3
+MAT,5
+ESURF
+ALLSEL,ALL
+ESEL,S,TYPE,,2,2
+NSEL
+NSEL,R,LOC,Y
+NSEL,R,LOC,X,30,100
+TYPE,4
+REAL,3
+MAT,5
+ESURF
+ALLSEL,ALL
+NSEL,S,LOC,X,100           !* APPLY CONSTRAINTS
+D,ALL,ALL
+NSEL,ALL
+FINISH
+/SOLU
+ESEL,S,TYPE,,2
+NSLE,S
+NSEL,R,LOC,X
+NSEL,R,LOC,Y,1.5           !* APPLY DISPLACEMENT LOADING ON TOP
+D,ALL,UY,10
+NSEL,ALL
+ESEL,ALL
+ESEL,S,TYPE,,1
+NSLE,S
+NSEL,R,LOC,X
+NSEL,R,LOC,Y,-1.5          !* APPLY DISPLACEMENT LOADING ON BOTTOM
+D,ALL,UY,-10
+NSEL,ALL
+ESEL,ALL
+NLGEOM,ON
+AUTOTS,ON
+TIME,1
+NSUBST,40,40,40
+OUTRES,ALL,ALL
+/OUT,SCRATCH
+SOLVE                      !* PERFORM SOLUTION
+FINISH
+/POST26
+NSEL,S,LOC,Y,1.5
+NSEL,R,LOC,X,0
+*GET,NTOP,NODE,0,NUM,MAX
+NSEL,ALL
+NSOL,2,NTOP,U,Y,UY
+RFORCE,3,NTOP,F,Y,FY
+PROD,4,3, , ,RF, , ,20
+/out,czm_con_182,out
+prvar,2,4
+/OUT,SCRATCH
+/TITLE,VM248CON, DCB: REACTION AT TOP NODE VERSES PRESCRIBED DISPLACEMENT
+/AXLAB,X,DISP U (mm)
+/AXLAB,Y,REACTION FORCE R (N)
+/YRANGE,0,60
+XVAR,2
+PLVAR,4
+PRVAR,UY,RF
+*GET,TMAX,VARI,4,EXTREM,TMAX   !* TIME CORRESPONDING TO MAX RFORCE
+FINISH
+/POST1
+SET, , , , ,TMAX               !* RETRIEVE RESULTS AT TMAX
+NSEL,S,NODE, ,NTOP             !* SELECT NODE NTOP
+/OUT,
+*GET,RF_NTOP,NODE,NTOP,RF,FY   !* FY RFORCE AT NODE NTOP
+*GET,UY_NTOP,NODE,NTOP,U,Y     !* DISP AT NODE NTOP CORRESPONDING TO RFORCE
+RF_MAX = RF_NTOP*20            !* PLANE STRAIN OPTION AND WIDTH = 20 mm
+SET,LAST                       !* RETRIEVE RESULTS AT LAST SUBSTEP
+*GET,RF_END,NODE,NTOP,RF,FY    !* FY RFORCE AT NODE NTOP AT LAST SUBSTEP
+*GET,UY_END,NODE,NTOP,U,Y      !* DISP AT NODE NTOP CORRESPONDING TO RFORCE
+RF_END = RF_END*20             !* PLANE STRAIN OPTION AND WIDTH = 20 mm
+*DIM,LABEL,CHAR,2,2
+*DIM,VALUE,,2,3
+*DIM,VALUE2,,2,3
+LABEL(1,1) = 'RFORCE','DISP '
+LABEL(1,2) = 'FY (N)','UY (mm)'
+*VFILL,VALUE(1,1),DATA,60.0,1.0
+*VFILL,VALUE(1,2),DATA,RF_MAX,UY_NTOP
+*VFILL,VALUE(1,3),DATA,ABS(RF_MAX/60.0),ABS(UY_NTOP/1.0)
+*VFILL,VALUE2(1,1),DATA,24,10.0
+*VFILL,VALUE2(1,2),DATA,RF_END,UY_END
+*VFILL,VALUE2(1,3),DATA,ABS(RF_END/24.0),ABS(UY_END/10.0)
+SAVE,INF4
+FINISH
+/CLEAR,NOSTART
+/OUT,SCRATCH
+
+
+
+/TITLE, VM248, DELAMINATION OF DOUBLE CANTILEVER BEAM - 2D PLANE STRAIN
+C*** USING CONTA172
+/PREP7
+ET,1,PLANE183              !* 2D 8-NODE STRUCTURAL SOLID ELEMENT
+KEYOPT,1,3,2               !* PLANE STRAIN
+ET,2,PLANE183
+KEYOPT,2,3,2
+! DEFINE CONTACT ELEMENTS
+ET,3,CONTA172
+ET,4,TARGE169
+KEYOPT,3,12,2
+MP,EX,4,1.353E5            !* E11 = 135.3 GPA
+MP,EY,4,9.0E3              !* E22 =   9.0 GPA
+MP,EZ,4,9.0E3              !* E33 =   9.0 GPA
+MP,GXY,4,5.2E3             !* G12 =   5.2 GPA
+MP,PRXY,4,0.24
+MP,PRXZ,4,0.24
+MP,PRYZ,4,0.46
+GMAX = 0.004
+TNMAX = 25                 !* TENSILE STRENGTH
+TB,CZM,5,,,EXPO            !* COHESIVE ZONE MATERIAL
+TBDATA,1,TNMAX,GMAX,1000.0
+RECTNG,0,100,0,1.5         !* DEFINE AREAS
+RECTNG,0,100,0,-1.5
+LSEL,S,LINE,,2,8,2         !* DEFINE LINE DIVISION
+LESIZE,ALL,1.5
+LSEL,INVE
+LESIZE,ALL, , ,200
+ALLSEL,ALL
+TYPE,1                     !* MESH AREA 2
+MAT,4
+LOCAL,11,0,0,0,0
+ESYS,11
+AMESH,2
+CSYS,0
+TYPE,2                     !* MESH AREA 1
+ESYS,11
+AMESH,1
+CSYS,0
+! GENERATE CONTACT ELEMENTS
+ESEL,S,TYPE,,1
+NSLE
+NSEL,R,LOC,Y
+NSEL,R,LOC,X,30,100
+TYPE,3
+REAL,3
+MAT,5
+ESURF
+ALLSEL,ALL
+ESEL,S,TYPE,,2,2
+NSEL
+NSEL,R,LOC,Y
+NSEL,R,LOC,X,30,100
+TYPE,4
+REAL,3
+MAT,5
+ESURF
+ALLSEL,ALL
+NSEL,S,LOC,X,100           !* APPLY CONSTRAINTS
+D,ALL,ALL
+NSEL,ALL
+FINISH
+/SOLU
+ESEL,S,TYPE,,2
+NSLE,S
+NSEL,R,LOC,X
+NSEL,R,LOC,Y,1.5           !* APPLY DISPLACEMENT LOADING ON TOP
+D,ALL,UY,10
+NSEL,ALL
+ESEL,ALL
+ESEL,S,TYPE,,1
+NSLE,S
+NSEL,R,LOC,X
+NSEL,R,LOC,Y,-1.5          !* APPLY DISPLACEMENT LOADING ON BOTTOM
+D,ALL,UY,-10
+NSEL,ALL
+ESEL,ALL
+NLGEOM,ON
+AUTOTS,ON
+TIME,1
+NSUBST,40,40,40
+OUTRES,ALL,ALL
+/OUT,SCRATCH
+SOLVE                      !* PERFORM SOLUTION
+FINISH
+/POST26
+NSEL,S,LOC,Y,1.5
+NSEL,R,LOC,X,0
+*GET,NTOP,NODE,0,NUM,MAX
+NSEL,ALL
+NSOL,2,NTOP,U,Y,UY
+RFORCE,3,NTOP,F,Y,FY
+PROD,4,3, , ,RF, , ,20
+/out,czm_con_183,out
+prvar,2,4
+/OUT,SCRATCH
+/TITLE,VM248CON, DCB: REACTION AT TOP NODE VERSES PRESCRIBED DISPLACEMENT
+/AXLAB,X,DISP U (mm)
+/AXLAB,Y,REACTION FORCE R (N)
+/YRANGE,0,60
+XVAR,2
+PLVAR,4
+PRVAR,UY,RF
+*GET,TMAX,VARI,4,EXTREM,TMAX   !* TIME CORRESPONDING TO MAX RFORCE
+FINISH
+/POST1
+SET, , , , ,TMAX               !* RETRIEVE RESULTS AT TMAX
+NSEL,S,NODE, ,NTOP             !* SELECT NODE NTOP
+/OUT,
+*GET,RF_NTOP,NODE,NTOP,RF,FY   !* FY RFORCE AT NODE NTOP
+*GET,UY_NTOP,NODE,NTOP,U,Y     !* DISP AT NODE NTOP CORRESPONDING TO RFORCE
+RF_MAX = RF_NTOP*20            !* PLANE STRAIN OPTION AND WIDTH = 20 mm
+SET,LAST                       !* RETRIEVE RESULTS AT LAST SUBSTEP
+*GET,RF_END,NODE,NTOP,RF,FY    !* FY RFORCE AT NODE NTOP AT LAST SUBSTEP
+*GET,UY_END,NODE,NTOP,U,Y      !* DISP AT NODE NTOP CORRESPONDING TO RFORCE
+RF_END = RF_END*20             !* PLANE STRAIN OPTION AND WIDTH = 20 mm
+*DIM,LABEL,CHAR,2,2
+*DIM,VALUE,,2,3
+*DIM,VALUE2,,2,3
+LABEL(1,1) = 'RFORCE','DISP '
+LABEL(1,2) = 'FY (N)','UY (mm)'
+*VFILL,VALUE(1,1),DATA,60.0,1.0
+*VFILL,VALUE(1,2),DATA,RF_MAX,UY_NTOP
+*VFILL,VALUE(1,3),DATA,ABS(RF_MAX/60.0),ABS(UY_NTOP/1.0)
+*VFILL,VALUE2(1,1),DATA,24,10.0
+*VFILL,VALUE2(1,2),DATA,RF_END,UY_END
+*VFILL,VALUE2(1,3),DATA,ABS(RF_END/24.0),ABS(UY_END/10.0)
+SAVE,INF5
+FINISH
+/CLEAR,NOSTART
+/OUT,SCRATCH
+
+
+
+/TITLE, VM248CON, DELAMINATION OF DOUBLE CANTILEVER BEAM - 3D
+C*** USING CONTA174 WITH DROPPED MIDSIDE NODES
+/PREP7
+ET,1,SOLID185	           !* 3D 8-NODE STRUCTURAL SOLID ELEMENT
+KEYOPT,1,2,2               !* PLANE STRAIN
+ET,2,SOLID185
+KEYOPT,2,2,2
+! DEFINE CONTACT ELEMENTS
+ET,3,CONTA174
+ET,4,TARGE170
+KEYOPT,3,12,2
+MP,EX,4,1.353E5            !* E11 = 135.3 GPA
+MP,EY,4,9.0E3              !* E22 =   9.0 GPA
+MP,EZ,4,9.0E3              !* E33 =   9.0 GPA
+MP,GXY,4,5.2E3             !* G12 =   5.2 GPA
+MP,GYZ,4,5.2E3
+MP,GXZ,4,3.08E3
+MP,PRXY,4,0.24
+MP,PRXZ,4,0.24
+MP,PRYZ,4,0.46
+GMAX = 0.004
+TNMAX = 25                 !* TENSILE STRENGTH
+TB,CZM,5,,,EXPO            !* COHESIVE ZONE MATERIAL
+TBDATA,1,TNMAX,GMAX,1000.0
+BLC4,0,0,100,1.5,1         !* DEFINE VOLUMES
+BLC4,0,0,100,-1.5,1
+LSEL,S,LINE,,10,11,1       !* DEFINE LINE DIVISION
+LSEL,A,LINE,,22,23,1
+LESIZE,ALL,,,1
+LSEL,S,LINE,,7,17,10
+LESIZE,ALL,,,200
+LSEL,S,LINE,,6,18,12
+LESIZE,ALL,1.5
+ALLSEL,ALL
+TYPE,1                     !* MESH VOLUME 2
+MAT,4
+LOCAL,11,0,0,0,0
+ESYS,11
+VMESH,2
+CSYS,0
+TYPE,2                     !* MESH VOLUME 1
+ESYS,11
+VMESH,1
+CSYS,0
+! GENERATE CONTACT ELEMENTS
+ESEL,S,TYPE,,1
+NSLE
+NSEL,R,LOC,Y
+NSEL,R,LOC,X,30,100
+TYPE,3
+REAL,3
+MAT,5
+ESURF
+ALLSEL,ALL
+ESEL,S,TYPE,,2,2
+NSEL
+NSEL,R,LOC,Y
+NSEL,R,LOC,X,30,100
+TYPE,4
+REAL,3
+MAT,5
+ESURF
+ALLSEL,ALL
+NSEL,S,LOC,X,100           !* APPLY CONSTRAINTS
+D,ALL,ALL
+NSEL,ALL
+D,ALL,UZ,0
+FINISH
+/SOLU
+ESEL,S,TYPE,,2
+NSLE,S
+NSEL,R,LOC,X
+NSEL,R,LOC,Y,1.5           !* APPLY DISPLACEMENT LOADING ON TOP
+D,ALL,UY,10
+NSEL,ALL
+ESEL,ALL
+ESEL,S,TYPE,,1
+NSLE,S
+NSEL,R,LOC,X
+NSEL,R,LOC,Y,-1.5          !* APPLY DISPLACEMENT LOADING ON BOTTOM
+D,ALL,UY,-10
+NSEL,ALL
+ESEL,ALL
+NLGEOM,ON
+AUTOTS,ON
+TIME,1
+NSUBST,40,40,40
+OUTRES,ALL,ALL
 /OUT,SCRATCH
+SOLVE                      !* PERFORM SOLUTION
+FINISH
+/POST26
+NSEL,S,LOC,Y,1.5
+NSEL,R,LOC,X,0
+NSEL,R,LOC,Z,0
+*GET,NTOP,NODE,0,NUM,MAX
+NSEL,ALL
+NSOL,2,NTOP,U,Y,UY
+RFORCE,3,NTOP,F,Y,FY
+PROD,4,3, , ,RF, , ,20
+/out,czm_con_185,out
+prvar,2,4
+/OUT,SCRATCH
+/TITLE,VM248CON, DCB: REACTION AT TOP NODE VERSES PRESCRIBED DISPLACEMENT
+/AXLAB,X,DISP U (mm)
+/AXLAB,Y,REACTION FORCE R (N)
+/YRANGE,0,60
+XVAR,2
+PLVAR,4
+PRVAR,UY,RF
+*GET,TMAX,VARI,4,EXTREM,TMAX   !* TIME CORRESPONDING TO MAX RFORCE
+FINISH
+/POST1
+SET, , , , ,TMAX               !* RETRIEVE RESULTS AT TMAX
+NSEL,S,NODE, ,NTOP             !* SELECT NODE NTOP
+/OUT,
+*GET,RF_NTOP,NODE,NTOP,RF,FY   !* FY RFORCE AT NODE NTOP
+*GET,UY_NTOP,NODE,NTOP,U,Y     !* DISP AT NODE NTOP CORRESPONDING TO RFORCE
+RF_MAX = RF_NTOP*40 	       !* PLANE STRAIN OPTION AND WIDTH = 20 mm
+SET,LAST                       !* RETRIEVE RESULTS AT LAST SUBSTEP
+*GET,RF_END,NODE,NTOP,RF,FY    !* FY RFORCE AT NODE NTOP AT LAST SUBSTEP
+*GET,UY_END,NODE,NTOP,U,Y      !* DISP AT NODE NTOP CORRESPONDING TO RFORCE
+RF_END = RF_END*40 	       !* PLANE STRAIN OPTION AND WIDTH = 20 mm
+*DIM,LABEL,CHAR,2,2
+*DIM,VALUE,,2,3
+*DIM,VALUE2,,2,3
+LABEL(1,1) = 'RFORCE','DISP '
+LABEL(1,2) = 'FY (N)','UY (mm)'
+*VFILL,VALUE(1,1),DATA,60.0,1.0
+*VFILL,VALUE(1,2),DATA,RF_MAX,UY_NTOP
+*VFILL,VALUE(1,3),DATA,ABS(RF_MAX/60.0),ABS(UY_NTOP/1.0)
+*VFILL,VALUE2(1,1),DATA,24,10.0
+*VFILL,VALUE2(1,2),DATA,RF_END,UY_END
+*VFILL,VALUE2(1,3),DATA,ABS(RF_END/24.0),ABS(UY_END/10.0)
+SAVE,INF6
+/OUT,SCRATCH
+
+
 
 RESUME,INF1
 /COM
 /OUT,vm248,vrt
-/COM,------------------- VM248 RESULTS COMPARISON --------------
+/COM,------------------- VM248 RESULTS COMPARISON -------------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 /COM,MAX RFORCE AND CORRESPONDING DISP USING INTER202:
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
@@ -397,14 +809,53 @@
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
 /COM,
 /COM,RFORCE CORRESPONDING TO DISP U = 10.0 USING INTER205:
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
-/COM,-----------------------------------------------------------
+/COM,
+/NOPR
+RESUME,INF4
+/COM,MAX RFORCE AND CORRESPONDING DISP USING CONTA172 (DROPPED MIDSIDE NODES):
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
+/COM,
+/COM,RFORCE CORRESPONDING TO DISP U = 10.0 USING CONTA172 (DROPPED MIDSIDE NODES):
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
+/COM,
+/NOPR
+RESUME,INF5
+/COM,MAX RFORCE AND CORRESPONDING DISP USING CONTA172:
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
+/COM,
+/COM,RFORCE CORRESPONDING TO DISP U = 10.0 USING CONTA172:
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
+/COM,
+/NOPR
+RESUME,INF6
+/COM,MAX RFORCE AND CORRESPONDING DISP USING CONTA174 (DROPPED MIDSIDE NODES):
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
+/COM,
+/COM,RFORCE CORRESPONDING TO DISP U = 10.0 USING CONTA174 (DROPPED MIDSIDE NODES):
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
+(1X,A8,A8,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
+/COM,---------------------------------------------------------------
 /OUT
-FINI
+FINISH
 *LIST,vm248,vrt
 /DELETE,INF1
 /DELETE,INF2
 /DELETE,INF3
+/DELETE,INF4
+/DELETE,INF5
+/DELETE,INF6
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm249.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm249.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM249
 JPGPRF,500,100,1                 !* MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM249, GASKET MATERIAL UNDER UNIAXIAL COMPRESSION LOAD
 /COM,   REF: ANY NONLINEAR MATERIAL VERIFICATION TEXT
 /COM,   USING 2D 4-NODE INTER192 GASKET ELEMENTS
 /PREP7
 MP, EX, 1,15.2E6*6890
 MP,NUXY, 1, 0.21
 MP,DENS,1,7203
+TB,GASKET,2,,  ,PARA
+TBDATA,2,0.1e-7                  ! tension stable stiffness
+TBDATA,3,0.1e-5                  ! tension stress cap
 TB,GASKET,2,,13,COMP             !* COMPRESSION CURVE
 TBPT,,0.508000E-04, 0.161226E+07
 TBPT,,0.101600E-03, 0.520884E+07
 TBPT,,0.152400E-03, 0.113134E+08
 TBPT,,0.203200E-03, 0.200499E+08
 TBPT,,0.254000E-03, 0.259960E+08
 TBPT,,0.304800E-03, 0.290345E+08
@@ -232,14 +235,15 @@
 NSEL,ALL
 /OUT,SCRATCH
 SOLVE
 /OUT
 NSEL,S,LOC,Y,2.02
 SF,ALL,PRES,0                !* 2ND LOAD STEP -- UNLOAD THE MODEL
 NSEL,ALL
+/OUT,SCRATCH
 SOLVE
 NSEL,S,LOC,Y,2.02            !* 3RD LOAD STEP -- RELOAD THE MODEL
 SF,ALL,PRES,157147000
 NSEL,ALL
 /OUT,SCRATCH
 SOLVE
 /OUT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm25.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm25.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM25
 /PREP7
 SMRT,OFF
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM25, STRESSES IN A LONG CYLINDER
 C*** STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 213, PROB. 1
 C***  INTERNAL PRESSURE 
 ANTYPE,STATIC        ! STATIC ANALYSIS
 ET,1,PLANE183,,,1,   ! AXISYMM
 MP,EX,1,30E6         ! MATERIAL PROPERTIES
 MP,DENS,1,.00073
 MP,NUXY,1,0.3        ! DEFINE KEYPOINTS, LINES, AND AREAS
-K,1,4 
-K,2,8
-KGEN,2,1,2,1,,1
-L,1,2,7 
-ESIZE,.5 
-LESIZE,1,,,14 
-MSHK,1                    ! MAPPED AREA MESH
-MSHA,0,2D                 ! USING QUADS
-A,3,1,2,4 
-AMESH,1
+N,1,4 
+N,2,4+4/14
+N,3,4+4/14,0.5
+N,4,4,0.5
+N,5,4+4/28
+N,6,4+4/14,0.25
+N,7,4+4/28,0.5
+N,8,4,0.25
+E,1,2,3,4,5,6,7,8
+EGEN,14,8,1,,,,,,,,4/14  
+NUMMRG,NODE
+EGEN,2,111,1,14,,,,,,,,0.5
+NUMMRG,NODE
 SAVE,MODEL           ! SAVE MODEL FOR SECOND LOAD CASE
 NSEL,S,LOC,Y,0       ! SET UP LONG CYLINDER EFFECT
 D,ALL,UY
 NSEL,S,LOC,Y,1   
 CP,1,UY,ALL          ! COUPLE AXIAL DISPLACEMENTS AT UNCONSTRAINED Y EDGE
 NSEL,ALL
 FINISH
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm250.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm250.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM250
 JPGPRF,500,100,1                 !* MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM250, GASKET MATERIAL UNDER UNIAXIAL COMPRESSION LOAD
 /COM,   REF: ANY NONLINEAR MATERIAL VERIFICATION TEXT
 /COM,   USING 3D 8-NODE INTER195 GASKET ELEMENTS
 /PREP7
@@ -111,19 +111,22 @@
 NSEL,S,LOC,Z,0
 D,ALL,UZ
 NSEL,ALL
 FINISH
 /out,scratch
 /SOLU
 NLGEOM,ON
-NSUBST,50,50,50
+NSUBST,50,5000,50
 OUTRES,ALL,-10
 NSEL,S,LOC,Z,2.02
 SF,ALL,PRES,44006400         !* 1ST LOAD STEP -- LOAD THE MODEL
 NSEL,ALL
+cnvtol,f,,0.006
+cnvtol,u,,0.05
+
 SOLVE
 NSEL,S,LOC,Z,2.02
 SF,ALL,PRES,0                !* 2ND LOAD STEP -- UNLOAD THE MODEL
 NSEL,ALL
 SOLVE
 NSEL,S,LOC,Z,2.02            !* 3RD LOAD STEP -- RELOAD THE MODEL
 SF,ALL,PRES,157147000
@@ -213,19 +216,23 @@
 NSEL,S,LOC,Z,0
 D,ALL,UZ
 NSEL,ALL
 FINISH
 /out,scratch
 /SOLU
 NLGEOM,ON
-NSUBST,50,50,50
+NSUBST,50,5000,50
 OUTRES,ALL,-10
 NSEL,S,LOC,Z,2.02
 SF,ALL,PRES,44006400         !* 1ST LOAD STEP -- LOAD THE MODEL
 NSEL,ALL
+
+cnvtol,f,,0.006
+cnvtol,u,,0.05
+
 SOLVE
 NSEL,S,LOC,Z,2.02
 SF,ALL,PRES,0                !* 2ND LOAD STEP -- UNLOAD THE MODEL
 NSEL,ALL
 SOLVE
 NSEL,S,LOC,Z,2.02            !* 3RD LOAD STEP -- RELOAD THE MODEL
 SF,ALL,PRES,157147000
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm251.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm251.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM251
 JPGPRF,500,100,1                !* MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM251, SHAPE MEMORY ALLOY UNDER UNIAXIAL TENSION LOAD
 /COM,   REF: FERDINANDO AURICHIO, ROBERT L. TAYLOR, JACOB LUBLINER
 /COM,   "SHAPE-MEMORY ALLOYS: MACROMODELLING AND NUMERICAL SIMULATIONS
 /COM,   OF SUPERELASTIC BEHAVIOR"
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm252.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm252.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM252
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE,VM252,GURSON BAR-NECKING BENCHMARK WITH APPLIED DISPLACEMENT
 /COM, REFERENCE:
 /COM, N. ARAVAS, "ON THE NUMERICAL INTEGRATION OF A CLASS OF PRESSURE
 /COM, DEPENDENT PLASTICITY MODELS." INT. J. FOR NUMERICAL METHODS IN
@@ -64,16 +64,14 @@
 ALLS
 FINISH
 *CREATE,MACRO,MAC		  ! MACRO FOR SOLUTION AND POST PROCESSING
 /SOLU                             ! NON-LINEAR SOLUTION
 OUTRES,ALL,ALL
 NLGEOM,ON
 NROPT,UNSYM
-SOLCONTROL,ON
-CNVTOL,F,1.0,0.1
 NSUBST,MYSUBST,MYSUBST,MYSUBST
 ALLS
 /OUTPUT,SCRATCH
 SOLVE
 /OUT
 FINISH
 /POST1                            ! REACTION FORCES AT TOP OF BAR
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm253.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm253.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,vm253
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE,VM253,GURSON HYDROSTATIC TENSION BENCHMARK
 /COM, REFERENCE:
 /COM, N. ARAVAS, "ON THE NUMERICAL INTEGRATION OF A CLASS OF PRESSURE
 /COM, DEPENDENT PLASTICITY MODELS." INT. J. FOR NUMERICAL METHODS IN
@@ -55,22 +55,23 @@
 D,ALL,UY,UAPP
 NSEL,S,LOC,Z,1
 D,ALL,UZ,UAPP
 ALLS
 NLGEOM,ON                    ! NON-LINEAR SOLUTION
 NROPT,UNSYM
 AUTOTS,OFF
-SOLCONTROL,ON
 CNVTOL,F,1.0,1E-5
 NSUBST,100,100,100
 OUTRES,ALL,ALL
 /OUTPUT,SCRATCH
 SOLVE
 /OUT
+/NOPR
 FINISH
+/GOPR
 *CREATE,MACRO,MAC            ! MACRO FOR PLOTTING AND DATA COLLECTION
 /POST26                      ! VOLUMETRIC PRESSURE VS. VOLUMETRIC STRAIN
 NSOL,2,NODE(1,0,0),U,X
 EXP,3,2,,,ONE,,,1E-10,1.0
 ADD,4,2,3
 NLOG,5,4,,,EPSV,,,1.0,3.0    ! X-AXIS ADJUSTMENT
 ESOL,6,1,,NL,HPRES
@@ -115,22 +116,21 @@
 D,ALL,UY,UAPP
 NSEL,S,LOC,Z,1
 D,ALL,UZ,UAPP
 ALLS
 NLGEOM,ON                    ! NON-LINEAR SOLUTION
 NROPT,UNSYM
 AUTOTS,OFF
-SOLCONTROL,ON
 CNVTOL,F,1.0,1E-5
 NSUBST,100,100,100
 OUTRES,ALL,ALL
 /OUTPUT,SCRATCH
 SOLVE
-/OUT
 FINISH
+/OUT
 MACRO
 SAVE,TABLE_2
 RESUME,TABLE_1
 /COM,
 /OUT,vm253,vrt
 /COM,--------------- VM253 RESULTS COMPARISON -------------------
 /COM,
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm254.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm254.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM254
 JPGPRF,500,100,1                                ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/TITLE, VM254 CAMPBELL DIAGRAMS AND CRITICAL SPEEDS USING SYMMETRIC ORTHOTROPIC BEARINGS
+/TITLE, VM254, CAMPBELL DIAGRAMS AND CRITICAL SPEEDS USING SYMMETRIC ORTHOTROPIC BEARINGS
 /COM,   REF: "THE DYNAMICS OF ROTOR-BEARING SYSTEMS USING FINITE ELEMENTS"
 /COM,   JOURNAL OF ENG. FOR INDUSTRY - MAY 1976, PG: 598-600
 C***    USING PIPE16
 /COM
 JPGPRF,500,100,1
 /SHOW,JPEG
 /OUT,SCRATCH
@@ -369,9 +369,10 @@
 *VWRITE,LABEL(1,4),VALUE(4,1),VALUE(4,2),VALUE(4,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 /COM,
 /COM,----------------------------------------------------------
 /OUT,
 FINISH
 *LIST,vm254,vrt
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm255.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm255.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM255
 /SHOW,JPEG
 JPGPRF,500,100,1           !* MACRO TO SET PREFS FOR JPEG PLOTS
 /TITLE,VM255,DELAMINATION OF DOUBLE CANTILEVER BEAM USING DEBONDING
 /COM,   REF: ALFANO, G. AND CRISFIELD, M. A.,
 /COM,   "FINITE ELEMENT INTERFACE MODELS FOR THE DELAMINATION ANALYSIS
 /COM,   OF LAMINATED COMPOSITES: MECHANICAL AND COMPUTATIONAL ISSUES"
@@ -11,15 +11,16 @@
 ET,1,PLANE182              !* 2D 4-NODE STRUCTURAL SOLID ELEMENT
 KEYOPT,1,1,2               !* ENHANCE STRAIN FORMULATION
 KEYOPT,1,3,2               !* PLANE STRAIN
 ET,2,PLANE182
 KEYOPT,2,1,2
 KEYOPT,2,3,2
 ET,3,TARGE169              !* 2D TARGET ELEMENT
-ET,4,CONTA171              !* 2D CONTACT ELEMENT
+ET,4,CONTA172              !* 2D 3-NODE CONTACT ELEMENT
+KEYOPT,4,10,1              !* USE CONSTANT CONTACT STIFFNESS
 KEYOPT,4,12,5              !* BONDED ALWAYS CONTACT
 MP,EX,1,1.353E5            !* E11 = 135.3 GPA
 MP,EY,1,9.0E3              !* E22 =   9.0 GPA
 MP,EZ,1,9.0E3              !* E33 =   9.0 GPA
 MP,GXY,1,5.2E3             !* G12 =   5.2 GPA
 MP,PRXY,1,0.24
 MP,PRXZ,1,0.24
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm256.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm303.dat`

 * *Files 27% similar despite different names*

```diff
@@ -1,332 +1,419 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM256
-/COM,   VERIFICATION MANUAL FOR FRACTURE MECHANCIS, REL 11.0
-/TITLE,VM256 FRACTURE MECHANICS STRESS INTENSITY  - CRACK IN A 2D PLATE
-/COM    REFERENCE: BROWN AND SRAWLEY, ASTM SPECIAL TECHNICAL PUBLICATION NO. 410.
-/COM    ****** CRACK IN 2-DIMENSIONS USING 2-D PLANE183 ELEMENT  ******
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM303
+/TITLE,VM303,1-D STEADY-STATE THERMAL CONDUCTION IN A REINFORCED BLOCK
+/COM,
+/COM, REFERENCE: LATIF M. JIJI, "HEAT CONDUCTION", 3RD ED.
+/COM,
+
+/COM, PARAMETER FOR CREATING THE CDB FILES TO STORE GEOMETRY AND MESH DATA
+_GEOMGEN = 0     ! SET TO 1 TO WRITE CDB FILES IF ANY INPUT FILE MODIFICATIONS
+
+/OUT,vm303_SCRATCH
+!-----------------------------------------------------------------
+!!!!! PART 1&2 PREP:
+!-----------------------------------------------------------------
 /PREP7
-ET,1,PLANE183,,,2              ! PLANE183 (PLANE STRAIN)
-MP,EX,1,30E6
-MP,NUXY,1,0.3
-K,1                           ! DEFINE KEYPOINTS AND LINE SEGMENTS
-K,2,4
-K,3,4,5
-K,4,-1,5
-K,5,-1
-L,1,2
-L,2,3
-LESIZE,2,,,4
-L,3,4
-LESIZE,3,,,4
-L,4,5,
-LESIZE,4,,,6,.2
-L,5,1
-ESIZE,,5
-KSCON,1,.15,0,8               ! DEFINE CRACK TIP ELEMENT SIZE, NO SINGULAR ELEMENTS
-AL,1,2,3,4,5
-DL,1,1,SYMM                   ! APPLY SOLID MODEL BOUNDARY CONDITIONS
-DL,4,1,SYMM
-SFL,3,PRES,-.5641895
-AMESH,1
-OUTPR,ALL
-FINISH
-/SOLU
-ANTYPE,STATIC
-OUTRES,ALL,ALL
-NSEL,S,LOC,X,0,10
-NSEL,R,LOC,Y,0
-D,ALL,UY,0
-ALLSEL,ALL
-NSEL,S,LOC,X,0
-NSEL,R,LOC,Y,0
-D,ALL,UX,0
-ALLSEL,ALL
-NSEL,S,LOC,X,0
-NSEL,R,LOC,Y,0
-CM,CRACKTIP,NODE             ! DEFINE CRACK TIP NODE COMPONENT
-ALLSEL,ALL
-CINT,NEW,1                   ! DEFINE CRACK ID
-CINT,TYPE,SIFS               ! DEFINE CRACK TYPE
-CINT,CTNC,CRACKTIP           ! DEFINE CRACK TIP NODE COMPONENT
-CINT,SYMM,ON                 ! SYMMETRY ON
-CINT,NCON,6                  ! NUMBER OF COUNTOURS
-CINT,NORM,0,2                ! DEFINE CRACK PLANE NORMAL
-CINT,LIST
-ALLSEL,ALL
-/OUT,SCRATCH
-SOLVE
-FINI
-/POST1
-/OUT,
-PRCINT,1,1,K1                  ! PRINT K VALUES 
-*GET,K,CINT,1,CTIP,1,,5,,K1    ! GET K VALUE FOR CRACK TIP NODE 
-*STATUS,K
-/OUT,SCRATCH
-*DIM,LABEL,CHAR,1,
-*DIM,VALUE,,1,3
-LABEL(1,1) = 'KI ',
-*VFILL,VALUE(1,1),DATA,1.0249     ! STRESS INTENSITY VALUE OBTAINED FROM REFERENCE
-*VFILL,VALUE(1,2),DATA,K
-*VFILL,VALUE(1,3),DATA,ABS(K/1.0249)
-SAVE,TABLE_1
-FINISH
-/CLEAR, NOSTART                ! CLEAR DATABASE FOR 2ND SOLUTION
-/OUT,
+*IF,_GEOMGEN,EQ,1,THEN
 
+HEAT = 6         ! HEAT GENERATION IN REINFORCEMENT (W/mm^3)
 
-/COM ************* CRACK IN 3D PLATE USING SOLID 185 ELEMENT ******************* C
+MP,KXX,1,1       ! THERMAL CONDUCTIVITY OF REINFORCEMENT (W/mm.C)
+MP,KXX,2,1.E-12  ! THERMAL CONDUCTIVITY OF BLOCK (NON-CONDUCTOR)
 
-/PREP7
-SMRT,OFF
-/TITLE, VM256, FRACTURE MECHANICS STRESS INTENSITY  - CRACK IN A FINITE WIDTH PLATE
-/COM,     ****** CRACK IN 3-DIMENSIONS USING SOLID185
-/COM,
-ET,1,SOLID185          ! SOLID 185 ELEMENT
-ET,2,SOLID185          ! ELEMENTS AROUND THE CRACK TIP
-MP,EX,1,3E7
-MP,NUXY,1,0.3
-CSYS,1                 ! CYLINDRICAL COORDINATE SYSTEM
-N,1
-NGEN,9,20,1
-N,11,0.8
-N,171,0.8,180
-FILL,11,171,7,31,20
-CSYS,0                ! CARTESIAN COORDINATE SYSTEM
-FILL,1,11,9,2,1,9,20,3
-N,15,4
-N,75,4,5
-FILL,15,75,2,35,20
-N,155,-1,5
-FILL,75,155,3,95,20
-N,172,-1
-FILL,155,172,5,177,-1,,,.15
-FILL,11,15,3,,,7,20,3
-NGEN,2,200,1,177,,,,.25
-/OUT,SCRATCH
-E,2,22,1,1,202,222,201,201
-EGEN,8,20,-1
-E,2,3,23,22,202,203,223,222
-EGEN,8,20,-1
-EGEN,9,1,-8
-EGEN,5,1,73,78
-E,171,151,173,172,371,351,373,372
-E,151,131,174,173,351,331,374,373
-E,131,132,175,174,331,332,375,374
-EGEN,3,1,-1
-E,134,135,155,177,334,335,355,377
+! BLOCK GEOMETRY AND MESHING
+BLOCK,0,10,0,10,0,10
+ET,1,278
+TYPE,1
+MAT,2
+ESIZE,0.5
+MSHAPE,0,3D
+MSHKEY,1
+VSWEEP,1,1,2
+ALLS
+
+! REINFORCEMENT SECTION DEFINITION
+SECT,2,REINF,DISC
+SECD,1,0.0004,MESH
+SECC,,1
+SLIST
+
+! REINFORCEMENT (MESH200) GEOMETRY AND MESHING
+ET,2,200,2
 TYPE,2
-EMODIF,1                    ! MODIFY ELEMENTS 1 TO 8 FROM TYPE,1 TO TYPE,2
-*REPEAT,8,1
-NUMMRG,NODE                 ! MERGE COINCIDENT NODES
-ALLSEL,ALL
-/OUT,
-NSEL,S,LOC,X,0
-NSEL,R,LOC,Y,0
-NLIST
-CM,CRACKTIP,NODE            ! CRACK TIP NODE COMPONENT
-ALLSEL,ALL
-NSEL,S,LOC,X,-1
-DSYM,SYMM,X                 ! SYMMETRY BOUNDARY CONDITIONS
-NSEL,S,LOC,X,0,4
-NSEL,R,LOC,Y,0
-DSYM,SYMM,Y                 ! SYMMETRY BOUNDARY CONDITIONS
-ALLSEL,ALL
-D,ALL,UZ,0
-ALLSEL,ALL
-NSEL,S,LOC,Y,5
-SF,ALL,PRES,-0.5641895      ! SURFACE PRESSURE
-ALLSEL,ALL
+MAT,1
+SECNUM,2
+NUMSTR,LINE,1001
+K,1001,0,5,5
+K,2001,10,5,5
+L,1001,2001     ! LENGTH OF THE 1-D REINFORCEMENT = 10 mm
+LESIZE,1001,,,20
+LMESH,1001
+ALLS
+
+! APPLY HEAT GENERATION ON MESH200
+ESEL,S,ENAME,,200
+BFE,ALL,HGEN,1,HEAT
+ALLS
+
+! EMBEDDED LINK33 GEOMETRY AND MESHING
+ET,3,33
+TYPE,3
+MAT,1
+R,2,0.0004
+REAL,2
+NUMSTR,LINE,1001
+K,3001,0,5,5
+K,4001,10,5,5
+L,3001,4001
+
+LESIZE,1002,,,20
+LMESH,1002
+ALLS
+
+CDWRITE,db,vm303_1,cdb
+*ELSE
+ CDREAD,db,vm303_1,cdb
+*ENDIF
+
+!-----------------------------------------------------------------
+!!!!! PART 1: SOLUTION WITH SOLID278 + REINF264  !!!!!
+!-----------------------------------------------------------------
+
+! GENERATE REINFORCING ELEMENTS FROM MESH200
+SECNUM,2
+EREINF
+ALLS
+
+! LIST MAPPED BODY LOADS
+ESEL,S,ENAME,,264
+BFELIST
+
+! APPLY BOUNDARY TEMPERATURES
+NSEL,S,LOC,X,0.0
+D,ALL,TEMP,20
+ALLS
+NSEL,S,LOC,X,10.0
+D,ALL,TEMP,80
+ALLS
+
 FINI
+
 /SOLU
-AUTOTS,ON
-NSUBST,10
+TIME,1
+DELTIM,1
 OUTRES,ALL,ALL
-CINT,NEW,1                    ! CRACK ID
-CINT,TYPE,SIFS               ! DEFINE CRACK TYPE
-CINT,CTNC,CRACKTIP,NODE(-1,0,0)    !DEFINE CRACK TIP COMPONENT
-CINT,NCON,6                   ! NO OF CONTOURS
-CINT,SYMM,ON                  ! SYMMETRY ON
-CINT,NORM,0,2                 ! CRACK PLANE NORMAL
-CINT,LIST
-ALLSEL,ALL
-SAVE
-/NERR,0,,,,
-/OUT,SCRATCH
+ALLS
 SOLVE
 FINI
+
 /POST1
+SET,LAST
 /OUT,
-PRCINT,1,1,K1                  ! PRINT K VALUES 
-*GET,K,CINT,1,CTIP,NODE(0,0,0),,5,,K1    ! GET K VALUE FOR CRACK TIP NODE 
-*STATUS,K
-*DIM,LABEL,CHAR,1,
-*DIM,VALUE,,1,3
-LABEL(1,1) = 'KI ',
-*VFILL,VALUE(1,1),DATA,1.0249     ! STRESS INTENSITY VALUE OBTAINED FROM REFERENCE
-*VFILL,VALUE(1,2),DATA,K
-*VFILL,VALUE(1,3),DATA,ABS(K/1.0249)
-SAVE,TABLE_2
-FINISH
-/CLEAR, NOSTART                ! CLEAR DATABASE FOR 3RD SOLUTION
-/OUT,
+ESEL,S,ENAME,,264
+PRNSOL,BFE,TEMP
 
+*GET,MIN_GID,ELEM,,EGID,MIN
+*GET,MAX_GID,ELEM,,EGID,MAX
 
-/COM ************* CRACK IN 3D PLATE USING SOLID 186 ELEMENT ******************* C
+*DO,I,MIN_GID,MAX_GID
+  *GET,TMIN,MEMBER,I,TEMP,MIN
+  *GET,TMAX,MEMBER,I,TEMP,MAX
+*ENDDO
+/OUT,vm303_SCRATCH,,,append
 
+ALLS
+*DIM,LABEL,CHAR,1,1
+*DIM,VALUE,,1,3
+LABEL(1,1)='TMAX (C)'
+*VFILL,VALUE(1,1),DATA,128.00   ! ANALYTICAL RESULT
+*VFILL,VALUE(1,2),DATA,TMAX
+*VFILL,VALUE(1,3),DATA,ABS(TMAX/128.00)
+/COM,
+/OUT,vm303,vrt
+/COM,------- VM303 1: SOLID278 + REINF264 RESULTS COMPARISON ---------
+/COM,
+/COM,             |   TARGET   |   Mechanical APDL     |   RATIO
+/COM,
+*VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,'   ',F14.7,'  ',F14.7,'   ',1F15.3)
+/COM,-----------------------------------------------------------------
+/OUT,vm303_SCRATCH,,,append
+FINISH
+
+!-----------------------------------------------------------------
+!!!!! PART 2: SOLUTION WITH SOLID278 + LINK33 (2-NODED) !!!!!
+!-----------------------------------------------------------------
 
+/CLEAR,NOST
 /PREP7
-SMRT,OFF
-/TITLE,VM256 FRACTURE MECHANICS STRESS INTENSITY  - CRACK IN A FINITE WIDTH PLATE
-/COM,     ****** CRACK IN 3-DIMENSIONS USING SOLID186
-/COM,
-ET,1,PLANE183
-ET,2,186                      ! SOLID ELEMENT 186
-MP,EX,1,30E6
-MP,NUXY,1,0.3
-K,1                           ! DEFINE KEYPOINTS AND LINE SEGMENTS
-K,2,4
-K,3,4,5
-K,4,-1,5
-K,5,-1
-L,1,2
-L,2,3
-LESIZE,2,,,4
-L,3,4
-LESIZE,3,,,4
-L,4,5,
-LESIZE,4,,,6,.2
-L,5,1
-ESIZE,,5
-KSCON,1,.15,0,8               ! DEFINE CRACK TIP ELEMENT SIZE, NO SINGULAR ELEMENTS
-AL,1,2,3,4,5
-AMESH,1
+CDREAD,db,vm303_1,cdb
 
-TYPE,2
-ESIZE,,2
-VEXT,1,,,0,0,0.25
-ALLSEL
-ESEL,S,ENAME,,183
-ACLEAR,1
-ALLSEL
+EEMBED
+
+! APPLY HEAT GENERATION ON LINK33
+ESEL,S,ENAME,,33
+BFE,ALL,HGEN,1,HEAT
+ALLS
+
+! LIST MAPPED BODY LOADS
+ESEL,S,ENAME,,33
+BFELIST
+
+! APPLY BOUNDARY TEMPERATURES
+NSEL,S,LOC,X,0.0
+D,ALL,TEMP,20
+ALLS
+NSEL,S,LOC,X,10.0
+D,ALL,TEMP,80
+ALLS
 
-/OUT,
-NSEL,S,LOC,X,0
-NSEL,R,LOC,Y,0
-NLIST
-CM,CRACKTIP,NODE            ! CRACK TIP NODE COMPONENT
-ALLSEL,ALL
-NSEL,S,LOC,X,-1
-DSYM,SYMM,X                 ! SYMMETRY BOUNDARY CONDITIONS
-NSEL,S,LOC,X,0,4
-NSEL,R,LOC,Y,0
-DSYM,SYMM,Y                 ! SYMMETRY BOUNDARY CONDITIONS
-ALLSEL,ALL
-D,ALL,UZ,0
-ALLSEL,ALL
-NSEL,S,LOC,Y,5
-SF,ALL,PRES,-0.5641895      ! SURFACE PRESSURE
-ALLSEL,ALL
 FINI
+
 /SOLU
-AUTOTS,ON
-NSUBST,10
+TIME,1
+DELTIM,1
 OUTRES,ALL,ALL
-CINT,NEW,1                    ! CRACK ID
-CINT,TYPE,SIFS               ! DEFINE CRACK TYPE
-CINT,CTNC,CRACKTIP,NODE(-1,0,0)     !DEFINE CRACK TIP COMPONENT
-CINT,NCON,6                   ! NO OF CONTOURS
-CINT,SYMM,ON                  ! SYMMETRY ON
-CINT,NORM,0,2                 ! CRACK PLANE NORMAL
-CINT,LIST
-ALLSEL,ALL
-SAVE
-/NERR,0,,,,
-/OUT,SCRATCH
+ALLS
 SOLVE
 FINI
+
 /POST1
+SET,LAST
 /OUT,
-PRCINT,1,1,K1                  ! PRINT K VALUES 
-*GET,K,CINT,1,CTIP,NODE(0,0,0),,5,,K1    ! GET K VALUE FOR CRACK TIP NODE 
-*STATUS,K
-*DIM,LABEL,CHAR,1,
-*DIM,VALUE,,1,3
-LABEL(1,1) = 'KI ',
-*VFILL,VALUE(1,1),DATA,1.0249     ! STRESS INTENSITY VALUE OBTAINED FROM REFERENCE
-*VFILL,VALUE(1,2),DATA,K
-*VFILL,VALUE(1,3),DATA,ABS(K/1.0249)
-SAVE,TABLE_3
-FINISH
-RESUME,TABLE_1
+ESEL,S,ENAME,,33
+PRNSOL,BFE,TEMP
+NSLE
+/SHOW
+PLNSOL,TEMP
+/SHOW,CLOSE
+*GET,TMIN,plnsol,0,MIN
+*GET,TMAX,plnsol,0,MAX
 
-/COM
-/OUT,vm256,vrt
-/COM,------------------- VM256 RESULTS COMPARISON --------------
-/COM,
-/COM,           |  TARGET  |   Mechanical APDL  |  RATIO
+/OUT,vm303_SCRATCH,,,append
+
+ALLS
+*DIM,LABEL,CHAR,1,1
+*DIM,VALUE,,1,3
+LABEL(1,1)='TMAX (C)'
+*VFILL,VALUE(1,1),DATA,128.00   ! ANALYTICAL RESULT
+*VFILL,VALUE(1,2),DATA,TMAX
+*VFILL,VALUE(1,3),DATA,ABS(TMAX/128.00)
 /COM,
-/COM, ****************************************
-/COM,  USING PLANE 183 ELEMENT (2-D ANALYSIS)
-/COM, *****************************************
+/OUT,vm303,vrt,,append
+/COM,---- VM303 2: SOLID278 + LINK33 (2-NODED) RESULTS COMPARISON ----
 /COM,
-*VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
-/NOPR
-RESUME,TABLE_2
-/GOPR
-/COM,
-/COM, *****************************************
-/COM,  USING SOLID 185 ELEMENT (3-D ANALYSIS)
-/COM, *****************************************
-/COM,
-*VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
-/NOPR
-RESUME,TABLE_3
-/GOPR
-/COM,
-/COM, ********************************************************
-/COM,  USING SOLID 186 ELEMENT - SURFACE CRACK (3-D ANALYSIS)
-/COM, ********************************************************
+/COM,             |   TARGET   |   Mechanical APDL     |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
-/NOPR
-/COM,
-/COM,-----------------------------------------------------------
-/OUT
+(1X,A8,'   ',F14.7,'  ',F14.7,'   ',1F15.3)
+/COM,-----------------------------------------------------------------
+/OUT,vm303_SCRATCH,,,append
 FINISH
-*LIST,vm256,vrt
-
-
-
-
-
-
-
-
-
-
-
 
+!-----------------------------------------------------------------
+!!!!! PART 3&4 PREP:
+!-----------------------------------------------------------------
 
+/CLEAR,NOST
 
+_GEOMGEN = 0     ! SET TO 1 TO WRITE CDB FILES IF ANY INPUT FILE MODIFICATIONS
 
+/PREP7
+*IF,_GEOMGEN,EQ,1,THEN
 
+HEAT = 6         ! HEAT GENERATION IN REINFORCEMENT (W/mm^3)
 
+MP,KXX,1,1       ! THERMAL CONDUCTIVITY OF REINFORCEMENT (W/mm.C)
+MP,KXX,2,1.E-12  ! THERMAL CONDUCTIVITY OF BLOCK (NON-CONDUCTOR)
 
+! BLOCK GEOMETRY AND MESHING
+BLOCK,0,10,0,10,0,10
+ET,1,279
+TYPE,1
+MAT,2
+ESIZE,0.5
+MSHAPE,0,3D
+MSHKEY,1
+VSWEEP,1,1,2
+ALLS
+
+! REINFORCEMENT SECTION DEFINITION
+SECT,2,REINF,DISC
+SECD,1,0.0004,MESH
+SECC,,1
+SLIST
 
+! REINFORCEMENT (MESH200) GEOMETRY AND MESHING
+ET,2,200,2
+TYPE,2
+MAT,1
+SECNUM,2
+NUMSTR,LINE,1001
+K,1001,0,5,5
+K,2001,10,5,5
+L,1001,2001     ! LENGTH OF THE 1-D REINFORCEMENT = 10 mm
+LESIZE,1001,,,20
+LMESH,1001
+ALLS
+
+! APPLY HEAT GENERATION ON MESH200
+ESEL,S,ENAME,,200
+BFE,ALL,HGEN,1,HEAT
+ALLS
+
+! EMBEDDED LINK33 GEOMETRY AND MESHING
+ET,3,33
+KEYOPT,3,4,1    ! 3-NODED LINK33
+TYPE,3
+MAT,1
+R,2,0.0004
+REAL,2
+NUMSTR,LINE,1001
+K,3001,0,5,5
+K,4001,10,5,5
+L,3001,4001
+
+LESIZE,1002,,,20
+LMESH,1002
+ALLS
+
+CDWRITE,db,vm303_2,cdb
+*ELSE
+ CDREAD,db,vm303_2,cdb
+*ENDIF
+
+!-----------------------------------------------------------------
+!!!!! PART 3: SOLUTION WITH SOLID279 + REINF264  !!!!!
+!-----------------------------------------------------------------
+
+! GENERATE REINFORCING ELEMENTS FROM MESH200
+SECNUM,2
+EREINF
+ALLS
+
+! LIST MAPPED BODY LOADS
+ESEL,S,ENAME,,264
+BFELIST
+
+! APPLY BOUNDARY TEMPERATURES
+NSEL,S,LOC,X,0.0
+D,ALL,TEMP,20
+ALLS
+NSEL,S,LOC,X,10.0
+D,ALL,TEMP,80
+ALLS
 
+FINI
 
+/SOLU
+TIME,1
+DELTIM,1
+OUTRES,ALL,ALL
+ALLS
+SOLVE
+FINI
 
+/POST1
+SET,LAST
+/OUT,
+ESEL,S,ENAME,,264
+PRNSOL,BFE,TEMP
 
+*GET,MIN_GID,ELEM,,EGID,MIN
+*GET,MAX_GID,ELEM,,EGID,MAX
 
+*DO,I,MIN_GID,MAX_GID
+  *GET,TMIN,MEMBER,I,TEMP,MIN
+  *GET,TMAX,MEMBER,I,TEMP,MAX
+*ENDDO
+/OUT,vm303_SCRATCH,,,append
 
+ALLS
+*DIM,LABEL,CHAR,1,1
+*DIM,VALUE,,1,3
+LABEL(1,1)='TMAX (C)'
+*VFILL,VALUE(1,1),DATA,128.00   ! ANALYTICAL RESULT
+*VFILL,VALUE(1,2),DATA,TMAX
+*VFILL,VALUE(1,3),DATA,ABS(TMAX/128.00)
+/COM,
+/OUT,vm303,vrt,,append
+/COM,------- VM303 3: SOLID279 + REINF264 RESULTS COMPARISON ---------
+/COM,
+/COM,             |   TARGET   |   Mechanical APDL     |   RATIO
+/COM,
+*VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,'   ',F14.7,'  ',F14.7,'   ',1F15.3)
+/COM,-----------------------------------------------------------------
+/OUT,vm303_SCRATCH,,,append
+FINISH
 
+!-----------------------------------------------------------------
+!!!!! PART 4: SOLUTION WITH SOLID279 + LINK33 (3-NODED) !!!!!
+!-----------------------------------------------------------------
+/CLEAR,NOST
+/PREP7
+CDREAD,db,vm303_2,cdb
 
+EEMBED
 
+! APPLY HEAT GENERATION ON LINK33
+ESEL,S,ENAME,,33
+BFE,ALL,HGEN,1,HEAT
+ALLS
+
+! LIST MAPPED BODY LOADS
+ESEL,S,ENAME,,33
+BFELIST
+
+! APPLY BOUNDARY TEMPERATURES
+NSEL,S,LOC,X,0.0
+D,ALL,TEMP,20
+ALLS
+NSEL,S,LOC,X,10.0
+D,ALL,TEMP,80
+ALLS
 
+FINI
 
+/SOLU
+TIME,1
+DELTIM,1
+OUTRES,ALL,ALL
+ALLS
+SOLVE
+FINI
 
+/POST1
+SET,LAST
+/OUT,
+ESEL,S,ENAME,,33
+PRNSOL,BFE,TEMP
+NSLE
+/SHOW
+PLNSOL,TEMP
+/SHOW,CLOSE
+*GET,TMIN,plnsol,0,MIN
+*GET,TMAX,plnsol,0,MAX
 
+/OUT,vm303_SCRATCH,,,append
 
+ALLS
+*DIM,LABEL,CHAR,1,1
+*DIM,VALUE,,1,3
+LABEL(1,1)='TMAX (C)'
+*VFILL,VALUE(1,1),DATA,128.00   ! ANALYTICAL RESULT
+*VFILL,VALUE(1,2),DATA,TMAX
+*VFILL,VALUE(1,3),DATA,ABS(TMAX/128.00)
+/COM,
+/OUT,vm303,vrt,,append
+/COM,---- VM303 4: SOLID279 + LINK33 (3-NODED) RESULTS COMPARISON ----
+/COM,
+/COM,             |   TARGET   |   Mechanical APDL     |   RATIO
+/COM,
+*VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,'   ',F14.7,'  ',F14.7,'   ',1F15.3)
+/COM,-----------------------------------------------------------------
+/OUT
+FINISH
+*LIST,vm303,vrt
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm257.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm257.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM257
 JPGPRF,500,100,1                     ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE,VM257,SWING COMPRISING TWO RIGID LINKS AND A BEAM WITH MIDSPAN MASS
 /COM    O.A. BAUCHAU. G. DAMILANO AND N.J. THERON
 /COM    NUMERICAL INTEGRATION OF NON-LINEAR ELASTIC MULTI-BODY SYSTEMS
 /COM    INTERNATIONAL JOURNAL FOR NUMERICAL METHODS IN  ENGINEERING,
@@ -80,15 +80,15 @@
 TOT_TIME = 1.0
 TIME,TOT_TIME
 NSUBST,1000,10E5,1000
 CNVTOL,F                   ! FORCE CONVERGENCE CHECK
 CNVTOL,M, , , ,1E-3        ! MOMENT CONVERGENCE CHECK
 CNVTOL,U                   ! DISPLACEMENT CONVERGENCE CHECK
 CNVTOL,ROT                 ! ROTATION CONVERGENCE CHECK
-/OUT,scratch
+/OUT,vm257_SCRATCH
 SOLVE
 /OUT
 FINISH
 /AUTO,1
 /DIST,  1, 0
 /REPLO  
 /VIEW,1,,,1
@@ -224,15 +224,15 @@
 NSUBST,1000,1000,1000      
 CNVTOL,U                   ! DISPLACEMENT CONVERGENCE CHECK
 CNVTOL,ROT                 ! ROTATION CONVERGENCE CHECK
 CNVTOL,F                   ! FORCE CONVERGENCE CHECK
 CNVTOL,M, , , ,0.01        ! MOMENT CONVERGENCE CHECK
 PRED,OFF
 LNSRCH,OFF
-/OUT,scratch
+/OUT,vm257_SCRATCH,,,APPEND
 SOLVE
 FINISH
 /DIST,1,0
 /AUTO,1
 /REPLO
 /VIEW,1,,,1
 /ANG,1
@@ -303,9 +303,10 @@
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
 /COM,-----------------------------------------------------------
 /COM,
 /OUT
 FINISH
 *LIST,vm257,vrt
+/OUT,vm257_SCRATCH,,,APPEND
 /DELETE,TABLE_1
 /DELETE,TABLE_2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm258.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm258.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM258
 /TITLE,VM258,SPIN-UP MANEUVER OF A FLEXIBLE BEAM
 /COM,   J.C. SIMO AND L. VU-QUOC
 /COM    ON THE DYNAMICS IN SPACE OF RODS UNDERGOING LARGE MOTIONS-
 /COM,   -A GEOMETRICALLY EXACT APPROACH
 /COM,   COMPUTER METHODS IN APPLIED MECHANICS AND ENGINEERING, VOL. 66,
 /COM,   125-161 (1988.
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm259.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm259.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM259
 JPGPRF,500,100,1
 /SHOW,JPEG
 /COM,  VERIFICATION MANUAL FOR SPRS ANALYSIS WITH MISSING MASS AND RIGID RESPONSES, REL 12.0
 /TITLE,VM259,MISSING MASS WITH RIGID RESPONSES EFFECTS IN SPECTRUM ANALYSIS FOR BM3 PIPING MODEL
 /COM, REFERENCE: " REEVALUATION OF REGULATORY GUIDANCE ON MODAL RESPONSE COMBINATION 
 /COM,              METHODS FOR SEISMIC RESPONSE SPECTRUM ANALYSIS"
@@ -623,32 +623,7 @@
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 /NOPR
 /COM,
 /COM,---------------------------------------------------------------------------------------
 /OUT
 *LIST,vm259,vrt
 FINISH
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm26.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm26.dat`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,vm26
 /FILNAM,vm26
 /PREP7
-/TITLE, VM26  LARGE DEFLECTION OF A CANTILEVERED PLATE
+/TITLE, VM26, LARGE DEFLECTION OF A CANTILEVERED PLATE
 /COM   REF: BATHE AND DVORKIN, " A FORMULATION OF GENERAL SHELL ELEMENTS... "
 /COM                             IJNME, VOL 22, NO. 3 (1986) PAGE 720
 /COM   USING SHELL181 ELEMENTS
-/OUT,SCRATCH
+/OUT,vm26_SCRATCH
 /NOPR
-SMRT,OFF 
 ANTYPE,STATIC           ! STATIC ANALYSIS
 NLGEOM,ON               ! LARGE DEFLECTION OPTION
 ET,1,SHELL181,,,2
 SECTYPE,1,SHELL
 SECDATA,1,1,0,5         ! PLATE THICKNESS = 1
 MP,EX,1,1800            ! MATERIAL PROPERTIES
 MP,NUXY,1,0
-K,1                     ! DEFINE KEYPOINTS
-K,2,12
-K,3,12,1
-K,4,,1
-L,1,2                   ! DEFINE LINE SEGMENTS 
-L,3,4
-LESIZE,ALL,,,2          ! 2 DIVISIONS ALONG LENGTH
-ESIZE,,1                ! ONE DIVISION ON UNSPECIFIED LINE SEGMENTS
-A,1,2,3,4
-AMESH,1                 ! CREATE MESH
+N,1                     ! DEFINE MODEL
+N,2,12
+N,3,6
+N,4,12,1
+N,5,0,1
+N,6,6,1
+E,1,3,6,5
+E,3,2,4,6
 NSEL,S,LOC,X
 D,ALL,ALL               ! FIXED END B.C.'S
 NSEL,S,LOC,X,12
 CP,1,ROTY,ALL           ! COUPLE ROTATIONS AT FREE END
 TORQ=7.854              ! DEFINE HALF TOTAL LOAD
 F,2,MY,TORQ
 NSEL,ALL                ! RESELECT ALL NODES 
 FINISH
-/SOLU    
+/SOLU
+DMPOPT,RNNN,YES    
 AUTOTS,ON               ! USE AUTOMATIC LOAD STEPPING
 NSUBST,10,100,10        ! START WITH MAX OF 10 SUBSTEPS FOR EACH LOAD STEP
 CNVTOL,F,1,1.0E-2		! FORCE CONVERGENCE
 CNVTOL,U,1,1.0E-2		! DISPLACEMENT CONVERGENCE
 LNSRCH,ON               ! USE LINE SEARCH METHOD
 OUTPR,BASIC,LAST        ! BASIC PRINTOUT IN THE LAST SUBSTEP
 OUTRES,ALL,ALL          ! WRITE SOLUTION TO THE RESULTS FILE FOR EACH SUBSTEP
 SOLVE
 FINISH
-! THE FOLLOWING 4 COMMANDS ARE NOT NEEDED SINCE THE INITIAL AND THE
-! RESTART ANALYSES ARE IN ONE Mechanical APDL RUN. THE USE OF THESE COMMANDS WAS DONE 
-! IN ORDER TO DEMONSTRATE THE USE OF THE FILES NEEDED FOR A RESTART 
-/COPY,vm26,rdb,,vm26r,rdb      ! COPY THE FILES NEEDED FOR RESTART TO
-/COPY,vm26,ldhi,,vm26r,ldhi    ! FILES NAMED VM26R.***
-/COPY,vm26,r001,,vm26r,r001    !
-/COPY,vm26,rst,,vm26r,rst      ! NEEDED FOR POSTPROCESSOR ONLY
-/CLEAR,NOSTART                 ! CLEAR THE DATA BASE
-/FILNAM,vm26r                  ! CONTINUE WITH FILES NAMED VM26R.***
+
+/CLEAR,NOSTART          ! CLEAR THE DATA BASE
 /SOLU      
 ANTYPE,,REST            ! RESTART ANALYSIS
 F,2,MY,TORQ*2           ! APPLY FULL LOAD
 SOLVE
 FINISH
 /POST1
 RSYS,SOLU               ! CHOOSE "AS-GENERATED" COORDINATE SYSTEM
@@ -73,42 +64,42 @@
 LABEL(1,1) = 'UX,NODE ','UZ,NODE ','ROTY,NOD','STS_X,N_'
 LABEL(1,2) = '4 (mm)  ','4 (mm)  ','E 4(rad)','1 N/mm^2'
 *VFILL,VALUE(1,1),DATA,-2.9,-6.5,1.26,94.25
 *VFILL,VALUE(1,2),DATA,UX_N4,UZ_N4,ROTY_N4,STRSS_N1
 *VFILL,VALUE(1,3),DATA,ABS(UX_N4/2.9),ABS(UZ_N4/6.5),ABS(ROTY_N4/1.26),ABS(STRSS_N1/94.25)
 SAVE,TABLE_1
 FINISH
-/DELETE,vm26r,rdb
-/DELETE,vm26r,ldhi
-/DELETE,vm26r,r001
-/DELETE,vm26r,rst
-/CLEAR,NOSTART
 
-/TITLE, VM26  LARGE DEFLECTION OF A CANTILEVERED PLATE
+/CLEAR,NOSTART
+/TITLE, VM26, LARGE DEFLECTION OF A CANTILEVERED PLATE
 /COM          USING SHELL281 ELEMENTS
 /PREP7
-smrt,off
 /NOPR
 ANTYPE,STATIC           ! STATIC ANALYSIS
 NLGEOM,ON               ! LARGE DEFLECTION OPTION
 ET,1,SHELL281
 SECTYPE,1,SHELL
 SECDATA,1,1,0,5		! PLATE THICKNESS = 1
 MP,EX,1,1800            ! MATERIAL PROPERTIES
 MP,NUXY,1,0
-K,1                     ! DEFINE KEYPOINTS
-K,2,12
-K,3,12,1
-K,4,,1
-L,1,2                   ! DEFINE LINE SEGMENTS 
-L,3,4
-LESIZE,ALL,,,2          ! 2 DIVISIONS ALONG LENGTH
-ESIZE,,1                ! ONE DIVISION ON UNSPECIFIED LINE SEGMENTS
-A,1,2,3,4
-AMESH,1                 ! CREATE MESH
+N,1                     ! DEFINE MODEL
+N,2,12
+N,3,3
+N,4,6
+N,5,9
+N,6,12,1
+N,7,12,0.5
+N,8,0,1
+N,9,9,1
+N,10,6,1
+N,11,3,1
+N,12,0,0.5
+N,13,6,0.5
+E,1,4,10,8,3,13,11,12
+E,4,2,6,10,5,7,9,13
 NSEL,S,LOC,X
 D,ALL,ALL               ! FIXED END B.C.'S
 NSEL,S,LOC,X,12
 CP,1,ROTY,ALL           ! COUPLE ROTATIONS AT FREE END
 TORQ=7.854              ! DEFINE HALF TOTAL LOAD
 F,2,MY,TORQ
 NSEL,ALL                ! RESELECT ALL NODES
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm260.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm260.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM260
 /OUT,SCRATCH
 JPGPRF,500,100,1
 /SHOW,JPEG
 /COM, VERFICATION MANUAL FOR TWO DIMENSIONAL CONSOLIDATION PROBLEM
 /TITLE,VM260,TWO DIMENSIONAL CONSOLIDATION SETTLEMENT UNDER A RECTANGULAR LOAD
 C*** USING CPT212
@@ -11,14 +11,15 @@
 /COM,
 /PREP7
 W=1						! RECTANGULAR LOAD HALF-WIDTH
 E=1000						! YOUNG'S MODULUS
 A=4						! REFINEMENT COEFFICIENT
 R=100						! LOADING
 ET,1,CPT212					! 2D 4 NODE COUPLED PORE PRESSURE ELEMENT
+KEYOPT,1,12,1 			         
 KEYOPT,1,3,2					! PLANE STRAIN CONDISTIONS
 RECT,0,6*W,0,-9*W				! AREA 6*W BY 9*W
 LESIZE,3,,,12*A/W				! 12*A ELEMENTS ON HORIZONTAL EDGES
 LESIZE,4,,,18*A/W				! 18*A ELEMENTS ON VERTICAL EDGES
 AMAP,1,1,2,3,4
 
 MP,EX,1,E
@@ -160,14 +161,15 @@
 C*** USING CPT213
 /PREP7
 W=1							! RECTANGULAR LOAD HALF-WIDTH
 E=1000							! YOUNG'S MODULUS
 A=4							! REFINEMENT COEFFICIENT
 R=100							! LOADING
 ET,1,CPT213						! 2D 8 NODE COUPLED PORE PRESSURE ELEMENT
+KEYOPT,1,12,1 			         
 KEYOPT,1,3,2						! PLANE STRAIN CONDISTIONS
 RECT,0,6*W,0,-9*W					! AREA 6*W BY 9*W
 LESIZE,3,,,6*A/W					! 6*A ELEMENTS ON HORIZONTAL EDGES
 LESIZE,4,,,9*A/W					! 9*A ELEMENTS ON VERTICAL EDGES
 AMAP,1,1,2,3,4
 
 MP,EX,1,E
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm261.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm261.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM261
 JPGPRF,500,100,1
 /SHOW,JPEG
 /COM, VERIFICATION MANUAL FOR ROTATING BEAM WITH INTERNAL VISCOUS DAMPING
 /TITLE,VM261,ROTATING BEAM WITH INTERNAL VISCOUS DAMPING
 /COM,  REFERENCE: " FINITE ELEMENT SIMULATION OF ROTOR-BEARING SYSTEMS
 /COM,               WITH INTERNAL DAMPING",ASME JOURNAL OF ENGINEERING 
@@ -162,8 +162,9 @@
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,4),VALUE(4,1),VALUE(4,2),VALUE(4,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 /COM, ----------------------------------------------------------------------------
 /OUT,
 *LIST,vm261,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm262.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm262.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM262
 JPGPRF,500,100,1
 /SHOW,JPEG
 /COM,VERFICATION MANUAL FOR TWO DIMENSIONAL THERMAL FRACTURAL PROBLEM
 /TITLE,VM262,TWO DIMENSIONAL FRACTURAL PROBLEM UNDER THERMAL LOAD
 /COM, REFERENCE: "W.K.WILSON, ET AL., THE USE OF THE J-INTEGRAL IN THERMAL STRESS CRACK PROBLEMS
 /COM,             INTERNATIONAL JOURNAL OF FRACTURE, 1979,PG:377-387
 /COM,
-/OUT,SCRATCH
+
+/COM, PARAMETER FOR CREATING THE CDB FILES TO STORE GEOMETRY AND MESH DATA
+/COM,
+_GEOMGEN = 0   ! SET TO 1 TO WRITE CDB FILES IF ANY INPUT FILE MODIFICATIONS
+PARSAV
+/OUT,vm262_scratch
+
 /PREP7
+*IF,_GEOMGEN,EQ,1,THEN
 A=1                    ! CRACK LENGTH
 W=2*A                  ! WIDTH
 L=4*W                  ! LENGTH
 L2=L/2                 ! HALF OF LENGTH
 E=1E5                  ! YOUNG'S MODULUS 
 NU=0.3                 ! POISSONS RATIO
 T0=10                  ! TEMPERATURES AT THE RIGHT SIDE
@@ -37,14 +44,19 @@
 KEYOPT,1,3,2            ! PLANE STRAIN
 
 ESIZE,A/6
 KSCON,1,A/12,1,8
 AMESH,1
 ESIZE,W/6
 AMESH,2
+ALLSEL,ALL
+CDWRITE,DB,vm262,cdb
+ *ELSE
+  CDREAD,DB,vm262,cdb
+*ENDIF
 
 NSEL,S,LOC,X,0,W/2      ! SYMMETRICAL CONDITIONS
 NSEL,R,LOC,Y,0
 D,ALL,UY,0
 NSEL,ALL
 
 NSEL,S,LOC,Y,L2         ! TOP EDGE FIXED
@@ -79,15 +91,15 @@
 CINT,NORM,,
 CINT,LIST
 ALLSEL
 /OUT,
 SOLVE
 FINISH
 
-/OUT,SCRATCH
+/OUT,vm262_scratch,,,APPEND
 /POST1
 PRCINT,1
 *GET,J1,CINT,1,CTIP,1,,1
 *GET,J2,CINT,1,CTIP,1,,2
 *GET,J3,CINT,1,CTIP,1,,3
 *GET,J4,CINT,1,CTIP,1,,4
 *GET,J5,CINT,1,CTIP,1,,5
@@ -102,17 +114,17 @@
 *STAT,K1_EXPECT
 *DIM,LABEL,CHAR,1,1
 *DIM,VALUE,,1,3
 LABEL(1,1) = 'K1'
 *VFILL,VALUE(1,1),DATA,K1_EXPECT
 *VFILL,VALUE(1,2),DATA,K1
 *VFILL,VALUE(1,3),DATA,ABS(K1/K1_EXPECT)
-SAVE,TABLE_1
+SAVE,vm262_TABLE_1
 FINISH
-RESUME,TABLE_1
+RESUME,vm262_TABLE_1
 /COM,
 /OUT,vm262,vrt
 /COM,
 /COM,
 /COM, ----------------------VM262 RESULTS COMPARISON------------------------
 /COM,
 /COM,           |  TARGET  |   Mechanical APDL  |  RATIO
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm263.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm263.dat`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM263
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE,VM263,CRITICAL SPEEDS FOR ROTOR-BEARING SYSTEM WITH AXISYMMETRIC ELEMENTS
 C*** USING SOLID272
 /COM,  REF: "THE DYNAMICS OF ROTOR-BEARING SYSTEMS USING FINITE ELEMENTS"
 /COM,        JOURNAL OF ENG. FOR INDUSTRY - MAY 1976
@@ -139,15 +139,15 @@
 
 /COM, MODELING DISC ELEMENT
 ET,2,SOLID272,,3
 TYPE,2
 MP,EX,2,2.078E11
 MP,DENS,2,7806
 MP,NUXY,2,0.33
-TH = 0.028											! THICKNESS OF THE DISC
+TH = 0.0254											! THICKNESS OF THE DISC
 RADD = 0.0495										! OUTER RADIUS OF THE DISC
 RADS = 0.0203										! INNER RADIUS OF THE DISC
 K,100,8.89E-2-(TH/2),RADS,0
 K,101,8.89E-2-(TH/2),RADD,0
 K,102,8.89E-2+(TH/2),RADD,0
 K,103,8.89E-2+(TH/2),RADS,0
 A,100,101,102,103
@@ -290,15 +290,344 @@
 *VFILL,VALUE(12,1),DATA,20162.25         						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
 *VFILL,VALUE(12,2),DATA,CRIC12
 *VFILL,VALUE(12,3),DATA,ABS(CRIC12/20162)
 SAVE,INF1
 FINISH
 /CLEAR,NOSTART
 
+/TITLE,VM263,CRITICAL SPEEDS FOR ROTOR-BEARING SYSTEM WITH AXISYMMETRIC ELEMENTS
+C*** USING SOLID272 AND CMS SUBSTRUCTURE ANALYSIS
+
+/PREP7
+MP,EX,1,2.078e+11
+MP,DENS,1,7806
+MP,NUXY,1,0.33
+ET,1,SOLID272,,3										! 3 CIRCUMFERENTIAL NODES
+TYPE,1
+NBDIAM = 18											! SHAFT SECTION PROPERTIES
+*DIM,DIAM,ARRAY,NBDIAM
+DIAM(1) = 1.02E-2
+DIAM(2) = 2.04E-2
+DIAM(3) = 1.52E-2
+DIAM(4) = 4.06E-2
+DIAM(5) = DIAM(4)
+DIAM(6) = 6.6E-2
+DIAM(7) = DIAM(6)
+DIAM(8) = 5.08E-2
+DIAM(9) = DIAM(8)
+DIAM(10) = 2.54E-2
+DIAM(11) = DIAM(10)
+DIAM(12) = 3.04E-2
+DIAM(13) = DIAM(12)
+DIAM(14) = 2.54E-2
+DIAM(15) = DIAM(14)
+DIAM(16) = 7.62E-2
+DIAM(17) = 4.06E-2
+DIAM(18) = DIAM(17)
+
+/COM, MODELING SHAFT ELEMENTS
+K,1,,,,
+K,2,,DIAM(1)/2,,
+K,3,1.27E-2,DIAM(1)/2,,
+K,4,1.27E-2,0,0
+A,1,2,3,4
+
+K,5,1.27E-2,DIAM(2)/2,0
+K,6,5.08E-2,DIAM(2)/2,0
+K,7,5.08E-2,DIAM(3)/2,0
+K,8,5.08E-2,0,0
+A,4,3,5,6,7,8
+
+K,9,7.62E-2,DIAM(3)/2,0
+K,10,7.62E-2,0,0
+A,8,7,9,10
+
+K,11,7.62E-2,DIAM(4)/2
+K,12,8.89E-2,DIAM(4)/2
+K,13,8.89E-2,0,0
+A,10,9,11,12,13
+
+K,14,10.16E-2,DIAM(5)/2
+K,15,10.16E-2,0,0
+A,13,12,14,15
+
+K,16,10.16E-2,DIAM(6)/2
+K,17,10.67E-2,DIAM(6)/2
+K,18,10.67E-2,3.04E-2/2
+K,19,10.67E-2,0,0
+A,15,14,16,17,18,19
+
+K,20,11.43E-2,DIAM(7)/2
+K,21,11.43E-2,DIAM(8)/2
+K,22,11.43E-2,3.56E-2/2
+K,23,11.43E-2,3.04E-2/2
+A,18,17,20,21,22,23
+
+K,24,12.7E-2,DIAM(8)/2,0
+K,25,12.7E-2,3.56E-2/2,0
+A,22,21,24,25
+
+K,26,12.7E-2,0,0
+K,27,13.46E-2,DIAM(9)/2
+K,28,13.46E-2,DIAM(10)/2
+K,29,13.46E-2,0,0
+A,26,25,24,27,28,29
+
+K,30,16.51E-2,DIAM(10)/2
+K,31,16.51E-2,0,0
+A,29,28,30,31
+
+K,32,19.05E-02,DIAM(11)/2
+K,33,19.05E-02,0,0
+A,31,30,32,33
+
+K,34,19.05E-2,DIAM(12)/2
+K,35,22.86E-02,DIAM(12)/2
+K,36,22.86E-02,0,0
+A,33,32,34,35,36
+
+K,37,26.67E-2,DIAM(13)/2
+K,38,26.67E-2,DIAM(14)/2
+K,39,26.67E-2,0,0
+A,36,35,37,38,39
+
+K,40,28.7E-2,DIAM(14)/2,0
+K,41,28.7E-2,0,0
+A,39,38,40,41
+
+K,42,30.48E-2,DIAM(15)/2,0
+K,43,30.48E-2,0,0
+A,41,40,42,43
+
+K,44,30.48E-2,DIAM(16)/2
+K,45,31.5E-2,DIAM(16)/2
+K,46,31.5E-2,DIAM(17)/2
+K,47,31.5E-2,0,0
+A,43,42,44,45,46,47
+
+K,48,34.54E-2,DIAM(17)/2,,
+K,49,34.54E-2,3.04E-2/2,,
+K,50,34.54E-2,0,0
+A,47,46,48,49,50
+
+K,51,35.5E-2,DIAM(18)/2
+K,52,35.5E-2,3.04E-2/2
+A,49,48,51,52
+ESIZE,0.5E-2
+SECT,1,AXIS
+SECDATA,1,0,0,0,1,0,0
+AMESH,ALL
+
+/COM, MODELING DISC ELEMENT
+ET,2,SOLID272,,3
+TYPE,2
+MP,EX,2,2.078E11
+MP,DENS,2,7806
+MP,NUXY,2,0.33
+TH = 0.0254										! THICKNESS OF THE DISC
+RADD = 0.0495										! OUTER RADIUS OF THE DISC
+RADS = 0.0203										! INNER RADIUS OF THE DISC
+K,100,8.89E-2-(TH/2),RADS,0
+K,101,8.89E-2-(TH/2),RADD,0
+K,102,8.89E-2+(TH/2),RADD,0
+K,103,8.89E-2+(TH/2),RADS,0
+A,100,101,102,103
+TYPE,2
+MAT,2
+AMESH,19
+SECT,2,AXIS
+SECDATA,1,0,0,0,1,0,0
+ALLSEL,ALL
+
+/COM, GENERATING AXISYMMETRIC SOLID ELEMENTS FOR DISC AND SHAFT
+NAXIS
+ALLSEL,ALL
+NUMMRG,NODE
+NUMMRG,KP
+ALLSEL,ALL
+FINISH
+
+/COM, GENERATION PASS
+/COM,
+
+/FILNAM,rotor_disc
+/SOLUTION
+ANTYPE,SUBSTRUCTURE
+SEOPT,rotor_disc,3,									! GENERATE K,M and C MATRICES
+CMSOPT,FIX,20										! FIXED INTERFACE METHOD
+M,NODE(16.51E-02,0,0),ALL								! MASTER NODES FOR BEARING DEFINITION
+M,NODE(28.70E-02,0,0),ALL
+NSEL,S,LOC,Y,0
+NSEL,R,LOC,Z,0
+M,ALL,ALL										! MASTER NODES FOR DEFINING BC
+ALLSEL,ALL
+
+NSEL,S,LOC,X,0
+NSEL,A,LOC,X,35.5E-02
+M,ALL,ALL										! MASTER NODES FOR INTERFACES
+ALLSEL,ALL
+OMEGA,1,0,0										! OMEGA ALONG X AXIS
+CORIOLIS,ON,,,ON									! CORIOLIS ON IN A STATIONARY REFERENCE FRAME
+SOLVE
+SAVE
+FINISH
+/CLEAR,NOSTART
+
+/COM, USE PASS
+/COM,
+
+/FILNAM,use
+/PREP7
+ET,1,MATRIX50
+TYPE,1
+SE,rotor_disc									! SUPER ELEMENT OF SHAFT + DISC
+
+ESEL,S,ELEM,,1
+CM,rot1,ELEM										! ELEMENT COMPONENT
+ESEL,ALL
+
+/COM, MODELING SYMMETRIC BEARINGS 
+ET,3,COMBIN14
+KEYOPT,3,2,2										! BEARING IN Y DIRECTION
+ET,5,COMBIN14
+KEYOPT,5,2,3										! BEARING IN Z DIRECTION
+R,3,4.378E+7
+R,5,4.378E+7
+DIST = 0.000										! FOR VISUALIZATION
+N,10000,16.51E-2,DIST,0
+N,20000,16.51E-2,0,DIST
+N,10001,28.70E-2,DIST,0
+N,20001,28.70E-2,0,DIST
+TYPE,3
+REAL,3
+E,NODE(16.51E-02,0,0),10000
+E,NODE(28.70E-02,0,0),10001
+TYPE,5
+REAL,5
+E,NODE(16.51E-02,0,0),20000
+E,NODE(28.70E-02,0,0),20001
+
+/COM, CONSTRAINING ALL BEARING NODES
+D,10000,ALL,0
+D,10001,ALL,0
+D,20000,ALL,0
+D,20001,ALL,0
+ALLSEL,ALL
+
+/COM, SUPPRESSING AXIAL MOTION IN THE SHAFT
+NSEL,S,LOC,Y,0
+NSEL,R,LOC,Z,0
+D,ALL,UX,0
+NSEL,ALL
+FINI
+
+/COM, PERFORMING CAMPBELL ANALYSIS USING QRDAMP EIGEN SOLVER
+/SOLU
+ANTYPE,MODAL
+MODOPT,DAMP,25,1.0,,								      	! COMPUTE COMPLEX EIGEN MODES USING DAMP SOLVER
+MXPAND,25,,,YES										! EXPAND ALL THE MODES WITH STRESS CALCULATION ON
+CORIOLIS,ON,,,ON									! CORIOLIS ON IN A STATIONARY REFERENCE FRAME
+RATIO = 4*ATAN(1)/30	
+
+*DIM,SPIN,,7
+SPIN(1) = 0
+SPIN(2) = 10000
+SPIN(3) = 20000
+SPIN(4) = 40000
+SPIN(5) = 60000
+SPIN(6) = 80000
+SPIN(7) = 100000
+											! CONVERT RPM INTO RADIANS/SECOND
+*DO,I,1,7
+CMOMEGA,rot1,SPIN(I)*RATIO								! SOLVE FOR DIFFERENT ROTATIONAL VELOCITY
+SOLVE
+*ENDDO
+FINI
 
+/POST1
+file,use,rst
+/OUT,
+PRCAMP,ON,2.0,RPM,,rot1								! PRINT CAMPBELL VALUES FOR SLOPE = 2.0 IN RPM
+PLCAMP,,2.,RPM,,rot1
+*GET,CRIC1,CAMP,1,VCRI,,,
+*GET,CRIC2,CAMP,2,VCRI,,,
+*GET,CRIC3,CAMP,3,VCRI,,,
+*GET,CRIC4,CAMP,4,VCRI,,,
+*GET,CRIC5,CAMP,5,VCRI,,,
+*GET,CRIC6,CAMP,6,VCRI,,,
+
+PRCAMP,ON,4.,RPM,,rot1					 	   			! PRINT CAMPBELL VALUES FOR SLOPE = 4.0 IN RPM
+PLCAMP,,4.,RPM,,rot1
+*GET,CRIC7,CAMP,1,VCRI,,,
+*GET,CRIC8,CAMP,2,VCRI,,,
+*GET,CRIC9,CAMP,3,VCRI,,,
+*GET,CRIC10,CAMP,4,VCRI,,,
+*GET,CRIC11,CAMP,5,VCRI,,,
+*GET,CRIC12,CAMP,6,VCRI,,,
+
+/OUT,SCRATCH
+*DIM,LABEL,CHAR,1,12
+*DIM,VALUE,,12,3
+LABEL(1,1) = 'CRIC1'
+LABEL(1,2) = 'CRIC2'
+LABEL(1,3) = 'CRIC3'
+LABEL(1,4) = 'CRIC4'
+LABEL(1,5) = 'CRIC5'
+LABEL(1,6) = 'CRIC6'
+LABEL(1,7) = 'CRIC7'
+LABEL(1,8) = 'CRIC8'
+LABEL(1,9) = 'CRIC9'
+LABEL(1,10) = 'CRIC10'
+LABEL(1,11) = 'CRIC11'
+LABEL(1,12) = 'CRIC12'
+/COM,
+/COM, WHIRL SPEEDS OBTAINED FOR SLOPE = 2.0 (REFERENCE RESULTS FOR WHIRL RATIO 1/2)
+/COM,
+*VFILL,VALUE(1,1),DATA,7929             						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/2
+*VFILL,VALUE(1,2),DATA,CRIC1
+*VFILL,VALUE(1,3),DATA,ABS(CRIC1/7929)
+*VFILL,VALUE(2,1),DATA,8350             						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/2
+*VFILL,VALUE(2,2),DATA,CRIC2
+*VFILL,VALUE(2,3),DATA,ABS(CRIC2/8350)
+*VFILL,VALUE(3,1),DATA,23760             						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/2
+*VFILL,VALUE(3,2),DATA,CRIC3
+*VFILL,VALUE(3,3),DATA,ABS(CRIC3/23760)
+*VFILL,VALUE(4,1),DATA,24602             						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/2
+*VFILL,VALUE(4,2),DATA,CRIC4
+*VFILL,VALUE(4,3),DATA,ABS(CRIC4/24602)
+*VFILL,VALUE(5,1),DATA,34820             						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/2
+*VFILL,VALUE(5,2),DATA,CRIC5
+*VFILL,VALUE(5,3),DATA,ABS(CRIC5/34820)
+*VFILL,VALUE(6,1),DATA,42776             						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/2
+*VFILL,VALUE(6,2),DATA,CRIC6
+*VFILL,VALUE(6,3),DATA,ABS(CRIC6/42776)
+/COM,
+/COM, WHIRL SPEEDS OBTAINED FOR SLOPE = 4.0 (REFERENCE RESULTS FOR WHIRL RATIO 1/4)
+/COM,
+*VFILL,VALUE(7,1),DATA,4015              						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
+*VFILL,VALUE(7,2),DATA,CRIC7
+*VFILL,VALUE(7,3),DATA,ABS(CRIC7/4015)
+*VFILL,VALUE(8,1),DATA,4120.25           						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
+*VFILL,VALUE(8,2),DATA,CRIC8
+*VFILL,VALUE(8,3),DATA,ABS(CRIC8/4120)
+*VFILL,VALUE(9,1),DATA,11989.25          						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
+*VFILL,VALUE(9,2),DATA,CRIC9
+*VFILL,VALUE(9,3),DATA,ABS(CRIC9/11989)
+*VFILL,VALUE(10,1),DATA,12200            						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
+*VFILL,VALUE(10,2),DATA,CRIC10
+*VFILL,VALUE(10,3),DATA,ABS(CRIC10/12200)
+*VFILL,VALUE(11,1),DATA,18184.25         						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
+*VFILL,VALUE(11,2),DATA,CRIC11
+*VFILL,VALUE(11,3),DATA,ABS(CRIC11/18184)
+*VFILL,VALUE(12,1),DATA,20162.25         						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
+*VFILL,VALUE(12,2),DATA,CRIC12
+*VFILL,VALUE(12,3),DATA,ABS(CRIC12/20162)
+SAVE,INF2
+FINISH
+/CLEAR,NOSTART
 
 
 /TITLE,VM263,CRITICAL SPEEDS FOR ROTOR-BEARING SYSTEM WITH AXISYMMETRIC ELEMENTS
 C*** USING SOLID273
 /PREP7
 *DIM,SPIN,,7
 SPIN(1) = 0
@@ -429,15 +758,15 @@
 
 /COM, MODELING DISC ELEMENT
 ET,2,SOLID273,,3
 TYPE,2
 MP,EX,2,2.078E11
 MP,DENS,2,7806
 MP,NUXY,2,0.33
-TH = 0.028											! THICKNESS OF THE DISC
+TH = 0.0254										! THICKNESS OF THE DISC
 RADD = 0.0495										! OUTER RADIUS OF THE DISC
 RADS = 0.0203										! INNER RADIUS OF THE DISC
 K,100,8.89E-2-(TH/2),RADS,0
 K,101,8.89E-2-(TH/2),RADD,0
 K,102,8.89E-2+(TH/2),RADD,0
 K,103,8.89E-2+(TH/2),RADS,0
 A,100,101,102,103
@@ -490,35 +819,35 @@
 D,ALL,UX,0
 NSEL,ALL
 FINI
 
 /COM, PERFORMING CAMPBELL ANALYSIS USING QRDAMP EIGEN SOLVER
 /SOLU
 ANTYPE,MODAL
-MODOPT,DAMP,25,1.0,,								      ! COMPUTE COMPLEX EIGEN MODES USING DAMP SOLVER
+MODOPT,DAMP,25,1.0,,								      	! COMPUTE COMPLEX EIGEN MODES USING DAMP SOLVER
 MXPAND,25,,,YES										! EXPAND ALL THE MODES WITH STRESS CALCULATION ON
-CORIOLIS,ON,,,ON										! CORIOLIS ON IN A STATIONARY REFERENCE FRAME
+CORIOLIS,ON,,,ON									! CORIOLIS ON IN A STATIONARY REFERENCE FRAME
 RATIO = 4*ATAN(1)/30									! CONVERT RPM INTO RADIANS/SECOND
 *DO,I,1,7
 OMEGA,SPIN(I)*RATIO									! SOLVE FOR DIFFERENT ROTATIONAL VELOCITY
 SOLVE
 *ENDDO
 FINI
 /POST1
 /OUT,
-PRCAMP,ON,2.0,RPM										! PRINT CAMPBELL VALUES FOR SLOPE = 2.0 IN RPM
+PRCAMP,ON,2.0,RPM									! PRINT CAMPBELL VALUES FOR SLOPE = 2.0 IN RPM
 PLCAMP,,2.,RPM
 *GET,CRIC1,CAMP,1,VCRI,,,
 *GET,CRIC2,CAMP,2,VCRI,,,
 *GET,CRIC3,CAMP,3,VCRI,,,
 *GET,CRIC4,CAMP,4,VCRI,,,
 *GET,CRIC5,CAMP,5,VCRI,,,
 *GET,CRIC6,CAMP,6,VCRI,,,
 
-PRCAMP,ON,4.,RPM					 	   				! PRINT CAMPBELL VALUES FOR SLOPE = 4.0 IN RPM
+PRCAMP,ON,4.,RPM					 	   			! PRINT CAMPBELL VALUES FOR SLOPE = 4.0 IN RPM
 PLCAMP,,4.,RPM
 *GET,CRIC7,CAMP,1,VCRI,,,
 *GET,CRIC8,CAMP,2,VCRI,,,
 *GET,CRIC9,CAMP,3,VCRI,,,
 *GET,CRIC10,CAMP,4,VCRI,,,
 *GET,CRIC11,CAMP,5,VCRI,,,
 *GET,CRIC12,CAMP,6,VCRI,,,
@@ -577,15 +906,15 @@
 *VFILL,VALUE(10,3),DATA,ABS(CRIC10/12200)
 *VFILL,VALUE(11,1),DATA,18184.25         						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
 *VFILL,VALUE(11,2),DATA,CRIC11
 *VFILL,VALUE(11,3),DATA,ABS(CRIC11/18184)
 *VFILL,VALUE(12,1),DATA,20162.25         						! CRITICAL SPEED VALUE OBTAINED FROM REFERENCE/4
 *VFILL,VALUE(12,2),DATA,CRIC12
 *VFILL,VALUE(12,3),DATA,ABS(CRIC12/20162)
-SAVE,INF2
+SAVE,INF3
 FINISH
 /CLEAR,NOSTART
 
 RESUME,INF1
 /COM
 /OUT,vm263,vrt
 /COM,------------ vm263 RESULTS COMPARISON --------------
@@ -605,17 +934,34 @@
 *VWRITE,LABEL(1,4),VALUE(4,1),VALUE(4,2),VALUE(4,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,5),VALUE(5,1),VALUE(5,2),VALUE(5,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,6),VALUE(6,1),VALUE(6,2),VALUE(6,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 /COM,
-/COM, ---------------SOLID273---------------
-/NOPR
+/NOPR,
+/COM,
 RESUME,INF2
+/COM, ------SOLID272+SUBSTRUCTURE ANALYSIS----------
+*VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,2),VALUE(2,1),VALUE(2,2),VALUE(2,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,3),VALUE(3,1),VALUE(3,2),VALUE(3,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,4),VALUE(4,1),VALUE(4,2),VALUE(4,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,5),VALUE(5,1),VALUE(5,2),VALUE(5,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,6),VALUE(6,1),VALUE(6,2),VALUE(6,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+/COM,
+/COM,
+RESUME,INF3
+/COM, ---------------SOLID273---------------
 *VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,2),VALUE(2,1),VALUE(2,2),VALUE(2,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,3),VALUE(3,1),VALUE(3,2),VALUE(3,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,4),VALUE(4,1),VALUE(4,2),VALUE(4,3)
@@ -639,29 +985,47 @@
 *VWRITE,LABEL(1,10),VALUE(10,1),VALUE(10,2),VALUE(10,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,11),VALUE(11,1),VALUE(11,2),VALUE(11,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,12),VALUE(12,1),VALUE(12,2),VALUE(12,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 /COM
+/COM,
+RESUME,INF2
+/COM, ------SOLID272+SUBSTRUCTURE ANALYSIS----------
+*VWRITE,LABEL(1,7),VALUE(7,1),VALUE(7,2),VALUE(7,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,8),VALUE(8,1),VALUE(8,2),VALUE(8,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,9),VALUE(9,1),VALUE(9,2),VALUE(9,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,10),VALUE(10,1),VALUE(10,2),VALUE(10,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,11),VALUE(11,1),VALUE(11,2),VALUE(11,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+*VWRITE,LABEL(1,12),VALUE(12,1),VALUE(12,2),VALUE(12,3)
+(1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
+/COM,
 /COM, ---------------SOLID273---------------
 /NOPR
-RESUME,INF2
+RESUME,INF3
 *VWRITE,LABEL(1,7),VALUE(7,1),VALUE(7,2),VALUE(7,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,8),VALUE(8,1),VALUE(8,2),VALUE(8,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,9),VALUE(9,1),VALUE(9,2),VALUE(9,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,10),VALUE(10,1),VALUE(10,2),VALUE(10,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,11),VALUE(11,1),VALUE(11,2),VALUE(11,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 *VWRITE,LABEL(1,12),VALUE(12,1),VALUE(12,2),VALUE(12,3)
 (1X,A8,'   ',F10.4,'  ',F14.4,'   ',F15.3)
 /COM
 /OUT
+/GOPR
 FINISH
 *LIST,vm263,vrt
 /DELETE,INF1
 /DELETE,INF2
+/DELETE,INF3
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm264.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm264.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM264
 JPGPRF,500,100,1
 /SHOW,JPEG
 /COM,VERFICATION MANUAL FOR ONE-DIMENSIONAL CONSOLIDATION SETTLEMENT
 /TITLE,VM264, ONE DIMENSIONAL CONSOLIDATION SETTLEMENT
 C*** USING CPT213
 /COM, REFERENCE: "K.TERZAGHI, THEORETICAL SOIL MECHANICS, WILEY, NEW YORK, 1942"
 /COM,
 /PREP7
 ET,1,CPT213              ! 2-D 8-NODE COUPLED PORE-PRESSURE ELEMENT
+KEYOPT,1,12,1 			         
 KEYOPT,1,3,2             ! PLANE STRAIN
 H=-10                    ! DEPTH OF CONSOLIDATION (M)
 W=1                      ! WIDTH OF ELEMENT (M)
 RECTNG,0,W,0,H           ! GEOMETRY
 ESIZE,W
 AMESH,1
 MP,EX,1,5.8E5            ! YOUNG'S MODULUS
@@ -92,14 +93,15 @@
 /OUT,SCRATCH
 
 
 /TITLE,VM264, ONE DIMENSIONAL CONSOLIDATION SETTLEMENT
 C*** USING CPT215
 /PREP7
 ET,1,CPT215              ! 3-D 8-NODE COUPLED PORE-PRESSURE ELEMENT
+KEYOPT,1,12,1 			         
 H=-10                    ! DEPTH OF CONSOLIDATION (M)
 W=1                      ! WIDTH AND DEPTH OF ELEMENT (M)
 BLC4,0,0,W,H,W           ! GEOMETRY
 ESIZE,W/4
 VMESH,1
 MP,EX,1,5.8E5            ! YOUNG'S MODULUS
 MP,NUXY,1,0.0            ! POISSON'S RATIO
@@ -182,14 +184,15 @@
 
 
 
 /TITLE,VM264, ONE DIMENSIONAL CONSOLIDATION SETTLEMENT
 C*** USING CPT216
 /PREP7
 ET,1,CPT216              ! 3-D 20 NODE COUPLED PORE-PRESSURE ELEMENT
+KEYOPT,1,12,1 			         
 H=-10                    ! DEPTH OF CONSOLIDATION (M)
 W=1                      ! WIDTH AND DEPTH OF ELEMENT (M)
 BLC4,0,0,W,H,W           ! GEOMETRY
 ESIZE,W
 VMESH,1
 MP,EX,1,5.8E5            ! YOUNG'S MODULUS
 MP,NUXY,1,0.0            ! POISSON'S RATIO
@@ -271,14 +274,15 @@
 
 
 
 /TITLE,VM264, ONE DIMENSIONAL CONSOLIDATION SETTLEMENT
 C*** USING CPT217
 /PREP7
 ET,1,CPT217              ! 3-D 10 NODE COUPLED PORE-PRESSURE ELEMENT
+KEYOPT,1,12,1 			         
 H=-10                    ! DEPTH OF CONSOLIDATION (M)
 W=1                      ! WIDTH AND DEPTH OF ELEMENT (M)
 BLC4,0,0,W,H,W           ! GEOMETRY
 ESIZE,W
 VMESH,1
 MP,EX,1,5.8E5            ! YOUNG'S MODULUS
 MP,NUXY,1,0.0            ! POISSON'S RATIO
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm265.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm265.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM265
 /PREP7
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM265, ELASTIC ROD IMPACTING A RIGID WALL
-/stitle,1,Reason COMPARE differences are acceptable:
-/stitle,2,Convergence Difference
 C***     N.J. CARPENTER, R.L. TAYLOR AND M.G.KATONA,   
 C***     "LAGRANGE CONSTRAINTS FOR TRANSIENT FINITE ELEMENT SURFACE CONTACT"   
 C***     INTERNATIONAL JOURNAL FOR NUMERICAL METHODS IN ENGINEERING, VOL.32,103-128 (1991)
 /PREP7 
 ANTYPE,TRANS                 ! NONLINEAR TRANSIENT DYNAMIC ANALYSIS                
 ET,1,SHELL181                ! 4-NODE STRUCTURAL SHELL
 ET,3,CONTA177                ! 3D LINE-TO-SURFACE CONTACT
@@ -58,15 +56,15 @@
 D,ALL,UZ
 D,ALL,ROTX
 D,ALL,ROTY
 D,ALL,ROTZ
 NSEL,ALL
 ESEL,S,TYPE,,1               
 NSLE
-IC,ALL,UX,,202.2             ! INITIAL VELOCITY
+IC,ALL,VELX,202.2             ! INITIAL VELOCITY
 ALLSEL,ALL
 FINISH
 /SOLU
 NLGEOM,ON                    ! INLCUDE LARGE DEFLECTION EFFECTS
 TRNOPT,FULL, , , , ,HHT      ! FULL METHOD WITH HHT ALGORITHM
 TINTP,0.0	                 ! NO NUMERICAL DAMPING
 TIME,2.0E-4                  ! TIME TO ALLOW IMPACT AND RELEASE OF THE ROD
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm266.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm266.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM266
 /PREP7
 JPGPRF,500,100,1                ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM266, 3D CROSSING BEAMS IN CONTACT WITH FRICTION
-/stitle,1,Reason COMPARE differences are acceptable:
-/stitle,2,Convergence Difference
 C***     G.ZAVARISE AND P. WRIGGERS   
 C***     "CONTACT WITH FRICTION BETWEEN BEAMS IN 3-D SPACE"   
 C***     INTERNATIONAL JOURNAL FOR NUMERICAL METHODS IN ENGINEERING, VOL.49,977-1006 (2000)
+/OUT,SCRATCH
 /PREP7 
 ANTYPE,0                        ! STATIC ANALYSIS                
 ET,1,BEAM188                    ! 3-D 2-NODE BEAM
 KEYO,1,3,2                      ! QUADRATIC SHAPE FUNCTIONS ALONG THE LENGTH
 ET,2,BEAM188                    ! 3-D 2-NODE BEAM
 KEYO,2,3,2                      ! QUADRATIC SHAPE FUNCTIONS ALONG THE LENGTH
 SECTYPE,1,BEAM,CTUBE            ! CIRCULAR TUBE SECTION TYPE FOR BEAMS
 SECDATA,0.06,0.12793            ! INNER AND OUTER RADIUS
 R,2,0.2,0.2                     ! RADIUS ON THE TARGET AND CONTACT SIDES
 RMODIF,2,3,-1.0E+4              ! NORMAL CONTACT STIFFNESS-ABSOLUTE VALUE
 RMODIF,2,12,-1.0E+4             ! TANGENTIAL CONTACT STIFFNESS-ABSOLUTE VALUE
-ET,3,CONTA176                   ! 3D LINE-TO-LINE CONTACT
+ET,3,CONTA177                   ! 3D LINE-TO-SURFACE CONTACT
 KEYOPT,3,2,1                    ! PENALTY FUNCTION
-KEYOPT,3,3,1                    ! CROSSING BEAMS
+KEYOPT,3,3,4                    ! CROSSING BEAMS(FORCE-BASED)
 ET,4,TARGE170                   ! 3D TARGET SEGMENT
 MP,EX,1,1.0E+8                  ! YOUNG'S MODULUS 
 MP,NUXY,1,0.0                   ! POISSON'S RATIO
 MP,MU,1,0.1                     ! FRICTION COEFFICIENT
 K,1,0,0,0                       ! GEOMETRY OF BEAMS
 K,2,14,0,0
 K,3,4,-5,1
@@ -62,20 +61,18 @@
 DK,2,UX,0.18                    ! HORIZONTAL DISPLACEMENT OF RIGHT END
 DK,2,UZ,1.8                     ! OUT-OF-PLANE DISPLACEMENT OF RIGHT END
 FINI
 /SOLU
 NLGEOM,ON
 NSUBST,60,100,60
 OUTRES,ALL,ALL
-/OUT,SCRATCH
 SOLVE
 FINI
 /POST1
 ESEL,S,ELEM,,30                 ! ELEMENT IN CONTACT
-/OUT,
 SET,1,30                        ! TIME WHEN CONTACT IS INITIATED
 ETABLE,PRES3,CONT,PRES          ! NORMAL CONTACT FORCE AT SUBSTEP30
 ETABLE,SFRIC3,CONT,SFRIC        ! FRICTIONAL CONTACT FORCE AT SUBSTEP30
 *GET,NFORCE3,ETAB,1,ELEM,30     ! NORMAL CONTACT FORCE AT SUBSTEP30-COMPARE WITH STEP 3 IN REFERENCE
 *GET,TFORCE3,ETAB,2,ELEM,30     ! FRICTIONAL CONTACT FORCE AT SUBSTEP30-COMPARE WITH STEP 3 IN REFERENCE
 SET,1,40                    
 ETABLE,PRES4,CONT,PRES          ! NORMAL CONTACT FORCE AT SUBSTEP40
@@ -89,14 +86,15 @@
 *GET,TFORCE5,ETAB,6,ELEM,30     ! FRICTIONAL CONTACT FORCE AT SUBSTEP50-COMPARE WITH STEP 5 IN REFERENCE                
 SET,1,60                        ! LAST SUBSTEP
 ETABLE,PRES6,CONT,PRES          ! NORMAL CONTACT FORCE AT SUBSTEP60 (LAST)
 ETABLE,SFRIC6,CONT,SFRIC        ! FRICTIONAL CONTACT FORCE AT SUBSTEP60(LAST)
 *GET,NFORCE6,ETAB,7,ELEM,30     ! NORMAL CONTACT FORCE AT SUBSTEP60-COMPARE WITH STEP 6 IN REFERENCE
 *GET,TFORCE6,ETAB,8,ELEM,30     ! FRICTIONAL CONTACT FORCE AT SUBSTEP60-COMPARE WITH STEP 6 IN REFERENCE
 ESEL,ALL
+/OUT,
 *DIM,LABEL2,CHAR,4,1
 *DIM,VALUE2,,4,3
 LABEL2(1,1) = 'NFORCE3  ','NFORCE4 ','NFORCE5 ','NFORCE6 '
 *VFILL,VALUE2(1,1),DATA,17.0,33.8,50.4,67.0
 *VFILL,VALUE2(1,2),DATA,NFORCE3,NFORCE4,NFORCE5,NFORCE6
 *VFILL,VALUE2(1,3),DATA,(NFORCE3/17.0),(NFORCE4/33.8),(NFORCE5/50.4),(NFORCE6/67.0)
 *DIM,LABEL1,CHAR,4,1
@@ -107,46 +105,46 @@
 *VFILL,VALUE1(1,3),DATA,(TFORCE3/1.7),(TFORCE4/3.38),(TFORCE5/5.04),(TFORCE6/6.7)
 FINISH
 /COM
 /OUT,vm266,vrt
 /COM,----------------- VM266 RESULTS COMPARISON ---------------
 /COM,
 /COM,
-/COM,FORCE-BASED CONTACT: K(3)=1
+/COM,FORCE-BASED CONTACT: K(3)=4
 /COM,NORMAL-CONTACT FORCE   |  TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL2(1),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
 (1X,A20,'   ',F10.4,'  ',F14.4,'    ',1F15.3)
 /COM,
 /COM,
 /COM,TANG-CONTACT FORCE     |  TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL1(1),VALUE1(1,1),VALUE1(1,2),VALUE1(1,3)
 (1X,A20,'   ',F10.4,'  ',F14.4,'    ',1F15.3)
 /COM,
 /COM, --------------------------------------------------------
-/OUT
+/OUT,
 FINISH
-!
 /CLEAR,NOSTART
 
+/OUT,SCRATCH
 /PREP7 
 ANTYPE,0                        ! STATIC ANALYSIS                
 ET,1,BEAM188                    ! 3-D 2-NODE BEAM
 KEYO,1,3,2                      ! QUADRATIC SHAPE FUNCTIONS ALONG THE LENGTH
 ET,2,BEAM188                    ! 3-D 2-NODE BEAM
 KEYO,2,3,2                      ! QUADRATIC SHAPE FUNCTIONS ALONG THE LENGTH
 SECTYPE,1,BEAM,CTUBE            ! CIRCULAR TUBE SECTION TYPE FOR BEAMS
 SECDATA,0.06,0.12793            ! INNER AND OUTER RADIUS
 R,2,0.2,0.2                     ! RADIUS ON THE TARGET AND CONTACT SIDES
 T_RATIO=5.71425                 ! AREA RATIO TO CONVERT TO TRACTION CONTACT
 T_STIFF=(-1.0E4)*T_RATIO        ! SCALED ABSOLUTE VALUE OF CONTACT STIFFNESS
 RMODIF,2,3,T_STIFF              ! APPLY NORMAL CONTACT STIFFNESS-ABSOLUTE VALUE
 RMODIF,2,12,T_STIFF             ! APPLY TANGENTIAL CONTACT STIFFNESS-ABSOLUTE VALUE
-ET,3,CONTA176                   ! 3D LINE-TO-LINE CONTACT
+ET,3,CONTA177                   ! 3D LINE-TO-SURFACE CONTACT
 KEYOPT,3,2,1                    ! PENALTY FUNCTION
 KEYOPT,3,3,3                    ! CROSSING BEAMS WITH TRACTION CONTACT
 ET,4,TARGE170                   ! 3D TARGET SEGMENT
 MP,EX,1,1.0E+8                  ! YOUNG'S MODULUS 
 MP,NUXY,1,0.0                   ! POISSON'S RATIO
 MP,MU,1,0.1                     ! FRICTION COEFFICIENT
 K,1,0,0,0                       ! GEOMETRY OF BEAMS
@@ -180,24 +178,23 @@
 ALLSEL,ALL
 DK,2,ALL                        ! CLAMPED RIGHT END OF HORIZONTAL BEAM
 DK,3,ALL                        ! CLAMPED BOTH ENDS OF VERTICAL BEAM
 DK,4,ALL
 DK,2,UX,0.18                    ! HORIZONTAL DISPLACEMENT OF RIGHT END
 DK,2,UZ,1.8                     ! OUT-OF-PLANE DISPLACEMENT OF RIGHT END
 FINI
-/SOLU
+/SOLUTION
 NLGEOM,ON
 NSUBST,60,100,60
 OUTRES,ALL,ALL
 /OUT,SCRATCH
 SOLVE
-FINI
+FINISH
 /POST1
 ESEL,S,ELEM,,30                 ! ELEMENT IN CONTACT
-/OUT,
 SET,1,30                        ! TIME WHEN CONTACT IS INITIATED
 ETABLE,PRES3,CONT,PRES          ! NORMAL CONTACT PRESSURE AT SUBSTEP30
 ETABLE,SFRIC3,CONT,SFRIC        ! FRICTIONAL CONTACT PRESSURE AT SUBSTEP30
 *GET,NPRES3,ETAB,1,ELEM,30      ! NORMAL CONTACT PRESSURE AT SUBSTEP30-COMPARE WITH STEP 3 IN REFERENCE
 *GET,TPRES3,ETAB,2,ELEM,30      ! FRICTIONAL CONTACT PRESSURE AT SUBSTEP30-COMPARE WITH STEP 3 IN REFERENCE
 SET,1,40                    
 ETABLE,PRES4,CONT,PRES          ! NORMAL CONTACT PRESSURE AT SUBSTEP40
@@ -211,28 +208,29 @@
 *GET,TPRES5,ETAB,6,ELEM,30      ! FRICTIONAL CONTACT PRESSURE AT SUBSTEP50-COMPARE WITH STEP 5 IN REFERENCE                
 SET,1,60                        ! LAST SUBSTEP
 ETABLE,PRES6,CONT,PRES          ! NORMAL CONTACT PRESSURE AT SUBSTEP60 (LAST)
 ETABLE,SFRIC6,CONT,SFRIC        ! FRICTIONAL CONTACT PRESSURE AT SUBSTEP60(LAST)
 *GET,NPRES6,ETAB,7,ELEM,30      ! NORMAL CONTACT PRESSURE AT SUBSTEP60-COMPARE WITH STEP 6 IN REFERENCE
 *GET,TPRES6,ETAB,8,ELEM,30      ! FRICTIONAL CONTACT PRESSURE AT SUBSTEP60-COMPARE WITH STEP 6 IN REFERENCE
 ESEL,ALL
+/OUT,
 *DIM,LABEL2,CHAR,4,1
 *DIM,VALUE2,,4,3
 LABEL2(1,1) = 'NPRES3  ','NPRES4 ','NPRES5 ','NPRES6 '
 *VFILL,VALUE2(1,1),DATA,17.0*T_RATIO,33.8*T_RATIO,50.4*T_RATIO,67.0*T_RATIO
 *VFILL,VALUE2(1,2),DATA,NPRES3,NPRES4,NPRES5,NPRES6
 *VFILL,VALUE2(1,3),DATA,(NPRES3/97.14),(NPRES4/193),(NPRES5/288),(NPRES6/383)
 *DIM,LABEL1,CHAR,4,1
 *DIM,VALUE1,,4,3
 LABEL1(1,1) = 'TPRES3  ','TPRES4 ','TPRES5 ','TPRES6 '
 *VFILL,VALUE1(1,1),DATA,1.7*T_RATIO,3.38*T_RATIO,5.04*T_RATIO,6.7*T_RATIO
 *VFILL,VALUE1(1,2),DATA,TPRES3,TPRES4,TPRES5,TPRES6
 *VFILL,VALUE1(1,3),DATA,(TPRES3/9.714),(TPRES4/19.3),(TPRES5/28.8),(TPRES6/38.3)
 FINISH
-/COM
+/COM --------------------------------------------------------------------------
 /OUT,vm266,vrt,,APPEND
 /COM,
 /COM,
 /COM,TRACTION-BASED CONTACT: K(3)=3
 /COM,NORMAL-CONTACT PRESSURE |  TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL2(1),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm267.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm267.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM267
 JPGPRF,500,100,1					 
 /TITLE,VM267, INCLINED CRACK IN 2D PLATE UNDER UNIFORM TENSION LOADING
 /COM, REFERENCE: "T.L.ANDERSON, FRACTURE MECHANICS: FUNDAMENTALS AND APPLICATIONS.
 /COM,             CRC PRESS, BOCA RATON, FL, 1995"
 /COM,
 /SHOW,JPEG
@@ -45,14 +45,19 @@
 SMALL_CIRCULAR_RADIUS = (FIRST_ROW_RADIUS*4)*MM_TO_M
 
 !AREAS CREATION
 WPSTYLE,,,,,,,,1
 WPROTA,ALPHA,,
 CSWPLA,11,0
 
+_geomgen=0
+_exit=0
+
+*if,_geomgen,eq,1,then
+
 RECTNG,RECTNG_OFFSET,RECTNG_OFFSET+RECTNG_LENGHT,0,RECTNG_HEIGHT
 RECTNG,RECTNG_OFFSET,RECTNG_OFFSET+RECTNG_LENGHT,-RECTNG_HEIGHT,0
 
 CYL4,HALF_CRACK_LENGHT,0,SMALL_CIRCULAR_RADIUS,180
 CYL4,HALF_CRACK_LENGHT,0,TORUS_MINOR_RADIUS,180
 ASBA,1,4,,DELETE,KEEP
 ASBA,4,3,,DELETE,KEEP
@@ -133,14 +138,26 @@
 AMESH,8
 AMAP,5,19,15,7,18
 AMAP,7,19,15,21,24
 AMESH,9,11,2
 MOPT,TRANS,2
 AMESH,12,13
 ALLSEL
+cdwrite,all,vm267,cdb
+
+*if,_exit,eq,1,then
+   /exit,nosave
+*endif
+
+*else
+
+/out,scratch
+/PREP7 
+   cdread,db,vm267,cdb
+*endif
 FINISH
 
 /SOLU
 ALLSEL
 CSYS,0
 NSEL,S,LOC,X,-L_RECTANGLE_LENGHT
 D,ALL,UX,0
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm268.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm268.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM268
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE,VM268,MULLINS EFFECT ON A RUBBER TUBE MODEL SUBJECTED TO TENSION LOADING 
 /COM, REFERENCE: "R.W.OGDEN, ET AL., A PSEUDO-ELASTIC MODEL FOR THE MULLINS EFFECT IN FILLED RUBBER  
 /COM,             ROYAL SOCIETY OF LONDON PROCEEDINGS SERIES A, VOL.455,1999,PG:2861-2877
 /COM,
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm269.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm269.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM269
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE,VM269, DEFORMATION OF TUBE AND SPHERE UNDER AXISYMMETRIC BOUNDARY CONDITIONS
 /COM, REFERENCE: "Z.YOSIBASH, AXISYMMETRIC PRESSURE BOUNDARY LOADING FOR FINITE DEFORMATION
 /COM,             ANALYSIS USING P-FEM, COMPUT. METHODS APPL. MECH. ENGRG., 196(2007)
 /COM,             :1261-1277"
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm27.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm27.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM27
 /PREP7
 /TITLE, VM27, THERMAL EXPANSION TO CLOSE A GAP 
 C***   INTROD. TO STRESS ANALYSIS, HARRIS, 1ST PRINTING, PAGE 58, PROB. 8
 C***           CONTA178 AND LINK180 ELEMENTS (3-D)
 ET,1,LINK180
 ET,2,CONTA178
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm270.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm270.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM270
 JPGPRF,500,100,1
 /SHOW,JPEG
 /TITLE, VM270, FORCES IN PERMANENT MAGNETS (TEAM WORKSHOP PROBLEM 23)
 /COM,   REFEENCE: " N.IDA, J.P.A.BASTOS, FORCES IN PERMANENT MAGNETS, TEAM
 /COM,             WORKSHOP PROBLEM 23, PROCEEDINGS OF THE TEAM WORKSHOP IN
 /COM, 		THE SIXTH ROUND, OKAYAMA, PP.49-56.
 /COM,
-/OUT,SCRATCH
+/NOPR
 /PREP7
 ! DIMENSIONS AND PARAMETERS
 MM = 0.001
 PI = ACOS(-1)
 
 ! CONFIGURATION A
 ! SAMARIUM-COBALT MAGNET AND LARGER COIL ! ELECTROMAGNET ! LARGER COIL
@@ -146,45 +146,45 @@
 
 ESEL,S,MAT,,3
 CM,MAGNET,ELEM
 ESEL,ALL
 ALLSEL,ALL
 FINISH
 
-/OUT,
 ! *** SOLVE WITH MAXWELL FORCE OPTION
 /SOLU
 ANTYPE, STATIC
+/OUT,SCRATCH
 SOLVE
+/OUT
 FINISH
 
-/OUT,SCRATCH
 /POST1
 ESEL,S,MAT,,3
 NSLE
 ESLN
 EMFT            			! SUM UP FMAG FORCES ACTING ON THE PERMANENT MAGNET
 ALLSEL,ALL
 FY_TAR1=1.150*9.81E-3		! TARGET (MEASURED) FORCE FY
 FY_OBT1 = _FYSUM			! FORCE OBTAINED FROM MECHANICAL APDL
 FINISH
 
-/OUT,
 ! *** SOLVE WITH LORENTZ FORCE OPTION
 /PREP7
 KEYOPT,1,7,0
 KEYOP,1,8,1				! ELECTROMAGNETIC FORCE CALCULATION USING LORENTZ
 FINISH
 
 /SOLU
 ANTYPE,STATIC
+/OUT,SCRATCH
 SOLVE
+/OUT
 FINISH
 
-/OUT,SCRATCH
 /POST1
 ESEL,S,MAT,,2
 NSLE
 EMFT            			! SUM UP FMAG FORCES ACTING ON THE COIL
 ALLS
 FY_TAR2=-1.150*9.81E-3		! TARGET (MEASURED) FORCE FY
 FY_OBT2 = _FYSUM			! FORCE OBTAINED FROM MECHANICAL APDL
@@ -220,7 +220,8 @@
 *VWRITE,LABEL(1,2),VALUE(2,1),VALUE(2,2),VALUE(2,3)
 (1X,A3,' ',F10.4,'  ',F14.4,'   ',F17.3)
 /COM,
 /COM,-------------------------------------------------------------------------
 /OUT
 *LIST,vm270,vrt
 FINISH
+/DEL,SCRATCH
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm272.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm272.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM272
 JPGPRF,500,100,1
 /TITLE,VM272, TWO AND THREE DIMENSIONAL FRICTIONAL HERTZ CONTACT
 /COM, REFERENCE: YANG, B., LAURSEN, T.A., MEGN, X. TWO DIMENSIONAL MORTAR CONTACT
 /COM, METHODS FOR LARGE DEFORMATION FRICTIONAL SLIDING, IJNME VOL.62, PP 1183-1225.
 /COM, (2005)
 /COM, ANALYTICAL SOLUTION FROM REFERENCE:  JOHNSON KL, "CONTACT MECHANICS"
 /COM, CAMBRIDGE UNIVERSITY PRESS: CAMBRIDGE, 1985.
 /COM,
 C***  USING 2D LOWER ORDER ELEMENTS
 /PREP7
 /NOPR
-MP,EX,1,200.0				!YOUNG'S MODULUS (N/mm^2)
-MP,NUXY,1,0.3				!POISSON'S RATIO
+MP,EX,1,200.0			!YOUNG'S MODULUS (N/mm^2)
+MP,NUXY,1,0.3			!POISSON'S RATIO
 MP,MU,1,0.2				!COEFFICIENT OF FRICTION
 
 ET,1,PLANE182			!2D STRUCTURAL SOLID
 ET,2,PLANE182			!2D STRUCTURAL SOLID
 KEYO,1,3,2				!PLANE STRAIN
 KEYO,2,3,2				!PLANE STRAIN
 
 
-PCIRC,8, ,0,90, 				!CONTACT SIDE
-PCIRC,8, ,90,180,   			!CREATE SEMICIRCLES
-RECT,0,1,7,8				!CREATE RECTANGLES
+PCIRC,8, ,0,90, 		!CONTACT SIDE
+PCIRC,8, ,90,180,   	!CREATE SEMICIRCLES
+RECT,0,1,7,8			!CREATE RECTANGLES
 RECT,-1,0,7,8   				
-WPOFF,0,16  				!TARGET SIDE
-PCIRC,8, ,180,270,  			!CREATE SEMICIRCLES
+WPOFF,0,16  			!TARGET SIDE
+PCIRC,8, ,180,270,  	!CREATE SEMICIRCLES
 PCIRC,8, ,270,360,  
 WPAVE,0,0,0 
 !*  
-RECT,0,1,8,9				!CREATE RECTANGLES
+RECT,0,1,8,9			!CREATE RECTANGLES
 RECT,-1,0,8,9   
 
 AOVLAP,1,3				!COMBINES THE AREAS
 AOVLAP,2,4
 AOVLAP,6,7
 AOVLAP,5,8
 
-ASEL,S,,,1,2				!DELETES EXCESS GEOMETIES
+ASEL,S,,,1,2			!DELETES EXCESS GEOMETIES
 ASEL,A,,,6,9,3
 ALLSEL,BELOW,AREA   
 ADEL,ALL
 LSEL,U,,,2,6,4
 LSEL,U,,,20,30,10
 LDEL,ALL
 KSEL,U,,,2,4,2
 KSEL,U,,,10,16,3
 KSEL,U,,,18,21,3
 KSEL,U,,,29
 KDEL,ALL
 
 ALLSEL
 
-AGLUE,3,10,11,12			!MERGES EXISTING AREAS
+AGLUE,3,10,11,12		!MERGES EXISTING AREAS
 
 AGLUE,4,7,13,14
 
 K,2,4					!CREATES POINTS AND AREAS
 K,6,-4   				!TO DIVIDE THE GEOMETRY
 K,7,4,16 				!AND MESH IT EXACTLY AS NEEDED
 K,9,-4,16
@@ -110,15 +110,15 @@
 LESI,18,,,40
 LESI,23,,,40
 LESI,21,,,40
 LESI,7,,,40
 LESI,5,,,40
 LESI,6,,,40
 
-MSHAPE,0,2D 				!MESH TYPE IS SELECTED
+MSHAPE,0,2D 			!MESH TYPE IS SELECTED
 MSHKEY,1
 
 /OUT,SCRATCH
 TYPE,1					!BOTTOM IS MESHED WITH TYPE 1
 AMESH,1
 AMESH,3
 AMESH,12
@@ -130,193 +130,192 @@
 AMESH,4
 AMESH,6
 AMESH,2
 AMESH,9
 AMESH,10
 AMESH,13
 
-ET,3,CONTA171				!2D 2-NODE SURFACE SURFACE CONTACT
+ET,3,CONTA172			!2D 3-NODE SURFACE SURFACE CONTACT
 KEYO,3,4,3				!DETECTION BY MORTAR
-KEYO,3,10,2				!CONTACT STIFFNESS BY STRESS
+KEYO,3,10,0				!CONTACT STIFFNESS BY STRESS
+KEYO,3,5,1              !CLOSE INITIAL GAP
 
-ET,4,TARGE169				!TARGET ELEMENTS
-LSEL,S,,,5,6,1				!CHOOSE LOCATION FOR CONTACT
+ET,4,TARGE169			!TARGET ELEMENTS
+LSEL,S,,,5,6,1			!CHOOSE LOCATION FOR CONTACT
 NSLL,S,1
 ESLN,S
 
 TYPE,3					!MESH WITH CONTACT ELEMENTS
 REAL,3
 ESURF
 
 TYPE,4					!CHOOSE LOCATION FOR TARGET
 LSEL,S,,,1,2,1
 NSLL,S,1
 ESLN,S
 
 ESURF					!MESH WITH TARGET ELEMENTS
 
-ET,5,SURF153				!2D SURFACE EFFECT ELEMENTS
+ET,5,SURF153			!2D SURFACE EFFECT ELEMENTS
 
 LSEL,S,,,3				!PICK THE TOP OF THE MODEL
 LSEL,A,,,18,19
 LSEL,A,,,21
 NSLL,S,1
 ESLN,S
 TYPE,5
 REAL,5
-ESURF						!ADD SURFACE ELEMENTS
+ESURF					!ADD SURFACE ELEMENTS
 
-ET,10,CONTA171				!2D 2-NODE SURFACE SURFACE CONTACT ELEMENT
-KEYOP,10,2,2				!CONTACT STIFFNESS BY STRESS
-KEYOP,10,4,2				!DETECTION BY TARGET NORMAL
-KEYOP,10,12,5				!ALWAYS BONDED
-LSEL,S,,,3					!PICK THE TOP OF THE MODEL
+ET,10,CONTA172			!2D 3-NODE SURFACE SURFACE CONTACT ELEMENT
+KEYOP,10,2,2			!CONTACT STIFFNESS BY STRESS
+KEYOP,10,4,2			!DETECTION BY TARGET NORMAL
+KEYOP,10,12,5			!ALWAYS BONDED
+LSEL,S,,,3				!PICK THE TOP OF THE MODEL
 LSEL,A,,,18,19
 LSEL,A,,,21
 NSLL,S,1
 ESLN,S
 TYPE,10
 REAL,10
-ESURF						!MESH WITH CONTACT ELEMENTS
-N,100000,,16				!ADD A PILOT NODE
-ET,11,TARGE169,,1				!TARGET ELEMENTS FOR PILOT
-TYPE,11					
+ESURF					!MESH WITH CONTACT ELEMENTS
+N,100000,,16			!ADD A PILOT NODE
+ET,11,TARGE169,,1		!TARGET ELEMENTS FOR PILOT
+TYPE,11				
 TSHAP,PILOT
 E,100000				!MAKE THE PILOT ELEMENT
-D,100000,ROTZ,0				!SET BOUNDARY CONDITIONS
+D,100000,ROTZ,0			!SET BOUNDARY CONDITIONS
 ALLSE						
 
 NSEL,S,LOC,Y
 D,ALL,ALL
 ALLSEL
 /GOLIST
 R,3
-!!! using auto damping
-!RMOD,3,11,-0.001 			!CONTACT DAMPING IN FIRST STEP				
-					!DO NOT ALLOW MUCH ELASTIC SLIP
 FINISH
 
-/SOLU
-OUTRES,ALL,ALL				!SOLUTION OPTIONS
+/SOLUTION
+ANTYPE,STATIC
+OUTRES,ALL,ALL			!SOLUTION OPTIONS
 NSUB,250,2500,15
 ESEL,S,ENAME,,SURF153
-SFE,ALL,1,PRES,1,0.625 			!SMALL AXIAL PRESSURE LOAD
+SFE,ALL,1,PRES,1,0.625 	!SMALL AXIAL PRESSURE LOAD
 ALLSEL
 CNVTOL,U,,0.0001
 CNVTOL,F,,0.0001
 NROP,UNSYM
 NLGEOM,ON				!LARGE DEFLECTION
 SOLVE					!SOLVE FIRST LOADSTEP
 NSUB,6,100,6
 ESEL,S,ENAME,,153
 SFE,ALL,2,PRES,1,-0.05851		!SMALL TANGENTIAL LOAD
 ALLSEL
-!RMOD,3,11,-1E-8				!ALLOW VERY LITTLE DAMPING
+!RMOD,3,11,-1E-8		!ALLOW VERY LITTLE DAMPING
 SOLVE
 FINISH
 /POST1
 SET,LAST
 PI=ACOS(-1)				!PARAMS FOR ANALYTIC SOLUTION
 P=10					!CALCULATED BELOW
 R=8
 V=0.3
 E=200
 U=0.2
 Q=0.93622
-B=2*SQRT(P*R*((1-V**2)/(PI*E)))	!MAXIMUM X-LOCATION OF CONTACT
+B=2*SQRT(P*R*((1-V**2)/(PI*E)))	    !MAXIMUM X-LOCATION OF CONTACT
 SNMAX=SQRT((P*E)/(PI*(1-V**2)*R))	!MAXIMUM CONTACT PRESSURE
-C=B*SQRT(1-(Q/(U*P)))			!LOCATION OF STICK-SLIP BOUNDARY
+C=B*SQRT(1-(Q/(U*P)))			    !LOCATION OF STICK-SLIP BOUNDARY
 
 
-ESEL,S,TYPE,,3				!PICK THE IMPORTANT CONTACT ELEMENTS
-NSEL,S,LOC,X,0,B				!AND NODES
+ESEL,S,TYPE,,3			!PICK THE IMPORTANT CONTACT ELEMENTS
+NSEL,S,LOC,X,0,B		!AND NODES
 ESLN,R
 NSLE
 NSEL,U,LOC,X,-0.1,-0.001
 ESLN,R,1
-ETAB,PRES_I,SMISC,1			!TABULATE THE PRESSURE AND FRICTION RESULTS
-ETAB,FRIC_I,SMISC,3			!AT LEFT NODE OF ALL ELEMENTS FOR USE BELOW
+ETAB,PRES_I,SMISC,1		!TABULATE THE PRESSURE AND FRICTION RESULTS
+ETAB,FRIC_I,SMISC,3		!AT LEFT NODE OF ALL ELEMENTS FOR USE BELOW
 ETAB,CSTAT,NMISC,1
 
 
 *GET,NUMNODE1,NODE,,COUNT			!GET THE NUMBER OF NODES IN SELECTION
-X=NUMNODE1						!STORE THIS NUMBER
-*DIM,LOCARRAY1,ARRAY,NUMNODE1+1,2		!MAKE AN ARRAY FOR NODE NUMBER AND X LOC
+X=NUMNODE1						    !STORE THIS NUMBER
+*DIM,LOCARRAY1,ARRAY,NUMNODE1+1,2	!MAKE AN ARRAY FOR NODE NUMBER AND X LOC
 *GET,NODENUM,NODE,,NUM,MIN			!GET FIRST NODE NUMBER
 
-*DO,I,1,X				!LOOP THROUGH SELECTION TO FILL ARRAY
+*DO,I,1,X				            !LOOP THROUGH SELECTION TO FILL ARRAY
    LOCARRAY1(I,1)=NX(NODENUM)		!X LOCATIONS
-   LOCARRAY1(I,2)=NODENUM		!NODE NUMBER
+   LOCARRAY1(I,2)=NODENUM		    !NODE NUMBER
    *GET,NODENUM,NODE,NODENUM,NXTH	!GET THE NEXT NODE NUMBER
 *ENDDO					!REPEAT
 
 LOCARRAY1(NUMNODE1+1,1)=B			!ADD AN ENTRY FOR THEORETICAL MAX CONTA
 LOCARRAY1(NUMNODE1+1,2)=0
 
-*GET,NUMELEM1,ELEM,,COUNT		!GET THE NUMBER OF ELEMENTS IN SELECTION
+*GET,NUMELEM1,ELEM,,COUNT		    !GET THE NUMBER OF ELEMENTS IN SELECTION
 *DIM,RES1,ARRAY,NUMELEM1+1,6		!MAKE AN ARRAY FOR ALL RESULTS NEEDED
-*GET,ELEMNUM,ELEM,,NUM,MIN		!GET FIRST ELEMENT NUMBER
+*GET,ELEMNUM,ELEM,,NUM,MIN	    	!GET FIRST ELEMENT NUMBER
 
-*DO,K,1,NUMELEM1					!LOOP THROUGH ELEMENTS IN SELECTION
+*DO,K,1,NUMELEM1				    	!LOOP THROUGH ELEMENTS IN SELECTION
    *GET,RES1(K,1),ELEM,ELEMNUM,NODE,1	!FILL ARRAY WITH NODE NUMBER
    *GET,RES1(K,2),ETAB,1,ELEM,ELEMNUM	!FILL ARRAY WITH TABULATED RESULT: PRES
    *GET,RES1(K,3),ETAB,2,ELEM,ELEMNUM	!FILL ARRAY WITH TABULATED RESULT: FRIC
    *GET,RES1(K,4),ETAB,3,ELEM,ELEMNUM	!FILL ARRAY WITH TABULATED RESULT: STAT
 
    *GET,ELEMNUM,ELEM,ELEMNUM,NXTH	!GET THE NEXT ELEMENT NUMBER
 *ENDDO					!REPEAT
 
-RES1(NUMELEM1+1,1)=0			!ADD AN ENTRY FOR THEORETICAL MAX CONTA
+RES1(NUMELEM1+1,1)=0			    !ADD AN ENTRY FOR THEORETICAL MAX CONTA
 RES1(NUMELEM1+1,2)=0
 RES1(NUMELEM1+1,3)=0
 RES1(NUMELEM1+1,4)=0
 
 J=1
-*DOWHILE,J				!BUBBLE SORT OF NODES TO MATCH ELEMENT
-   J=0					!RESULTS WITH NODE NUMBERS AND
-   *DO,I,1,X				!ORDER THE ARRAY BY X LOCATION
+*DOWHILE,J			            	!BUBBLE SORT OF NODES TO MATCH ELEMENT
+   J=0					            !RESULTS WITH NODE NUMBERS AND
+   *DO,I,1,X				        !ORDER THE ARRAY BY X LOCATION
       VAR1=LOCARRAY1(I,1)
       VAR2=LOCARRAY1(I+1,1)
       *IF,VAR1,GT,VAR2,THEN
          TEMP1=LOCARRAY1(I,1)
          LOCARRAY1(I,1)=LOCARRAY1(I+1,1)
          LOCARRAY1(I+1,1)=TEMP1
          TEMP2=LOCARRAY1(I,2)
          LOCARRAY1(I,2)=LOCARRAY1(I+1,2)
          LOCARRAY1(I+1,2)=TEMP2
          J=1
       *ENDIF	
    *ENDDO
 *ENDDO
 
-					!CALCULATE ANALYTICAL SOLUTION FOR PRESSURE
-*DO,I,1,NUMELEM1+1			!AND FRICTION RELATIONSHIP WITH X LOCATION
+					                !CALCULATE ANALYTICAL SOLUTION FOR PRESSURE
+*DO,I,1,NUMELEM1+1			        !AND FRICTION RELATIONSHIP WITH X LOCATION
 	
-   LOCX=LOCARRAY1(I,1)			!LOOP THROUGH ALL NODES
-   *IF,LOCX,LT,B,THEN			!IF(1) NODE IS WITHIN CONTACT RANGE
-      					!EQUATION FOR PRESSURE
+   LOCX=LOCARRAY1(I,1)			    !LOOP THROUGH ALL NODES
+   *IF,LOCX,LT,B,THEN			    !IF(1) NODE IS WITHIN CONTACT RANGE
+      					            !EQUATION FOR PRESSURE
       RES1(I,5)=SNMAX*SQRT(1-(((LOCARRAY1(I,1))/B)**2))
-      *IF,LOCX,LT,C,THEN		!IF(2) NODE IS WITHIN STICK RANGE
-      					!EQUATION FOR FRICTION
+      *IF,LOCX,LT,C,THEN		    !IF(2) NODE IS WITHIN STICK RANGE
+      					            !EQUATION FOR FRICTION
          RES1(I,6)=(U*SNMAX/B)*(SQRT(B**2-LOCX**2)-SQRT(C**2-LOCX**2))
       
-      *ELSE				!ELSE(2) NODE IS WITHIN SLIDE RANGE
-      					!EQUATION FOR FRICTION
+      *ELSE				            !ELSE(2) NODE IS WITHIN SLIDE RANGE
+      					            !EQUATION FOR FRICTION
          RES1(I,6)=U*RES1(I,5)	
       
       *ENDIF
-   *ELSE				!ELSE(1) ASSIGN AS ZERO TO AVIOD DIVIDING
-      RES1(I,5)=0			!BY ZERO
+   *ELSE				            !ELSE(1) ASSIGN AS ZERO TO AVIOD DIVIDING
+      RES1(I,5)=0		        	!BY ZERO
       RES1(I,6)=0
    *ENDIF
 *ENDDO
 
 PARSAV,ALL,vm272-1,parm
 
-*DIM,LABEL1,,7				!CONTACT PRESSURE LISTING
+*DIM,LABEL1,,7				        !CONTACT PRESSURE LISTING
 *DIM,VALUE1,,7,3
 J=1
 *DO,I,1,NUMELEM1,4
   LABEL1(J)=LOCARRAY1(I,1)
   VALUE1(J,1)=RES1(I,5)
   VALUE1(J,2)=RES1(I,2)
   ZERO1=RES1(I,5)
@@ -327,15 +326,15 @@
      VALUE1(J,3)=0  
   *ELSE
      VALUE1(J,3)=ABS(RES1(I,2)/RES1(I,5))
   *ENDIF
   J=J+1
 *ENDDO
 
-*DIM,LABEL2,,7			!CONTACT FRICTION LISTING
+*DIM,LABEL2,,7			            !CONTACT FRICTION LISTING
 *DIM,VALUE2,,7,3
 J=1
 *DO,I,1,NUMELEM1,4
   LABEL2(J)=LOCARRAY1(I,1)
   VALUE2(J,1)=RES1(I,6)
   VALUE2(J,2)=RES1(I,3)
   ZERO1=RES1(I,6)
@@ -366,42 +365,44 @@
 /COM,
 /COM,2D LOW FRIC   |  TARGET   |  Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL2(1),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
 (6X,F5.3,6X,' ',F6.4,6X,'  ',F6.4,6X,'  ',F5.3)
 /COM,
 /OUT,
+rlist,all
+etlist,all
 FINI
 /CLEAR,NOSTART
 
 /OUT,
 C***  USING 3D LOWER ORDER ELEMENTS
 /PREP7
 /NOPR
 MP,EX,1,200.0				!YOUNG'S MODULUS (N/mm^2)
 MP,NUXY,1,0.3				!POISSON'S RATIO
-MP,MU,1,0.2				!COEFFICIENT OF FRICTION
+MP,MU,1,0.2				    !COEFFICIENT OF FRICTION
 
 ET,1,SOLID185				!3D STRUCTURAL SOLID
 ET,2,SOLID185				!3D STRUCTURAL SOLID
 
 
 PCIRC,8, ,0,90, 			!CONTACT SIDE
-PCIRC,8, ,90,180,   			!CREATE SEMICIRCLES
+PCIRC,8, ,90,180,   		!CREATE SEMICIRCLES
 RECT,0,1,7,8				!CREATE RECTANGLES
 RECT,-1,0,7,8   				
 WPOFF,0,16  				!TARGET SIDE
-PCIRC,8, ,180,270,  			!CREATE SEMICIRCLES
+PCIRC,8, ,180,270,  		!CREATE SEMICIRCLES
 PCIRC,8, ,270,360,  
 WPAVE,0,0,0 
 !*  
 RECT,0,1,8,9				!CREATE RECTANGLES
 RECT,-1,0,8,9   
 
-AOVLAP,1,3				!COMBINES THE AREAS
+AOVLAP,1,3				    !COMBINES THE AREAS
 AOVLAP,2,4
 AOVLAP,6,7
 AOVLAP,5,8
 
 ASEL,S,,,1,2				!DELETES EXCESS GEOMETIES
 ASEL,A,,,6,9,3
 ALLSEL,BELOW,AREA   
@@ -417,35 +418,35 @@
 
 ALLSEL
 
 AGLUE,3,10,11,12			!MERGES EXISTING AREAS
 
 AGLUE,4,7,13,14
 
-K,2,4					!CREATES POINTS AND AREAS
-K,6,-4   				!TO DIVIDE THE GEOMETRY
-K,7,4,16 				!AND MESH IT EXACTLY AS NEEDED
+K,2,4					    !CREATES POINTS AND AREAS
+K,6,-4   				    !TO DIVIDE THE GEOMETRY
+K,7,4,16 				    !AND MESH IT EXACTLY AS NEEDED
 K,9,-4,16
 
 A,3,2,8,12
 A,7,20,24,23
 A,20,9,28,24
 A,11,6,3,12
 
-APTN,2,7				!PARTITIONS OVERLAPPING AREAS 
-APTN,9,13				!INTO SEPERATE ENTIITES
+APTN,2,7				    !PARTITIONS OVERLAPPING AREAS 
+APTN,9,13				    !INTO SEPERATE ENTIITES
 APTN,8,10
 APTN,5,11
 
 AGLUE,1,3,7,8,11,12
 
 AGLUE,2,4,6,9,10,13  
 
-LESI,27,,,8				!SETS NUMBER OF ELEMENTS
-LESI,33,,,8				!ALONG EACH LINE
+LESI,27,,,8				    !SETS NUMBER OF ELEMENTS
+LESI,33,,,8				    !ALONG EACH LINE
 LESI,9,,,8
 LESI,10,,,8
 LESI,15,,,8
 
 LESI,34,,,16
 LESI,17,,,16
 LESI,8,,,16
@@ -480,81 +481,81 @@
 
 K,30,0,0 ,0
 K,31,0,0 ,1
 K,32,0,16,0
 K,33,0,16,1
 L,30,31,1
 L,32,33,1
-VDRAG,1,3,12,8,7,11,12			!DRAGS THE BOTTOM INTO A VOLUME
+VDRAG,1,3,12,8,7,11,12		!DRAGS THE BOTTOM INTO A VOLUME
 VDRAG,4,6,2,9,10,13,28
 
 
 MSHAPE,0,3D 				!MESH TYPE IS SELECTED
 MSHKEY,1
 
 
 /OUT,SCRATCH
-TYPE,1					!BOTTOM IS MESHED WITH TYPE 1
+TYPE,1					    !BOTTOM IS MESHED WITH TYPE 1
 VMESH,1
 VMESH,2
 VMESH,3
 VMESH,4
 VMESH,5
 VMESH,6
 
-TYPE,2					!TOP IS MESHED WITH TYPE 2
+TYPE,2					    !TOP IS MESHED WITH TYPE 2
 VMESH,7
 VMESH,8
 VMESH,9
 VMESH,10
 VMESH,11
 VMESH,12
 
-ET,3,CONTA173				!3D 4-NODE SURFACE SURFACE CONTACT
-KEYO,3,4,3				!DETECTION BY MORTAR
-KEYO,3,10,2				!CONTACT STIFFNESS BY STRESS
-
+ET,3,CONTA174			    !3D 8-NODE SURFACE SURFACE CONTACT
+KEYO,3,4,3				    !DETECTION BY MORTAR
+KEYO,3,10,0				    !CONTACT STIFFNESS BY STRESS
+KEYO,3,5,1                  !CLOSE INITIAL GAP
 ET,4,TARGE170				!TARGET ELEMENTS
 ASEL,S,,,35,41,6
 NSLA,S,1
 ESLN,S
 
-TYPE,3					!MESH WITH CONTACT ELEMENTS
+TYPE,3					    !MESH WITH CONTACT ELEMENTS
 REAL,3
 ESURF
 
-TYPE,4					!CHOOSE LOCATION FOR TARGET
+TYPE,4					    !CHOOSE LOCATION FOR TARGET
 ASEL,S,,,14,18,4
 NSLA,S,1
 ESLN,S
-ESURF					!MESH WITH TARGET ELEMENTS
+ESURF					    !MESH WITH TARGET ELEMENTS
 
 ET,5,SURF154				!3D SURFACE EFFECT ELEMENTS
 
 ASEL,S,,,51,55,4			!PICK THE TOP OF THE MODEL
 ASEL,A,,,45,48,3
 NSLA,S,1
 ESLN,S
 TYPE,5
 REAL,5
-ESURF					!ADD SURFACE ELEMENTS
+ESURF					    !ADD SURFACE ELEMENTS
 
-ET,10,CONTA173				!3D 4-NODE SURFACE SURFACE CONTACT ELEMENT
+ET,10,CONTA174				!3D 8-NODE SURFACE SURFACE CONTACT ELEMENT
 KEYOP,10,2,2				!CONTACT STIFFNESS BY STRESS
 KEYOP,10,4,2				!DETECTION BY TARGET NORMAL
 KEYOP,10,12,5				!ALWAYS BONDED
 ASEL,S,,,51,55,4			!PICK THE TOP OF THE MODEL
 ASEL,A,,,45,48,3
 NSLA,S,1
 ESLN,S
 TYPE,10
 REAL,10
-ESURF					!MESH WITH CONTACT ELEMENTS
+ESURF					    !MESH WITH CONTACT ELEMENTS
 N,100000,,16				!ADD A PILOT NODE
-ET,11,TARGE170,,1				!TARGET ELEMENTS FOR PILOT
+ET,11,TARGE170,,1			!TARGET ELEMENTS FOR PILOT
 TYPE,11					
 TSHAP,PILOT
 E,100000					!MAKE THE PILOT ELEMENT
 D,100000,ROTZ,0				!SET BOUNDARY CONDITIONS
 ALLSE						
 
 NSEL,S,LOC,Y
@@ -563,150 +564,148 @@
 D,ALL,UZ
 NSEL,S,LOC,Y,16
 D,ALL,ROTX
 D,ALL,ROTY
 
 /GOLIST
 R,3
-!!! using auto damping
-!RMOD,3,11,-0.001 			!CONTACT DAMPING IN FIRST STEP	
-RMOD,3,23,1E-4
+RMOD,3,3,10                 !HIGH FKN TO MINIMIZE PENETRATION
+RMOD,3,4,0.01               !SMALL FTOLN TO MINIMIZE PENETRATION
+RMOD,3,23,1E-4 
 FINISH
 
 /SOLU
 OUTRES,ALL,ALL				!SOLUTION OPTIONS
 NSUB,200,500,10
 ESEL,S,ENAME,,154
-SFE,ALL,1,PRES,1,0.625 			!SMALL AXIAL PRESSURE LOAD
+SFE,ALL,1,PRES,1,0.625 		!SMALL AXIAL PRESSURE LOAD
 ALLSEL
 CNVTOL,U,,0.0001
 CNVTOL,F,,0.0001
 NROP,UNSYM
-NLGEOM,ON				!LARGE DEFLECTION
-SOLVE					!SOLVE FIRST LOADSTEP
+NLGEOM,ON				    !LARGE DEFLECTION
+SOLVE					    !SOLVE FIRST LOADSTEP
 NSUB,4,10,1
 
 NSEL,S,LOC,X,-4,-8
 ESLN,S,1
 ESEL,R,ENAME,,154
-SFE,ALL,3,PRES,1,0.05851		!SMALL TANGENTIAL LOAD
+SFE,ALL,3,PRES,1,0.05851	!SMALL TANGENTIAL LOAD
 NSEL,S,LOC,X,-4,8
 ESLN,S,1
 ESEL,R,ENAME,,154
 SFE,ALL,3,PRES,1,-0.05851
 ALLSEL
-!!! using auto damping
-!RMOD,3,11,-1E-8				!ALLOW VERY LITTLE DAMPING
 SOLVE
 FINISH
 
 /POST1
 SET,LAST
 /OUT
-PI=ACOS(-1)				!PARAMS FOR ANALYTIC SOLUTION
-P=10					!CALCULATED BELOW
+PI=ACOS(-1)				    !PARAMS FOR ANALYTIC SOLUTION
+P=10					    !CALCULATED BELOW
 R=8
 V=0.3
 E=200
 U=0.2
 Q=0.93622
 B=2*SQRT(P*R*((1-V**2)/(PI*E)))		!MAXIMUM X-LOCATION OF CONTACT
 SNMAX=SQRT((P*E)/(PI*(1-V**2)*R))	!MAXIMUM CONTACT PRESSURE
-C=B*SQRT(1-(Q/(U*P)))			!LOCATION OF STICK-SLIP BOUNDARY
+C=B*SQRT(1-(Q/(U*P)))			    !LOCATION OF STICK-SLIP BOUNDARY
 
 
 ESEL,S,TYPE,,3				!PICK THE IMPORTANT CONTACT ELEMENTS
 NSEL,S,LOC,X,0,B			!AND NODES
 ESLN,R
 ESEL,U,ELEM,,4000
 NSLE,S
 NSEL,R,LOC,Z,1
 ETAB,PRES_I,SMISC,1			!TABULATE THE PRESSURE AND FRICTION RESULTS
 ETAB,TAUR_I,SMISC,5			!AT LEFT NODE OF ALL ELEMENTS FOR USE BELOW
 ETAB,TAUS_I,SMISC,9
 ETAB,CSTAT,NMISC,1
 
 
-*GET,NUMNODE2,NODE,,COUNT		!GET THE NUMBER OF NODES IN SELECTION
-X=NUMNODE2				!STORE THIS NUMBER
-*DIM,LOCARRAY2,ARRAY,NUMNODE2+1,2		!MAKE AN ARRAY FOR NODE NUMBER AND X LOC
-*GET,NODENUM,NODE,,NUM,MIN		!GET FIRST NODE NUMBER
+*GET,NUMNODE2,NODE,,COUNT		    !GET THE NUMBER OF NODES IN SELECTION
+X=NUMNODE2				            !STORE THIS NUMBER
+*DIM,LOCARRAY2,ARRAY,NUMNODE2+1,2	!MAKE AN ARRAY FOR NODE NUMBER AND X LOC
+*GET,NODENUM,NODE,,NUM,MIN		    !GET FIRST NODE NUMBER
 
-*DO,I,1,X				!LOOP THROUGH SELECTION TO FILL ARRAY
+*DO,I,1,X				            !LOOP THROUGH SELECTION TO FILL ARRAY
    LOCARRAY2(I,1)=NX(NODENUM)		!X LOCATIONS
-   LOCARRAY2(I,2)=NODENUM		!NODE NUMBER
+   LOCARRAY2(I,2)=NODENUM		    !NODE NUMBER
    *GET,NODENUM,NODE,NODENUM,NXTH	!GET THE NEXT NODE NUMBER
-*ENDDO					!REPEAT
+*ENDDO					            !REPEAT
 
 LOCARRAY2(NUMNODE2+1,1)=B			!ADD AN ENTRY FOR THEORETICAL MAX CONTA
 LOCARRAY2(NUMNODE2+1,2)=0
 
-*GET,NUMELEM2,ELEM,,COUNT		!GET THE NUMBER OF ELEMENTS IN SELECTION
+*GET,NUMELEM2,ELEM,,COUNT		    !GET THE NUMBER OF ELEMENTS IN SELECTION
 *DIM,RES2,ARRAY,NUMELEM2+1,6		!MAKE AN ARRAY FOR ALL RESULTS NEEDED
-*GET,ELEMNUM,ELEM,,NUM,MIN		!GET FIRST ELEMENT NUMBER
+*GET,ELEMNUM,ELEM,,NUM,MIN		    !GET FIRST ELEMENT NUMBER
 
-*DO,K,1,NUMELEM2				!LOOP THROUGH ELEMENTS IN SELECTION
+*DO,K,1,NUMELEM2				        !LOOP THROUGH ELEMENTS IN SELECTION
    *GET,RES2(K,1),ELEM,ELEMNUM,NODE,1	!FILL ARRAY WITH NODE NUMBER
    *GET,RES2(K,2),ETAB,1,ELEM,ELEMNUM	!FILL ARRAY WITH TABULATED RESULT: PRES
-   *GET,TAUS,ETAB,2,ELEM,ELEMNUM	!FILL ARRAY WITH TABULATED RESULT: FRIC
+   *GET,TAUS,ETAB,2,ELEM,ELEMNUM	    !FILL ARRAY WITH TABULATED RESULT: FRIC
    *GET,TAUR,ETAB,3,ELEM,ELEMNUM
    RES2(K,3)=SQRT(TAUR**2+TAUS**2)
    *GET,RES2(K,4),ETAB,4,ELEM,ELEMNUM	!FILL ARRAY WITH TABULATED RESULT: STAT
 
-   *GET,ELEMNUM,ELEM,ELEMNUM,NXTH	!GET THE NEXT ELEMENT NUMBER
+   *GET,ELEMNUM,ELEM,ELEMNUM,NXTH	    !GET THE NEXT ELEMENT NUMBER
 *ENDDO					!REPEAT
 
-RES2(NUMELEM2+1,1)=0			!ADD AN ENTRY FOR THEORETICAL MAX CONTA
+RES2(NUMELEM2+1,1)=0			        !ADD AN ENTRY FOR THEORETICAL MAX CONTA
 RES2(NUMELEM2+1,2)=0
 RES2(NUMELEM2+1,3)=0
 RES2(NUMELEM2+1,4)=0
 
 J=1
-*DOWHILE,J				!BUBBLE SORT OF NODES TO MATCH ELEMENT
-   J=0					!RESULTS WITH NODE NUMBERS AND
-   *DO,I,1,X				!ORDER THE ARRAY BY X LOCATION
+*DOWHILE,J				                !BUBBLE SORT OF NODES TO MATCH ELEMENT
+   J=0					                !RESULTS WITH NODE NUMBERS AND
+   *DO,I,1,X				            !ORDER THE ARRAY BY X LOCATION
       VAR1=LOCARRAY2(I,1)
       VAR2=LOCARRAY2(I+1,1)
       *IF,VAR1,GT,VAR2,THEN
          TEMP1=LOCARRAY2(I,1)
          LOCARRAY2(I,1)=LOCARRAY2(I+1,1)
          LOCARRAY2(I+1,1)=TEMP1
          TEMP2=LOCARRAY2(I,2)
          LOCARRAY2(I,2)=LOCARRAY2(I+1,2)
          LOCARRAY2(I+1,2)=TEMP2
          J=1
       *ENDIF	
    *ENDDO
 *ENDDO
 
-				!CALCULATE ANALYTICAL SOLUTION FOR PRESSURE
-*DO,I,1,NUMELEM2+1			!AND FRICTION RELATIONSHIP WITH X LOCATION
+				                        !CALCULATE ANALYTICAL SOLUTION FOR PRESSURE
+*DO,I,1,NUMELEM2+1			            !AND FRICTION RELATIONSHIP WITH X LOCATION
 	
-   LOCX=LOCARRAY2(I,1)			!LOOP THROUGH ALL NODES
-   *IF,LOCX,LT,B,THEN			!IF(1) NODE IS WITHIN CONTACT RANGE
-      					!EQUATION FOR PRESSURE
+   LOCX=LOCARRAY2(I,1)			        !LOOP THROUGH ALL NODES
+   *IF,LOCX,LT,B,THEN			        !IF(1) NODE IS WITHIN CONTACT RANGE
+      					                !EQUATION FOR PRESSURE
       RES2(I,5)=SNMAX*SQRT(1-(((LOCARRAY2(I,1))/B)**2))
-      *IF,LOCX,LT,C,THEN		!IF(2) NODE IS WITHIN STICK RANGE
-      					!EQUATION FOR FRICTION
+      *IF,LOCX,LT,C,THEN		        !IF(2) NODE IS WITHIN STICK RANGE
+      					                !EQUATION FOR FRICTION
          RES2(I,6)=(U*SNMAX/B)*(SQRT(B**2-LOCX**2)-SQRT(C**2-LOCX**2))
       
-      *ELSE				!ELSE(2) NODE IS WITHIN SLIDE RANGE
-      					!EQUATION FOR FRICTION
+      *ELSE				                !ELSE(2) NODE IS WITHIN SLIDE RANGE
+      					                !EQUATION FOR FRICTION
          RES2(I,6)=U*RES2(I,5)	
       
       *ENDIF
-   *ELSE				!ELSE(1) ASSIGN AS ZERO TO AVIOD DIVIDING
-      RES2(I,5)=0			!BY ZERO
+   *ELSE				                !ELSE(1) ASSIGN AS ZERO TO AVIOD DIVIDING
+      RES2(I,5)=0		            	!BY ZERO
       RES2(I,6)=0
    *ENDIF
 *ENDDO
 
 PARSAV,ALL,vm272-2,parm
 
-*DIM,LABEL3,,7				!CONTACT PRESSURE LISTING
+*DIM,LABEL3,,7				            !CONTACT PRESSURE LISTING
 *DIM,VALUE3,,7,3
 J=1
 *DO,I,1,NUMELEM2,4
   LABEL3(J)=LOCARRAY2(I,1)
   VALUE3(J,1)=RES2(I,5)
   VALUE3(J,2)=RES2(I,2)
   ZERO1=RES2(I,5)
@@ -717,15 +716,15 @@
      VALUE3(J,3)=0  
   *ELSE
      VALUE3(J,3)=ABS(RES2(I,2)/RES2(I,5))
   *ENDIF
   J=J+1
 *ENDDO
 
-*DIM,LABEL4,,7			!CONTACT FRICTION LISTING
+*DIM,LABEL4,,7			                !CONTACT FRICTION LISTING
 *DIM,VALUE4,,7,3
 J=1
 *DO,I,1,NUMELEM2,4
   LABEL4(J)=LOCARRAY2(I,1)
   VALUE4(J,1)=RES2(I,6)
   VALUE4(J,2)=RES2(I,3)
   ZERO1=RES2(I,6)
@@ -757,64 +756,66 @@
 /COM,3D LOW FRIC   |  TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL4(1),VALUE4(1,1),VALUE4(1,2),VALUE4(1,3)
 (6X,F5.3,6X,' ',F6.4,6X,'  ',F6.4,6X,'  ',F5.3)
 /COM,
 /OUT,
 *LIST,vm272,vrt
+etlist,all
+rlist,all
 FINI
 /CLEAR,NOSTART
 
 /OUT,SCRATCH
 /SHOW,PNG
 
 
 PARRES,      ,vm272-1,parm
 PARRES,CHANGE,vm272-2,parm
 *DIM,RES_TABLE1,TABLE,NUMELEM1+1,6   !CREATE A "TABLE" DATA FORMAT FOR CLEANER
-RES_TABLE1(0,1)=0		     !PLOTTING THAN POSSIBLE WITH ARRAYS ALONE
-RES_TABLE1(0,2)=0		     !ZERO COLUMN FILLED WITH ZEROS
+RES_TABLE1(0,1)=0		             !PLOTTING THAN POSSIBLE WITH ARRAYS ALONE
+RES_TABLE1(0,2)=0		             !ZERO COLUMN FILLED WITH ZEROS
 RES_TABLE1(0,3)=0
 RES_TABLE1(0,4)=0
 RES_TABLE1(0,5)=0
 RES_TABLE1(0,6)=0
 
-					!HIGH MESH DENSITY/LOWER ORDER
-*DO,I,1,NUMELEM1+1		     !LOOP THROUGH NODE ARRAY
-   N_NODE=LOCARRAY1(I,2)	     !STORE THE NODE NUMBER
-   *DO,J,1,NUMELEM1+1		     !LOOP THROUGH ELEMENT RESULT ARRAY
+					                 !HIGH MESH DENSITY/LOWER ORDER
+*DO,I,1,NUMELEM1+1		             !LOOP THROUGH NODE ARRAY
+   N_NODE=LOCARRAY1(I,2)	         !STORE THE NODE NUMBER
+   *DO,J,1,NUMELEM1+1		         !LOOP THROUGH ELEMENT RESULT ARRAY
 
-      TEMP=RES1(J,1)		     !STORE LEFT NODE OF EACH ELEMENT
+      TEMP=RES1(J,1)		         !STORE LEFT NODE OF EACH ELEMENT
       *IF,TEMP,EQ,N_NODE,THEN	     !IF THEY ARE THE SAME NODE
-	 RES_TABLE1(I,3) =RES1(J,2)   !FILL TABLE WITH 2D LOWER ORDER PRESSURE
-	 RES_TABLE1(I,4) =RES1(J,3)   !FILL TABLE WITH 2D LOWER ORDER FRICTION
-	 RES_TABLE1(I,5) =RES2(J,2)   !FILL TABLE WITH 3D LOWER ORDER PRESSURE
-	 RES_TABLE1(I,6) =RES2(J,3)   !FILL TABLE WITH 3D LOWER ORDER FRICTION	
+	 RES_TABLE1(I,3) =RES1(J,2)      !FILL TABLE WITH 2D LOWER ORDER PRESSURE
+	 RES_TABLE1(I,4) =RES1(J,3)      !FILL TABLE WITH 2D LOWER ORDER FRICTION
+	 RES_TABLE1(I,5) =RES2(J,2)      !FILL TABLE WITH 3D LOWER ORDER PRESSURE
+	 RES_TABLE1(I,6) =RES2(J,3)      !FILL TABLE WITH 3D LOWER ORDER FRICTION	
       *ENDIF
    *ENDDO
 *ENDDO
-     				     !CALCULATE ANALYTICAL SOLUTION FOR PRESSURE
-*DO,I,1,NUMELEM1+1		     !AND FRICTION RELATIONSHIP WITH X LOCATION
-   RES_TABLE1(I,0)=LOCARRAY1(I,1)     !FILL THE ZERO COLUMN OF THE TABLE (X-AXIS)
-
-   LOCX=LOCARRAY1(I,1)  	     !LOOP THROUGH ALL NODES
-   *IF,LOCX,LT,B,THEN		     !IF(1) NODE IS WITHIN CONTACT RANGE
-				     !EQUATION FOR PRESSURE
+     				                !CALCULATE ANALYTICAL SOLUTION FOR PRESSURE
+*DO,I,1,NUMELEM1+1		            !AND FRICTION RELATIONSHIP WITH X LOCATION
+   RES_TABLE1(I,0)=LOCARRAY1(I,1)   !FILL THE ZERO COLUMN OF THE TABLE (X-AXIS)
+
+   LOCX=LOCARRAY1(I,1)  	        !LOOP THROUGH ALL NODES
+   *IF,LOCX,LT,B,THEN		        !IF(1) NODE IS WITHIN CONTACT RANGE
+				                    !EQUATION FOR PRESSURE
       RES_TABLE1(I,1)=RES1(I,5)
-      *IF,LOCX,LT,C,THEN	     !IF(2) NODE IS WITHIN STICK RANGE
-				     !EQUATION FOR FRICTION
+      *IF,LOCX,LT,C,THEN	        !IF(2) NODE IS WITHIN STICK RANGE
+				                    !EQUATION FOR FRICTION
      	 RES_TABLE1(I,2)=RES1(I,6)
 
-      *ELSE			     !ELSE(2) NODE IS WITHIN SLIDE RANGE
-				     !EQUATION FOR FRICTION
+      *ELSE			                !ELSE(2) NODE IS WITHIN SLIDE RANGE
+				                    !EQUATION FOR FRICTION
      	 RES_TABLE1(I,2)=RES1(I,6)    
 
       *ENDIF
-   *ELSE			     !ELSE(1) ASSIGN AS ZERO TO AVIOD DIVIDING
-      RES_TABLE1(I,1)=0  	     !BY ZERO
+   *ELSE			                !ELSE(1) ASSIGN AS ZERO TO AVIOD DIVIDING
+      RES_TABLE1(I,1)=0  	        !BY ZERO
       RES_TABLE1(I,2)=0
    *ENDIF
 *ENDDO
 
 /OUT,
 /TITLE,FRICTIONAL HERTZIAN CONTACT LOWER ORDER
 /GCOLUMN,1,ANA_PRE		  !ASSIGNS ANALYTICAL PRESSURE
@@ -831,7 +832,8 @@
 /GMARKER,6,3  
 /XRANGE,0,0.7
 /AXLAB,X,X DISTANCE FROM CENTER   !X-AXIS LABEL
 /AXLAB,Y,CONTACT RESULTS	  !Y-AXIS LABEL
 /YRANGE,0,10
 *VPLO,RES_TABLE1(1,0),RES_TABLE1(1,1),2,3,4,5,6
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm273.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm273.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM273
 /TITLE,VM273, SHAPE MEMORY ALLOY WITH THERMAL EFFECT UNDER UNIAXIAL LOAD
 /COM,   REF: FERDINANDO AURICHIO, LORENZA PETRINI
 /COM,   "IMPROVEMENTS AND ALGORITHMICAL CONSIDERATIONS ON A RECENT
 /COM,   THREE-DIMENSIONAL MODEL DESCRBING STRESS-INDUCED SOLID
 /COM,   PHASE TRANSFORMATIONS"
 /COM,   INT. J. NUMER. METH. ENGNG. 55 (2002) 1255-1284
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm274.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm274.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM274
 /TITLE,VM274,STABILIZING SQUEAL DAMPING
 C***
 /PREP7
 			        !MATERIAL MODEL 1
 MP,EX,1,2.1E11		!YOUNG'S MODULUS (N/m^2)
 MP,NUXY,1,0.3		!POISSON'S RATIO
 MP,DENS,1,8000		!DENSITY (kg/m^3)
 
 			        !MATERIAL MODEL 2 
 MP,MU,2,0.5		    !COEFFICIENT OF FRICTION
 
 
 ET,1,SOLID185		!3D 8-NODE STRUCTURAL SOLID
-ET,2,CONTA173		!3D 4-NODE SURFACE-TO-SURFACE CONTACT
-KEYOPT,2,2,0		!AUGUMENTED LAGRANGET ALGORITHM
-KEYOPT,2,10,2		!UPDATE CONTACT STIFFNESS EACH ITERATION
+ET,2,CONTA174		!3D 8-NODE SURFACE-TO-SURFACE CONTACT
+KEYOPT,2,2,0		!AUGUMENTED LAGRANGE ALGORITHM
 ET,3,TARGE170		!3-D TARGET SEGMENT
 KEYOPT,3,2,1		!BOUNDARY CONDITIONS SET BY USER
 ET,4,MASS21		    !STRUCTURAL MASS
 KEYOPT,4,2,1		!COORDINATE SYSTEM ALIGNED TO NODE         
 ET,5,COMBIN14		!SPRING-DAMPER
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm275.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm275.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /verify,vm275
 /title,vm275,Mode lock-in and friction induced vibration on a Pin-Disc Model
 /com,
 /com,  This verification manual highlights the mode coupling 
 /com,  phenomenon on a pin-disc set up using brake squeal analysis.
 /com,  The brake squeal analysis is performed using all 3 methods
 /com,
@@ -98,15 +98,15 @@
 csys,0  
     
     
 et,3,conta175               ! Defining Frictional Contact Pair
 mp,mu,3,0.152               ! Coefficient of Friction
 keyopt,3,2,0                ! Augumented Lagrangian
 keyopt,3,9,2                ! Include penetration or gap with ramped effects
-keyopt,3,10,2               ! Update contact stiffness each iteration
+keyopt,3,10,0               ! Update contact stiffness each iteration
 keyopt,3,12,0               ! Standard Contact
 
 
     
 et,4,targe170
     
 r,3 
@@ -184,15 +184,15 @@
 mxpand,30,,,
 /out,
 solve   
 fini
     
 /post1  
 file,,rstp  
-set,1,7
+set,1,7,,IMAG
 *get,unstablemode1,active,0,set,freq
 *stat,unstablemode1
 *dim,label,char,1,2
 *dim,value,,1,3
 
 label(1,1)='Mode'
 
@@ -244,15 +244,15 @@
 mxpand,30,,,
 /out,
 solve   
 fini
     
 /post1  
 file,,rstp  
-set,1,7
+set,1,7,,IMAG
 *get,unstablemode2,active,0,set,freq
 *stat,unstablemode2
 *dim,label,char,1,2
 *dim,value,,1,3
 
 label(1,1)='Mode'
 
@@ -293,15 +293,15 @@
 /out,
 solve   
 fini
      
     
 /post1  
 file,,rst  
-set,1,7
+set,1,7,,IMAG
 *get,unstablemode3,active,0,set,freq
 *stat,unstablemode3
 *dim,label,char,1,2
 *dim,value,,1,3
 
 label(1,1)='Mode'
 
@@ -353,9 +353,10 @@
 /com, --------------------------------------------------------------------------------
 /out,
 *list,vm275,vrt
 /delete,table_1
 /delete,table_2
 /delete,table_3
 finish
+/exit,nosave
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm276.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm276.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /verify,vm276
 /title,vm276,Constant Diffusion Flux in a Plane Sheet
 /com,
 /com,
 /com, Reference: Crank,J. The Mathematics of Diffusion.
 /com, 2nd printing, Bristol: Oxford University Press
 /com, 1975, pg 47-48
@@ -50,14 +50,15 @@
 
 /SOLU
 ANTYPE,TRANS
 OUTRES,ALL,ALL
 KBC,1			! STEPPED LOAD
 NSUB,SUB
 TIME,T
+AUTOTS,OFF
 SOLVE
 FINISH
 
 /POST1
 *DIM,CONCENTRATION_,TABLE,SUB,2
 *DIM,MASS_,TABLE,SUB,2
 
@@ -124,8 +125,9 @@
 *VWRITE,MASS_(35,0),MASS_(35,2),MASS_(35,1),MASS_RATIO(35,1)
 (,F15.0,'       ',G14.5,'        ',G14.5,'          ',F8.3)
 /COM
 /COM ------------------------------------------------------------------------
 /OUT,
 *list,vm276,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm277.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm277.dat`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /verify,vm277
 /title,vm277,Hall Plate in a Uniform Magnetic Field
 /COM,
 /COM, Reference: Meijer,G. "Smart Sensor Systems"
 /COM, John Wiley & Sons, Ltd.2008,pp 252
 /COM,
 
@@ -28,15 +28,15 @@
 MP,RSVX,1,RHO
 MP,MURX,1,MU
 BLOCK,-A,A,-B,B,0,C		! HALL PLATE
 BLOCK,-A,-A+A/8,B,B-B/8,C/2,C	! SENSOR CONNECTIONS
 BLOCK,-A,-A+A/8,-B,-B+B/8,C/2,C
 BLOCK,A,A-A/8,B,B-B/8,C/2,C
 BLOCK,A,A-A/8,-B,-B+B/8,C/2,C
-ESIZE,C
+ESIZE,C/2
 MSHA,1,3D			! TETRAHEDRAL
 VOVLAP,ALL
 VMESH,ALL
 
 W1=NODE(-A,B,C)			! NODES FOR WIRE MODELING
 W2=NODE(A,-B,C)
 *GET,N_MAX,NODE,,NUM,MAX	! GET MAX NODE NUMBER
@@ -83,26 +83,30 @@
 
 /VIEW,,1,2,3
 EPLOT
 FINISH
 
 /SOLU
 OUTRES,ALL,ALL
+/OUT,SCRATCH
 SOLVE
 VBASE=VOLT(ND4)-VOLT(ND3)	! OFFSET VOLTAGE = OUTPUT VOLTAGE AT B=0 T
 DFLX,ALL,,,BZ			! UNIFORM B-FIELD BZ IN THE +Z-DIRECTION
 ALLS
 SOLVE
+/OUT
 FINISH
 
 /POST1
 SET,LAST,LAST
 VSEL,S,VOLU,,6
 NSLV
+/OUT,SCRATCH
 FSUM
+/OUT
 *GET,_I,FSUM,,ITEM,AMPS		! CURRENT THROUGH PLATE
 ALLS
 
 PLVECT,B,,,,VECT,ELEM,ON,0
 /VIEW,,,,1
 PLNSOL,VOLT
 *DIM,VALUE,,1,3
@@ -120,8 +124,9 @@
 *VWRITE,VALUE(1,2),VALUE(1,1),VALUE(1,3)
 ('         ',G14.5,'         ',G14.5,'          ',F8.3)
 /COM,
 /COM, ------------------------------------------------------------------------
 /OUT,
 *list,vm277,vrt
 FINISH
-
+/EXIT,NOSAVE
+/DEL,SCRATCH
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm278.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm278.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM278
 /TITLE, VM278, BEAMS CONTACT TRACTION
 C***  REFERENCE
 C***
 C***
 /PREP7
 LENGDE=100			! MODELING PARAMETERS
@@ -22,15 +22,15 @@
 MP,C,1,434			! SPECIFIC HEAT PLAIN CARBON STEEL: 434 J/(kg*K)
 MP,ALPX,1,12E-6			! COEFFICIENT OF THERMAL EXPANSION
 !*** CONTACT MATERIAL PROPERTIES ***
 !-------------------------------------
 MP,MU,2,0.2			! COEFFICIENT OF FRICTION
 !*** ELEMENT TYPES ***
 !---------------------
-ET,1,PIPE289			! 3-D 3-NODE PIPE
+ET,1,PIPE289,,,,2		! 3-D 3-NODE PIPE
 ET,2,CONTA177			! 3-D LINE-TO-SURFACE CONTACT
 KEYOPT,2,2,1			! PENALTY FUNCTION ALGORITHM
 KEYOPT,2,3,1  			! TRACTION-BASED CONTACT TYPE
 ET,3,170			! 3-D TARGET SEGMENT
 !*** SECTION DATA ***
 !--------------------
 ! EXAMPLE SECTION:
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm279.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm279.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM279
 /COM,   VERIFICATION MANUAL FOR FRACTURE MECHANCIS,
-/TITLE,VM279 T-STRESS FOR A CRACK IN A 2D PLATE
+/TITLE,VM279, T-STRESS FOR A CRACK IN A 2D PLATE
 /COM    REFERENCE: STRESS INTENSITY FACTORS, T-STRESSES, WEIGHT 
 /COM    FUNCTIONS BY THEO FETT,INSTITUTE OF CERAMICS IN
 /COM    MECHANICAL ENGINEERING (IKM),UNIVERSITY OF KARLSRUHE(TH)
 /COM    ****CRACK IN 2-DIMENSIONS USING 2-D PLANE183 ELEMENT***
 /OUT,SCRATCH
 /PREP7
 E=207000        	           ! YOUNGS MODULUS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm28.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm28.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM28
 /PREP7
 /TITLE, VM28,  TRANSIENT HEAT TRANSFER IN AN INFINITE SLAB
 /COM,   "HEAT TRANSFER", HOLMAN, 4TH ED., PG. 106
 /NOPR
 ANTYPE,TRANS
 ET,1,PLANE77
@@ -20,28 +20,32 @@
 NLIST,ALL                           ! LIST NODES ALONG LENGTH
 NSEL,S,LOC,Y,1
 SF,ALL,CONV,50,1000                 ! APPLY CONVECTION TO TOP SURFACE
 NSEL,ALL
 TUNIF,0                             ! DEFINE INITIAL TEMPERATURES, T(0)
 FINISH
 /SOLU    
-SOLCONTROL,0
 KBC,1                               ! STEP BOUNDARY CONDITIONS
 DELTIM,10                           ! MINIMUM TIME STEP
 TIME,2000.0                         ! TIME AT END OF TRANSIENT
 OUTRES,,ALL
 AUTOTS,ON
+NEQIT,25
+CNVTOL,HEAT,,,,1.0
+TINTP,,,,0.5,,0.2
+/OUT,SCRATCH
 SOLVE
 FINISH
 /POST26
 NSOL,2,11,TEMP,,T11                 ! STORE TEMPERATURES AT SELECT NODES
 NSOL,3,9,TEMP,,T9
 NSOL,4,7,TEMP,,T7
 NSOL,5,5,TEMP,,T5
 NSOL,6,1,TEMP,,T1
+/OUT,
 PRVAR,2,3,4,5,6                     ! PRINT TEMPERATURE SOLUTION VS. TIME
 *GET,TEMP_11,NODE,11,TEMP
 *GET,TEMP_9,NODE,9,TEMP
 *GET,TEMP_7,NODE,7,TEMP
 *GET,TEMP_5,NODE,5,TEMP
 
 *DIM,LABEL,CHAR,4,2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm280.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm280.dat`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM280
 /SHOW,JPEG
 JPGPRF,500,100,1                        !* MACRO TO SET PREFS FOR JPEG PLOTS
 /TITLE,VM280, CONDUCTION IN A DOUBLY INSULATED PIPE CARRYING STEAM
 C*** USING SOLID278
 /COM,  REF: KOTHANDARAMAN,C.P.,
 /COM, "FUNDAMENTALS OF HEAT AND MASS TRANSFER"-3RD EDITION, 
@@ -118,30 +118,95 @@
 LABEL(1,1) = 'TEMP @ x','TEMP @ x', 'TEMP @ x', 'TEMP @ x'
 LABEL(1,2) = '=0.06','=0.0675 ','=0.1175','=0.1675'
 LABEL(1,3) = 'T (C)','T (C)','T (C)', 'T (C)'
 *VFILL,VALUE(1,1),DATA,222.3,222.2,77.04,48.03
 *VFILL,VALUE(1,2),DATA,temp_0.06,temp_0.0675,temp_0.1175,temp_0.1675
 *VFILL,VALUE(1,3),DATA,ABS(temp_0.06/222.3),ABS(temp_0.0675/222.2),ABS(temp_0.1175/77.04),ABS(temp_0.1675/48.03)
 SAVE,TABLE2
+FINI
+/CLEAR,NOSTART
+
+
+C*** USING SOLID291 - 3-D 10-NODE THERMAL SOLID 
+/PREP7
+CSYS,1
+ET,1,SOLID291				!*3-D 10-NODE THERMAL SOLID                       
+MP,KXX,1,49				    !*CONDUCTIVITY OF THE PIPE MATERIAL	       
+MP,KXX,2,0.15				!*CONDUCTIVITY OF FIRST LAYER OF INSULATION
+MP,KXX,3,0.48				!*CONDUCTIVITY OF SECOND LAYER OF INSULATION
+
+CYL4,,,0.06,0,0.0675,90,0.25  		!*DEFINE THE GEOMETRY OF THE SYSTEM IN METERS
+CYL4,,,0.0675,0,0.1175,90,0.25
+CYL4,,,0.1175,0,0.1675,90,0.25
+VPTN,ALL				!*PARTITIONING OF THE ENTITIES
+ESIZE,0.01				!*MESH VOLUMES
+/OUT,vm280_SCRATCH	
+MAT,1
+TYPE,1
+VMESH,1
+ALLSEL,ALL
+MAT,2
+TYPE,1
+VMESH,4
+ALLSEL,ALL
+MAT,3
+TYPE,1
+VMESH,5
+ALLSEL,ALL
+FINI
+/SOLU
+NSEL,S,LOC,X,0.06	
+SF,ALL,CONV,85,230	       
+ALLSEL,ALL
+NSEL,S,LOC,X,0.1675	
+SF,ALL,CONV,18,35	       
+ALLSEL,ALL
+ANTYPE,STATIC
+SOLVE
+FINI
+/POST1
+PLNSOL,TEMP
+*GET,TEMP_0.06,NODE,NODE(0.06,0,0),TEMP,,
+*GET,TEMP_0.0675,NODE,NODE(0.0675,0,0),TEMP
+*GET,TEMP_0.1175,NODE,NODE(0.1175,0,0),TEMP
+*GET,TEMP_0.1675,NODE,NODE(0.1675,0,0),TEMP
+
+
+*DIM,LABEL,CHAR,4,3
+*DIM,VALUE,,4,3
+LABEL(1,1) = 'TEMP @ x','TEMP @ x', 'TEMP @ x', 'TEMP @ x'
+LABEL(1,2) = '=0.06','=0.0675 ','=0.1175','=0.1675'
+LABEL(1,3) = 'T (C)','T (C)','T (C)', 'T (C)'
+*VFILL,VALUE(1,1),DATA,222.3,222.2,77.04,48.03
+*VFILL,VALUE(1,2),DATA,temp_0.06,temp_0.0675,temp_0.1175,temp_0.1675
+*VFILL,VALUE(1,3),DATA,ABS(temp_0.06/222.3),ABS(temp_0.0675/222.2),ABS(temp_0.1175/77.04),ABS(temp_0.1675/48.03)
+SAVE,TABLE3
 
 /NOPR
 /COM
 /OUT,vm280,vrt
 /COM,------------------- VM280 RESULTS COMPARISON --------------
 /COM,
 /COM,                       |   TARGET   |   MECHANICAL APDL   |   RATIO
 /COM,
 RESUME,TABLE1
 /COM, TEMPERATURES AT THE INTERFACE FOR SOLID278
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),LABEL(1,3),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,A5,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
+/COM,
 RESUME,TABLE2
 /COM, TEMPERATURES AT THE INTERFACE FOR SOLID279
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),LABEL(1,3),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,A5,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
 /COM,
+RESUME,TABLE3
+/COM, TEMPERATURES AT THE INTERFACE FOR SOLID291
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),LABEL(1,3),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,A5,'   ',F10.3,'  ',1F14.3,'   ',1F15.3)
+/COM,
 /COM,------------------------------------------------------------------
 /OUT,
 FINI
 *LIST,vm280,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm281.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm281.dat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM281
 /TITLE,VM281,EFFECT OF STRESS STIFFENING AND SPIN SOFTENING ON A ROTATING PLATE
 /COM,
 /COM, REFERENCE: NASA TECHNICAL MEMORANDUM 89861,PAGE 14,FIGURE 7
 /COM,
 
 /COM, =====================================================================
@@ -481,12 +481,13 @@
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,'   ',A8,'   'F12.3,'    ',F12.3,'    ',F8.3)
 /COM,
 /COM,---------------------------------------------------------------------------------
 /OUT,
 *LIST,vm281,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm282.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm282.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM282
 /TITLE,VM282,STEADY STATE VIBRATION ANALYSIS OF PISTON-FLUID SYSTEM
 /COM, --------------------------------------------------------------
 /COM, REFERENCE:
 /COM, F. AXISA and J. ANTUNES, MODELLING OF MECHANICAL SYSTEMS: 
 /COM, FLUID-STRUCTURE INTERACTION, VOLUME 3, 2007, PAGE:486.
 /COM, --------------------------------------------------------------
@@ -211,7 +211,8 @@
 (1X,A8,A8,'   ',F12.3,'  ',F16.3,'   ',1F15.3)
 /COM,----------------------------------------------------------
 
 /OUT,
 FINISH
 *LIST,vm282,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm283.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm283.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM283 
 /TITLE,VM283,Low Reduced Frequency Model for Visco-thermal Fluid with Thin Structure
 /COM,
 /COM, REFERENCE:
 /COM, W. M. BELTMAN, "Viscothermal Wave Propagation Including Acousto-elastic Interaction", 
 /COM, THESIS, SECTION6.3, PP128-136, ISBN 90-3651217-4, 1998.
 /COM, 
@@ -133,15 +133,16 @@
 NSEL,A,LOC,Z,zz(5)
 NSEL,R,LOC,X,-LX
 D,ALL,UZ,0,,,,UX,UY
 ALLSEL,ALL
 NSEL,S,LOC,Z,zz(6)
 SF,ALL,PORT,1                       ! PORT NUMBER
 NSEL,R,LOC,X,LX
-BF,ALL,JS,1                         ! MASS SOURCE RATE
+!BF,ALL,JS,1                         ! MASS SOURCE RATE
+BF,ALL,MASS,1
 ALLSEL,ALL
 
 NSEL,S,LOC,Z,zz(1)
 SF,ALL,IMPD,z0                      ! IMPEDANCE
 SF,ALL,PORT,2                       ! PORT NUMBER
 CM,N_IMPD,node
 ALLSEL,ALL
@@ -220,8 +221,9 @@
 *VWRITE,Frq(1),TL1(1),TL2(1),RATIO(1,1)
 (3X,A8,'   ',3X,A8,'   ',3X,A8,'  ',2X,F5.3,'  ')
 /COM,
 /COM, ---------------------------------------------------------------
 /OUT,
 *list,vm283,vrt
 FINISH
+/EXIT,NOSAVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm29.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm29.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM29
 /PREP7
 /TITLE, VM29, FRICTION ON A SUPPORT BLOCK
 C***VECTOR MECHANICS FOR ENGINEERS, BEER AND JOHNSTON, 1962, PAGE 283, PROB. 8.2
 ANTYPE,STATIC
 ET,1,CONTAC12
-R,1,-20,1E6                ! THETA = -20, STIFFNESS = 1E6
+R,1,-20,1E7                ! THETA = -20, STIFFNESS = 1E7
 MP,MU,1,.3                 ! COEFFICIENT OF FRICTION
 N,1                        ! CREATE NODES
 N,2
 E,1,2                      ! CREATE ELEMENT
 D,1,ALL                    ! BOUNDARY CONDITIONS AND LOADS
 F,2,FX,-5.7674             ! STICKING LOAD
 F,2,FY,-100
@@ -36,15 +36,15 @@
 *VFILL,VALUE_C1(1,2),DATA,NORM_FC1,SLID_FC1
 *VFILL,VALUE_C1(1,3),DATA,ABS(NORM_FC1/95.942),ABS(SLID_FC1/28.783)
 SAVE,TABLE_1
 FINISH
 /SOLU
 F,2,FX,-5.76720            ! SLIDING LOAD
 /OUT,SCRATCH
-SOLVE                      ! gRPC dies here for some reason
+SOLVE
 FINISH
 /POST1
 ETAB,NOR_FC2,SMISC,1
 ETAB,SLI_FC2,SMISC,2
 /OUT,
 *GET,NORM_FC2,ELEM,1,ETAB,NOR_FC2
 *GET,SLID_FC2,ELEM,1,ETAB,SLI_FC2
@@ -64,29 +64,29 @@
 /COM,
 /PREP7
 ANTYPE,STATIC
 ET,1,CONTA178                   ! USING CONTA178 ELEMENTS
 KEYOPT,1,2,1                    ! PURE PENALTY METHOD
 KEYOPT,1,5,0                    ! CONTACT NORMAL BASED ON REAL CONSTANTS
 KEYOPT,1,10,0                   ! STANDARD CONTACT BEHAVIOR
-R,1,-1E6,,,-1E6,,0.3420201      ! DEFINE FKN,START,FKS,NX,NY,NZ
+R,1,-1E7,,,-1E7,,0.3420201      ! DEFINE FKN,START,FKS,NX,NY,NZ
 RMORE,0.939692,0                   
 N,1,0,0,0
 N,2,0,0,0
 MP,MU,1,.3                 ! COEFFICIENT OF FRICTION
 MP,EX,1,1.0
 TYPE,1
 MAT,1
 REAL,1
 E,1,2                      ! CREATE ELEMENT
 D,1,ALL                    ! BOUNDARY CONDITIONS AND LOADS
 D,2,UZ                     ! 2D ONLY
 F,2,FX,-5.7674             ! STICKING LOAD
 F,2,FY,-100
-NSUBST,1		! LIMIT TO ONE ITERATION TO PREVENT DIVERGENCE
+NSUBST,1,                  ! LIMIT TO ONE ITERATION TO PREVENT DIVERGENCE
 AUTOTS,ON
 TIME,1.0
 OUTPR,BASIC,ALL            ! PRINT NODAL DOF, REACTION & ELEMENT SOLUTION
 OUTPR,NLOAD,ALL            ! PRINT ELEMENT NODAL LOADS
 KBC,1                      ! STEP CHANGE IN B.C.'S
 FINISH
 /SOLU    
@@ -100,17 +100,17 @@
 /OUT,
 *GET,NORM_FC3,ELEM,1,ETAB,NOR_FC3
 *GET,SLID_FC3,ELEM,1,ETAB,SLI_FC3
 *DIM,LABEL,CHAR,2,2
 *DIM,VALUE_C3,,2,3
 LABEL(1,1) = 'NORMAL ','SLIDING '
 LABEL(1,2) = 'FORCE lb','FORCE lb'
-*VFILL,VALUE_C3(1,1),DATA,-95.942,28.783
+*VFILL,VALUE_C3(1,1),DATA,-95.942,-28.783
 *VFILL,VALUE_C3(1,2),DATA,NORM_FC3,SLID_FC3
-*VFILL,VALUE_C3(1,3),DATA,ABS(NORM_FC3/95.942),ABS(SLID_FC3/28.783)
+*VFILL,VALUE_C3(1,3),DATA,ABS(NORM_FC3/95.942),ABS(SLID_FC3/(-28.783))
 SAVE,TABLE_3
 FINISH
 /SOLU
 F,2,FX,-5.76720            ! SLIDING LOAD
 /OUT,SCRATCH
 SOLVE
 FINISH
@@ -119,17 +119,17 @@
 ETAB,SLI_FC4,SMISC,2
 /OUT,
 *GET,NORM_FC4,ELEM,1,ETAB,NOR_FC4
 *GET,SLID_FC4,ELEM,1,ETAB,SLI_FC4
 *DIM,VALUE_C4,,2,3
 LABEL(1,1) = 'NORMAL ','SLIDING '
 LABEL(1,2) = 'FORCE lb','FORCE lb'
-*VFILL,VALUE_C4(1,1),DATA,-95.942,28.783
+*VFILL,VALUE_C4(1,1),DATA,-95.942,-28.783
 *VFILL,VALUE_C4(1,2),DATA,NORM_FC4,SLID_FC4
-*VFILL,VALUE_C4(1,3),DATA,ABS(NORM_FC4/95.942),ABS(SLID_FC4/28.783)
+*VFILL,VALUE_C4(1,3),DATA,ABS(NORM_FC4/95.942),ABS(SLID_FC4/(-28.783))
 SAVE,TABLE_4
 
 RESUME,TABLE_1
 /COM
 /OUT,vm29,vrt
 /COM,------------------- VM29 RESULTS COMPARISON ---------------
 /COM,
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm3.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm3.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM3
 /PREP7
 /TITLE, VM3, THERMALLY LOADED SUPPORT STRUCTURE
 C***      STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 30, PROB. 9
 ANTYPE,STATIC             ! STATIC ANALYSIS
 ET,1,LINK180
 SECTYPE,1,LINK
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm30.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm30.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM30
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 SMRT,OFF
 /TITLE, VM30, SOLID MODEL OF SURFACE FILLET
 /COM,   REF:  NAFEMS BENCHMARKS FOR FINITE ELEMENT PRE-PROCESSORS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm31.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm31.dat`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM31
-/PREP7
-/TITLE, VM31, CABLE SUPPORTING HANGING LOADS
+/TITLE,VM31,CABLE SUPPORTING HANGING LOADS
 C***VECTOR MECHANICS FOR ENGINEERS, BEER AND JOHNSTON, 1962, PAGE 260, PROB. 7.8
+/PREP7
 ANTYPE,STATIC
 ET,1,LINK180
-SECTYPE,1,LINK   
+SECTYPE,1,LINK
 SECDATA,0.1         ! AREA = .1
 MP,EX,1,20E6
 N,1                 ! DEFINE NODES
 N,2,20,-5.56
 N,3,30,-5
 N,4,45,5.83
 N,5,60,20
 E,1,2               ! DEFINE ELEMENTS
 EGEN,4,1,1
-INIS,SET,CSYS,-2    ! ARBITRARY SMALL INITIAL STRAIN 
+INIS,SET,CSYS,-2    ! ARBITRARY SMALL INITIAL STRAIN
 INIS,SET,DTYP,EPEL
 INIS,DEFINE,,,,,1E-7
 NSUBST,3
 OUTPR,,3
 OUTPR,NLOAD,3       ! PRINT NODAL FORCES
 KBC,1               ! STEP CHANGE B.C.'S
 D,1,ALL,,,5,4       ! BOUNDARY CONDITIONS AND LOADS
 D,2,UZ,,,4
 F,2,FY,-6
 F,3,FY,-12
 F,4,FY,-4
 FINISH
-/SOLU 
-NLGEOM,ON           ! LARGE DEFLECTION TURNED ON   
+/SOLU
+NLGEOM,ON           ! LARGE DEFLECTION TURNED ON
 /OUT,SCRATCH
 SOLVE
 FINISH
 /POST26
-RFORCE,2,1,F,X 
-RFORCE,3,1,F,Y 
+RFORCE,2,1,F,X
+RFORCE,3,1,F,Y
 STORE
 /OUT,
 *GET,AX,VARI,2,EXTREM,VMAX
 *GET,AY,VARI,3,EXTREM,VMAX
 FINISH
 /POST1
 ETABLE,MFX,SMISC,1
@@ -50,19 +50,86 @@
 LABEL(1,1) = 'AX, (kip','AY, (kip','MAX TENS'
 LABEL(1,2) = 's)      ','s)      ',' (kips) '
 *VFILL,VALUE(1,1),DATA,-18.000,5.0000,24.762
 *VFILL,VALUE(1,2),DATA,AX,AY,MX_FOR_X
 *VFILL,VALUE(1,3),DATA,ABS(AX/18.000) ,ABS(AY/5.000),ABS(MX_FOR_X/24.762)
 /COM
 /OUT,vm31,vrt
+/COM,
 /COM,------------------- VM31 RESULTS COMPARISON ---------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
+/COM,*** LINK180 ***
+/COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
 /COM,-----------------------------------------------------------
-
 /OUT
 FINISH
-*LIST,vm31,vrt
+!
+/CLEAR,NOSTART
+/PREP7
+ANTYPE,STATIC
+ET,1,CABLE280
+SECTYPE,1,LINK
+SECDATA,0.1         ! AREA = .1
+MP,EX,1,20E6
+N,1                 ! DEFINE NODES
+N,6,10,-2.78
+N,2,20,-5.56
+N,7,25,-5.28
+N,3,30,-5
+N,8,37.5,0.415
+N,4,45,5.83
+N,9,52.5,12.915
+N,5,60,20
+E,1,2,6             ! DEFINE ELEMENTS
+EGEN,4,1,-1
+INIS,SET,CSYS,-2    ! ARBITRARY SMALL INITIAL STRAIN
+INIS,SET,DTYP,EPEL
+INIS,DEFINE,,,,,1E-7
+NSUBST,3
+OUTPR,,3
+OUTPR,NLOAD,3       ! PRINT NODAL FORCES
+KBC,1               ! STEP CHANGE B.C.'S
+D,1,ALL,,,5,4       ! BOUNDARY CONDITIONS AND LOADS
+D,2,UZ,,,4
+F,2,FY,-6
+F,3,FY,-12
+F,4,FY,-4
+FINISH
+/SOLU
+NLGEOM,ON           ! LARGE DEFLECTION TURNED ON
+/OUT,SCRATCH
+SOLVE
+FINISH
+/POST26
+RFORCE,2,1,F,X
+RFORCE,3,1,F,Y
+STORE
+/OUT,
+*GET,AX,VARI,2,EXTREM,VMAX
+*GET,AY,VARI,3,EXTREM,VMAX
+FINISH
+/POST1
+ETABLE,MFX,SMISC,1
+*GET,MX_FOR_X,ELEM,4,ETAB,MFX
 
+*DIM,LABEL,CHAR,3,2
+*DIM,VALUE,,3,3
+LABEL(1,1) = 'AX, (kip','AY, (kip','MAX TENS'
+LABEL(1,2) = 's)      ','s)      ',' (kips) '
+*VFILL,VALUE(1,1),DATA,-18.000,5.0000,24.762
+*VFILL,VALUE(1,2),DATA,AX,AY,MX_FOR_X
+*VFILL,VALUE(1,3),DATA,ABS(AX/18.000) ,ABS(AY/5.000),ABS(MX_FOR_X/24.762)
+/COM
+/OUT,vm31,vrt,,append
+/COM,
+/COM,*** CABLE280 ***
+/COM,
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
+/COM,-----------------------------------------------------------
+/OUT,
+FINISH
+*LIST,vm31,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm32.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm32.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM32
 /PREP7
 /TITLE, VM32, THERMAL STRESSES IN A LONG CYLINDER
 !           STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 234, PROB. 1
 !           THERMAL SOLUTION ***
 ET,1,PLANE55,,,1       ! AXISYMMETRIC KEYOPT(S) OPTION
 ET,2,PLANE55,,,1
@@ -42,15 +42,15 @@
 LABEL_1(1,1) = 'T (C) X=','T (C) X=','T (C) X='
 LABEL_1(1,2) = '.1875 in','.2788 in','0.625 in'
 SAVE,TABLE_1
 
 FINISH
 /PREP7
 !           STRESS SOLUTION, STATIC ANALYSIS   ***
-ETCHG,TTS              ! CHANGE ELEMENT TYPE PLANE55 TO PLANE42
+ETCHG,TTS              ! CHANGE ELEMENT TYPE PLANE55 TO PLANE182
 KEYOPT,1,1,2
 KEYOPT,1,3,1
 KEYOPT,2,1,2
 KEYOPT,2,3,1
 MP,EX,1,30E6           ! DEFINE STRUCTURAL PROPERTIES
 MP,ALPX,,1.435E-5
 MP,NUXY,1,.3
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm33.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm33.dat`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM33
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
-SMRT,OFF
 /TITLE, VM33, TRANSIENT THERMAL STRESS IN A CYLINDER
 /COM,   REF: ROARK AND YOUNG "FORMULAS FOR STRESS AND STRAIN",5TH
 /COM,   EDITION, MCGRAW-HILL, PG. 585
 /COM,
 ET,1,SOLID5                    ! SOLID5 UX,UY,UZ,TEMP,VOLT,MAG DOF SET
 MP,KXX,1,625E-6                ! DEFINE THERMAL CONDUCTIVITY
 MP,EX,1,30E6                   ! MODULUS OF ELASTICITY
@@ -16,26 +15,22 @@
 MP,DENS,1,.284                 ! DENSITY (LB/IN**3)
 MP,C,1,.10                     ! SPECIFIC HEAT
 CSYS,1
 H=.20                          ! MODEL HEIGHT
 TH=2.5                         ! MODEL HALF-ANGLE
 A=1                            ! INNER RADIUS
 B=3                            ! OUTER RADIUS
-K,1,A,TH                       ! DEFINE KEYPOINTS
-K,2,B,TH
-KGEN,2,1,2,1,,,H
-KGEN,2,1,4,1,,-(TH*2)
-L,1,2                          ! DEFINE LINE SEGMENTS
-*REPEAT,4,2,2
-LESIZE,ALL,,,15,5
-ESIZE,,1
-V,1,2,4,3,5,6,8,7              ! DEFINE VOLUME
-MSHK,1                         ! MAPPED VOLUME MESH
-MSHA,0,3D                      ! USING HEX
-VMESH,1                        ! MESH VOLUME
+N,1,A,TH                       ! DEFINE KEYPOINTS
+N,16,B,TH
+FILL,1,16,14,2,1,,,5 
+NGEN,2,16,1,16,1,,,H 
+NGEN,2,32,1,32,1,,-(TH*2)
+E,1,2,18,17,33,34,50,49
+EGEN,15,1,-1
+SAVE                           ! SAVE DB FOR LATER USE
 NSEL,S,LOC,Y,TH
 NSEL,A,LOC,Y,-TH
 DSYM,SYMM,Y,1                  ! DEFINE STRUCTURAL B.C.
 NSEL,S,LOC,Z
 DSYM,SYMM,Z,1
 NSEL,S,LOC,Z,H                 ! SELECT NODES ON TOP SURFACE
 CP,1,UZ,ALL                    ! COUPLE ALL NODES IN UZ
@@ -57,21 +52,21 @@
 DELTIM,1,,60                   ! MINIMUM TIME STEP OF 1 SEC
 TIME,430                       ! TIME AT END OF LOAD STEP
 SOLVE
 FINISH
 /out
 /POST1
 *GET,IN_STRS,NODE,1,S,Y
-*GET,OUT_STRS,NODE,2,S,Y
+*GET,OUT_STRS,NODE,16,S,Y
 FINISH
 /POST26
 NSOL,2,1,TEMP                  ! STORE TEMP AT INNER RADIUS
-NSOL,3,2,TEMP                  ! STORE TEMP AT OUTER RADIUS
+NSOL,3,16,TEMP                 ! STORE TEMP AT OUTER RADIUS
 ESOL,4,1,1,S,Y,SYB             ! STORE SY AT INNER RADIUS
-ESOL,5,15,2,S,Y,SYC            ! STORE SY AT OUTER RADIUS
+ESOL,5,15,16,S,Y,SYC            ! STORE SY AT OUTER RADIUS
 ADD,6,3,2,,DELT,,,1,-1         ! CALCULATE DELTA TEMP. (OUTER-INNER)
 PRVAR,2,3,4,5,6                ! PRINT VARIABLES VS. TIME
 /GRID,1
 /AXLAB,Y,DELT
 PLVAR,6                        ! DISPLAY DELTA TEMP. VS TIME
 /AXLAB,Y,SY
 PLVAR,4,5                      ! DISPLAY SY VS. TIME
@@ -93,53 +88,38 @@
 (1X,A8,A8,'   ',F10.0,'  ',F14.0,'   ',1F15.3)
 /OUT
 FINISH
 !
 /CLEAR,NOSTART
 /UNITS,BIN
 /PREP7
-SMRT,OFF
+RESUME
 ET,1,SOLID226,11,0             ! SOLID226 UX,UY,UZ,TEMP
+EMID,ADD
 MP,KXX,1,625E-6*9.34E3         ! DEFINE THERMAL CONDUCTIVITY, LBF/(S-F)
 MP,EX,1,30E6                   ! MODULUS OF ELASTICITY, PSI
 MP,NUXY,1,.3                   ! POISSON'S RATIO
 MP,ALPX,1,8.4E-6               ! COEFFICIENT OF THERMAL EXPANSION, 1/F
 MP,DENS,1,.284                 ! DENSITY (LB/IN**3)
 MP,C,1,0.10*9.34E3             ! SPECIFIC HEAT, LBF-IN/(F-LB)
-CSYS,1
-H=.20                          ! MODEL HEIGHT
-TH=2.5                         ! MODEL HALF-ANGLE
-A=1                            ! INNER RADIUS
-B=3                            ! OUTER RADIUS
-K,1,A,TH                       ! DEFINE KEYPOINTS
-K,2,B,TH
-KGEN,2,1,2,1,,,H
-KGEN,2,1,4,1,,-(TH*2)
-L,1,2                          ! DEFINE LINE SEGMENTS
-*REPEAT,4,2,2
-LESIZE,ALL,,,15,5
-ESIZE,,1
-V,1,2,4,3,5,6,8,7              ! DEFINE VOLUME
-MSHK,1                         ! MAPPED VOLUME MESH
-MSHA,0,3D                      ! USING HEX
-VMESH,1                        ! MESH VOLUME
 NSEL,S,LOC,Y,TH
 NSEL,A,LOC,Y,-TH
 DSYM,SYMM,Y,1                  ! DEFINE STRUCTURAL B.C.
 NSEL,S,LOC,Z
 DSYM,SYMM,Z,1
 NSEL,S,LOC,Z,H                 ! SELECT NODES ON TOP SURFACE
 CP,1,UZ,ALL                    ! COUPLE ALL NODES IN UZ
 NSEL,S,LOC,X,B                 ! SELECT NODES AT OUTER RADIUS
 D,ALL,TEMP,500                 ! DEFINE FINAL SURFACE TEMPERATURE
 NSEL,ALL
 FINISH
 /out,scratch
 /SOLU
 ANTYPE,TRANS                   ! TRANSIENT ANALYSIS
+TIMINT,OFF,STRUC               ! SUPPRESS STRUCTURAL DYNAMICS
 CNVTOL,HEAT                    ! CONVERGENCE BASED ON HEAT FLOWS
 CNVTOL,F                       !  AND FORCES ONLY
 AUTOTS,ON                      ! AUTOMATIC TIME STEPPING
 OUTRES,,ALL                    ! RESULTS FOR ALL TIME POINTS
 KBC,0                          ! RAMP LOAD OVER LOAD STEP
 TREF,70                        ! SET REFERENCE TEMPERATURE
 TUNIF,70                       ! SET INITIAL UNIFORM TEMPERATURE
@@ -147,21 +127,21 @@
 DELTIM,1,,60                   ! MINIMUM TIME STEP OF 1 SEC
 TIME,430                       ! TIME AT END OF LOAD STEP
 SOLVE
 FINISH
 /out
 /POST1
 *GET,IN_STRS,NODE,1,S,Y
-*GET,OUT_STRS,NODE,2,S,Y
+*GET,OUT_STRS,NODE,16,S,Y
 FINISH
 /POST26
 NSOL,2,1,TEMP                  ! STORE TEMP AT INNER RADIUS
-NSOL,3,2,TEMP                  ! STORE TEMP AT OUTER RADIUS
+NSOL,3,16,TEMP                  ! STORE TEMP AT OUTER RADIUS
 ESOL,4,1,1,S,Y,SYB             ! STORE SY AT INNER RADIUS
-ESOL,5,15,2,S,Y,SYC            ! STORE SY AT OUTER RADIUS
+ESOL,5,15,16,S,Y,SYC            ! STORE SY AT OUTER RADIUS
 ADD,6,3,2,,DELT,,,1,-1         ! CALCULATE DELTA TEMP. (OUTER-INNER)
 PRVAR,2,3,4,5,6                ! PRINT VARIABLES VS. TIME
 /GRID,1
 /AXLAB,Y,DELT
 PLVAR,6                        ! DISPLAY DELTA TEMP. VS TIME
 /AXLAB,Y,SY
 PLVAR,4,5                      ! DISPLAY SY VS. TIME
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm34.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm34.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM34
 /TITLE, VM34, BENDING OF A TAPERED PLATE (BEAM)
 C***     INTROD. TO STRESS ANALYSIS, HARRIS, 1ST PRINTING, PAGE 114, PROB. 61
 C***     PLATE ELEMENTS (SHELL63)
 /PREP7
 ANTYPE,STATIC               ! STATIC ANALYSIS
 ET,1,SHELL63,2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm35.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm35.dat`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,41 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM35
 /PREP7
-SMRT,OFF
-/TITLE,VM35: BIMETALLIC LAYERED CANTILEVER PLATE WITH THERMAL LOADING
+/TITLE,VM35, BIMETALLIC LAYERED CANTILEVER PLATE WITH THERMAL LOADING
 C***     ROARK AND YOUNG, FORMULAS FOR STRESS AND STRAIN, PP. 113-114.
 C*** USING SHELL281
 ANTYPE,STATIC
 ET,1,SHELL281
 SECTYPE,1,SHELL
 SECDATA,0.05,1,0       ! LAYER 1: 0.05 THICK, MAT'L 1, THETA 0 
 SECDATA,0.05,2,0       ! LAYER 2: 0.05 THICK, MAT'L 2, THETA 0,
 MP,EX,1,3E7            ! MATERIAL PROPERTIES
 MP,EX,2,3E7
 MP,ALPX,1,1E-5
 MP,ALPX,2,2E-5
 MP,NUXY,1,0
 MP,NUXY,2,0
-K,1                    ! DEFINE GEOMETRY
-K,2,,1
-K,3,10,1
-K,4,10
-A,1,2,3,4
-ESIZE,2                ! ELEMENT SIDE LENGTHS = 2
-AMESH,1
+N,1                    ! DEFINE GEOMETRY
+N,12,,1
+N,22,10,1
+N,11,10
+FILL,1,11,9,2,1
+FILL,12,22,9,13,1
+FILL,1,12,1,23  
+FILL,3,14,1,24
+FILL,5,16,1,25
+FILL,7,18,1,26
+FILL,9,20,1,27
+FILL,11,22,1,28
+E,1,12,14,3,23,13,24,2
+E,3,14,16,5,24,15,25,4
+E,5,16,18,7,25,17,26,6
+E,7,18,20,9,26,19,27,8
+E,9,20,22,11,27,21,28,10
 NSEL,S,LOC,X
 NSEL,R,LOC,Y,.5
 D,ALL,ALL              ! FIX ONE END OF CANTILEVER
 NSEL,S,LOC,Y,0.5
 DSYM,SYMM,Y            ! SYMMETRY PLANE DOWN CENTERLINE
 NSEL,ALL
 TREF,70
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm36.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm81.dat`

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,142 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM36
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM81
 /PREP7
-/TITLE, VM36, LIMIT MOMENT ANALYSIS
-!           MECHANICS OF SOLIDS, CRANDALL AND DAHL, 1959, PAGE 389, EX. 8.9
-ANTYPE,STATIC
-ET,1,BEAM188,,,3
-ET,2,COMBIN40,,,5,             ! ROTY D.O.F. SPRING
-SECT,1,BEAM,RECT
-SECD,3.93597,3.93597
-R,2,1E12,,,,27777.8           ! DEFINE REAL CONSTANTS FOR COMBIN ELEMENTS
-R,3,1,,,,1E6
-MP,EX,1,30E6                  ! DEFINE MATERIAL PROPERTIES
-MP,NUXY,1,.3
-N,1                           ! BEGIN NODES DEFINITION
-N,2,100
-N,3,100
-N,4,150
-N,5,150
-E,1,2                         ! DEFINE BEAM ELEMENTS
-E,3,4
-TYPE,2                        ! DEFINE BREAKAWAY HINGE ELEMENTS
-REAL,2  
-E,2,3  
-E,4,5
-REAL,3  
-E,2,3  
-E,4,5                         ! EXTRA ELEMENTS FOR SOLUTION STABILITY
-OUTPR,ALL,ALL                 
-CNVTOL,M,27778,.001
-CP,1,UX,2,3                   ! COUPLE TRANSLATIONS ACROSS PLASTIC HINGE
-CPLGEN,1,UZ                   ! GENERATE 2ND SET IN DIRECTION UZ W/ SAME NODES
-CPSGEN,2,2,1,2,1              ! GENERATE TWO ADDITIONAL SETS W/ DIFFERENT NODES
-DSYM,SYMM,Y                   ! CONSTRAIN MODEL SYMMETRICALLY IN Y DIRECTION
-D,1,UZ                        ! CONSTRAIN SIMPLY SUPPORTED END AGAINST DISP.
-D,4,UZ,,,,,UX                 ! CONSTRAIN RIGID END AGAINST TWO DIRECTIONAL DISP
-D,5,ROTY                      ! CONSTRAIN RIGID END AGAINST ROTATIONAL MOVEMENT
-F,2,FZ,-1000                  ! APPLY ELASTIC FORCE AT HINGE B
+/TITLE, VM81, TRANSIENT RESPONSE OF A DROP CONTAINER (NONLINEAR)
+C***        VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND. PRINTING, PAGE 110,
+C***        EX. 4.6-1, USING NON-LINEAR TRANSIENT DYNAMIC ANALYSIS
+ET,1,COMBIN40,,,2,,,2    ! SPRING, MASS, GAP COMBINATION ELEMENT
+R,1,1973.92,,.5,1        ! SPRING STIFFNESS, MASS, AND GAP
+N,1                      ! DEFINE NODES AND ELEMENT
+N,2
+E,2,1
 FINISH
 /SOLU    
-SOLCONTROL,0
-/OUT,SCRATCH
-SOLVE                         ! WRITE LOAD STEP
+ANTYPE,TRANS             ! NONLINEAR TRANSIENT DYNAMIC ANALYSIS
+OUTRES,ALL,ALL
+TIME,1E-6
+D,2,UY
+ACEL,,386                ! BOUNDARY CONDITIONS AND LOADING
+KBC,1                    ! STEPPED BOUNDARY CONDITIONS
+CNVTOL,U,-1
+CNVTOL,F,1,0.001         ! FORCE CONVERGENCE CRITERIA
+NSUBS,1,1,1
+AUTOTS,OFF
+TINTP,,,,0.5,0.5,0.2
+SOLVE
+NSUBST,110,110,1
+TIME,.11
+SOLVE
 FINISH
-
-/POST26
-/OUT,
-RFORCE,2,1,F,Z
-RFORCE,3,5,M,Y
-STORE
-*GET,RA,VARI,2,EXTREM,VMAX 
-*GET,MC,VARI,3,EXTREM,VMAX 
-*GET,UB,NODE,2,U,Z
-*DIM,LABEL1,CHAR,3,2
+/POST26                  ! TIME-HISTORY POSTPROCESSOR
+NSOL,2,1,U,Y
+NSOL,3,1,VEL,Y           ! VELOCITY
+PRVAR,2,3
+*GET,Y1,VARI,2,RTIME,.072
+*GET,V1,VARI,3,RTIME,.072
+*GET,Y2,VARI,2,RTIME,.1
+*GET,Y3,VARI,2,RTIME,.101
+*DIM,LABEL1,CHAR,3,1
 *DIM,VALUE1,,3,3
-LABEL1(1,1) = 'DEFLECTI','REACTION','MOMENT_C'
-LABEL1(1,2) = 'ON (in) ','_A (lb) ',' (ib-lb)'
-*VFILL,VALUE1(1,1),DATA,-.02829,148.15,27778
-*VFILL,VALUE1(1,2),DATA,UB,RA,MC
-*VFILL,VALUE1(1,3),DATA,ABS(UB/.02829) ,ABS(RA/148.15 ),ABS(MC/27778)
-SAVE,TABLE_1
-FINISH
-
-/SOLUTION
-
-NSUBST,3                      ! USE CONVERGENCE CRITERIA,3 SUBSTEPS MAX
-OUTPR,ALL,LAST                ! PRINT LAST ITERATION.
-F,2,FZ,-1388.8                ! APPLY VALUE SLIGHTLY SMALLER THAN PL TO HINGE B
-/OUT,SCRATCH
-SOLVE
-FINI
-
-/POST1
-/OUT,
-ESEL,S,ELEM,,3,4
-ETABLE,ELEM_STAT,NMISC,1	    !RETRIEVE THE STATUS(COMBIN40)
-ESEL,ALL
-PRETAB,
-
-/GRAPHICS,POWER
-/ESHAPE,1
-/VIEW,1,1,1,1
-/SHOW
-
-PLETAB,ELEM_STAT                    !PLOT ELEMENT TABLE(COMBIN40 STATUS)
-*GET,PLETAB_MAX1,PLNSOL,0,MAX
-*GET,PLETAB_MIN1,PLNSOL,0,MIN
-
+LABEL1(1,1) = 'TIME sec','Y, in   ','V,in/sec'
+*VFILL,VALUE1(1,1),DATA,.07198,-1.00,-27.79
+*VFILL,VALUE1(1,2),DATA,.072,Y1,V1
+*VFILL,VALUE1(1,3),DATA,ABS(.072/.07198),ABS(Y1/1),ABS(V1/27.79)
 *DIM,LABEL2,CHAR,2,2
 *DIM,VALUE2,,2,3
-LABEL2(1,1) = 'HINGE','HINGE'
-LABEL2(1,2) = '@B','@C'
-*VFILL,VALUE2(1,1),DATA,1.0,2.0
-*VFILL,VALUE2(1,2),DATA,PLETAB_MIN1,PLETAB_MAX1
-*VFILL,VALUE2(1,3),DATA,ABS(PLETAB_MIN1/1.0) ,ABS(PLETAB_MAX1/2)
-SAVE,TABLE_2
-
-FINI
+LABEL2(1,1) = 't=.1 sec','t=1.01 s'
+LABEL2(1,2) = ' Y, in  ','ec Y, in'
+*VFILL,VALUE2(1,1),DATA,-1.5505,-1.5502
+*VFILL,VALUE2(1,2),DATA,Y2,Y3
+*VFILL,VALUE2(1,3),DATA,ABS(Y2/1.5505),ABS(Y3/1.5502)
+SAVE,TABLE1
+FINISH
+/CLEAR, NOSTART ! CLEAR THE DATABASE
+/PREP7
+/TITLE, VM81, TRANSIENT RESPONSE OF A DROP CONTAINER (QUASI-LINEAR)
+ET,1,MASS21,,,4          ! TWO-DIMENSIONAL MASS ELEMENT
+R,1,.5                   ! MASS
+N,1                      ! DEFINE NODE AND ELEMENT
+E,1
+D,1,UX
+GP,2,1,FY,1973.92,1      ! GAP CONDITION
+FINISH
 
 /SOLU
-
-F,2,FZ,-1390                  ! APPLY VALUE SLIGHTLY LARGER THAN PL TO HINGE B
-!                               LARGE DISPLACEMENT VALUES INDICATE COLLAPSE
-!                               AND PLASTIC DEFORMATION
-/OUT,SCRATCH
+ANTYPE,MODAL
+MODOPT,LANB,1           ! PERFORM MODAL SOLVE USING LANB EIGENSOLVER
+MXPAND,1
+ACEL,,386               ! CREATING LOAD VECTOR
 SOLVE
-
 FINISH
 
-/POST1
-/OUT,
-ESEL,S,ELEM,,3,4
-ETABLE,ELEM_STAT,NMISC,1		!RETRIEVE THE STATUS(COMBIN40)
-ESEL,ALL
-PRETAB,
-
-PLETAB,ELEM_STAT			!PLOT ELEMENT TABLE(COMBIN40 STATUS)
-
-*GET,PLETAB_MAX2,PLNSOL,0,MAX
-*GET,PLETAB_MIN2,PLNSOL,0,MIN
+/SOLU    
+ANTYPE,TRANS             ! TRANSIENT DYNAMIC ANALYSIS
+TRNOPT,MSUP,1,,,,,YES    ! MODE SUPERPOSITION TRANSIENT ANALYSIS, VAOUT=YES
+DELTIM,1E-3
+ACEL,0,0,0
+LVSCALE,0
+KBC,1
+OUTRES,ALL,ALL
+SOLVE
 
-*DIM,LABEL3,CHAR,2,2
-*DIM,VALUE3,,2,3
-LABEL3(1,1) = 'HINGE','HINGE'
-LABEL3(1,2) = '@B','@C'
-*VFILL,VALUE3(1,1),DATA,-2.0,2.0
-*VFILL,VALUE3(1,2),DATA,PLETAB_MIN2,PLETAB_MAX2
-*VFILL,VALUE3(1,3),DATA,ABS(ABS(PLETAB_MIN2)/2.0) ,ABS(PLETAB_MAX2/2.0)
-SAVE,TABLE_3
-FINI
+TIME,.110
+KBC,1                    ! STEPPED BOUNDARY CONDITIONS
+LVSCALE,1.0              ! SCALING THE LOAD VECTOR 
+SOLVE
+FINISH
 
-RESUME,TABLE_1
+/POST26                 ! TIME-HISTORY POSTPROCESSOR
+FILE,,rdsp              ! REDUCED DISPLACEMENTS FILE
+NSOL,2,1,U,Y
+NSOL,3,1,VEL,Y          ! CALCULATE VELOCITY
+PRVAR,2,3
+*GET,Y1,VARI,2,RTIME,.072
+*GET,V1,VARI,3,RTIME,.072
+*GET,Y2,VARI,2,RTIME,.1
+*GET,Y3,VARI,2,RTIME,.101
+*DIM,LABEL1,CHAR,3,1
+*DIM,VALUE1,,3,3
+LABEL1(1,1) = 'TIME sec','Y, in   ','V,in/sec'
+*VFILL,VALUE1(1,1),DATA,.07198,-1.00,-27.79
+*VFILL,VALUE1(1,2),DATA,.072,Y1,V1
+*VFILL,VALUE1(1,3),DATA,ABS(.072/.07198),ABS(Y1/1),ABS(V1/27.79)
+*DIM,LABEL2,CHAR,2,2
+*DIM,VALUE2,,2,3
+LABEL2(1,1) = 't=.1 sec','t=1.01 s'
+LABEL2(1,2) = ' Y, in  ','ec Y, in'
+*VFILL,VALUE2(1,1),DATA,-1.5505,-1.5502
+*VFILL,VALUE2(1,2),DATA,Y2,Y3
+*VFILL,VALUE2(1,3),DATA,ABS(Y2/1.5505),ABS(Y3/1.5502)
+SAVE,TABLE2
+RESUME,TABLE1
 /COM
-/OUT,vm36,vrt
-/COM,------------------- VM36 RESULTS COMPARISON ---------------
-/COM,
-/COM,                 |   TARGET   |   ANSYS   |   RATIO
-/COM,
-/COM,RESULTS FOR P=1000 LBS (ELASTIC):
+/OUT,vm81,vrt
+/COM,------------------- VM81 RESULTS COMPARISON --------------
 /COM,
-*VWRITE,LABEL1(1,1),LABEL1(1,2),VALUE1(1,1),VALUE1(1,2),VALUE1(1,3)
-(1X,A8,A8,'   ',F11.5,'  ',F11.5,'   ',1F5.3)
+/COM,FULL DYNAMIC     |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
+/COM,AT IMAPACT
+*VWRITE,LABEL1(1,1),VALUE1(1,1),VALUE1(1,2),VALUE1(1,3)
+(1X,A8,'   ',F18.4,'  ',F14.4,'   ',1F15.3)
 /COM,
-/NOPR
-/COM,RESULTS FOR P=1388.8 LBS:
-/COM
-RESUME,TABLE_2
+/COM,AT ZERO VELOCITY
 *VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
-(1X,A8,A8,'   ',F11.5,'  ',F11.5,'   ',1F5.3)
+(1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
 /NOPR
+RESUME,TABLE2
+/GOPR
 /COM,
-/COM,RESULTS FOR P=1390 LBS :
-/COM
-RESUME,TABLE_3
-*VWRITE,LABEL3(1,1),LABEL3(1,2),VALUE3(1,1),VALUE3(1,2),VALUE3(1,3)
-(1X,A8,A8,'   ',F11.5,'  ',F11.5,'   ',1F5.3)
+/COM,MODE SUPERPOSITION|   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-/COM,-----------------------------------------------------------
+/COM,AT IMAPACT
+*VWRITE,LABEL1(1,1),VALUE1(1,1),VALUE1(1,2),VALUE1(1,3)
+(1X,A8,'   ',F18.4,'  ',F14.4,'   ',1F15.3)
 /COM,
+/COM,AT ZERO VELOCITY
+*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
+(1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
 
+/COM,----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm36,vrt
+*LIST,vm81,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm38.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm38.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM38
 /PREP7
 /TITLE, VM38, PLASTIC LOADING OF A THICK-WALLED CYLINDER UNDER PRESSURE
 C***      STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 388, ART. 70
 
 C***     USING PLANE182
 ET,1,PLANE182,3,,1            ! AXISYMMETRIC SOLID,SIMPLIFIED ENHANCED STRAIN FORMULATION
 ET,2,SURF153,,,1,1           ! AXISYMMETRIC 2-D SURFACE EFFECT ELEMENT WITHOUT
                              !  MIDSIDE NODES
 REAL,2
 R,2,,,,,,,
 RMORE,1                      ! UNIT THICKNESS
 MP,EX,1,30E6
 MP,NUXY,1,.3
-TB,BKIN,1,1                  ! BILINEAR KINEMATIC HARDENING
+TB,PLAS,1,1,,BKIN            ! BILINEAR KINEMATIC HARDENING
 TBTEMP,70
 TBDATA,1,30000,0             ! YIELD STRESS AND ZERO TANGENT MODULUS
 N,1,4                        ! DEFINE NODES
 N,6,8
 FILL
 NGEN,2,10,1,6,1,,1
 E,11,1,2,12                  ! DEFINE ELEMENTS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm39.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm54.dat`

 * *Files 27% similar despite different names*

```diff
@@ -1,154 +1,243 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM39
-/PREP7    
-JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
-/SHOW,JPEG
-/TITLE, VM39, BENDING OF A CIRCULAR PLATE WITH A CENTER HOLE
-C***          STR. OF MATLS., TIMOSHENKO, PART 2, 3RD ED., PAGE 111, EQNS. (E,F)
-C***          USING SHELL63 ELEMENTS
-ANTYPE,STATIC
-ET,1,SHELL63
-R,1,.25                     ! DEFINE PLATE THICKNESS = .25
-MP,EX,1,30.E6
-MP,NUXY,1,.3
-CSYS,1                      ! DEFINE CYLINDRICAL C.S.
-N,1,10                      ! BEGIN NODE DEFINITION
-N,7,30
-FILL,,,,,,,,3               ! USE 3:1 SPACING RATIO FOR FILLING IN NODES 
-NGEN,2,10,1,7,1,,10
-NROTAT,1,17,1
-E,1,2,12,11                 ! DEFINE FIRST ELEMENT
-EGEN,6,1,1                  ! GENERATE NEXT 5 ELEMENTS 
-D,1,ALL,,,11,10             ! CONSTRAIN INNER EDGE IN ALL D.O.F.
-D,2,UY,,,7,,ROTX,ROTZ       ! CONSTRAIN LOWER EDGE AGAINST ROTATIONS IN X & Z
-D,12,UY,,,17,,ROTX,ROTZ     ! CONSTRAIN UPPER EDGE AGAINST ROTATIONS IN X & Z
-F,7,MY,-26.18,,17,10        ! APPLY MOMENT LOAD AT OUTER EDGE
-OUTPR,BASIC,1
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM54
+/PREP7
+/TITLE, VM54, VIBRATION OF A ROTATING CANTILEVER BLADE
+C*** CARNEGIE,W., VIBRATIONS OF ROTATING CANTILEVER BLADING,
+C*** JOURNAL OF MECHANICAL ENGINEERING SCIENCE,PG. 239,VOL.1,NO.3,1959.
+ET,1,SHELL63,,,,,,,1     ! FOUR NODE SHELL, SUPPRESS STRESS PRINTOUT
+R,1,3E-3                 ! THICKNESS OF SHELL
+MP,EX,1,217E9            ! MATERIAL, STEEL
+MP,NUXY,1,0.3
+MP,DENS,1,7850
+N,1,-.014,,.150          ! DEFINE NODES
+N,9,-.014,,.478
+FILL
+NGEN,2,9,1,9,1,.028
+E,1,2,11,10              ! DEFINE ELEMENTS
+EGEN,8,1,-1
 FINISH
-*CREATE,SOLVIT,MAC
 /SOLU    
+ANTYPE,STATIC            ! STATIC ANALYSIS, PRESTRESS
+PSTRES,ON                ! PRESTRESS ANALYSIS
+D,1,ALL,,,10,9           ! BOUNDARY CONDITIONS AND LOADING
+OMEGA,314.159265         ! SPINNING LOAD
+OUTPR,,1
 /OUT,SCRATCH
 SOLVE
 FINISH
-/POST1
-/WINDOW,1,TOP               ! SET UP WINDOW 1 FOR DISPLACEMENT CONTOUR DISPLAY
-/PLOPTS,MINM,OFF	    ! TURN OFF MN AND MX DUE TO INSTABILITY
-PLNSOL,U,Z                  ! DISPLAY PERPENDICULAR DISPLACEMENTS AS CONTOURS
-/WINDOW,1,OFF               ! TURN OFF WINDOW 1
-/NOERASE                    ! TURN OFF AUTOMATIC ERASE BETWEEN DISPLAYS
-/WINDOW,2,BOT               ! SET UP WINDOW 2 FOR EDGE DISPLACEMENT DISPLAY
-/VIEW,2,,-1                 ! CHANGE VIEW FOR WINDOW 2
-PLDISP,1                    ! DISPLAY UNDISPLACED & DISPLACED SHAPES
+/SOLU    
+ANTYPE,MODAL             ! MODAL ANALYSIS
+MODOPT,LANB,5            ! LANB EXTRACTION METHOD, EXTRACT 5 MODES
+PSTRES,ON                ! PRESTRESS ANALYSIS
+SOLVE
 /OUT,
-SHELL,TOP
-ESEL,,,,1                   ! SELECT INNER ELEMENT(ELEM #1) 
-ETABLE,MOMX,SMISC,4         ! RETRIEVE MOMENT(X) AND SX AT TOP
-ETABLE,SIGX,S,X
-PRETAB,GRP1                 ! PRINT STORED VALUES
-*GET,M1,ETAB,1,ELEM,1
-*GET,P1,ETAB,2,ELEM,1
-ESEL,,,,6                   ! SELECT OUTER ELEMENT(ELEM#6)
-ETABLE,REFL
-PRETAB,GRP1                 ! PRINT STORED VALUES 
-*GET,M2,ETAB,1,ELEM,6
-*GET,P2,ETAB,2,ELEM,6
-ESEL,ALL                        
-RSYS,1
-PRNSOL,S,COMP               ! PRINT NODAL STRESSES
-NSEL,S,LOC,X,30             ! SELECT NODES AT R=A     
-PRNSOL,DOF                  ! PRINT DISPLACEMENTS
-*GET,DEF,NODE,7,U,Z
-*GET,ROT,NODE,7,ROT,Y
-*DIM,LABEL,CHAR,2,2
-*DIM,VALUE,,2,3
-LABEL(1,1) = 'DEFLECTI','MX_SLOPE'
-LABEL(1,2) = 'ON (in) ','(rad)   '
-*VFILL,VALUE(1,1),DATA,.049064,-.0045089
-*VFILL,VALUE(1,2),DATA,DEF,ROT
-*VFILL,VALUE(1,3),DATA,ABS(DEF/.049064 ) ,ABS( ROT/.0045089)
-*DIM,LABEL2,CHAR,2,2
-*DIM,VALUE2,,2,3
-LABEL2(1,1) = 'MOMENT ','PRESSURE'
-LABEL2(1,2) = 'in-lb/in',' psi  '
-*VFILL,VALUE2(1,1),DATA,-13.783,-1323.2
-*VFILL,VALUE2(1,2),DATA,M1,P1
-*VFILL,VALUE2(1,3),DATA,ABS(M1/13.783),ABS(P1/1323.2)
-*DIM,VALUE3,,2,3
-*VFILL,VALUE3(1,1),DATA,-10.127,-972.22
-*VFILL,VALUE3(1,2),DATA,M2,P2
-*VFILL,VALUE3(1,3),DATA,ABS(M2/10.127),ABS(P2/972.22)
+*GET,FREQ,MODE,1,FREQ
+*DIM,LABEL,CHAR,1,2
+*DIM,VALUE,,1,3
+LABEL(1,1) = '     f, '
+LABEL(1,2) = 'Hz      '
+*VFILL,VALUE(1,1),DATA,52.75 
+*VFILL,VALUE(1,2),DATA,FREQ 
+*VFILL,VALUE(1,3),DATA,ABS(FREQ /52.75)
 FINISH
-*END
-SOLVIT
 SAVE,TABLE_1
-/CLEAR, NOSTART                ! CLEAR DATABASE FOR SECOND SOLUTION
-/TITLE, VM39, BENDING OF A CIRCULAR PLATE WITH A CENTER HOLE
+/CLEAR, NOSTART
+
+/TITLE, VM54, VIBRATION OF A ROTATING CANTILEVER BLADE
+C***          USING SOLSH190 ELEMENTS
+/PREP7
+SMRT,OFF
+ET,1,SOLSH190,,,,,,,1    ! ANALYZE AGAIN USING 3-D SOLSH190, SUPPRESS STRESS PRINTOUT
+THICK = 3E-3		 ! THCIKNESS = 3E-3
+R,1,THICK
+MP,EX,1,217E9            ! MATERIAL, STEEL
+MP,NUXY,1,0.3
+MP,DENS,1,7850
+N,1,-.014,,.150          ! DEFINE NODES
+N,9,-.014,,.478
+FILL
+NGEN,2,9,1,9,1,.028
+NGEN,2,18,1,18,1,,THICK
+E,1,2,11,10,19,20,29,28  ! DEFINE ELEMENTS
+EGEN,8,1,-1
+FINISH
+/SOLU    
+ANTYPE,STATIC            ! STATIC ANALYSIS, PRESTRESS
+RESCONTROL,LINEAR,ALL,1  ! NEEDED FOR PERTURBATION ANALYSIS
+D,1,ALL,,,10,9           ! BOUNDARY CONDITIONS AND LOADING
+D,19,ALL,,,28,9		 !
+OMEGA,314.159265         ! SPINNING LOAD
+OUTPR,,1
+/OUT,SCRATCH
+SOLVE
+FINISH
+
+/SOLU
+ANTYPE,STATIC,RESTART,,,PERTURB     ! RESTART FROM LAST LOAD STEP AND SUB STEP
+PERTURB,MODAL,,,PARKEEP             ! PERFORM PERTURBED MODAL SOLVE
+SOLVE,ELFORM                        ! REGENERATE ELEMENT MATRICES
+
+OUTPR,ALL,NONE
+MODOPT,LANB,5
+MXPAND,5
+SOLVE
+/OUT,
+*GET,FREQ,MODE,1,FREQ
+*DIM,LABEL,CHAR,1,2
+*DIM,VALUE,,1,3
+LABEL(1,1) = '     f, '
+LABEL(1,2) = 'Hz      '
+*VFILL,VALUE(1,1),DATA,52.75 
+*VFILL,VALUE(1,2),DATA,FREQ 
+*VFILL,VALUE(1,3),DATA,ABS(FREQ /52.75)
+FINISH
+SAVE,TABLE_2
+/CLEAR, NOSTART
+
+/TITLE, VM54, VIBRATION OF A ROTATING CANTILEVER BLADE
 C***          USING SHELL181 ELEMENTS
-/PREP7    
-ANTYPE,STATIC
-ET,1,SHELL181, , ,2
+/PREP7
+ET,1,SHELL181, , ,2,,,,1 ! SUPPRESS STRESS PRINTOUT
 SECT,1,SHELL
-SECD,.25,1                  ! DEFINE PLATE THICKNESS = .25
-MP,EX,1,30.E6
-MP,NUXY,1,.3
-CSYS,1                      ! DEFINE CYLINDRICAL C.S.
-N,1,10                      ! BEGIN NODE DEFINITION
-N,7,30
-FILL,,,,,,,,3               ! USE 3:1 SPACING RATIO FOR FILLING IN NODES 
-NGEN,2,10,1,7,1,,10
-NROTAT,1,17,1
-E,1,2,12,11                 ! DEFINE FIRST ELEMENT
-EGEN,6,1,1                  ! GENERATE NEXT 5 ELEMENTS 
-D,1,ALL,,,11,10             ! CONSTRAIN INNER EDGE IN ALL D.O.F.
-D,2,UY,,,7,,ROTX,ROTZ       ! CONSTRAIN LOWER EDGE AGAINST ROTATIONS IN X & Z
-D,12,UY,,,17,,ROTX,ROTZ     ! CONSTRAIN UPPER EDGE AGAINST ROTATIONS IN X & Z
-F,7,MY,-26.18,,17,10        ! APPLY MOMENT LOAD AT OUTER EDGE
+SECD,3E-3,1              ! THICKNESS OF SHELL
+MP,EX,1,217E9            ! MATERIAL, STEEL
+MP,NUXY,1,0.3
+MP,DENS,1,7850
+CSYS,4
+WPRO, ,-90
+RECTNG,-0.014,0.014,-0.150,-0.478
+LSEL,S,LINE,,1,3,2
+LESIZE,ALL, , ,1
+LSEL,INVE
+LESIZE,ALL, , ,9
+LSEL,ALL
+AMESH,1
+FINISH
+/OUT,SCRATCH
+/SOLU    
+ANTYPE,STATIC            ! STATIC ANALYSIS, PRESTRESS
+RESCONTROL,LINEAR,ALL,1  ! NEEDED FOR PERTURBATION ANALYSIS
+NSEL,S,LOC,Y,-0.150
+D,ALL,ALL
+NSEL,ALL
+OMEGA,314.159265         ! SPINNING LOAD
 OUTPR,NSOL,1
 OUTPR,RSOL,1
+SOLVE
 FINISH
-SOLVIT
-SAVE,TABLE_2
-/NOPR
+/SOLU
+ANTYPE,STATIC,RESTART,,,PERTURB     ! RESTART FROM LAST LOAD STEP AND SUB STEP
+PERTURB,MODAL,,,PARKEEP             ! PERFORM PERTURBED MODAL SOLVE
+SOLVE,ELFORM                        ! REGENERATE ELEMENT MATRICES
+
+OUTPR,ALL,NONE
+MODOPT,LANB,5
+MXPAND,5
+SOLVE
+/OUT,
+*GET,FREQ,MODE,1,FREQ
+*DIM,LABEL,CHAR,1,2
+*DIM,VALUE,,1,3
+LABEL(1,1) = '     f, '
+LABEL(1,2) = 'Hz      '
+*VFILL,VALUE(1,1),DATA,52.75 
+*VFILL,VALUE(1,2),DATA,FREQ 
+*VFILL,VALUE(1,3),DATA,ABS(FREQ /52.75)
+FINISH
+SAVE,TABLE_3
+
+/CLEAR, NOSTART
+/TITLE, VM54, VIBRATION OF A ROTATING CANTILEVER BLADE
+C***          USING SHELL281 ELEMENTS
+/PREP7
+ET,1,SHELL281, , ,,,,,1 ! SUPPRESS STRESS PRINTOUT
+SECT,1,SHELL
+SECD,3E-3,1              ! THICKNESS OF SHELL
+MP,EX,1,217E9            ! MATERIAL, STEEL
+MP,NUXY,1,0.3
+MP,DENS,1,7850
+CSYS,4
+WPRO, ,-90
+RECTNG,-0.014,0.014,-0.150,-0.478
+LSEL,S,LINE,,1,3,2
+LESIZE,ALL, , ,1
+LSEL,INVE
+LESIZE,ALL, , ,9
+LSEL,ALL
+AMESH,1
+FINISH
+/SOLU    
+ANTYPE,STATIC            ! STATIC ANALYSIS, PRESTRESS
+RESCONTROL,LINEAR,ALL,1  ! NEEDED FOR PERTURBATION ANALYSIS
+NSEL,S,LOC,Y,-0.150
+D,ALL,ALL
+NSEL,ALL
+OMEGA,314.159265         ! SPINNING LOAD
+OUTPR,NSOL,1
+OUTPR,RSOL,1
+/OUT,SCRATCH
+SOLVE
+FINISH
+/SOLU
+ANTYPE,STATIC,RESTART,,,PERTURB     ! RESTART FROM LAST LOAD STEP AND SUB STEP
+PERTURB,MODAL,,,PARKEEP             ! PERFORM PERTURBED MODAL SOLVE
+SOLVE,ELFORM                        ! REGENERATE ELEMENT MATRICES
+
+OUTPR,ALL,NONE
+MODOPT,LANB,5
+MXPAND,5
+SOLVE
+/OUT,
+*GET,FREQ,MODE,1,FREQ
+*DIM,LABEL,CHAR,1,2
+*DIM,VALUE,,1,3
+LABEL(1,1) = '     f, '
+LABEL(1,2) = 'Hz      '
+*VFILL,VALUE(1,1),DATA,52.75 
+*VFILL,VALUE(1,2),DATA,FREQ 
+*VFILL,VALUE(1,3),DATA,ABS(FREQ /52.75)
+FINISH
+SAVE,TABLE_4
+FINISH
+/CLEAR,NOSTART
+
 RESUME,TABLE_1
 /COM
-/OUT,vm39,vrt
-/COM,------------------- VM39 RESULTS COMPARISON --------------
+/OUT,vm54,vrt
+/COM,------------------- VM54 RESULTS COMPARISON ---------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-/COM,RESULTS USING SHELL63:
+/COM, SHELL63
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.7,'  ',F14.7,'   ',1F15.3)
-/COM,
-/COM,X=10.81 in
-/COM,
-*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
-(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
-/COM,
-/COM,X=27.1 in
-/COM,
-*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE3(1,1),VALUE3(1,2),VALUE3(1,3)
-(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
 /NOPR
 RESUME,TABLE_2
-/GOPR
 /COM,
-/COM,RESULTS USING SHELL181:
+/COM, SOLSH190 USING LINEAR PERTURBATION ANALYSIS
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.7,'  ',F14.7,'   ',1F15.3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
+/NOPR
+RESUME,TABLE_3
 /COM,
-/COM,X=10.81 in
+/COM, SHELL181 USING LINEAR PERTURBATION ANALYSIS
 /COM,
-*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE2(1,1),VALUE2(1,2),VALUE2(1,3)
-(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
+/NOPR
+RESUME,TABLE_4
 /COM,
-/COM,X=27.1 in
+/COM, SHELL281 USING LINEAR PERTURBATION ANALYSIS
 /COM,
-*VWRITE,LABEL2(1,1),LABEL2(1,2),VALUE3(1,1),VALUE3(1,2),VALUE3(1,3)
-(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
-/COM,----------------------------------------------------------
+*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(1X,A8,A8,'   ',F10.2,'  ',F14.2,'   ',1F15.3)
+/COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm39,vrt
+*LIST,vm54,vrt
+/DELETE,TABLE_1
+/DELETE,TABLE_2
+/DELETE,TABLE_3
+/DELETE,TABLE_4
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm4.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm4.dat`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM4
 /PREP7
 /TITLE, VM4, DEFLECTION OF A HINGED SUPPORT
 C***     STR. OF MATL., TIMOSHENKO, PART 1, 3RD ED., PAGE 10, PROB. 2
 L=15*12                         ! LENGTH OF BAR IN INCHES
 *AFUN,DEG                       ! TRIG FUNCTIONS IN DEGREES 
 THETA=30                        ! ANGLE TO BE USED TO CALCULATE A AND B
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm40.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm40.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 140 (11/26/2011) REF. VERIF. MANUAL: REL. 140
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM40
 /PREP7                
 MP,PRXY,,0.3
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM40, LARGE DEFLECTION AND ROTATION OF A BEAM PINNED AT ONE END
 C***           REFERENCE - ANY BASIC MATHEMATICS BOOK
@@ -14,31 +14,34 @@
 SECD,1,1,0.1,1,1,1    ! ARBITRARY GEOMETRIC PROPERTIES
 MP,EX,1,30E6          ! DEFINE MATERIAL PROPERTIES
 MP,DENS,1,1E-10       ! DEFINE DENSITY OF ALMOST ZERO
 N,1                   ! BEGIN NODAL DEFINITION
 N,2,10
 E,1,2                 ! DEFINE ELEMENT
 FINISH
-/out,scratch
+/OUT,SCRATCH
 /SOLU    
-SOLCONTROL,0
 D,1,ROTZ,PI*2         ! ONE COMPLETE REVOLUTION
 D,1,UX,,,,,UY         ! CONSTRAIN NODE 1 (PINNED END OF BEAM)
 D,ALL,UZ
 D,ALL,ROTX
 D,ALL,ROTY
-NSUBST,24
+NSUBST,24,24,1
 TIME,.15              ! TIME STEP OF 0.00625 SEC. (.15/24)
 OUTRES,NSOL,1         ! SAVE NODAL DOF SOLUTION FOR EVERY SUBSTEP
 OUTRES,ESOL,1         ! SAVE ELEMENT SOLUTION FOR EVERY SUBSTEP
 CNVTOL,F,1,0.00001    ! CONVERGENCE CRITERION BASED UPON FORCES
 CNVTOL,M,1,0.00001    ! CONVERGENCE CRITERION BASED UPON MOMENTS
+AUTOTS,OFF
+NEQIT,25
+TINTP,,,,0.5,0.5,0.2
+KBC,0
 SOLVE
 FINISH
-/out
+/OUT
 /POST26
 NSOL,2,2,U,X,UX        ! DEFINE NODE 2 UX DISP AS VARIABLE 2
 NSOL,3,2,U,Y,UY        ! DEFINE NODE 2 UY DISP AS VARIABLE 3
 NSOL,4,1,ROT,Z,ROTZ    ! DEFINE NODE 1 ROTZ AS VARIABLE 4
 ESOL,6,1,,SMISC,36,SDIR! GET AXIAL STRESS OF ELEMENT AT NODE 2
 DERIV,5,4,,,INPUT_W    ! CALCULATE DERIVATIVE OF VAR. 4 WRT VARIABLE 1 (TIME)
 PRVAR,2,3,4,5,6        ! PRINT VARIABLES 1 THRU 6
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm41.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm80.dat`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,73 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM41
-/PREP7
-MP,PRXY,,0.3
-/TITLE, VM41, SMALL DEFLECTION OF A RIGID BEAM
-!COM           REFERENCE - ANY BASIC STRENGTH OF MATERIAL BOOK
-!COM           USING THICK BEAM GEOMETRY
-ET,1,MATRIX27,,,4          ! KEYOPT(3)=4, INPUT DATA AS 12 X 12 STIFFNESS MATRIX
-ET,2,BEAM188
-R,1                        ! TABLE 1 REAL CONSTANTS FOR MATRIX27 STIFFNESS MATRIX
-RMODIF,1,51,10000          ! MODIFY POSITIONS 51, 57 AND 78 IN TABLE 1
-RMODIF,1,78,10000          ! RMODIF USED, RATHER THAN RMORE, FOR EASIER INPUT
-RMODIF,1,57,-10000
-SECT,2,BEAM,ASEC           ! RIGID BEAM PROPERTIES
-SECD,100,1000,1,1000,,1
-MP,EX,1,30E6
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM80
+/PREP7    
+JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
+/SHOW,JPEG
+/TITLE, VM80, PLASTIC RESPONSE TO A SUDDENLY APPLIED CONSTANT FORCE
+C***           INTRODUCTION TO STRUCT. DYNAMICS, BIGGS, PAGE 69, ART. 2.7
+ANTYPE,TRANS        ! FULL TRANSIENT DYNAMIC ANALYSIS
+ET,1,LINK180
+ET,2,MASS21,,,4     ! TWO-DIMENSIONAL MASS
+SECTYPE,1,LINK   
+SECDATA,.278		    ! AREA (A)
+R,2,0.0259          ! MASS
+MP,EX,1,30E3
+TB,PLAS,1,1,,BKIN   ! BILINEAR KINEMATIC HARDENING STRESS-STRAIN CURVE
+TBTEMP,0
+TBDATA,1,162.9,0    ! YIELD STRESS AND TANGENT MODULUS
 N,1
-N,2
-N,3,10
-E,1,2                      ! STIFFNESS MATRIX ELEMENT
-TYPE,2
-SECN,2
-E,2,3                      ! BEAM ELEMENT
-OUTPR,ALL,1                ! PRINT ALL ITEMS
-D,1,ROTZ
-D,2,UX,,,,,UY
-F,3,FY,-10
+N,2,,-100
+E,1,2
 D,ALL,UZ
-D,ALL,ROTX
-D,ALL,ROTY
+TYPE,2
+REAL,2
+E,1
 FINISH
 /SOLU    
+KBC,1               ! STEP BOUNDARY CONDITIONS
+TIME,4E-3           ! TIME AT THE END OF LOAD STEP 1
+D,1,UX,,,2
+D,2,UY
+F,1,FY,30           ! APPLY F1
+NSUBST,10,10,1     ! 10 SUBSTEPS FOR  TIME STEP OF .0004
+OUTPR,BASIC,1       ! PRINT BASIC SOLUTION FOR EACH SUBSTEP
+OUTRES,NSOL,1       ! STORE NODAL SOLUTION FOR EACH SUBSTEP
+AUTOTS,OFF
+TINTP,,,,0.5,0.5,0.2
 /OUT,SCRATCH
 SOLVE
+TIME,.14            ! FINAL TIME SLIGHTLY MORE THAN 1 CYCLE OF VIBRATION
+NSUBST,68,68,1     ! 68 REPEATS FOR TIME STEP OF 0.002 
+OUTPR,BASIC,8       ! PRINT BASIC SOLUTION FOR EVERY 8TH SUBSTEP
+SOLVE
 FINISH
 /POST26
 /OUT,
-ESOL,2,2,,SMISC,32,SBEN
-STORE
-*GET,STRS_BEN,VARI,2,EXTREM,VMAX
-FINISH
-/POST1
-*GET,DEF_X,NODE,3,U,X
-*GET,DEF_Y,NODE,3,U,Y
-*GET,ROT_Z,NODE,3,ROT,Z
+NSOL,2,1,U,Y,UY       ! STORE UY DISPLACEMENTS OF NODE 1 AGAINST TIME
+PRVAR,2               ! PRINT VARIABLE 2 (DISPLACEMENT UY OF NODE 1) V/S TIME
+/GRID,1               ! TURN THE GRID ON FOR DISPLAY
+/AXLAB,Y,DISPLACEMENT ! MAKE Y-AXIS LABEL AS DISP FOR DISPLAY
+PLVAR,2               ! DISPLAY VARIABLE 2 (DISPLACEMENT UY OF NODE 1) V/S TIME
+*GET,YMAX,VARI,2,EXTREM,VMAX
+*GET,TMAX,VARI,2,EXTREM,TMAX
+*GET,YMIN,VARI,2,RTIME,.122 
+TMIN = .122
 *DIM,LABEL,CHAR,4,2
 *DIM,VALUE,,4,3
-LABEL(1,1) = 'DEFLECTI','DEFLECTI','ROTATION','SIG_BEND'
-LABEL(1,2) = 'ON_X(in)','ON_Y(in)','   (rad)','   (psi)'
-*VFILL,VALUE(1,1),DATA,0,-.1,-.01,0
-*VFILL,VALUE(1,2),DATA,DEF_X,DEF_Y,ROT_Z,STRS_BEN
-*VFILL,VALUE(1,3),DATA,0,ABS(DEF_Y/.1 ),ABS(ROT_Z/.01),0
-SAVE,TABLE_1
-FINISH
-/PREP7
-!COM         USING CONSTRAINT EQUATIONS
-SECN,2                     ! BEAM PROPERTIES
-SECD,.0625,.00032552,.00001,.00032552,,1
-CE,1,,3,UY,1,2,ROTZ,-10    ! CONSTRAINT EQUATION
-FINISH
-/SOLU    
-/OUT,SCRATCH
-SOLVE
-FINISH
-/POST26
-/OUT,
-ESOL,2,2,,SMISC,32,SBEN
-STORE
-*GET,STRS_BEN,VARI,2,EXTREM,VMAX
-FINISH
-/POST1
-*GET,DEF_X,NODE,3,U,X
-*GET,DEF_Y,NODE,3,U,Y
-*GET,ROT_Z,NODE,3,ROT,Z 
-LABEL(1,1) = 'DEFLECTI','DEFLECTI','ROTATION','SIG_BEND'
-LABEL(1,2) = 'ON_X(in)','ON_Y(in)','   (rad)','   (psi)'
-*VFILL,VALUE(1,1),DATA,0,-.1,-.01,0
-*VFILL,VALUE(1,2),DATA,DEF_X,DEF_Y,ROT_Z,STRS_BEN
-*VFILL,VALUE(1,3),DATA,0,ABS(DEF_Y/.1 ),ABS(ROT_Z/.01),0
-SAVE,TABLE_2
-RESUME,TABLE_1
+LABEL(1,1) = 'Y_MAX, i','TIME, se','Y_MIN, i','TIME, se'
+LABEL(1,2) = 'n       ','c       ','n       ','c       '
+*VFILL,VALUE(1,1),DATA,.806,.0669,.438,.122
+*VFILL,VALUE(1,2),DATA,YMAX,TMAX,YMIN,TMIN
+*VFILL,VALUE(1,3),DATA,ABS(YMAX/.806),ABS(TMAX/.0669),ABS(YMIN/.438),ABS(TMIN/.122)
 /COM
-/OUT,vm41,vrt
-/COM,------------------- VM41 RESULTS COMPARISON ---------------
+/OUT,vm80,vrt
+/COM,------------------- VM80 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-/COM,RESULTS FOR THICK BEAM:
-/COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F13.2,'   ',1F15.3)
-/NOPR
-RESUME,TABLE_2
-/GOPR
-/COM,
-/COM,RESULTS WITH CONSTRAINT EQUATION:
-/COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.2,'  ',F13.2,'   ',1F15.3)
-/COM,-----------------------------------------------------------
+(1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
+/COM,----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm41,vrt
-
+*LIST,vm80,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm42.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm42.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM42
 /PREP7
 smrt,off
 /TITLE, VM42, BARREL VAULT ROOF UNDER SELF WEIGHT
 /COM, REF:  COOK, CONCEPTS AND APPL. OF F.E.A., 2ND ED., 1981, PP. 284-287.
 C***          USING SHELL181 ELEMENTS
 ANTYPE,STATIC
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm43.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm43.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM43
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 SMRT,OFF
 /TITLE, VM43, BENDING OF AN AXISYMMETRIC THICK PIPE UNDER GRAVITY LOADING
 C***           FORMULAS FOR STRESS AND STRAIN, ROARK, 4TH ED., PAGE 112, NO. 33
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm44.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm44.dat`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM44
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7    
 /TITLE, VM44, BENDING OF AN AXISYMMETRIC THIN PIPE UNDER GRAVITY LOADING
 C***          FORMULAS FOR STRESS AND STRAIN, ROARK, 4TH ED., PAGE 112, NO. 33
 ANTYPE,STATIC
@@ -24,16 +24,18 @@
 ACEL,386,,-386          ! GRAVITY AS THE SUM OF TWO HARMONICALLY VARYING LOADS
 MODE,1,1                ! MODE NUMBER 1, SYMMETRIC LOADING
 D,1,ALL                 ! FIXED END
 NSEL,S,LOC,Y,125
 DSYM,SYMM,Y             ! CENTER PLANE END
 NSEL,ALL
 FINISH
-/SOLU    
+/SOLU 
+/OUT,vm44_SCRATCH   
 SOLVE
+/OUT
 FINISH
 /POST1
 SET,1,1,,,,0.0          ! GET RESULTS AT 0 DEGREES
 /VUP,1,X                ! DEFINE X AXIS AS VERTICAL FOR VIEWING
 /WINDOW,1,TOP           ! DEFINE WINDOW 1 AS TOP HALF OF SCREEN 
 PLDISP,1                ! DISPLAY BOTH DISTORTED AND UNDISTORTED GEOMETRY
 PRNSOL,DOF              ! PRINT DEGREE OF FREEDOM VALUES
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm45.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm45.dat`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM45
 /PREP7
 /TITLE, VM45, NATURAL FREQUENCY OF A SPRING-MASS SYSTEM
 C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 6, EX. 1.2-2
 ANTYPE,MODAL
 MODOPT,LANB,1
 ET,1,COMBIN14,,,2     ! TWO-DIMENSIONAL LONGITUDINAL SPRING
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm46.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm46.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,38 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM46
 /TITLE, VM46, TWO DIMENSIONAL END NOTCHED FLEXURE PROBLEM
 /COM, REFERENCE:" J.F.MANDELL, ET AL., PREDICTION OF DELAMINATION IN 
 /COM,             WIND TURBINE BLADE STRUCTURAL DETAILS
 /COM,             JOURNAL OF SOLAR ENERGY ENGINEERING, VOL. 25, 2003, PG: 522-530
 /COM,
 /OUT,SCRATCH
 /PREP7
 ET,1,PLANE182               ! ELEMENT TYPE 182
 KEYOPT,1,3,2                ! PLANE STRAIN
 
 !MATERIAL PROPERTIES
 YOUNG = 210000              ! YOUNG'S MODULUS
-NU = 0.3                    ! POISSION'S RATIO
-MP,EX,1,YOUNG               !MPa
+NU = 0.3                    ! POISSON'S RATIO
+MP,EX,1,YOUNG               ! MPa
 MP,PRXY,1,NU
 L=30                        ! DISTANCE FROM THE SUPPORT POINT TO LOADING POINT
 H=0.6                       ! THICKNESS OF BEAM
 AA=10.0                     ! CRACK LENGTH
 D=3                         ! THE LEFT END TO SUPPORT POINT
 BB=0.2                      ! FINE MESH AREA
 PP=-10                      ! LOADING
 B=1                         ! SPECIMEN WIDTH
 NN=1                        ! CHANGE OF MESH SIZE
 
+_geomgen=0
+_exit=0
+
+*if,_geomgen,eq,1,then
+
 K,1,0,0
 K,2,2*(D+L)
 K,3,2*(D+L),2*H
 K,4,,2*H
 K,5,,H
 K,6,D+AA,H
 K,7,,H
@@ -69,15 +74,15 @@
 RMORE,0,1.0,1.0,0.0,,1.0
 KEYOPT,3,3,0
 KEYOPT,3,4,0
 KEYOPT,3,5,0
 KEYOPT,3,7,0
 KEYOPT,3,8,0
 KEYOPT,3,9,0
-KEYOPT,3,10,2   
+KEYOPT,3,10,0   
 KEYOPT,3,11,0   
 KEYOPT,3,12,0   
 KEYOPT,3,2,0
 
 LSEL,S,,,5,23,18                   ! Generate the target surface   
 CM,_TARGET,LINE 
 TYPE,2  
@@ -90,18 +95,14 @@
 CM,_CONTACT,LINE
 TYPE,3  
 NSLL,S,0
 ESLN,S,0
 ESURF   
 ALLSEL  
 
-FINISH
-
-/SOLU
-TIME,1
 KSEL,S,KP,,21
 NSLK,S
 D,ALL,UX
 D,ALL,UY
 ALLSEL
 KSEL,S,KP,,22
 NSLK,S
@@ -112,14 +113,34 @@
 F,ALL,FY,PP
 ALLSEL
 KSEL,S,KP,,6
 NSLK,S
 CM,TIPP,NODE
 ALLSEL,ALL
 
+
+
+cdwrite,all,vm46,cdb
+
+*if,_exit,eq,1,then
+   /exit,nosave
+*endif
+
+*else
+
+/out,scratch
+/PREP7 
+   cdread,db,vm46,cdb
+*endif
+
+FINISH
+
+/SOLU
+TIME,1
+
 CINT,NEW,1                    ! DEFINE CRACK ID
 CINT,TYPE,VCCT 
 CINT,CTNC,TIPP                ! DEFINE CRACK TIP NODE COMPONENT         
 CINT,SYMM,OFF                 ! SYMMETRY OFF
 CINT,NORMAL                   ! DEFINE CRACK PLANE NORMAL
 CINT,LIST
 ALLSEL,ALL
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm47.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm47.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM47
 /PREP7
 /TITLE, VM47, TORSIONAL FREQUENCY OF A SUSPENDED DISK
 C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 10, EX 1.3-2
 ANTYPE,MODAL
 MODOPT,LANB,1,,,     
 ET,1,COMBIN14,,,1    ! THREE-DIMENSIONAL TORSIONAL SPRING
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm48.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm50.dat`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,54 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM48
-/TITLE, VM48, NATURAL FREQUENCY OF A MOTOR-GENERATOR
-C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 10, EX 1.3-3
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM50
 /PREP7
-ET,1,BEAM188           ! 3D 2 NODE BEAM
-SECTYPE,1,BEAM,CSOLID
-SECDATA,0.375/2,20     ! RADIUS AND NUMBER OF DIVISION AROUND CIRCUMFERENCE
-
-ET,2,MASS21            ! GENERALIZED MASS
-R,2,,,,31E-3           ! REAL CONSTANT SET 2 IXX
-MP,EX,1,31.2E6         ! DEFINE MODULUS OF ELASTICITY
-MP,PRXY,,0.3
-N,1                    ! BEGIN NODE DEFINITION
-N,2,8
-E,1,2                  ! DEFINE PIPE ELEMENT
-TYPE,2                 ! DEFINE ACTIVE ELEMENT TYPE AS SET #2
-REAL,2                 ! DEFINE ACTIVE REAL CONSTANT TYPE AS SET #2
-E,2                    ! DEFINE MASS AT END OF PIPE
-OUTPR,BASIC,1
-D,ALL,ALL              ! CONSTRAIN ALL DOF'S
-DDELE,2,ROTX           ! RELEASE TORSIONAL DOF AT NODE 2
+/TITLE, VM50, FUNDAMENTAL FREQUENCY OF A SIMPLY SUPPORTED BEAM
+C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 18, EX 1.5-1
+ET,1,BEAM189         ! THREE DIMENSIONAL ELASTIC BEAM
+MP,EX,1,30E6         ! DEFINE MATERIAL PROPERTIES
+MP,DENS,1,728E-6
+MP,GXY,1,30E6/2.6
+SECT,1,BEAM,ASEC
+SECD,4,(4/3),1e-6,(4/3),,1e-6
+K,1                  ! BEGIN DEFINING KEYPOINTS
+K,2,80
+L,1,2                ! DEFINE LINE WITH
+LESIZE,ALL,,,4       !  4 DIVISIONS
+LMESH,1              ! MESH LINE
+ALLSEL,ALL
+D,ALL,UZ
+D,ALL,ROTY
+D,ALL,ROTX
 FINISH
-/SOLU 
-ANTYPE,MODAL  
-MODOPT,LANB,1,,, 
+/out,scratch
+/SOLU    
+ANTYPE,MODAL
+MODOPT,LANB,3,,,
+MXPAND,3             ! EXPAND FIRST MODE
+OUTPR,ALL,1
+DK,ALL,UX            ! CONSTRAIN ENDS OF BEAM IN DISP. X DOF
+DK,ALL,UY            ! CONSTRAIN ENDS OF BEAM IN DISP. Y DOF
 SOLVE
+FINISH
+/out
+/POST26
 *GET,FREQ,MODE,1,FREQ
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
-LABEL(1,1) = '      F,'
-LABEL(1,2) = ' (Hz)  '
-*VFILL,VALUE(1,1),DATA,48.781
+LABEL(1,1) = '       f'
+LABEL(1,2) = ', (Hz)  '
+*VFILL,VALUE(1,1),DATA,28.766 
 *VFILL,VALUE(1,2),DATA,FREQ
-*VFILL,VALUE(1,3),DATA,ABS(FREQ/48.781)
+*VFILL,VALUE(1,3),DATA,ABS(FREQ/28.766) 
 /COM
-/OUT,vm48,vrt
-/COM,------------------- VM48 RESULTS COMPARISON ---------------
+/OUT,vm50,vrt
+/COM,------------------- VM50 RESULTS COMPARISON ---------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
-/COM,----------------------------------------------------------
-
+/COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm48,vrt
+*LIST,vm50,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm49.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm49.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM49   
 /PREP7 
 SMRT,OFF 
 /TITLE, VM49, ELECTROSTATIC FIELD ANALYSIS OF QUADPOLE WIRES IN OPEN AIR
 C*** ANY BASIC STATIC AND DYNAMIC ELECTRICITY BOOK
 ANTYPE,STATIC
 ET,1,PLANE121                ! 2-D 8-NODE ELECTROSTATIC ELEMENT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm50.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm48.dat`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,49 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM50
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM48
+/TITLE, VM48, NATURAL FREQUENCY OF A MOTOR-GENERATOR
+C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 10, EX 1.3-3
 /PREP7
-/TITLE, VM50, FUNDAMENTAL FREQUENCY OF A SIMPLY SUPPORTED BEAM
-C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 18, EX 1.5-1
-ET,1,BEAM189         ! THREE DIMENSIONAL ELASTIC BEAM
-MP,EX,1,30E6         ! DEFINE MATERIAL PROPERTIES
-MP,DENS,1,728E-6
-MP,GXY,1,30E6/2.6
-SECT,1,BEAM,ASEC
-SECD,4,(4/3),1e-6,(4/3),,1e-6
-K,1                  ! BEGIN DEFINING KEYPOINTS
-K,2,80
-L,1,2                ! DEFINE LINE WITH
-LESIZE,ALL,,,4       !  4 DIVISIONS
-LMESH,1              ! MESH LINE
-ALLSEL,ALL
-D,ALL,UZ
-D,ALL,ROTY
-D,ALL,ROTX
+ET,1,BEAM188           ! 3D 2 NODE BEAM
+SECTYPE,1,BEAM,CSOLID
+SECDATA,0.375/2,20     ! RADIUS AND NUMBER OF DIVISION AROUND CIRCUMFERENCE
+
+ET,2,MASS21            ! GENERALIZED MASS
+R,2,,,,31E-3           ! REAL CONSTANT SET 2 IXX
+MP,EX,1,31.2E6         ! DEFINE MODULUS OF ELASTICITY
+MP,PRXY,,0.3
+N,1                    ! BEGIN NODE DEFINITION
+N,2,8
+E,1,2                  ! DEFINE PIPE ELEMENT
+TYPE,2                 ! DEFINE ACTIVE ELEMENT TYPE AS SET #2
+REAL,2                 ! DEFINE ACTIVE REAL CONSTANT TYPE AS SET #2
+E,2                    ! DEFINE MASS AT END OF PIPE
+OUTPR,BASIC,1
+D,ALL,ALL              ! CONSTRAIN ALL DOF'S
+DDELE,2,ROTX           ! RELEASE TORSIONAL DOF AT NODE 2
 FINISH
-/out,scratch
-/SOLU    
-ANTYPE,MODAL
-MODOPT,LANB,3,,,
-MXPAND,3             ! EXPAND FIRST MODE
-OUTPR,ALL,1
-DK,ALL,UX            ! CONSTRAIN ENDS OF BEAM IN DISP. X DOF
-DK,ALL,UY            ! CONSTRAIN ENDS OF BEAM IN DISP. Y DOF
+/SOLU 
+ANTYPE,MODAL  
+MODOPT,LANB,1,,, 
 SOLVE
-FINISH
-/out
-/POST26
 *GET,FREQ,MODE,1,FREQ
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
-LABEL(1,1) = '       f'
-LABEL(1,2) = ', (Hz)  '
-*VFILL,VALUE(1,1),DATA,28.766 
+LABEL(1,1) = '      F,'
+LABEL(1,2) = ' (Hz)  '
+*VFILL,VALUE(1,1),DATA,48.781
 *VFILL,VALUE(1,2),DATA,FREQ
-*VFILL,VALUE(1,3),DATA,ABS(FREQ/28.766) 
+*VFILL,VALUE(1,3),DATA,ABS(FREQ/48.781)
 /COM
-/OUT,vm50,vrt
-/COM,------------------- VM50 RESULTS COMPARISON ---------------
+/OUT,vm48,vrt
+/COM,------------------- VM48 RESULTS COMPARISON ---------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
-/COM,-----------------------------------------------------------
+/COM,----------------------------------------------------------
+
 /OUT
 FINISH
-*LIST,vm50,vrt
+*LIST,vm48,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm51.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm51.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/OUT,SCRATCH
 /VERIFY,VM51
 JPGPRF,500,100,1                ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
+_GEOMGEN_1=0                    ! SET THIS TO 1 TO UPDATE CDB FILE 
+_EXIT1=0                       ! SET THIS TO 1 TO EXIT WITHOUT SOLVING
+*IF,_GEOMGEN_1,EQ,1,THEN 
 /TITLE,VM51, FORCE BETWEEN CHARGED SPHERES
 C*** USING SOLID122
-!            THE ELECTROMAGNETIC FIELD,  SHADOWITZ, PAGE 61
+!         THE ELECTROMAGNETIC FIELD,  SHADOWITZ, PAGE 61
 /PREP7
 smrt,off $ shpp,warn
 mopt,amesh,alte
 mopt,qmesh,alte
 R1 = 1                          ! SPHERE RADIUS
 R2 = 3                          ! DISTANCE BETWEEN SPHERES
 R3 = 6                          ! RADIUS OF FINITE ELEMENT DOMAIN
@@ -85,26 +89,39 @@
 VEXT,ALL,,,R3                   ! EXTRUDE AREA IN RADIAL DIRECTION
 ALLSEL                          ! SELECT ALL ENTITIES
 
 /OUTPUT,SCRATCH
 NUMMRG,NODE
 NUMMRG,ELEM
 NUMMRG,KP
-/OUTPUT
+
 
 CSYS,0
 NSEL,S,LOC,Y,0                  ! SELECT SYMMETRY BOUNDARY
 D,ALL,VOLT,0                    ! CONSTRAIN BOUNDARY VOLT DOF
 CSYS,2                          ! SPHERICAL COORDINATE SYSTEM
 NSEL,S,LOC,X,10,12              ! SELECT OUTER NODES OF INFINITE DOMAIN
 ESLN,S
 SF,ALL,INF                      ! SET INFINITE FLAG
 NSEL,ALL
 OUTRES,ALL,ALL
+
+ALLSEL,ALL
+FINISH
+CDWRITE,db,vm51_case1,cdb
 FINISH
+*IF,_EXIT1,EQ,1,THEN
+/EXIT,NOSAVE
+*ENDIF
+
+*ELSE
+CDREAD,db,vm51_case1,cdb
+*ENDIF
+FINISH
+
 /SOLU
 ALLSEL
 ESEL,U,TYPE,,1,                 ! UNSELECT DUMMY MESHING ELEMENT 122
 ESEL,S,MAT,,2                   ! SELECT SPHERE ELEMENTS
 NSLE
 CSYS,11                         ! CUSTOM SPHERICAL COORDINATE SYSTEM
 NSEL,S,LOC,X,0.98*R1,1.02*R1    ! SELECT NODES ON SPHERE SURFACE
@@ -169,30 +186,32 @@
 NSLE
 /AUTO
 PLNSOL,EF,X                     ! PLOT NODAL RESULTS, RADIAL ELECTRIC FIELD
 PLNSOL,VOLT                     ! PLOT NODAL RESULTS, VOLTAGE DOF
 RSYS,0
 CSYS,11
 NSEL,S,LOC,X,R1
-EMFN
+EMFT
 YFORCE=_FYSUM*12                ! MULTIPLY TO ACCOUNT FOR 30 DEGREE SLICE
 *STATUS,YFORCE
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
 LABEL(1,1) = '   YFORC'
 LABEL(1,2) = 'E  (N)  '
 *VFILL,VALUE(1,1),DATA,-1.236E-11
 *VFILL,VALUE(1,2),DATA,YFORCE
 *VFILL,VALUE(1,3),DATA,ABS(YFORCE/1.236E-11)
 SAVE,INF1
 FINISH
 /CLEAR,NOSTART
 
-
-
+/OUT,SCRATCH
+_GEOMGEN_2=0                    ! SET THIS TO 1 TO UPDATE CDB FILE 
+_EXIT2=0                       ! SET THIS TO 1 TO EXIT WITHOUT SOLVING
+*IF,_GEOMGEN_2,EQ,1,THEN 
 
 /TITLE,VM51, FORCE BETWEEN CHARGED SPHERES
 C*** USING SOLID123
 /PREP7
 R1 = 1                          ! SPHERE RADIUS
 R2 = 3                          ! DISTANCE BETWEEN SPHERES
 R3 = 6                          ! RADIUS OF FINITE ELEMENT DOMAIN
@@ -250,25 +269,38 @@
 VEXT,ALL,,,R3                   ! EXTRUDE AREA IN RADIAL DIRECTION
 ALLSEL                          ! SELECT ALL ENTITIES
 
 /OUTPUT,SCRATCH
 NUMMRG,NODE
 NUMMRG,ELEM
 NUMMRG,KP
-/OUTPUT
+
 
 CSYS,0
 NSEL,S,LOC,Y,0                  ! SELECT SYMMETRY BOUNDARY
 D,ALL,VOLT,0                    ! CONSTRAIN BOUNDARY VOLT DOF
 CSYS,2                          ! SPHERICAL COORDINATE SYSTEM
 NSEL,S,LOC,X,10,12              ! SELECT OUTER NODES OF INFINITE DOMAIN
 ESLN,S
 SF,ALL,INF                      ! SET INFINITE FLAG
 NSEL,ALL
 OUTRES,ALL,ALL
+
+
+ALLSEL,ALL
+FINISH
+CDWRITE,db,vm51_case2,cdb
+FINISH
+*IF,_EXIT2,EQ,1,THEN
+/EXIT,NOSAVE
+*ENDIF
+
+*ELSE
+CDREAD,db,vm51_case2,cdb
+*ENDIF
 FINISH
 /SOLU
 ALLSEL
 VSEL,S,VOLU,,1,2
 ESLV,S,1                   	! SELECT SPHERE ELEMENTS
 NSLE
 CSYS,11                         ! CUSTOM SPHERICAL COORDINATE SYSTEM
@@ -333,15 +365,15 @@
 NSLE
 /AUTO
 PLNSOL,EF,X                     ! PLOT NODAL RESULTS, RADIAL ELECTRIC FIELD
 PLNSOL,VOLT                     ! PLOT NODAL RESULTS, VOLTAGE DOF
 RSYS,0
 CSYS,11
 NSEL,S,LOC,X,R1
-EMFN
+EMFT
 YFORCE=_FYSUM*12                 ! MULTIPLY TO ACCOUNT FOR 30 DEGREE SLICE
 *STATUS,YFORCE
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
 LABEL(1,1) = '   YFORC'
 LABEL(1,2) = 'E  (N)  '
 *VFILL,VALUE(1,1),DATA,-1.236E-11
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm52.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm52.dat`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM52
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM52, AUTOMOBILE SUSPENSION SYSTEM VIBRATIONS
 C***VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 181, EX 6.7-1
 ANTYPE,MODAL              ! MODE-FREQUENCY ANALYSIS
 MXPAND,2                  ! EXPAND MODES
@@ -34,15 +34,15 @@
 SECN,2
 E,3,4                      ! BEAM ELEMENT
 TYPE,2
 REAL,3
 E,4,5                      ! SPRING ELEMENT
 D,1,UX,,,5,4,UY            ! BOUNDARY CONDITIONS
 D,3,UX
-NSEL,S,NODE,2,4
+NSEL,S,NODE,,2,4
 D,ALL,UZ,,,,,ROTY,ROTX
 NSEL,ALL
 OUTPR,NSOL,1
 FINISH
 /SOLU    
 /OUT,SCRATCH
 SOLVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm53.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm59.dat`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM53
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM59
 /PREP7
-/TITLE, VM53, VIBRATION OF A STRING UNDER TENSION
-C***           VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND. PRINTING,
-C***           PAGE 264, ART. 8.2,  
-ANTYPE,STATIC              ! STATIC ANALYSIS
-ET,1,LINK180
-KEYOPT,1,3,1		   	   ! TENSION ONLY OPTION
-SECTYPE,1,LINK   
-SECDATA,306796E-8	         ! DEFINE AREA
+MP,PRXY,,0.3
+/TITLE, VM59, LATERAL VIBRATION OF AN AXIALLY LOADED BAR
+C***          VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 374, ART. 59
+ANTYPE,STATIC                ! STATIC ANALYSIS
+RESCONTROL,LINEAR,ALL,1      ! NEEDED FOR PERTURBATION ANALYSIS
+ET,1,BEAM188,,,3
+SECT,1,BEAM,RECT
+SECD,2,2
 MP,EX,1,30E6
-MP,DENS,1,73E-5
-N,1                        ! DEFINE NODES
-N,14,100
+MP,DENS,1,727973E-9
+N,1
+N,14,80
 FILL
-E,1,2                      ! DEFINE ELEMENTS
+E,1,2
 EGEN,13,1,1
-INIS,SET,CSYS,-2           ! ARBITRARY INITIAL STRAIN
-INIS,SET,DTYP,EPEL
-INIS,DEFINE,,,,,543248E-8
-OUTPR,BASIC,1
-D,ALL,ALL                  ! FIX ALL MOTIONS FOR STATIC STRESSES
+D,1,UY,,,14,,ROTX,ROTZ       ! B.C.'S AND LOADING
+D,1,UX,,,,,UZ
+D,14,UZ
+F,14,FX,-40E3
 FINISH
 /out,scratch
 /SOLU    
-RESCONTROL,LINEAR,ALL,1     ! NEEDED FOR PERTURBED ANALYSIS
+OUTPR,BASIC,1
 SOLVE
 FINISH
 /out
 /POST1
 ETABLE,STRS,LS,1
 *GET,STRSS,ELEM,13,ETAB,STRS
-FINISH
-/POST26
-RFORCE,2,1,F,X
-STORE
-*GET,FORCE,VARI,2,EXTREM,VMAX
+*GET,DEF,NODE,14,U,X
 PARSAV,ALL
+FINISH
 /out,scratch
 /SOLU    
-ANTYPE,STATIC,RESTART,,,PERTURB   ! RESTART FROM LAST LOAD STEP AND LAST SUB STEP
-PERTURB,MODAL,,,PARKEEP           ! PERFORM PERTURBED MODAL SOLVE
-SOLVE,ELFORM                      ! REFORM ELEMENT MATRICES
+ANTYPE,STATIC,RESTART,,,PERTURB	! RESTART STATIC SOLVE FROM LAST LOAD STEP AND SUB STEP
+PERTURB,MODAL,,,PARKEEP			! PERFORM PERTURBED MODAL SOLVE
+SOLVE,ELFORM				! REFORM ELEMENT MATRICES
 
 PARRES,CHANGE
-MODOPT,LANB,3              ! EXTRACT 3 MODES USING LANB EXTRACTION METHOD
-MXPAND,3                   ! EXPAND FIRST THREE MODES
-DDELE,2,UX,13              ! RELEASE INTERIOR DOFS
-DDELE,2,UY,13
+MXPAND,3                     ! EXPAND FIRST 3 MODES
+MODOPT,LANB,3                ! SELECT THE BLOCK LANCZOS EIGENSOLVER
 SOLVE
 /out
 *GET,FREQ1,MODE,1,FREQ
 *GET,FREQ2,MODE,2,FREQ
 *GET,FREQ3,MODE,3,FREQ
+
 *DIM,LABEL,CHAR,5,2
 *DIM,VALUE,,5,3
-LABEL(1,1) = '      F,','      SI','      f1','      f2','      f3'
-LABEL(1,2) = ' lb     ','GMA,psi ',', Hz    ',', Hz    ',', Hz    '
-*VFILL,VALUE(1,1),DATA,500,162974,74.708,149.42,224.12
-*VFILL,VALUE(1,2),DATA,ABS(FORCE),STRSS,FREQ1,FREQ2,FREQ3
-*VFILL,VALUE(1,3),DATA,ABS(FORCE/500),ABS(STRSS/162974),ABS(FREQ1/74.708)
-*VFILL,VALUE(4,3),DATA,ABS(FREQ2/149.42),ABS(FREQ3/224.12)
+LABEL(1,1) = 'DEFLECTI','SIGMA,  ','f1,     ','f2,     ','f3,     '
+LABEL(1,2) = 'ON, (in)','   (psi)','    (Hz)','    (Hz)','    (Hz)'
+*VFILL,VALUE(1,1),DATA,-.026667,-10000,17.055,105.32,249.39
+*VFILL,VALUE(1,2),DATA,DEF,STRSS,FREQ1,FREQ2,FREQ3
+*VFILL,VALUE(1,3),DATA,ABS(DEF/.026667),ABS(STRSS/10000),ABS(FREQ1/17.055)
+*VFILL,VALUE(4,3),DATA,ABS(FREQ2/105.32),ABS(FREQ3/249.39)
 /COM
-/OUT,vm53,vrt
-/COM,------------------- VM53 RESULTS COMPARISON ---------------
+/OUT,vm59,vrt
+/COM,------------------- VM59 RESULTS COMPARISON ---------------
 /COM,
-/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
+/COM,                     |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
+(1X,A8,A8,'   ',F14.6,'  ',F18.6,'   ',1F15.3)
+/COM,-----------------------------------------------------------
+/COM,
+/COM,-----------------------------------------------------------
+/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM59  NOT CONTAINED IN
+/COM,THIS TABLE
 /COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm53,vrt
+*LIST,vm59,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm55.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm55.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM55
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM55, VIBRATION OF A STRETCHED CIRCULAR MEMBRANE
 C***        VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE  439, EQN. 182
 ANTYPE,STATIC        ! STATIC ANALYSIS
 ET,1,SHELL208,,,2
@@ -31,15 +31,17 @@
 ETABLE,STRS,S,X
 *GET,STRSS,ELEM,9,ETAB,STRS
 PARSAV,ALL
 FINI
 /SOLU    
 ANTYPE,STATIC,RESTART,,,PERTURB		! RESTART STATIC SOLVE FROM LAST LOAD STEP AND SUB STEP
 PERTURB,MODAL,,,PARKEEP				! PERFORM PERTURBED MODAL SOLVE
+/OUT,SCRATCH
 SOLVE,ELFORM					! REFORM ELEMENT MATRICES
+/OUT,
 
 PARRES,CHANGE
 MXPAND,3             ! EXPAND FIRST 3 MODES
 MODOPT,LANB,9        ! EXTRACT FIRST 9 MODES
 /OUT,SCRATCH
 SOLVE
 /OUT,
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm56.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm56.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM56
 /PREP7
 SMRT,OFF
 /TITLE, VM56, HYPERELASTIC THICK CYLINDER UNDER INTERNAL PRESSURE
 /COM           REF: ODEN, J.T., "FINITE ELEMENTS OF NONLINEAR CONTINUA"
 /COM                MCGRAW-HILL, 1972, PP 325-331
 ANTYPE,STATIC
@@ -26,28 +26,29 @@
 AMESH,1                   ! CREATE NODES AND ELEMENTS
 TYPE,2
 EMODIF,1                  ! PRINT ONLY INNERMOST ELEMENT RESULTS
 BFUNIF,TEMP,30            ! UNIFORM TEMPERATURES
 D,ALL,UY,0                ! FIX ALL NODES AXIALLY
 FINISH
 /SOLU    
-SOLCONTROL,0
 /TITLE, PRESSURE = 90 PSI
 NEQIT,20                  ! MAXIMUM 20 EQUILIBRIUM ITERATIONS
 NSEL,S,LOC,X,7.0,7.0
 SF,ALL,PRES,90            ! APPLY INTERNAL PRESSURE OF 90 PSI
 NSEL,ALL
+/OUT,SCRATCH
 SOLVE
 /TITLE, PRESSURE = 150 PSI
 NSEL,S,LOC,X,7.0
 SF,ALL,PRES,150           ! APPLY INTERNAL PRESSURE OF 150 PSI
 NSEL,ALL
 SOLVE
 FINISH
 /POST1                    ! POSTPROCESS
+/OUT,
 SET,2
 ETABLE,SX1,S,X  
 AVPRIN,0,0, 
 ELM=0
 NSEL,S,LOC,X,6.5,8.5
 ESLN
 ELM=ELNEXT(ELM)
@@ -73,17 +74,17 @@
 /CLEAR,NOSTART ! CLEAR THE PREVIOUS DATABASE
 /PREP7
 SMRT,OFF
 /TITLE, VM56: HYPERELASTIC THICK CYLINDER UNDER INTERNAL PRESSURE
 ANTYPE,STATIC
 NLGEOM,ON
 ET,1,SOLID185              ! 3-D 8-NODE STRUCTURAL SOLID
-KEYOPT,1,2,1		   ! REDUCED INTEGRATION
+KEYOPT,1,2,1		       ! REDUCED  INTEGRATION
 ET,2,SOLID185              ! 3-D 8-NODE STRUCTURAL SOLID
-KEYOPT,2,2,1		   ! REDUCED INTEGRATION
+KEYOPT,2,2,1		       ! REDUCED INTEGRATION
 NU1 = 0.495
 DD  = 2*(1-2*NU1)/(80+20)
 TB,HYPER,1,1,2,MOONEY
 TBDATA,1,80,20,DD
 CSYS,1
 K,1,7,3.16                ! DEFINE KEYPOINTS
 K,2,7,3.16,.775
@@ -102,28 +103,29 @@
 TYPE,2
 EMODIF,1
 NROTAT,ALL                ! ROTATE ALL NODES INTO CYLINDRICAL COORDINATES
 D,ALL,UZ,0.0              ! CONSTRAIN ALL NODES AXIALLY
 D,ALL,UY,0.0              ! CONSTRAIN ALL NODES TANGENTIALLY
 FINISH
 /SOLU    
-SOLCONTROL,0
 /TITLE, PRESSURE = 90 PSI
 NEQIT,30                  ! MAXIMUM 30 EQUILIBRIUM ITERATIONS
 NSEL,S,LOC,X,7
 SF,ALL,PRES,90            ! INTERNAL PRESSURE OF 90 PSI
 NSEL,ALL
+/OUT,SCRATCH
 SOLVE
 /TITLE, PRESSURE = 150 PSI
 NSEL,S,LOC,X,7
 SF,ALL,PRES,150           ! INTERNAL PRESSURE OF 150 PSI
 NSEL,ALL
 SOLVE
 FINISH
 /POST1                    ! POSTPROCESS
+/OUT,
 SET,2
 ETABLE,SX1,S,X  
 AVPRIN,0,0, 
 ELM=0
 NSEL,S,LOC,X,6.5,8.5
 ESLN
 ELM=ELNEXT(ELM)
@@ -149,17 +151,17 @@
 /CLEAR,NOSTART ! CLEAR THE PREVIOUS DATABASE
 /PREP7
 SMRT,OFF
 /TITLE, VM56: HYPERELASTIC THICK CYLINDER UNDER INTERNAL PRESSURE
 ANTYPE,STATIC
 NLGEOM,ON
 ET,1,SOLID186             ! 3-D 20-NODE STRUCTURAL SOLID
-KEYOPT,1,2,1		  ! REDUCED INTEGRATION
+KEYOPT,1,2,0		      ! REDUCED INTEGRATION
 ET,2,SOLID186             ! 3-D 20-NODE STRUCTURAL SOLID
-KEYOPT,2,2,1		  ! REDUCED INTEGRATION
+KEYOPT,2,2,0		      ! REDUCED INTEGRATION
 NU1 = 0.495
 DD  = 2*(1-2*NU1)/(80+20)
 TB,HYPER,1,1,2,MOONEY
 TBDATA,1,80,20,DD
 CSYS,1
 K,1,7,3.16                ! DEFINE KEYPOINTS
 K,2,7,3.16,.775
@@ -178,28 +180,29 @@
 TYPE,2
 EMODIF,1
 NROTAT,ALL                ! ROTATE ALL NODES INTO CYLINDRICAL COORDINATES
 D,ALL,UZ,0.0              ! CONSTRAIN ALL NODES AXIALLY
 D,ALL,UY,0.0              ! CONSTRAIN ALL NODES TANGENTIALLY
 FINISH
 /SOLU   
-SOLCONTROL,0
 /TITLE, PRESSURE = 90 PSI
 NEQIT,30                  ! MAXIMUM 30 EQUILIBRIUM ITERATIONS
 NSEL,S,LOC,X,7
 SF,ALL,PRES,90            ! INTERNAL PRESSURE OF 90 PSI
 NSEL,ALL
+/OUT,SCRATCH
 SOLVE
 /TITLE, PRESSURE = 150 PSI
 NSEL,S,LOC,X,7
 SF,ALL,PRES,150           ! INTERNAL PRESSURE OF 150 PSI
 NSEL,ALL
 SOLVE
 FINISH
 /POST1                    ! POSTPROCESS
+/OUT,
 SET,2
 *GET,DEF,NODE,1,U,X
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
 LABEL(1,1) = 'UR(INNER'
 LABEL(1,2) = ' RAD),in'
 VALUE(1,1) = 7.180
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm57.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm57.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM57
 /PREP7
 /TITLE, VM57, TORSIONAL FREQUENCIES OF A DRILL PIPE
 C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND. PRINTING, PAGE 272, EX. 8.4-5
 C*** USING PIPE16 ELEMENTS
 /PREP7
 ET,1,PIPE16
@@ -66,15 +66,15 @@
 FINISH
 /SOLU    
 ANTYPE,MODAL						! MODE-FREQUENCY ANALYSIS
 MODOPT,LANB,2						! EXTRACT FIRST TWO MODES
 D,1,UX,,,13,,UY,UZ,ROTX,ROTY
 D,1,ROTZ
 OUTPR,,1
-MXPAND,2
+MXPAND,2,,,YES
 /OUT,SCRATCH
 SOLVE
 FINISH
 /POST1
 /OUT,
 *GET,FREQ1,MODE,1,FREQ
 *GET,FREQ2,MODE,2,FREQ
@@ -112,15 +112,15 @@
 /SOLU    
 ANTYPE,MODAL						! MODE-FREQUENCY ANALYSIS
 MODOPT,LANB,2						! EXTRACT FIRST TWO MODES
 D,ALL,ALL,0
 DDELE,ALL,ROTZ
 D,1,ROTZ
 OUTPR,,1
-MXPAND,2
+MXPAND,2,,,YES
 /OUT,SCRATCH
 SOLVE
 FINISH
 /POST1
 /OUT,
 *GET,FREQ1,MODE,1,FREQ
 *GET,FREQ2,MODE,2,FREQ
@@ -155,15 +155,15 @@
 FINISH
 /SOLU
 ANTYPE,MODAL						! MODE-FREQUENCY ANALYSIS
 MODOPT,LANB,2						! EXTRACT FIRST TWO MODES
 D,1,UX,,,13,,UY,UZ,ROTX,ROTY
 D,1,ROTZ
 OUTPR,,1
-MXPAND,2
+MXPAND,2,,,YES
 /OUT,SCRATCH
 SOLVE
 FINISH
 /POST1
 /OUT,
 *GET,FREQ1,MODE,1,FREQ
 *GET,FREQ2,MODE,2,FREQ
@@ -197,15 +197,15 @@
 TYPE,2
 REAL,2
 E,2								! MASS ELEMENT
 FINI
 /SOLU
 ANTYPE,MODAL
 MODOPT,LANB,2
-MXPAND,2
+MXPAND,2,,,YES
 D,ALL,ALL,0
 DDELE,ALL,ROTZ
 D,1,ROTZ,0
 OUTPR,,1
 /OUT,SCRATCH
 SOLVE
 FINISH
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm58.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm58.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM58
 /PREP7
 SMRT,OFF
 /TITLE, VM58, CENTERLINE TEMP. OF A HEAT GENERATING WIRE
 C*** HEAT, MASS AND MOMENTUM TRANS., ROHSENOW AND CHOI, 2ND. PR., P. 106,EX 6.5
 ANTYPE,STATIC
 ET,1,PLANE35              ! 2-D 6 NODE TRIANGULAR THERMAL SOLID
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm59.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm76.dat`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,92 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM59
-/PREP7
-MP,PRXY,,0.3
-/TITLE, VM59, LATERAL VIBRATION OF AN AXIALLY LOADED BAR
-C***          VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 374, ART. 59
-ANTYPE,STATIC                ! STATIC ANALYSIS
-RESCONTROL,LINEAR,ALL,1      ! NEEDED FOR PERTURBATION ANALYSIS
-ET,1,BEAM188,,,3
-SECT,1,BEAM,RECT
-SECD,2,2
-MP,EX,1,30E6
-MP,DENS,1,727973E-9
-N,1
-N,14,80
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM76
+/PREP7  
+JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
+/SHOW,JPEG
+/TITLE, VM76, HARMONIC RESPONSE OF A GUITAR STRING
+/COM, REFERENCE: BLEVINS, FORMULAS FOR NAT. FREQ. AND MODE SHAPE, TABLE 7-1.
+ANTYPE,STATIC       ! STATIC ANALYSIS, PRESTRESS
+ET,1,LINK180        ! TWO-DIMENSIONAL SPAR
+SECTYPE,1,LINK
+SECDATA,50671E-12   ! CROSS-SECTIONAL AREA OF STRING
+MP,EX,1,190E9       ! MATERIAL, STAINLESS STEEL
+MP,DENS,1,7920
+N,1                 ! DEFINE NODES
+N,31,.71
 FILL
-E,1,2
-EGEN,13,1,1
-D,1,UY,,,14,,ROTX,ROTZ       ! B.C.'S AND LOADING
-D,1,UX,,,,,UZ
-D,14,UZ
-F,14,FX,-40E3
+E,1,2               ! DEFINE ELEMENTS
+EGEN,30,1,1
+D,1,ALL             ! BOUNDARY CONDITIONS AND LOADING
+D,2,UY,,,31
+D,ALL,UZ
+F,31,FX,84
 FINISH
-/out,scratch
-/SOLU    
+/OUT,SCRATCH
+/SOLU
+RESCONTROL,LINEAR,LAST,LAST    
 OUTPR,BASIC,1
 SOLVE
 FINISH
-/out
-/POST1
-ETABLE,STRS,LS,1
-*GET,STRSS,ELEM,13,ETAB,STRS
-*GET,DEF,NODE,14,U,X
-PARSAV,ALL
+/SOLU    
+ANTYPE,STATIC,RESTART,,,PERTURB
+PERTURB,MODAL,,,PARKEEP
+SOLVE,ELFORM
+
+MODOPT,LANB,6       ! LANB EXTRACTION METHOD, 6 FREQ.
+DDEL,2,UY,30
+SOLVE
+/OUT,
+*GET,FREQ,MODE,1,FREQ
 FINISH
-/out,scratch
+PARSAV,ALL
+/DELETE,,rstp
+/OUT,SCRATCH
 /SOLU    
-ANTYPE,STATIC,RESTART,,,PERTURB	! RESTART STATIC SOLVE FROM LAST LOAD STEP AND SUB STEP
-PERTURB,MODAL,,,PARKEEP			! PERFORM PERTURBED MODAL SOLVE
-SOLVE,ELFORM				! REFORM ELEMENT MATRICES
+ANTYPE,STATIC,RESTART,,,PERTURB
+PERTURB,HARMONIC,,,PARKEEP
+SOLVE,ELFORM
 
 PARRES,CHANGE
-MXPAND,3                     ! EXPAND FIRST 3 MODES
-MODOPT,LANB,3                ! SELECT THE BLOCK LANCZOS EIGENSOLVER
+HROPT,FULL
+DDEL,2,UY,30
+HROUT,OFF           ! AMPLITUDE, PHASE ANGLE PRINTOUT
+F,8,FY,-1           ! FORCE AT X=.1657, NEAR QUARTER POINT
+KBC,1               ! STEP CHANGE FORCE
+HARFRQ,,2000        ! OBTAIN FREQUENCY EVERY EIGHT HERTZ
+NSUBST,250
+OUTPR,,NONE
+OUTRES,,1
 SOLVE
-/out
-*GET,FREQ1,MODE,1,FREQ
-*GET,FREQ2,MODE,2,FREQ
-*GET,FREQ3,MODE,3,FREQ
-
-*DIM,LABEL,CHAR,5,2
-*DIM,VALUE,,5,3
-LABEL(1,1) = 'DEFLECTI','SIGMA,  ','f1,     ','f2,     ','f3,     '
-LABEL(1,2) = 'ON, (in)','   (psi)','    (Hz)','    (Hz)','    (Hz)'
-*VFILL,VALUE(1,1),DATA,-.026667,-10000,17.055,105.32,249.39
-*VFILL,VALUE(1,2),DATA,DEF,STRSS,FREQ1,FREQ2,FREQ3
-*VFILL,VALUE(1,3),DATA,ABS(DEF/.026667),ABS(STRSS/10000),ABS(FREQ1/17.055)
-*VFILL,VALUE(4,3),DATA,ABS(FREQ2/105.32),ABS(FREQ3/249.39)
+FINISH
+/OUT,
+/POST26             ! TIME-HISTORY POSTPROCESSOR
+FILE,,rstp          
+NSOL,2,16,U,Y,DISP  ! RETRIEVE STRING MIDPOINT DISPLACEMENT RESPONSE
+PRVAR,2
+/AXLAB,Y,AMPL
+PLCPLX,0            ! DISPLAY AMPLITUDE OF COMPLEX VARIABLE (DEFAULT)
+PLVAR,2
+*DIM,LABEL,CHAR,1,2
+*DIM,VALUE,,1,3
+LABEL(1,1) = '      f,'
+LABEL(1,2) = ' Hz     '
+*VFILL,VALUE(1,1),DATA,322.2
+*VFILL,VALUE(1,2),DATA,FREQ
+*VFILL,VALUE(1,3),DATA,ABS(FREQ/322.2 )
 /COM
-/OUT,vm59,vrt
-/COM,------------------- VM59 RESULTS COMPARISON ---------------
+/OUT,vm76,vrt
+/COM,------------------- VM76 RESULTS COMPARISON --------------
 /COM,
-/COM,                     |   TARGET   |   Mechanical APDL   |   RATIO
+/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F14.6,'  ',F18.6,'   ',1F15.3)
-/COM,-----------------------------------------------------------
+(1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
+/COM,----------------------------------------------------------
 /COM,
 /COM,-----------------------------------------------------------
-/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM59  NOT CONTAINED IN
+/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM76  NOT CONTAINED IN
 /COM,THIS TABLE
 /COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm59,vrt
+*LIST,vm76,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm6.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm6.dat`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,83 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM6
 /PREP7
-SMRT,OFF
 /TITLE, VM6, PINCHED CYLINDER
 /COM,  REF: COOK, CONCEPTS AND APPL. OF FEA 2ND ED., 1981, PP. 284-287. 
 C***         USING SHELL181 ELEMENTS
 /PREP7
-SMRT,OFF
 ANTYPE,STATIC             
 ET,1,SHELL181, , ,2
 SECTYPE,1,SHELL
 SECDATA,0.094,1,0,5
 MP,EX,,10.5E6
 MP,NUXY,,.3125
 CSYS,1
-K,1,4.953                 ! DEFINE MODEL GEOMETRY
-K,2,4.953,,5.175
-KGEN,2,1,2,1,,90
-A,1,2,4,3
-ESIZE,,8
-AMESH,1
+N,1,4.953                 ! DEFINE FE MODEL 
+N,9,4.953,,5.175
+FILL
+NGEN,9,10,1,9,1,,90/8
+E,1,11,12,2
+EGEN,8,1,-1
+EGEN,8,10,-8
+SAVE                      ! SAVE DATABASE FOR LATER USE
 CSYS,0
 NSEL,S,LOC,X,0
 DSYM,SYMM,X,0
 NSEL,S,LOC,Y,0
 DSYM,SYMM,Y,0
 NSEL,S,LOC,Z,0
 DSYM,SYMM,Z,0
 NSEL,ALL
-FK,3,FY,-25
+TOP_NODE = NODE (4.953,90,0)
+F,TOP_NODE,FY,-25
 FINISH
 /SOLU    
 SOLVE
 FINISH
 /POST1
 NSEL,S,LOC,Y,4.953              ! SELECT NODE AT LOAD APPLICATION
 NSEL,R,LOC,Z,0
 NSEL,R,LOC,X,0
 PRNSOL,U,COMP                   ! PRINT DISPLACEMENTS AND VECTOR SUM
-TOP_NODE = NODE (4.953,90,0)
 *GET,DISP,NODE,TOP_NODE,U,Y
 *DIM,LABEL,CHAR,1
 *DIM,VALUE,,1,3
 LABEL(1) = 'DEF_IN'
 *VFILL,VALUE(1,1),DATA,0.1139
 *VFILL,VALUE(1,2),DATA,ABS(DISP)
 *VFILL,VALUE(1,3),DATA,ABS( DISP /0.1139 )
 SAVE,TABLE_1
 FINISH
 /CLEAR,NOSTART
 /TITLE, VM6, PINCHED CYLINDER
 C***         USING SHELL281 ELEMENTS
 /PREP7
-SMRT,OFF
-ANTYPE,STATIC             
+RESUME            
 ET,1,SHELL281
-SECTYPE,1,SHELL
-SECDATA,0.094,1,0,5
-MP,EX,,10.5E6
-MP,NUXY,,.3125
-CSYS,1
-K,1,4.953                 ! DEFINE MODEL GEOMETRY
-K,2,4.953,,5.175
-KGEN,2,1,2,1,,90
-A,1,2,4,3
-ESIZE,,8
-AMESH,1
+EMID,ADD
 CSYS,0
 NSEL,S,LOC,X,0
 DSYM,SYMM,X,0
 NSEL,S,LOC,Y,0
 DSYM,SYMM,Y,0
 NSEL,S,LOC,Z,0
 DSYM,SYMM,Z,0
 NSEL,ALL
-FK,3,FY,-25
+TOP_NODE = NODE (4.953,90,0)
+F,TOP_NODE,FY,-25
 FINISH
 /SOLU    
 SOLVE
 FINISH
 /POST1
 NSEL,S,LOC,Y,4.953              ! SELECT NODE AT LOAD APPLICATION
 NSEL,R,LOC,Z,0
 NSEL,R,LOC,X,0
 PRNSOL,U,COMP                   ! PRINT DISPLACEMENTS AND VECTOR SUM
-TOP_NODE = NODE (4.953,90,0)
 *GET,DISP,NODE,TOP_NODE,U,Y
 *DIM,LABEL,CHAR,1
 *DIM,VALUE,,1,3
 LABEL(1) = 'DEF_IN'
 *VFILL,VALUE(1,1),DATA,0.1139
 *VFILL,VALUE(1,2),DATA,ABS(DISP)
 *VFILL,VALUE(1,3),DATA,ABS( DISP /0.1139 )
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm60.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm60.dat`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM60
 /PREP7
 SMRT,OFF
-/TITLE,VM60: NATURAL FREQUENCY OF A CROSS-PLY LAMINATED SPHERICAL SHELL
+/TITLE,VM60, NATURAL FREQUENCY OF A CROSS-PLY LAMINATED SPHERICAL SHELL
 C*** THEORETICAL SOLUTION IS FROM J.N. REDDY
 C*** ASCE JOURNAL OF ENGINEERING MECHANICS VOL 110 #5  MAY,1984 PP794-809
 C*** USING SHELL281
 /PREP7
 SMRT,OFF
 ET,1,SHELL281
 KEYOPT,1,8,1              ! WRITE LAYER RESULTS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm61.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm61.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM61
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM61, LONGITUDINAL VIBRATION OF A FREE-FREE ROD
 C***VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 269, EX 8.3-1
 ANTYPE,MODAL                     ! MODE-FREQUENCY ANALYSIS
 ET,1,BEAM188
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm62.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm62.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM62
 /PREP7
 SMRT,OFF
 /TITLE, VM62, VIBRATION OF A WEDGE
 C***          VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 392, ART. 62
 C***          USING SHELL63 ELEMENTS WITH BENDING STIFFNESS OPTION
 ANTYPE,MODAL                    ! MODE-FREQUENCY ANALYSIS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm63.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm63.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM63
 /PREP7
 SMRT,OFF
 /TITLE, VM63, STATIC HERTZ CONTACT PROBLEM SOLVED USING CONTAC178 ELEMENTS
 /COM  REF:  TIMOSHENKO AND GOODIER, THEORY OF ELASTICITY, 3RD ED., ART. 140.
 ET,1,PLANE82,,,1        ! AXISYMMETRIC ELEMENTS
 ET,2,PLANE183,,,1
@@ -68,15 +68,17 @@
 D,ALL,UX,0
 NSEL,R,LOC,Y,0
 D,ALL,UY,0
 NSEL,ALL             
 LOAD=0
 *CREATE,LOADSTEP        ! MACRO TO INCREMENTALLY APPLY LOAD
 FK,8,FY,ARG1
+/OUT,vm63_SCRATCH
 SOLVE
+/OUT
 *END
 *DO,I,1,3
  LOAD=LOAD-10
  *USE,LOADSTEP,LOAD*6.2831853
 *ENDDO
 FINISH
 /POST1                  ! POSTPROCESS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm64.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm64.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM64
 /PREP7
 /TITLE, VM64, THERMAL EXPANSION TO CLOSE A GAP AT A RIGID SURFACE
 C***          INTRO. TO STRESS ANALYSIS, HARRIS, 1ST PRINTING, PAGE 58, PROB. 8
-C***          USING CONTAC26 AND PLANE182 ELEMENTS
+C***          USING CONTA175 AND PLANE182 ELEMENTS
 ANTYPE,STATIC                ! STATIC ANALYSIS
 ET,1,CONTA175                ! CONTACT ELEMENT
 R,1                          ! USE DEFAULTS
 KEYOPT,1,12,4                ! NO SEPARATION
+KEYOPT,1,10,1 
 ET,2,PLANE182,2,,3
 R,2,1                        ! THICKNESS = 1
 ET,3,TARGE169                ! TARGET SURFACE
 MP,EX,1,10.5E6
 MP,ALPX,1,12.5E-6
 MP,NUXY,1,0
 N,1,2,1
@@ -35,14 +36,15 @@
 BFUNIF,TEMP,170
 D,3,ALL,,,4
 D,1,UX,,,2,1
 OUTPR,BASIC,LAST
 FINISH
 /SOLU    
 /OUT,SCRATCH
+
 SOLVE
 FINISH
 /POST1
 /OUT,
 ETABLE,STRSX,S,X
 ETABLE,STRSY,S,Y
 *GET,STRSSX,ELEM,4,ETAB,STRSX
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm65.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm65.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM65
 /PREP7                 
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM65, TRANSIENT RESPONSE OF A BALL IMPACTING A FLEXIBLE SURFACE
 C***        VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND. PRINTING, PAGE 110,
 C***        EX. 4.6-1, USING NON-LINEAR TRANSIENT DYNAMIC ANALYSIS
@@ -27,24 +27,25 @@
 TYPE,3
 REAL,2
 TSHAP,LINE
 E,3,2                  ! TARGET ELEMENT
 ALLSEL,ALL
 FINISH
 /SOLU    
-SOLCONTROL,0
-NSUBST,10
+NSUBST,10,10,1
 ACEL,,386
 KBC,1                  ! STEP ACCELERATION CHANGE
 CNVTOL,F,1,1E-5        ! FORCE CONVERGENCE CRITERIA
 TIME,1E-3              ! RELEASE MASS USING SMALL TIME STEP
+AUTOTS,OFF
+TINTP,,,,0.5,0.5,0.2
 /OUT,SCRATCH
 SOLVE
 OUTRES,,1
-NSUBST,109             ! INTEGRATION TIME STEP OF 0.001 IN SECOND LOAD STEP
+NSUBST,109,109,1             ! INTEGRATION TIME STEP OF 0.001 IN SECOND LOAD STEP
 TIME,.11               ! TIME TO ALLOW THE MASS TO REACH ITS LARGEST DEFLECTION
 SOLVE
 FINISH
 /POST26
 /OUT,
 NSOL,2,1,U,Y,UY
 DERIV,3,2,1,,VEL1UY
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm66.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm66.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM66
 /PREP7
 SMRT,OFF
 /TITLE, VM66, VIBRATION OF A FLAT PLATE
 C***          VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 338, ART. 53
 C***          USING SHELL63 ELEMENTS WITH SHELL OPTION
 ANTYPE,MODAL                   ! MODE-FREQUENCY ANALYSIS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm67.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm67.dat`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM67
 /PREP7
 /TITLE, VM67, RADIAL VIBRATIONS OF A CIRCULAR RING FROM AN AXISYMMETRIC MODEL
 C***         VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE  425, ART. 68
 C***         (AXISYMMETRIC) AND 2
 ANTYPE,MODAL          ! MODE-FREQUENCY ANALYSIS
 ET,1,PLANE25
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm68.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm68.dat`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM68
 
 /PREP7
 /TITLE, VM68, PSD RESPONSE OF TWO DOF SPRING-MASS SYSTEM
 !     "VIBRATION ANALYSIS" R.K. VIERK ,2ND EDITION ,(CHAPTER 7)
 ET,1,COMBIN40            ! DISPLACEMENT ALONG X AXIS, MASS AT NODE I
 R,1,42832.,,0.50  
@@ -19,34 +19,40 @@
 FINISH
 
 /SOLU    
 ANTYPE,MODAL             ! PERFORM A MODAL ANALYSIS
 MODOPT,LANB,2            ! LANB EXTRACTION METHOD
                          ! EXTRACT 2 MODES FROM ENTIRE FREQUENCY RANGE
 MXPAND,2,,,YES           ! EXPAND 2 MODES, DO ELEMENT STRESS CALCULATIONS
-SOLVE 
+/OUT,vm68_SCRATCH
+SOLVE
+/OUT 
 *GET,FREQ1,MODE,1,FREQ
 *GET,FREQ2,MODE,2,FREQ
 FINISH
 
 /SOLU    
 ANTYPE,SPECTR            ! PERFORM SPECTRUM ANALYSIS
 SPOPT,PSD,2,ON           ! USE FIRST 2 MODES FROM MODAL ANALYSIS
 
 PSDUNIT,1,ACCG           ! USE G**2/HZ FOR PSD AND DIMENSION IN INCHES
 D,1,UX,1.0               ! APPLY SPECTRUM AT THE SUPPORT POINT
 PSDFRQ,1,1,10.0,100.0    ! FREQUENCY RANGE OF 10 TO 100 HERTZ
 PSDVAL,1,.1,.1           ! WHITE NOISE PSD, VALUES IN  G**2/HZ
+/OUT,vm68_SCRATCH,,,APPEND
 PFACT,1,BASE             ! BASE EXCITATION
+/OUT
 
 DMPRAT,0.02              ! 2% DAMPING
 PSDCOM                   ! COMBINE MODES FOR PSD, USE DEFAULT SIGNIFICANCE LEVEL
 
 PSDRES,ACEL,REL          ! CALCULATE RELATIVE ACCELERATION SOLUTIONS
+/OUT,vm68_SCRATCH,,,APPEND
 SOLVE
+/OUT 
 FINISH
 
 /POST1
 LCDEF,6,5,1              ! DEFINE LOAD STEP AND SUBSTEP FOR LOAD FACTOR OPERATION
 LCFACT,ALL,(1/386.4)     ! CONVERT ACCEL. RESULT TO G
 LCASE,6
 PRNSOL,U,COMP            ! PRINT NODAL SOLUTION RESULTS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm69.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm69.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM69
 /PREP7
 /TITLE, VM69, SEISMIC RESPONSE
 C***VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 78, EX 3.11-1
 ET,1,COMBIN40,,,,,,2
 R,1,9.8696,,1             ! SPRING CONSTANT = 9.8696, MASS = 1
 N,1
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm7.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm7.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM7
 /PREP7
 /TITLE, VM7, PLASTIC COMPRESSION OF A PIPE ASSEMBLY
 C***          MECHANICS OF SOLIDS, CRANDALL AND DAHL, 1959, PAGE 180, EX. 5.1
 C***          USING PIPE288, SOLID185 AND SHELL181 ELEMENTS
 THETA=6                              ! SUBTENDED ANGLE
 ET,1,PIPE288,,,,2
@@ -16,18 +16,18 @@
 SECDATA,4.9563384,0.5                ! OUTSIDE DIA. AND WALL THICKNESS FOR INSIDE TUBE (PIPE288)
 SECTYPE,4,PIPE
 SECDATA,8.139437,0.5                 ! OUTSIDE DIA. AND WALL THICKNESS FOR OUTSIDE TUBE (PIPE288)
 MP,EX  ,1,26.875E6                   ! STEEL
 MP,PRXY,1,0.3
 MP,EX  ,2,11E6                       ! ALUMINUM
 MP,PRXY,2,0.3
-TB,BKIN,1,1                          ! DEFINE NON-LINEAR MATERIAL PROPERTY FOR STEEL
+TB,PLAS,1,1,,BKIN                    ! DEFINE NON-LINEAR MATERIAL PROPERTY FOR STEEL
 TBTEMP,0
 TBDATA,1,86000,0
-TB,BKIN,2,1                          ! DEFINE NON-LINEAR MATERIAL PROPERTY FOR ALUMINUM
+TB,PLAS,2,1,,BKIN                    ! DEFINE NON-LINEAR MATERIAL PROPERTY FOR ALUMINUM
 TBTEMP,0
 TBDATA,1,55000,0
 N,1                                  ! GENERATE NODES AND ELEMENTS FOR PIPE288
 N,2,,,10
 MAT,1  
 SECNUM,3                             ! STEEL (INSIDE) TUBE
 E,1,2
@@ -62,15 +62,15 @@
 E,204,202,206,208
 C*** APPLY CONSTRAINTS TO PIPE288 MODEL
 D,1,ALL                              ! FIX ALL DOFS FOR BOTTOM END OF PIPE288
 D,2,UX,,,,,UY,ROTX,ROTY,ROTZ         ! ALLOW ONLY UZ DOF AT TOP END OF PIPE288 MODEL
 C*** APPLY CONSTRAINTS TO SOLID185 AND SHELL181 MODELS
 CP,1,UX,101,111,105,115              ! COUPLE NODES AT BOUNDARY IN RADIAL DIR FOR SOLID185
 CPSGEN,4,,1
-CP,5,UX,201,205,203,20               ! COUPLE NODES AT BOUNDARY IN RADIAL DIR FOR SHELL181
+CP,5,UX,201,205,203,207               ! COUPLE NODES AT BOUNDARY IN RADIAL DIR FOR SHELL181
 CPSGEN,2,,5
 CP,7,ROTY,201,205                    ! COUPLE NODES AT BOUNDARY IN ROTY DIR FOR SHELL181
 CPSGEN,4,,7
 NSEL,S,NODE,,101,212                 ! SELECT ONLY NODES IN SOLID185 AND SHELL181 MODELS
 NSEL,R,LOC,Y,0                       ! SELECT NODES AT THETA = 0 FROM THE SELECTED SET
 DSYM,SYMM,Y,1                        ! APPLY SYMMETRY BOUNDARY CONDITIONS
 NSEL,S,NODE,,101,212                 ! SELECT ONLY NODES IN SOLID185 AND SHELL181 MODELS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm70.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm70.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM70
 /PREP7
 MP,PRXY,,0.3
 /TITLE, VM70, SEISMIC RESPONSE OF A BEAM STRUCTURE
 C***           INTRODUCTION TO STRUCT. DYNAMICS, BIGGS, PAGE 262, ART. 6.4
 ET,1,BEAM189
 HEIGHT=14
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm71.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm71.dat`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM71
 /PREP7                    
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM71, TRANSIENT RESPONSE OF A SPRING, MASS, DAMPING SYSTEM
 C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 41, EX 2.2-1
 ET,1,COMBIN40,,,2         ! Y-DOF ELEMENT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm72.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm72.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM72
 /PREP7                    
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM72, LOGARITHMIC DECREMENT
 C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 45, EX 2.3-1
 ET,1,COMBIN40,,,2         ! Y DOF ELEMENT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm73.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm73.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM73
 /PREP7                       
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM73, FREE VIBRATION WITH COULOMB DAMPING
 C***           MECHANICAL VIBRATIONS, TSE, MORSE, AND HINKLE, PAGE 175, CASE 1
 ET,1,COMBIN40,,,,,,2         ! MASS AT NODE J OF ELEMENT
 R,1,1E4,,(10/386),,1.875,30
 N,1
 N,2
 E,1,2
 FINISH
 /SOLU    
-SOLCONTROL,0
 ANTYPE,TRANS                 ! NONLINEAR TRANSIENT DYNAMIC ANALYSIS
 TRNOPT, , , , , ,HHT
 D,1,UX
 IC,2,UX,-1,0                 ! STRETCH SPRING
 KBC,1                        ! STEP BOUNDARY CONDITION
 CNVTOL,F,1,0.001             ! FORCE CONVERGENCE CRITERIA
+CNVTOL,U,-1
 TIME,.2025
-NSUBST,404                   ! TO COMPLETE CIRCLE
+NSUBST,404,404,1          ! TO COMPLETE CIRCLE
 OUTRES,,1
+AUTOTS,OFF
+TINTP,,,,0.5,0.5,0.2
 SOLVE
 FINISH
 /POST26
 NSOL,2,2,U,X,UX              ! STORE UX DISPLACEMENT OF NODE 2 
 ESOL,3,1,,SMISC,1,F1         ! STORE FORCE F1 OF ELEMENT 1 AS VARIABLE 3
 PRVAR,2,3                    ! PRINT VARIABLES 2 AND 3
 /GRID,1                      ! TURN GRID ON
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm74.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm79.dat`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,83 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM74
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM79
 /PREP7
-/TITLE, VM74, TRANSIENT RESPONSE TO AN IMPULSIVE EXCITATION
-C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 99, ART. 4.1
+/TITLE, VM79, TRANSIENT RESPONSE OF A BI-LINEAR SPRING ASSEMBLY
+C***VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 150,FIG 5.6-1
 ET,1,COMBIN40,,,2,,,2    ! Y DOF ELEMENTS, MASS AT NODE J
-R,1,200,,.5              ! TWO DAMPING RATIOS
-R,2,200,14,.5
+R,1,200,,.5              ! K1 = 200; M = .5
 N,1
-N,4
-FILL
+N,2
 E,1,2
-REAL,2
-E,3,4
-D,1,UY,,,3,2
+GP,3,2,FY,-200,.75       ! GAP CONDITION
+D,1,UY,,,3,2             ! CONSTRAIN UY DOF AT NODES 1 AND 3
 FINISH
 
-/SOLU
-ANTYPE,MODAL            ! PERFORM MODAL SOLVE
-MODOPT,QRDAMP,2         ! USE QRDAMP EIGENSOLVER
-MXPAND,2
+/SOLUTION
+ANTYPE,MODAL
+MODOPT,LANB,1           ! PERFORM MODAL SOLVE USING LANB EIGENSOLVER
+MXPAND,1
 SOLVE
 FINISH
 
-/SOLU
+/SOLU    
 ANTYPE,TRANSIENT
-TRNOPT,MSUP,2           ! PERFORM MODE SUPERPOSITION TRANSIENT SOLVE
-F,2,FY,0,,4,2
+TRNOPT,MSUP,1            ! PERFORM MODE SUPERPOSITION TRANSIENT SOLVE
 DELTIM,25E-4             ! INTEGRATION TIME STEP
 KBC,1                    ! STEP BOUNDARY CONDITIONS
+F,2,FY
 OUTPR,BASIC,1
-SOLVE                   ! PSEUDO STATIC SOLVE
+SOLVE                    ! STATIC LOAD STEP
 
-TIME,25E-4
-F,2,FY,4000,,4,2        ! IMPULSE FORCE
-KBC,1
+TIME,25E-4               ! TIME AT END OF LOAD STEP
+F,2,FY,-4E3              ! APPLY 4000 LB. LOAD
 SOLVE
 
-TIME,.105                ! TIME TO ALLOW THE MASSES TO REACH LARGEST DEFLECTIONS
-F,2,FY,,,4,2             ! REMOVE FORCE
+TIME,.105
+F,2,FY,0                 ! REMOVE LOAD
 SOLVE
 FINISH
+
 /POST26
 FILE,,rdsp
 NSOL,2,2,U,Y,2UY          ! STORE UY DISPLACEMENTS OF APPROPRIATE NODES
-NSOL,4,4,U,Y,4UY
-NPRINT,.25
-PRVAR,2,4
-*GET,Y1,VARI,2,RTIME,.08
-*GET,Y2,VARI,2,RTIME,.1
-*GET,Y3,VARI,4,RTIME,.1
-*DIM,LABEL_1,CHAR,1,2
-*DIM,VALUE_1,,1,3
-LABEL_1(1,1) = 'Y,MAX in'
-LABEL_1(1,2) = ' NODE=2 '
-*VFILL,VALUE_1(1,1),DATA,.99957
-*VFILL,VALUE_1(1,2),DATA,Y1
-*VFILL,VALUE_1(1,3),DATA,ABS(Y1/.99957)
-*DIM,LABEL_2,CHAR,2,2
-*DIM,VALUE_2,,2,3
-LABEL_2(1,1) = 'Y, in   ','Y, in   '
-LABEL_2(1,2) = 'node=2  ','node=4  '
-*VFILL,VALUE_2(1,1),DATA,.90930,.34180
-*VFILL,VALUE_2(1,2),DATA,Y2,Y3
-*VFILL,VALUE_2(1,3),DATA,ABS(Y2/.90930),ABS(Y3/.34180)
+PRVAR,2
+*GET,Y1,VARI,2,RTIME,.09
+*GET,Y2,VARI,2,RTIME,.04
+*GET,Y3,VARI,2,RTIME,.07
+*GET,Y4,VARI,2,RTIME,.085
+*GET,Y5,VARI,2,RTIME,.105
+*DIM,LABEL_1,CHAR,3,2
+*DIM,VALUE_1,,3,4
+LABEL_1(1,1) = 'TIME    ','Y, in   ','Y, in   '
+LABEL_1(1,2) = 'sec     ','linear ','bilinear'
+*VFILL,VALUE_1(1,1),DATA,.040,-.68122,Y2
+*VFILL,VALUE_1(1,2),DATA,.070,-.97494,Y3
+*VFILL,VALUE_1(1,3),DATA,.085,-.99604,Y4
+*VFILL,VALUE_1(1,4),DATA,.105,-.88666,Y5
+*DIM,LABEL_2,CHAR,1,2
+*DIM,VALUE_2,,1,3
+LABEL_2(1,1) = 'Y, in   '
+LABEL_2(1,2) = 'MAX     '
+*VFILL,VALUE_2(1,1),DATA,-1.0417
+*VFILL,VALUE_2(1,2),DATA,Y1
+*VFILL,VALUE_2(1,3),DATA,ABS(Y1/1.0417)
 /COM
-/OUT,vm74,vrt
-/COM,------------------- VM74 RESULTS COMPARISON --------------
+/OUT,vm79,vrt
+/COM,------------------- VM79 RESULTS COMPARISON ----------------- 
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-/COM,TIME=.08 sec
+/COM,TIME=.09 sec
+/COM,
+*VWRITE,LABEL_2(1,1),LABEL_2(1,2),VALUE_2(1,1),VALUE_2(1,2),VALUE_2(1,3)
+(1X,A8,A8,'   ',F10.5,'  ',F10.5,'   ',1F5.3)
 /COM,
-*VWRITE,LABEL_1(1,1),LABEL_1(1,2),VALUE_1(1,1),VALUE_1(1,2),VALUE_1(1,3)
-(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
+/COM,COMPARISON OF Mechanical APDL LINEAR (VM74) AND BILINEAR SPRING RESULTS
 /COM,
-/COM,TIME=.1 sec
+*VWRITE,LABEL_1(1,1),LABEL_1(1,2),VALUE_1(1,1),VALUE_1(1,2),VALUE_1(1,3),VALUE_1(1,4)
+(1X,A8,A8,'   ',F8.5,'  ',F8.5,'  ',F15.5,'  ',F15.5)
 /COM,
-*VWRITE,LABEL_2(1,1),LABEL_2(1,2),VALUE_2(1,1),VALUE_2(1,2),VALUE_2(1,3)
-(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
-/COM,----------------------------------------------------------
+/COM,-------------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm74,vrt
+*LIST,vm79,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm75.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm75.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM75
+/out,scratch
 /PREP7                    
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM75, TRANSIENT RESPONSE TO A STEP EXCITATION
 C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 102, ART 4.3
 ET,1,COMBIN40,,,2,,,2     ! Y DOF ELEMENTS, MASS AT NODE J
 R,1,200,,.5               ! TWO DAMPING RATIOS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm76.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm84.dat`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,79 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM76
-/PREP7  
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM84
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/TITLE, VM76, HARMONIC RESPONSE OF A GUITAR STRING
-/COM, REFERENCE: BLEVINS, FORMULAS FOR NAT. FREQ. AND MODE SHAPE, TABLE 7-1.
-ANTYPE,STATIC       ! STATIC ANALYSIS, PRESTRESS
-ET,1,LINK180        ! TWO-DIMENSIONAL SPAR
-SECTYPE,1,LINK
-SECDATA,50671E-12   ! CROSS-SECTIONAL AREA OF STRING
-MP,EX,1,190E9       ! MATERIAL, STAINLESS STEEL
-MP,DENS,1,7920
-N,1                 ! DEFINE NODES
-N,31,.71
+/PREP7                  
+/TITLE, VM84, DISPLACEMENT PROPAGATION ALONG A BAR WITH FREE ENDS
+C***      VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 311, PROB. 2
+ET,1,LINK180
+SECTYPE,1,LINK   
+SECDATA,2                ! AREA = 2
+MP,EX,1,3E7
+MP,DENS,1,7202E-7
+N,1
+N,17,48E3
 FILL
-E,1,2               ! DEFINE ELEMENTS
-EGEN,30,1,1
-D,1,ALL             ! BOUNDARY CONDITIONS AND LOADING
-D,2,UY,,,31
+E,1,2
+EGEN,16,1,1
 D,ALL,UZ
-F,31,FX,84
+D,ALL,UY
 FINISH
 /OUT,SCRATCH
 /SOLU
-RESCONTROL,LINEAR,LAST,LAST    
-OUTPR,BASIC,1
+ANTYPE,MODAL
+MODOPT,LANB,17          ! PERFORM MODAL SOLVE USING LANB EIGENSOLVER
+MXPAND,17
 SOLVE
 FINISH
 /SOLU    
-ANTYPE,STATIC,RESTART,,,PERTURB
-PERTURB,MODAL,,,PARKEEP
-SOLVE,ELFORM
-
-MODOPT,LANB,6       ! LANB EXTRACTION METHOD, 6 FREQ.
-DDEL,2,UY,30
+ANTYPE,TRANSIENT
+TRNOPT,MSUP,17           ! PERFORM MODE SUPERPOSITION TRANSIENT SOLVE
+DELTIM,5E-3              ! INTEGRATION TIME STEP SIZE
+KBC,1                    ! STEP LOADING CONDITION
+OUTPR,BASIC,LAST
+F,17,FX                  ! DEFINE NULL FX LOAD AT NODE 17
 SOLVE
-/OUT,
-*GET,FREQ,MODE,1,FREQ
-FINISH
-PARSAV,ALL
-/DELETE,,rstp
-/OUT,SCRATCH
-/SOLU    
-ANTYPE,STATIC,RESTART,,,PERTURB
-PERTURB,HARMONIC,,,PARKEEP
-SOLVE,ELFORM
 
-PARRES,CHANGE
-HROPT,FULL
-DDEL,2,UY,30
-HROUT,OFF           ! AMPLITUDE, PHASE ANGLE PRINTOUT
-F,8,FY,-1           ! FORCE AT X=.1657, NEAR QUARTER POINT
-KBC,1               ! STEP CHANGE FORCE
-HARFRQ,,2000        ! OBTAIN FREQUENCY EVERY EIGHT HERTZ
-NSUBST,250
-OUTPR,,NONE
-OUTRES,,1
+OUTPR,BASIC,2
+OUTRES,NSOL,1 
+TIME,.24                 ! FINAL TIME INCLUDES 1/2 OF THE FUNDAMENTAL PERIOD
+F,17,FX,6000             ! APPLY FULL LOAD TO NODE 17
 SOLVE
 FINISH
+
 /OUT,
-/POST26             ! TIME-HISTORY POSTPROCESSOR
-FILE,,rstp          
-NSOL,2,16,U,Y,DISP  ! RETRIEVE STRING MIDPOINT DISPLACEMENT RESPONSE
-PRVAR,2
-/AXLAB,Y,AMPL
-PLCPLX,0            ! DISPLAY AMPLITUDE OF COMPLEX VARIABLE (DEFAULT)
-PLVAR,2
+/POST26
+FILE,,rdsp               ! REDUCED DISPLACEMENTS FILE
+NSOL,2,1,U,X,1UX         ! STORE APPROPRIATE NODAL DISPLACEMENTS
+NSOL,3,9,U,X,9UX
+NSOL,4,17,U,X,17UX
+DERIV,5,2,,,1VX          ! COMPUTE VELOCITIES
+DERIV,6,3,,,9VX
+DERIV,7,4,,,17VX
+/GRID,1                  ! TURN GRID ON
+/AXLAB,Y,DISP            ! Y-AXIS LABEL DISP
+PLVAR,2,3,4              ! DISPLAY VARIABLES 2, 3 AND 4
+/AXLAB,Y,VELO            ! Y-AXIS LABEL VELO
+PLVAR,5,6,7              ! DISPLAY VARIABLES 5, 6 AND 7
+PRTIME,0.230,0.240       ! APPROPRIATE TIME RANGE (.23 TO .24)
+PRVAR,4                  ! PRINT VARIABLE 4 (UX AT NODE 17)
+*GET,DEF,VARI,4,RTIME,.240
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
-LABEL(1,1) = '      f,'
-LABEL(1,2) = ' Hz     '
-*VFILL,VALUE(1,1),DATA,322.2
-*VFILL,VALUE(1,2),DATA,FREQ
-*VFILL,VALUE(1,3),DATA,ABS(FREQ/322.2 )
+LABEL(1,1) = '    DEF,'
+LABEL(1,2) = 'in      '
+*VFILL,VALUE(1,1),DATA,4.8 
+*VFILL,VALUE(1,2),DATA,DEF 
+*VFILL,VALUE(1,3),DATA,ABS(DEF/4.8)
 /COM
-/OUT,vm76,vrt
-/COM,------------------- VM76 RESULTS COMPARISON --------------
+/OUT,vm84,vrt
+/COM,------------------- VM84 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.1,'  ',F14.1,'   ',1F15.3)
+(1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
 /COM,----------------------------------------------------------
-/COM,
-/COM,-----------------------------------------------------------
-/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM76  NOT CONTAINED IN
-/COM,THIS TABLE
-/COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm76,vrt
+*LIST,vm84,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm77.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm77.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM77
 /OUT,SCRATCH
 /PREP7
 /TITLE, VM77, TRANSIENT RESPONSE TO A CONSTANT FORCE WITH A FINITE RISE TIME
-/stitle,1,Reason COMPARE differences are acceptable:
-/stitle,2,  acceptable differences
 C***           INTRODUCTION TO STRUCT. DYNAMICS, BIGGS, PAGE 50, EXAMPLE E
 C***           DISPLACEMENT PASS USING BEAM188 AND MASS21 ELEMENTS
 ET,1,BEAM188,,,3        ! BEAM USING CUBIC OPTION
 SECTYPE,1,BEAM,RECT
 SECDATA,18,1.647
-SECCONTROL,,,2e15       ! OVERRIDE THE PROGRAM-CALCULATED TRANSVERSE SHEAR STIFFNESS
+SECCONTROL,,,2e10       ! OVERRIDE THE PROGRAM-CALCULATED TRANSVERSE SHEAR STIFFNESS
 ET,2,MASS21,,,4         ! STRUCTURAL MASS
 R,2,.0259067            ! MASS
 MP,EX  ,1,30E3
 MP,PRXY,1,0.3
 N,1
 N,3,240
 FILL
@@ -57,16 +55,18 @@
 EXPASS,ON               ! EXPANSION PASS ON
 EXPSOL,,,0.092          ! TIME OF MAXIMUM RESPONSE
 SOLVE            
 FINISH
 
 /OUT,
 /POST1
+ESEL,S,TYPE,,1
 ETABLE,STRS,SMISC,33
 *GET,STRSS,ELEM,2,ETAB,STRS
+ALLSEL,ALL
 FINISH
 
 /POST26
 NSOL,2,2,U,Y
 STORE
 *GET,TMAX,VARI,2,EXTREM,TMAX
 *GET,YMAX,VARI,2,EXTREM,VMAX
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm78.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm78.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM78
 /PREP7
-/TITLE, VM78: TRANSVERSE SHEAR STRESSES IN A CANTILEVER BEAM
+/TITLE, VM78, TRANSVERSE SHEAR STRESSES IN A CANTILEVER BEAM
 C***          THEORY OF ELASTICITY, TIMESHENKO, PG. 35, ARTICLE 20 
 ANTYPE,STATIC
 ET,1,SHELL281		     ! 8-NODE LAYERED SHELL; STRESS & STRAIN PRINTOUT
 KEYOPT,1,8,2		     ! STORE RESULTS FOR ALL LAYERS
 SECTYPE,1,SHELL
 SECDATA,0.5,1,0,5,LAYER1
 SECDATA,0.5,1,0,5,LAYER2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm8.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm8.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM8
+/TITLE, VM8, MACRO TO CALCULATE DISTANCES BETWEEN POINTS
 *CREATE,MAC
 LENGTH              ! LABEL FOR THIS BLOCK IN THE USER FILE
 !
 !       THIS BLOCK IN THE USER FILE CALCULATES THE STRAIGHT LINE
 !       DISTANCE BETWEEN TWO POINTS IN SPACE DEFINED BY EITHER
 !       KEYPOINTS OR NODES ( CONTROLLED BY ARG1 ).  OTHER INPUT
 !       AND OUTPUT ARGUMENTS ARE DEFINED BELOW.
@@ -50,15 +51,14 @@
   /COM LENGTH BETWEEN NODES HAS BEEN DEFINED AS PARAMETER PDIS (FROM USERFILE)
 *ELSE
   /COM LENGTH BETWEEN KEYPOINTS DEFINED AS PARAMETER PDIS (FROM USERFILE)
 *ENDIF
 /GOPR                 ! TURN PRINTOUT BACK ON
 *END
 /PREP7
-/TITLE, VM8, MACRO TO CALCULATE DISTANCES BETWEEN POINTS
 C***         ANY BASIC GEOMETRY TEXT
 *ULIB,MAC                     ! ASSIGN MACRO LIBRARY FILE
 *ABBR,KLEN,*USE,LENGTH,1      ! ASSIGN ABBREVIATIONS FOR "CALLS" TO USERFILE
 *ABBR,NLEN,*USE,LENGTH,0
 N,1,1.5,2.5,3.5               ! DEFINE TEST NODE AND KEYPOINT LOCATIONS
 N,2,-3.7,4.6,-3
 K,3,100,0,30
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm80.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm90.dat`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,87 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM80
-/PREP7    
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM90
+/PREP7                    
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
-/TITLE, VM80, PLASTIC RESPONSE TO A SUDDENLY APPLIED CONSTANT FORCE
-C***           INTRODUCTION TO STRUCT. DYNAMICS, BIGGS, PAGE 69, ART. 2.7
-ANTYPE,TRANS        ! FULL TRANSIENT DYNAMIC ANALYSIS
-ET,1,LINK180
-ET,2,MASS21,,,4     ! TWO-DIMENSIONAL MASS
-SECTYPE,1,LINK   
-SECDATA,.278		    ! AREA (A)
-R,2,0.0259          ! MASS
-MP,EX,1,30E3
-TB,BKIN,1,1         ! BILINEAR KINEMATIC HARDENING STRESS-STRAIN CURVE
-TBTEMP,0
-TBDATA,1,162.9,0    ! YIELD STRESS AND TANGENT MODULUS
+/TITLE, VM90, HARMONIC RESPONSE OF A TWO-MASS-SPRING SYSTEM
+C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 178,EX 6.6-1
+ANTYPE,HARMIC             ! HARMONIC RESPONSE ANALYSIS
+HROPT,FULL                ! FULL HARMONIC RESPONSE
+HROUT,OFF                 ! PRINT RESULTS AS AMPLITUDES AND PHASE ANGLES
+ET,1,COMBIN14,,,2
+ET,2,MASS21,,,4
+R,1,200                   ! SPRING CONSTANT = 200
+R,2,.5                    ! MASS = 0.5
 N,1
-N,2,,-100
+N,4,1
+FILL
 E,1,2
-D,ALL,UZ
 TYPE,2
 REAL,2
-E,1
+E,2                       ! MASS ELEMENT
+TYPE,1
+REAL,1
+E,2,3                     ! SPRING ELEMENT
+TYPE,2
+REAL,2
+E,3                       ! MASS ELEMENT
+TYPE,1
+REAL,1
+E,3,4                     ! SPRING ELEMENT
+OUTPR,BASIC,1
+NSUBST,30                 ! 30 INTERVALS WITHIN FREQ. RANGE
+HARFRQ,,7.5               ! FREQUENCY RANGE FROM 0 TO 7.5 HZ
+KBC,1                     ! STEP BOUNDARY CONDITION
+D,1,UY,,,4
+D,1,UX,,,4,3
+F,2,FX,200
 FINISH
-/SOLU    
-SOLCONTROL,0
-KBC,1               ! STEP BOUNDARY CONDITIONS
-TIME,4E-3           ! TIME AT THE END OF LOAD STEP 1
-D,1,UX,,,2
-D,2,UY
-F,1,FY,30           ! APPLY F1
-NSUBST,10           ! 10 SUBSTEPS FOR  TIME STEP OF .0004
-OUTPR,BASIC,1       ! PRINT BASIC SOLUTION FOR EACH SUBSTEP
-OUTRES,NSOL,1       ! STORE NODAL SOLUTION FOR EACH SUBSTEP
 /OUT,SCRATCH
-SOLVE
-TIME,.14            ! FINAL TIME SLIGHTLY MORE THAN 1 CYCLE OF VIBRATION
-NSUBST,68           ! 68 REPEATS FOR TIME STEP OF 0.002 
-OUTPR,BASIC,8       ! PRINT BASIC SOLUTION FOR EVERY 8TH SUBSTEP
+/SOLU    
 SOLVE
 FINISH
+/OUT
 /POST26
-/OUT,
-NSOL,2,1,U,Y,UY       ! STORE UY DISPLACEMENTS OF NODE 1 AGAINST TIME
-PRVAR,2               ! PRINT VARIABLE 2 (DISPLACEMENT UY OF NODE 1) V/S TIME
-/GRID,1               ! TURN THE GRID ON FOR DISPLAY
-/AXLAB,Y,DISPLACEMENT ! MAKE Y-AXIS LABEL AS DISP FOR DISPLAY
-PLVAR,2               ! DISPLAY VARIABLE 2 (DISPLACEMENT UY OF NODE 1) V/S TIME
-*GET,YMAX,VARI,2,EXTREM,VMAX
-*GET,TMAX,VARI,2,EXTREM,TMAX
-*GET,YMIN,VARI,2,RTIME,.122 
-TMIN = .122
-*DIM,LABEL,CHAR,4,2
-*DIM,VALUE,,4,3
-LABEL(1,1) = 'Y_MAX, i','TIME, se','Y_MIN, i','TIME, se'
-LABEL(1,2) = 'n       ','c       ','n       ','c       '
-*VFILL,VALUE(1,1),DATA,.806,.0669,.438,.122
-*VFILL,VALUE(1,2),DATA,YMAX,TMAX,YMIN,TMIN
-*VFILL,VALUE(1,3),DATA,ABS(YMAX/.806),ABS(TMAX/.0669),ABS(YMIN/.438),ABS(TMIN/.122)
+FILE,,rst
+NSOL,2,2,U,X,2UX          ! STORE UX DISPLACEMENTS 
+NSOL,3,3,U,X,3UX
+PRVAR,2,3
+*GET,X1,VARI,2,RTIME,1.5
+*GET,X2,VARI,3,RTIME,1.5
+*GET,X3,VARI,2,RTIME,4
+*GET,X4,VARI,3,RTIME,4
+*GET,X5,VARI,2,RTIME,6.5
+*GET,X6,VARI,3,RTIME,6.5
+/GRID,1                   ! TURN GRID ON
+/AXLAB,Y,DISP             ! Y-AXIS LABEL DISP
+PLVAR,2,3                 ! DISPLAY VARIABLES 2 AND 3
+*DIM,LABEL,CHAR,6,2
+*DIM,VALUE,,6,3
+LABEL(1,1) = 'X1, in  ','X2, in  ','X1, in  ','X2, in  ','X1, in  ','X2, in  '
+LABEL(1,2) = 'f=1.5 Hz','f=1.5 Hz','f=4 Hz  ','f=4 Hz  ','f=6.5 Hz','f=6.5 Hz'
+*VFILL,VALUE(1,1),DATA,.82272,.46274,.51145,1.2153,.58513,.26966
+*VFILL,VALUE(1,2),DATA,ABS(X1),ABS(X2),ABS(X3),ABS(X4),ABS(X5),ABS(X6)
+V1 = ABS(X1/.82272)
+V2 = ABS(X2/.46274)
+V3 = ABS(X3/.51145)
+V4 = ABS(X4/1.2153)
+V5 = ABS(X5/.58513)
+V6 = ABS(X6/.26965)
+*VFILL,VALUE(1,3),DATA,V1,V2,V3,V4,V5,V6
 /COM
-/OUT,vm80,vrt
-/COM,------------------- VM80 RESULTS COMPARISON --------------
+/OUT,vm90,vrt
+/COM,------------------- VM90 RESULTS COMPARISON ---------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
-/COM,----------------------------------------------------------
+(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
+/COM,-----------------------------------------------------------
+/COM,
+/COM,-----------------------------------------------------------
+/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM90  NOT CONTAINED IN
+/COM,THIS TABLE
+/COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm80,vrt
+*LIST,vm90,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm82.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm82.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM82
 /OUT,SCRATCH
 /PREP7
 SMRT,OFF
 /TITLE, VM82, SIMPLY SUPPORTED LAMINATED PLATE UNDER PRESSURE
 C***    EXACT SOLUTIONS OF MODERATELY THICK LAMINATED SHELLS,
 C***    J.N. REDDY, JNL. OF ENGR. MECHANICS, VOL 110, NO.5, MAY'84.
@@ -72,14 +72,15 @@
 /OUT,SCRATCH
 /PREP7
 SMRT,OFF
 /TITLE, VM82, SIMPLY SUPPORTED LAMINATED PLATE UNDER PRESSURE
 C*** USING SOLSH190
 ANTYPE,STATIC
 ET,1,SOLSH190               ! 8 NODE LAYERED SOLID-SHELL
+KEYOPT,1,4,2                ! TRANSVERSE SHEAR
 KEYOPT,1,8,1                ! WRITE LAYER RESULTS
 SECTYPE,1,SHELL
 SECDATA,0.025,1,0           ! LAYER 1: 0.025 THK, THETA 0 
 SECDATA,0.025,1,90          ! LAYER 2: 0.025 THK, THETA 90
 SECDATA,0.025,1,90          ! LAYER 3: 0.025 THK, THETA 90
 SECDATA,0.025,1,0           ! LAYER 4: 0.025 THK, THETA 0
 MP,EX,1,25E6                ! ORTHOTROPIC MATERIAL PROPERTIES
@@ -223,29 +224,33 @@
 MP,EZ,1,1E6                 ! EZ=EY ASSUMED
 MP,GXY,1,5E5
 MP,GYZ,1,2E5
 MP,GXZ,1,5E5
 MP,PRXY,1,0.25              ! MAJOR POISSONS RATIO
 MP,PRYZ,1,0.01              ! MAJOR POISSONS RATIO
 MP,PRXZ,1,0.25              ! MAJOR POISSONS RATIO
+E11=29166.66666666          ! E11 TRANSVERSE SHEAR STIFFNESS
+E22=29166.66666666          ! E22 TRANSVERSE SHEAR STIFFNESS
+E12=0                       ! E12 TRANSVERSE SHEAR STIFFNESS
+SECCONTROL,E11,E22,E12      ! OVERWRITING SECTION PROPERTIES WITH USER DEFINED VALUES
 K,1                         ! CORNER KEYPOINTS OF QUADRANT (AREA)
 K,2,5
 K,3,5,5
 K,4,,5
 A,1,2,3,4
-ESIZE,,6                    ! 6X6 MESH USING QUARTER SYMMETRY
+ESIZE,,12                    ! 12X12 MESH USING QUARTER SYMMETRY
 AMESH,1
 NSEL,S,LOC,X,0
 DSYM,SYMM,X
 NSEL,S,LOC,Y,0
 DSYM,SYMM,Y
 NSEL,S,LOC,X,5              ! APPLY FREELY SUPPORTED B.C.
-D,ALL,UZ,,,,,UY
+D,ALL,,,,,,,UY,UZ,ROTX
 NSEL,S,LOC,Y,5
-D,ALL,UZ,,,,,UX
+D,ALL,UX,,,,,,UZ,,ROTY
 NSEL,ALL
 SFE,ALL,2,PRES,,1           ! APPLY UNIFORM PRESSURE 
 OUTPR,NSOL,1
 OUTPR,RSOL,1
 FINISH
 /SOLU    
 SOLVE
@@ -287,29 +292,33 @@
 MP,EZ,1,1E6                 ! EZ=EY ASSUMED
 MP,GXY,1,5E5
 MP,GYZ,1,2E5
 MP,GXZ,1,5E5
 MP,PRXY,1,0.25              ! MAJOR POISSONS RATIO
 MP,PRYZ,1,0.01              ! MAJOR POISSONS RATIO
 MP,PRXZ,1,0.25              ! MAJOR POISSONS RATIO
+E11=29166.66666666          ! E11 TRANSVERSE SHEAR STIFFNESS
+E22=29166.66666666          ! E22 TRANSVERSE SHEAR STIFFNESS
+E12=0                       ! E12 TRANSVERSE SHEAR STIFFNESS
+SECCONTROL,E11,E22,E12      ! OVERWRITING SECTION PROPERTIES WITH USER DEFINED VALUES
 K,1                         ! CORNER KEYPOINTS OF QUADRANT (AREA)
 K,2,5
 K,3,5,5
 K,4,,5
 A,1,2,3,4
 ESIZE,,6                    ! 6X6 MESH USING QUARTER SYMMETRY
 AMESH,1
 NSEL,S,LOC,X,0
 DSYM,SYMM,X
 NSEL,S,LOC,Y,0
 DSYM,SYMM,Y
 NSEL,S,LOC,X,5              ! APPLY FREELY SUPPORTED B.C.
-D,ALL,UZ,,,,,UY
+D,ALL,,,,,,,UY,UZ,ROTX
 NSEL,S,LOC,Y,5
-D,ALL,UZ,,,,,UX
+D,ALL,UX,,,,,,UZ,,ROTY
 NSEL,ALL
 SFE,ALL,2,PRES,,1           ! APPLY UNIFORM PRESSURE 
 OUTPR,NSOL,1
 OUTPR,RSOL,1
 FINISH
 /SOLU    
 SOLVE
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm83.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm83.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM83
 /PREP7                        
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM83, IMPACT OF A BLOCK ON A SPRING SCALE
 C***VECTOR MECHANICS FOR ENGINEERS, BEER AND JOHNSTON, 1962, PAGE 531, PROB 14.6
 C*** WITH THANKS TO ALAN GOULD
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm84.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm74.dat`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,109 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM84
-JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
-/SHOW,JPEG
-/PREP7                  
-/TITLE, VM84, DISPLACEMENT PROPAGATION ALONG A BAR WITH FREE ENDS
-C***      VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 311, PROB. 2
-ET,1,LINK180
-SECTYPE,1,LINK   
-SECDATA,2                ! AREA = 2
-MP,EX,1,3E7
-MP,DENS,1,7202E-7
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM74
+/PREP7
+/TITLE, VM74, TRANSIENT RESPONSE TO AN IMPULSIVE EXCITATION
+C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 99, ART. 4.1
+ET,1,COMBIN40,,,2,,,2    ! Y DOF ELEMENTS, MASS AT NODE J
+R,1,200,,.5              ! TWO DAMPING RATIOS
+R,2,200,14,.5
 N,1
-N,17,48E3
+N,4
 FILL
 E,1,2
-EGEN,16,1,1
-D,ALL,UZ
-D,ALL,UY
+REAL,2
+E,3,4
+D,1,UY,,,3,2
 FINISH
-/OUT,SCRATCH
+
 /SOLU
-ANTYPE,MODAL
-MODOPT,LANB,17          ! PERFORM MODAL SOLVE USING LANB EIGENSOLVER
-MXPAND,17
+ANTYPE,MODAL            ! PERFORM MODAL SOLVE
+MODOPT,QRDAMP,2         ! USE QRDAMP EIGENSOLVER
+MXPAND,2
+/OUT,vm74_SCRATCH
 SOLVE
+*DIM,CFREQ,,2,2
+*GET,CFREQ(1,1),MODE,1,FREQ
+*GET,CFREQ(1,2),MODE,1,DFRQ
+*GET,CFREQ(2,1),MODE,2,FREQ
+*GET,CFREQ(2,2),MODE,2,DFRQ
+*IF,CFREQ(1,1),LT,CFREQ(2,1),THEN
+    F1A=CFREQ(2,1)
+    CFREQ(2,1)=CFREQ(1,1)
+    CFREQ(1,1)=F1A
+    DF1A=CFREQ(2,2)
+    CFREQ(2,2)=CFREQ(1,2)
+    CFREQ(1,2)=DF1A
+    *DEL,F1A
+    *DEL,DF1A
+*ENDIF
+/OUT
+*STATUS,CFREQ
 FINISH
-/SOLU    
+
+/SOLU
 ANTYPE,TRANSIENT
-TRNOPT,MSUP,17           ! PERFORM MODE SUPERPOSITION TRANSIENT SOLVE
-DELTIM,5E-3              ! INTEGRATION TIME STEP SIZE
-KBC,1                    ! STEP LOADING CONDITION
-OUTPR,BASIC,LAST
-F,17,FX                  ! DEFINE NULL FX LOAD AT NODE 17
+TRNOPT,MSUP,2           ! PERFORM MODE SUPERPOSITION TRANSIENT SOLVE
+F,2,FY,0,,4,2
+DELTIM,25E-4             ! INTEGRATION TIME STEP
+KBC,1                    ! STEP BOUNDARY CONDITIONS
+OUTPR,BASIC,1
+/OUT,vm74_SCRATCH,,,APPEND
+SOLVE                   ! PSEUDO STATIC SOLVE
+/OUT
+
+TIME,25E-4
+F,2,FY,4000,,4,2        ! IMPULSE FORCE
+KBC,1
+/OUT,vm74_SCRATCH,,,APPEND
 SOLVE
+/OUT
 
-OUTPR,BASIC,2
-OUTRES,NSOL,1 
-TIME,.24                 ! FINAL TIME INCLUDES 1/2 OF THE FUNDAMENTAL PERIOD
-F,17,FX,6000             ! APPLY FULL LOAD TO NODE 17
+TIME,.105                ! TIME TO ALLOW THE MASSES TO REACH LARGEST DEFLECTIONS
+F,2,FY,,,4,2             ! REMOVE FORCE
+/OUT,vm74_SCRATCH,,,APPEND
 SOLVE
+/OUT
 FINISH
-
-/OUT,
 /POST26
-FILE,,rdsp               ! REDUCED DISPLACEMENTS FILE
-NSOL,2,1,U,X,1UX         ! STORE APPROPRIATE NODAL DISPLACEMENTS
-NSOL,3,9,U,X,9UX
-NSOL,4,17,U,X,17UX
-DERIV,5,2,,,1VX          ! COMPUTE VELOCITIES
-DERIV,6,3,,,9VX
-DERIV,7,4,,,17VX
-/GRID,1                  ! TURN GRID ON
-/AXLAB,Y,DISP            ! Y-AXIS LABEL DISP
-PLVAR,2,3,4              ! DISPLAY VARIABLES 2, 3 AND 4
-/AXLAB,Y,VELO            ! Y-AXIS LABEL VELO
-PLVAR,5,6,7              ! DISPLAY VARIABLES 5, 6 AND 7
-PRTIME,0.230,0.240       ! APPROPRIATE TIME RANGE (.23 TO .24)
-PRVAR,4                  ! PRINT VARIABLE 4 (UX AT NODE 17)
-*GET,DEF,VARI,4,RTIME,.240
-*DIM,LABEL,CHAR,1,2
-*DIM,VALUE,,1,3
-LABEL(1,1) = '    DEF,'
-LABEL(1,2) = 'in      '
-*VFILL,VALUE(1,1),DATA,4.8 
-*VFILL,VALUE(1,2),DATA,DEF 
-*VFILL,VALUE(1,3),DATA,ABS(DEF/4.8)
+FILE,,rdsp
+NSOL,2,2,U,Y,2UY          ! STORE UY DISPLACEMENTS OF APPROPRIATE NODES
+NSOL,4,4,U,Y,4UY
+NPRINT,.25
+PRVAR,2,4
+*GET,Y1,VARI,2,RTIME,.08
+*GET,Y2,VARI,2,RTIME,.1
+*GET,Y3,VARI,4,RTIME,.1
+*DIM,LABEL_1,CHAR,1,2
+*DIM,VALUE_1,,1,3
+LABEL_1(1,1) = 'Y,MAX in'
+LABEL_1(1,2) = ' NODE=2 '
+*VFILL,VALUE_1(1,1),DATA,.99957
+*VFILL,VALUE_1(1,2),DATA,Y1
+*VFILL,VALUE_1(1,3),DATA,ABS(Y1/.99957)
+*DIM,LABEL_2,CHAR,2,2
+*DIM,VALUE_2,,2,3
+LABEL_2(1,1) = 'Y, in   ','Y, in   '
+LABEL_2(1,2) = 'node=2  ','node=4  '
+*VFILL,VALUE_2(1,1),DATA,.90930,.34180
+*VFILL,VALUE_2(1,2),DATA,Y2,Y3
+*VFILL,VALUE_2(1,3),DATA,ABS(Y2/.90930),ABS(Y3/.34180)
 /COM
-/OUT,vm84,vrt
-/COM,------------------- VM84 RESULTS COMPARISON --------------
+/OUT,vm74,vrt
+/COM,------------------- VM74 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
+/COM,TIME=.08 sec
+/COM,
+*VWRITE,LABEL_1(1,1),LABEL_1(1,2),VALUE_1(1,1),VALUE_1(1,2),VALUE_1(1,3)
+(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
+/COM,
+/COM,TIME=.1 sec
+/COM,
+*VWRITE,LABEL_2(1,1),LABEL_2(1,2),VALUE_2(1,1),VALUE_2(1,2),VALUE_2(1,3)
+(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
 /COM,----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm84,vrt
+*LIST,vm74,vrt
+/DEL,SCRATCH
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm85.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm85.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM85
+/out,scratch
 /PREP7
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM85, TRANSIENT DISPLACEMENTS IN A SUDDENLY STOPPED MOVING BAR
 C***      VIBRATION PROBS. IN ENGR., TIMOSHENKO, 3RD. ED., PAGE 305, PROB. NO. 3
 ET,1,LINK180
 SECTYPE,1,LINK   
@@ -18,22 +19,23 @@
 ALLSEL,ALL
 D,ALL,UZ,0
 D,ALL,UY,0
 GP,1,20,FX,3E7,.64          ! GAP CONDITION
 FINISH
 /SOLU
 ANTYPE,MODAL
-MODOPT,LANB,17              ! PERFORM MODAL SOLVE USING LANB EIGENSOLVER
-MXPAND,17
+MODOPT,LANB,17,              ! PERFORM MODAL SOLVE USING LANB EIGENSOLVER
+MXPAND,17,,,YES
 /OUT,SCRATCH
 SOLVE
 FINISH
+/OUT,SCRATCH
 /SOLU    
 ANTYPE,TRANSIENT
-TRNOPT,MSUP,17              ! PERFORM MODE SUPERPOSITION TRANSIENT SOLVE
+TRNOPT,MSUP,	            ! PERFORM MODE SUPERPOSITION TRANSIENT SOLVE
 DELTIM,.0001                ! ITS DEFINITION
 KBC,1                       ! STEP BOUNDARY CONDITION
 F,1,FX,,,17                 ! DEFINE NULL FORCES ON ALL BAR NODES
 SOLVE
 
 TIME,.0004
 F,1,FX,57031.25,,17,16      ! FORCES REQUIRED TO ACHIEVE INITIAL VELOCITY
@@ -55,32 +57,29 @@
 PRVAR,2,3,4,5
 /AXLAB,Y,DISPLACEMENTS
 PLVAR,2,3,4,5
 DERIV,6,2,,,1 VX            ! COMPUTE VELOCITIES
 DERIV,7,3,,,17VX
 DERIV,8,5,,,9 VX
 /AXLAB,Y,VELOCITY
-/OUT,
 PLVAR,6,7,8
 *GET,D_0544,VARI,4,RTIME,.0544
 *GET,D_0557,VARI,4,RTIME,.0557
-
 *DIM,LABEL,CHAR,3,2
 *DIM,VALUE,,3,3
 LABEL(1,1) = 'D,in(T=.','D,in(T=.','D,in(T=.'
 LABEL(1,2) = '05573sec','0544sec)','0557sec)'
 *VFILL,VALUE(1,1),DATA,4.9329,0,0 
 *VFILL,VALUE(1,2),DATA,0,D_0544,D_0557
 *VFILL,VALUE(1,3),DATA,0,ABS(D_0544/4.9329),ABS(D_0557/4.9329)
 FINISH
 /SOLU    
 EXPASS,ON                   ! EXPANSION PASS
 EXPSOL,,,0.0557             ! EXPAND SOLUTION AT TIME CLOSEST TO THE THEORETICAL TIME POINT
 OUTPR,,1
-/OUT,SCRATCH
 SOLVE
 FINISH
 /POST1
 SET,LAST
 /OUT,
 ETABLE,STRS,LS,1
 *GET,STRSS,ELEM,1,ETAB,STRS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm86.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm87.dat`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM86
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM87
 /PREP7
-/TITLE, VM86, HARMONIC RESPONSE OF A DYNAMIC SYSTEM
-C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 56, EX 3.1-2
-C***                BY VISCOUS DAMPING APPROACH
-ANTYPE,HARMIC       ! HARMONIC RESPONSE ANALYSIS
-HROPT,FULL
-HROUT,OFF           ! PRINT COMPLEX DISP. AS AMPLITUDES AND PHASE ANGLES
+/TITLE, VM87, EQUIVALENT STRUCTURAL DAMPING
+C***         VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND. PRINTING, PAGE 72,
+C***         ART. 3.9, AND PAGE 56, EX. 3.1-2
+ANTYPE,HARMIC            ! HARMONIC RESPONSE ANALYSIS
+HROPT,FULL               ! FULL HARMONIC RESPONSE
+HROUT,OFF                ! PRINT COMPLEX DISP. AS AMPLITUDES AND PHASE ANGLES
 ET,1,COMBIN40,,,3,,,2
-R,1,200,6,.5        ! SPRING STIFFNESS = 200, C = 6, M = .5
+BETAD,.03                ! EQUIVALENT STRUCTURAL DAMPING
+R,1,200,,.5              ! SPRING STIFFNESS = 200, C = 0, M = 0.5
 N,1
 N,2
 E,1,2
 OUTPR,BASIC,1
-HARFRQ,,3.1831      ! HARMONIC FREQUENCY RANGE
+HARFRQ,,3.1831           ! HARMONIC FREQUENCY RANGE
 D,1,UZ
 F,2,FZ,10
 FINISH
 /SOLU    
+/OUT,SCRATCH
 SOLVE
 FINISH
 /POST26
 FILE,,rst
+/OUT,
 NSOL,2,2,U,Z,2UX
 PRVAR,2
 *GET,A,VARI,2,ITIME,3.1831
 *DIM,LABEL,CHAR,1,2
 *DIM,VALUE,,1,3
 LABEL(1,1) = 'AMPLITUD'
 LABEL(1,2) = 'E, in   '
 *VFILL,VALUE(1,1),DATA,.0833
 *VFILL,VALUE(1,2),DATA,ABS(A)
 *VFILL,VALUE(1,3),DATA,ABS(A/.0833)
 /COM
-/OUT,vm86,vrt
-/COM,------------------- VM86 RESULTS COMPARISON --------------
+/OUT,vm87,vrt
+/COM,------------------- VM87 RESULTS COMPARISON ---------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
 /COM,-----------------------------------------------------------
 /COM,
 /COM,-----------------------------------------------------------
-/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM86  NOT CONTAINED IN
+/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM87  NOT CONTAINED IN
 /COM,THIS TABLE
 /COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm86,vrt
+*LIST,vm87,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm87.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm88.dat`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,55 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM87
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM88
 /PREP7
-/TITLE, VM87, EQUIVALENT STRUCTURAL DAMPING
-C***         VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND. PRINTING, PAGE 72,
-C***         ART. 3.9, AND PAGE 56, EX. 3.1-2
-ANTYPE,HARMIC            ! HARMONIC RESPONSE ANALYSIS
-HROPT,FULL               ! FULL HARMONIC RESPONSE
-HROUT,OFF                ! PRINT COMPLEX DISP. AS AMPLITUDES AND PHASE ANGLES
-ET,1,COMBIN40,,,3,,,2
-BETAD,.03                ! EQUIVALENT STRUCTURAL DAMPING
-R,1,200,,.5              ! SPRING STIFFNESS = 200, C = 0, M = 0.5
+/TITLE, VM88, RESPONSE OF AN ECCENTRIC WEIGHT EXCITER
+! VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 60, EX 3.3-1
+ANTYPE,HARMIC              ! HARMONIC RESPONSE ANALYSIS
+HROPT,FULL                 ! FULL HARMONIC RESPONSE
+HROUT,OFF                  ! PRINT COMPLEX DISP. AS AMPLITUDES AND PHASE ANGLES
+ET,1,COMBIN40
+R,1,30,.11754533,.02590673 ! K = 30, C = .11754533, M = .02590673
 N,1
 N,2
-E,1,2
-OUTPR,BASIC,1
-HARFRQ,,3.1831           ! HARMONIC FREQUENCY RANGE
-D,1,UZ
-F,2,FZ,10
+E,2,1
 FINISH
 /SOLU    
-/OUT,SCRATCH
+OUTPR,BASIC,1
+HARFRQ,,5.415947           ! FREQUENCY RANGE FROM 0 TO 5.415947 HZ.
+D,1,UX
+F,2,FX,2.4
+SOLVE
+HARFRQ,,541.5947           ! FREQUENCY RANGE FROM 0 TO 541.5947 HZ.
+F,2,FX,24000
 SOLVE
 FINISH
 /POST26
 FILE,,rst
-/OUT,
-NSOL,2,2,U,Z,2UX
+NSOL,2,2,U,X,2UX
 PRVAR,2
-*GET,A,VARI,2,ITIME,3.1831
-*DIM,LABEL,CHAR,1,2
-*DIM,VALUE,,1,3
-LABEL(1,1) = 'AMPLITUD'
-LABEL(1,2) = 'E, in   '
-*VFILL,VALUE(1,1),DATA,.0833
-*VFILL,VALUE(1,2),DATA,ABS(A)
-*VFILL,VALUE(1,3),DATA,ABS(A/.0833)
+*GET,A1,VARI,2,ITIME,5.4159
+*GET,A2,VARI,2,RTIME,541.59
+*DIM,LABEL,CHAR,2,2
+*DIM,VALUE,,2,3
+LABEL(1,1) = 'AMP f=fn','AMP f=10'
+LABEL(1,2) = ', in    ','0fn, in '
+*VFILL,VALUE(1,1),DATA,.6,.08
+*VFILL,VALUE(1,2),DATA,ABS(A1),ABS(A2)
+*VFILL,VALUE(1,3),DATA,ABS(A1/.6),ABS(A2/.08)
 /COM
-/OUT,vm87,vrt
-/COM,------------------- VM87 RESULTS COMPARISON ---------------
+/OUT,vm88,vrt
+/COM,------------------- VM88 RESULTS COMPARISON ---------------
+
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
 /COM,-----------------------------------------------------------
 /COM,
 /COM,-----------------------------------------------------------
-/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM87  NOT CONTAINED IN
+/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM88  NOT CONTAINED IN
 /COM,THIS TABLE
 /COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm87,vrt
+*LIST,vm88,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm88.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm86.dat`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM88
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM86
 /PREP7
-/TITLE, VM88, RESPONSE OF AN ECCENTRIC WEIGHT EXCITER
-! VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 60, EX 3.3-1
-ANTYPE,HARMIC              ! HARMONIC RESPONSE ANALYSIS
-HROPT,FULL                 ! FULL HARMONIC RESPONSE
-HROUT,OFF                  ! PRINT COMPLEX DISP. AS AMPLITUDES AND PHASE ANGLES
-ET,1,COMBIN40
-R,1,30,.11754533,.02590673 ! K = 30, C = .11754533, M = .02590673
+/TITLE, VM86, HARMONIC RESPONSE OF A DYNAMIC SYSTEM
+C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 56, EX 3.1-2
+C***                BY VISCOUS DAMPING APPROACH
+ANTYPE,HARMIC       ! HARMONIC RESPONSE ANALYSIS
+HROPT,FULL
+HROUT,OFF           ! PRINT COMPLEX DISP. AS AMPLITUDES AND PHASE ANGLES
+ET,1,COMBIN40,,,3,,,2
+R,1,200,6,.5        ! SPRING STIFFNESS = 200, C = 6, M = .5
 N,1
 N,2
-E,2,1
+E,1,2
+OUTPR,BASIC,1
+HARFRQ,,3.1831      ! HARMONIC FREQUENCY RANGE
+D,1,UZ
+F,2,FZ,10
 FINISH
 /SOLU    
-OUTPR,BASIC,1
-HARFRQ,,5.415947           ! FREQUENCY RANGE FROM 0 TO 5.415947 HZ.
-D,1,UX
-F,2,FX,2.4
-SOLVE
-HARFRQ,,541.5947           ! FREQUENCY RANGE FROM 0 TO 541.5947 HZ.
-F,2,FX,24000
 SOLVE
 FINISH
 /POST26
 FILE,,rst
-NSOL,2,2,U,X,2UX
+NSOL,2,2,U,Z,2UX
 PRVAR,2
-*GET,A1,VARI,2,ITIME,5.4159
-*GET,A2,VARI,2,RTIME,541.59
-*DIM,LABEL,CHAR,2,2
-*DIM,VALUE,,2,3
-LABEL(1,1) = 'AMP f=fn','AMP f=10'
-LABEL(1,2) = ', in    ','0fn, in '
-*VFILL,VALUE(1,1),DATA,.6,.08
-*VFILL,VALUE(1,2),DATA,ABS(A1),ABS(A2)
-*VFILL,VALUE(1,3),DATA,ABS(A1/.6),ABS(A2/.08)
+*GET,A,VARI,2,ITIME,3.1831
+*DIM,LABEL,CHAR,1,2
+*DIM,VALUE,,1,3
+LABEL(1,1) = 'AMPLITUD'
+LABEL(1,2) = 'E, in   '
+*VFILL,VALUE(1,1),DATA,.0833
+*VFILL,VALUE(1,2),DATA,ABS(A)
+*VFILL,VALUE(1,3),DATA,ABS(A/.0833)
 /COM
-/OUT,vm88,vrt
-/COM,------------------- VM88 RESULTS COMPARISON ---------------
-
+/OUT,vm86,vrt
+/COM,------------------- VM86 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
 (1X,A8,A8,'   ',F10.4,'  ',F14.4,'   ',1F15.3)
 /COM,-----------------------------------------------------------
 /COM,
 /COM,-----------------------------------------------------------
-/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM88  NOT CONTAINED IN
+/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM86  NOT CONTAINED IN
 /COM,THIS TABLE
 /COM,-----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm88,vrt
+*LIST,vm86,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm89.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm89.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM89
 /PREP7
 /TITLE, VM89, NATURAL FREQUENCIES OF A TWO-MASS-SPRING SYSTEM
 C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 163,EX 6.2-2
 ANTYPE,MODAL       ! MODE-FREQUENCY ANALYSIS
 MODOPT,LANB,2
 ET,1,COMBIN14,,,2
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm9.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm9.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM9
 /PREP7
 /TITLE, VM9, LARGE LATERAL DEFLECTION OF UNEQUAL STIFFNESS SPRINGS
 /COM, REF: G.N. VANDERPLAATS, "NUMERICAL OPTIMIZATION TECHNIQUES FOR
 /COM,      ENGINEERING DESIGN", PP 72-73, MCGRAW-HILL, 1984
 ET,1,COMBIN14,,,2          ! UX AND UY DOF ELEMENT
 ET,3,COMBIN40,,,,,,2       ! ALL MASS IS AT NODE J, UX DOF ELEMENT
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm90.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm226.dat`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,160 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM90
-/PREP7                    
-JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
-/SHOW,JPEG
-/TITLE, VM90, HARMONIC RESPONSE OF A TWO-MASS-SPRING SYSTEM
-C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 178,EX 6.6-1
-ANTYPE,HARMIC             ! HARMONIC RESPONSE ANALYSIS
-HROPT,FULL                ! FULL HARMONIC RESPONSE
-HROUT,OFF                 ! PRINT RESULTS AS AMPLITUDES AND PHASE ANGLES
-ET,1,COMBIN14,,,2
-ET,2,MASS21,,,4
-R,1,200                   ! SPRING CONSTANT = 200
-R,2,.5                    ! MASS = 0.5
-N,1
-N,4,1
-FILL
-E,1,2
-TYPE,2
-REAL,2
-E,2                       ! MASS ELEMENT
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM226
+/TITLE,VM226,1D ADVECTION DIFFUSION PROBLEM
+/COM,
+/COM, REFERENCE: ANY STANDARD FLUID DYNAMICS OR HEAT TRANSFER 
+/COM,            TEXTBOOK WITH DIFFUSION EQUATION
+/COM,
+/COM, USING PLANE238 ELEMENTS
+/COM,
+D=0.01              ! DIFFUSIVITY, m^2/s
+V=0.01              ! TRANSPORT VELOCITY, m/s
+
+/PREP7
+ET,1,PLANE238       ! 2D 8 NODE DIFFUSION ELEMENT
+MP,DXX,1,D  
+
+RECT,0,1,0,0.1
 TYPE,1
-REAL,1
-E,2,3                     ! SPRING ELEMENT
-TYPE,2
-REAL,2
-E,3                       ! MASS ELEMENT
+MAT,1
+ESIZE,0.1
+AMESH,ALL
+
+NSEL,S,LOC,X,0
+D,ALL,CONC,0
+NSEL,S,LOC,X,1
+D,ALL,CONC,1
+ALLSEL,ALL
+BF,ALL,VELO,V       ! TRANSPORT VELOCITY
+FINISH
+
+/SOLUTION
+ANTYPE,STATIC
+KBC,1
+TIME,1.0
+OUTRES,ALL,ALL
+/OUT,SCRATCH
+SOLVE
+FINISH
+
+/POST1
+SET,LAST
+PLNSOL,CONC         ! NODAL CONCENTRATION VALUES AT TIME = 1.0seconds
+TNODE=NODE(0.5,0,0)
+CONST=V/D
+EXPECTED=(1.-EXP(.5*CONST))/(1.-EXP(1.*CONST))
+*GET,NVAL,NODE,TNODE,CONC
+*DIM,VALUE,,1,3
+*DIM,LABEL,CHAR,1,1
+LABEL(1,1) = 'CONC'
+*VFILL,VALUE(1,1),DATA,EXPECTED
+*VFILL,VALUE(1,2),DATA,NVAL
+*VFILL,VALUE(1,3),DATA,ABS(EXPECTED/NVAL)
+SAVE,TABLE_1
+FINISH
+/CLEAR,NOSTART
+
+/OUT,
+/COM,
+/COM, USING PLANE223 ELEMENTS
+/COM,
+/TITLE,VM226,1D ADVECTION DIFFUSION PROBLEM
+
+/PREP7
+ET,1,PLANE223,100001        ! COUPLED STRUCTURAL DIFFUSION ELEMENT
+
+D=0.01                      ! DIFFUSIVITY, m^2/s
+V=0.01                      ! TRANSPORT VELOCITY, m/s
+ACCELX=1E9                  ! ACCELERATION, m/sec^2
+T=200                       ! TEMPERATURE, C
+Toff=273                    ! TEMPERATURE OFFSET FROM ABSOLUTE ZERO TO ZERO
+
+MP,DXX,1,D
+MP,EX,1,1E9
+MP,NUXY,1,0.0
+MP,DENS,1,1
+
+V_k=3*V*(T+Toff)/ACCELX/D   ! STRESS-MIGRATION = C*D*V*ACCELX/(k*(t+toff))/3
+TB,MIGR,1
+TBDATA,1,,V_k
+
+RECT,0,1,0,0.1
 TYPE,1
-REAL,1
-E,3,4                     ! SPRING ELEMENT
-OUTPR,BASIC,1
-NSUBST,30                 ! 30 INTERVALS WITHIN FREQ. RANGE
-HARFRQ,,7.5               ! FREQUENCY RANGE FROM 0 TO 7.5 HZ
-KBC,1                     ! STEP BOUNDARY CONDITION
-D,1,UY,,,4
-D,1,UX,,,4,3
-F,2,FX,200
+MAT,1
+ESIZE,0.1
+AMESH,ALL
+
+NSEL,S,LOC,X,0
+D,ALL,CONC,0
+D,ALL,UX,0
+NSEL,S,LOC,X,1.0
+D,ALL,CONC,1
+ALLSEL,ALL
+
+NSEL,S,LOC,Y,0
+NSEL,A,LOC,Y,0.1
+D,ALL,UY,0
+ALLSEL,ALL
+
+TOFFST,Toff
+BF,ALL,TEMP,T
+
+ACEL,ACCELX
 FINISH
-/SOLU    
+
+/SOLUTION
+ANTYPE,STATIC
+KBC,1
+TIME,1.0
+OUTRES,ALL,ALL
+/OUT,SCRATCH
 SOLVE
 FINISH
-/POST26
-FILE,,rst
-NSOL,2,2,U,X,2UX          ! STORE UX DISPLACEMENTS 
-NSOL,3,3,U,X,3UX
-PRVAR,2,3
-*GET,X1,VARI,2,RTIME,1.5
-*GET,X2,VARI,3,RTIME,1.5
-*GET,X3,VARI,2,RTIME,4
-*GET,X4,VARI,3,RTIME,4
-*GET,X5,VARI,2,RTIME,6.5
-*GET,X6,VARI,3,RTIME,6.5
-/GRID,1                   ! TURN GRID ON
-/AXLAB,Y,DISP             ! Y-AXIS LABEL DISP
-PLVAR,2,3                 ! DISPLAY VARIABLES 2 AND 3
-*DIM,LABEL,CHAR,6,2
-*DIM,VALUE,,6,3
-LABEL(1,1) = 'X1, in  ','X2, in  ','X1, in  ','X2, in  ','X1, in  ','X2, in  '
-LABEL(1,2) = 'f=1.5 Hz','f=1.5 Hz','f=4 Hz  ','f=4 Hz  ','f=6.5 Hz','f=6.5 Hz'
-*VFILL,VALUE(1,1),DATA,.82272,.46274,.51145,1.2153,.58513,.26966
-*VFILL,VALUE(1,2),DATA,ABS(X1),ABS(X2),ABS(X3),ABS(X4),ABS(X5),ABS(X6)
-V1 = ABS(X1/.82272)
-V2 = ABS(X2/.46274)
-V3 = ABS(X3/.51145)
-V4 = ABS(X4/1.2153)
-V5 = ABS(X5/.58513)
-V6 = ABS(X6/.26965)
-*VFILL,VALUE(1,3),DATA,V1,V2,V3,V4,V5,V6
-/COM
-/OUT,vm90,vrt
-/COM,------------------- VM90 RESULTS COMPARISON ---------------
-/COM,
-/COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
-/COM,
-*VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.5,'  ',F14.5,'   ',1F15.3)
-/COM,-----------------------------------------------------------
-/COM,
-/COM,-----------------------------------------------------------
-/COM,NOTE: THERE ARE VERIFIED RESULTS IN VM90  NOT CONTAINED IN
-/COM,THIS TABLE
-/COM,-----------------------------------------------------------
-/OUT
+
+/POST1
+SET,LAST
+PLNSOL,CONC             ! NODAL CONCENTRATION VALUES AT TIME = 1.0seconds
+TNODE=NODE(0.5,0,0)
+CONST=V/D
+EXPECTED=(1.-EXP(.5*CONST))/(1.-EXP(1.*CONST))
+*GET,NVAL,NODE,TNODE,CONC
+*DIM,VALUE,,1,3
+*DIM,LABEL,CHAR,1,1
+LABEL(1,1) = 'CONC'
+*VFILL,VALUE(1,1),DATA,EXPECTED
+*VFILL,VALUE(1,2),DATA,NVAL
+*VFILL,VALUE(1,3),DATA,ABS(EXPECTED/NVAL)
+SAVE,TABLE_2
+FINISH
+RESUME,TABLE_1
+/COM,
+/OUT,vm226,vrt
+/COM,
+/COM, -------------------------VM226 RESULTS COMPARISON-------------------
+/COM,
+/COM, 
+/COM,           |  TARGET  |  Mechanical APDL  |   RATIO
+/COM,
+/COM,
+/COM, USING PURE DIFFUSION ELEMENTS - PLANE238
+/COM,
+/COM,
+*VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(2X,A8,'   ',F10.3,'  ',F10.3,'   ',F10.3)
+/COM,
+/COM,
+/NOPR
+RESUME,TABLE_2
+/GOPR
+/COM,
+/COM, USING COUPLED STRUCTURAL DIFFUSION ELEMENTS - PLANE223
+/COM,
+/COM,
+*VWRITE,LABEL(1,1),VALUE(1,1),VALUE(1,2),VALUE(1,3)
+(2X,A8,'   ',F10.3,'  ',F10.3,'   ',F10.3)
+/COM,
+/COM,
+/COM, ---------------------------------------------------------------------
+/OUT,
+*list,vm226,vrt
 FINISH
-*LIST,vm90,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm91.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm91.dat`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM91
 /PREP7                     
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /TITLE, VM91, LARGE ROTATION OF A SWINGING PENDULUM
 C*** VIBRATION THEORY AND APPLICATIONS, THOMSON, 2ND PRINTING, PAGE 138,EX 5.4-1
 /NOPR
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm92.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm93.dat`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,44 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
-/VERIFY,VM92
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
+/VERIFY,VM93
 /PREP7
-/TITLE, VM92, INSULATED WALL TEMPERATURE
-C***        PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 32, EX. 2-5
-ANTYPE,STATIC                ! THERMAL ANALYSIS
-ET,1,LINK34
-ET,2,LINK33
-R,1,1                        ! AREA = 1
-MP,KXX,1,.8
-MP,HF,1,12
-MP,KXX,2,.1
-MP,HF,2,2
+/TITLE, VM93, TEMPERATURE DEPENDENT CONDUCTIVITY
+C***        PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 25, EX. 2-2
+ANTYPE,STATIC
+ET,1,LINK33
+MP,KXX,1,.031,31E-6      ! TEMPERATURE-DEPENDENT CONDUCTIVITY
+R,1,1                    ! AREA = 1
 N,1
-N,2
-N,3,.75
-N,4,(14/12)                  ! 14 INCHES TO FEET
-N,5,(14/12)
+N,2,.25
 E,1,2
-TYPE,2
-E,2,3
-MAT,2
-E,3,4
-TYPE,1
-E,4,5
-D,1,TEMP,3000
-D,5,TEMP,80
+OUTPR,ALL,1
+OUTPR,VENG,NONE
+KBC,1                    ! STEP BOUNDARY CONDITIONS
+D,1,TEMP,300
+D,2,TEMP,100
 FINISH
 /SOLU    
 SOLVE
 FINISH
-/POST1
-PRNSOL,TEMP                  ! PRINT NODAL TEMPERATURES
-PRNLD,HEAT                   ! PRINT HEAT FLOW RATES
-*GET,TI,NODE,2,TEMP
-*GET,TO,NODE,4,TEMP
-FINISH
 /POST26
-ESOL,2,4,5,HEAT,,HEAT
+ESOL,2,1,2,HEAT,,HEAT
 STORE
 *GET,HEAT,VARI,2,EXTREM,VMAX
-*DIM,LABEL,CHAR,3,2
-*DIM,VALUE,,3,3
-LABEL(1,1) = 'Q, BTU/h','TI,     ','TO,     '
-LABEL(1,2) = 'r       ','F       ','F       '
-*VFILL,VALUE(1,1),DATA,513,2957,336
-*VFILL,VALUE(1,2),DATA,HEAT,TI,TO
-*VFILL,VALUE(1,3),DATA,ABS(HEAT/513) ,ABS(TI/2957),ABS(TO/336)
+*DIM,LABEL,CHAR,1,2
+*DIM,VALUE,,1,3
+LABEL(1,1) = 'Q, BTU/h'
+LABEL(1,2) = 'r       '
+*VFILL,VALUE(1,1),DATA,29.760 
+*VFILL,VALUE(1,2),DATA,HEAT
+*VFILL,VALUE(1,3),DATA,ABS(HEAT/29.760 ) 
 /COM
-/OUT,vm92,vrt
-/COM,------------------- VM92 RESULTS COMPARISON --------------
+/OUT,vm93,vrt
+/COM,------------------- VM93 RESULTS COMPARISON --------------
 /COM,
 /COM,                 |   TARGET   |   Mechanical APDL   |   RATIO
 /COM,
 *VWRITE,LABEL(1,1),LABEL(1,2),VALUE(1,1),VALUE(1,2),VALUE(1,3)
-(1X,A8,A8,'   ',F10.0,'  ',F14.0,'   ',1F15.3)
+(1X,A8,A8,'   ',F10.3,'  ',F14.3,'   ',1F15.3)
 /COM,----------------------------------------------------------
 /OUT
 FINISH
-*LIST,vm92,vrt
+*LIST,vm93,vrt
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm94.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm94.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM94
 /PREP7
 /TITLE, VM94, HEAT GENERATING PLATE
 C***        PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 42, EX. 2-9
 ANTYPE,STATIC
 ET,1,LINK33
 ET,2,LINK34
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm95.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm95.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM95
 /PREP7
 /TITLE, VM95, HEAT TRANSFER FROM A COOLING SPINE
 C***  PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 48, EQNS. 2-44,45
 C***  USING LINK33 AND LINK34 ELEMENTS
 ANTYPE,STATIC
 ET,1,LINK33
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm96.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm96.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM96
 JPGPRF,500,100,1             ! MACRO TO SET PREFS FOR JPEG PLOTS
 /SHOW,JPEG
 /PREP7
 smrt,off
 MOPT,VMESH,MAIN
 /TITLE, VM96, TEMPERATURE DISTRIBUTION IN A SHORT SOLID CYLINDER
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm97.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm97.dat`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM97
 /PREP7
 /TITLE, VM97, TEMPERATURE DISTRIBUTION ALONG A STRAIGHT FIN
 C***       PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 57, EX. 2-13
 ANTYPE,STATIC
 ET,1,SHELL131,,,2,1        ! CONDUCTING SHELL ELEMENTS
 ET,2,LINK34                ! CONVECTION ELEMENTS
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm98.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm98.dat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM98
 /PREP7
 /TITLE, VM98, TEMPERATURE DISTRIBUTION ALONG A TAPERED FIN
 C***       PRINCIPLES OF HEAT TRANSFER, KREITH, 2ND. PRINTING, PAGE 57, EX. 2-13
 C***       USING PLANE55 ELEMENTS
 ANTYPE,STATIC
 ET,1,PLANE55
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vm99.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm99.dat`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/COM,ANSYS MEDIA REL. 150 (11/8/2013) REF. VERIF. MANUAL: REL. 150
+/COM,ANSYS MEDIA REL. 2023R1 (11/04/2022) REF. VERIF. MANUAL: REL. 2023R1
 /VERIFY,VM99
 /PREP7
 /TITLE, VM99, TEMPERATURE DISTRIBUTION IN A TRAPEZOIDAL FIN
 C***      CONDUCTION HEAT TRANSFER, SCHNEIDER, 2ND. PRINTING, PAGE 164, ART. 7-8
 ANTYPE,STATIC
 ET,1,PLANE55
 MP,KXX,1,18
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc1.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc1.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc2.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc2.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc3.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc3.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc4.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc4.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc5.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc5.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc6.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc6.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc7.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc7.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmc8.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc8.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmd1.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd1.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmd2.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd2.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vmd3.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd3.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme1.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme1.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme2.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme2.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme3.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme3.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme4.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme4.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme5.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme5.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif/vme6.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme6.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/verif_files.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif_files.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/examples/wing.dat` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/wing.dat`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/component_queries.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/component_queries.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/connectivity_queries.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/connectivity_queries.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/core.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/core.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/geometry_queries.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/geometry_queries.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/inline_functions.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/inline_functions.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/line_queries.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/line_queries.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/nearest_queries.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/nearest_queries.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/normals_queries.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/normals_queries.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/scalar_queries.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/scalar_queries.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/inline_functions/selection_queries.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/selection_queries.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/jupyter.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/jupyter.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/krylov.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/krylov.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/launcher.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/launcher.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Module for launching MAPDL locally or connecting to a remote instance with gRPC."""
 
 import atexit
-from glob import glob
 import os
 import platform
 from queue import Empty, Queue
 import re
 import socket
 import subprocess
 import tempfile
@@ -16,18 +15,18 @@
 try:
     import ansys.platform.instancemanagement as pypim
 
     _HAS_PIM = True
 except ModuleNotFoundError:  # pragma: no cover
     _HAS_PIM = False
 
-import appdirs
+from ansys.tools.path import find_ansys, get_ansys_path, version_from_path
 
 from ansys.mapdl import core as pymapdl
-from ansys.mapdl.core import LINUX_DEFAULT_DIRS, LOG
+from ansys.mapdl.core import LOG
 from ansys.mapdl.core._version import SUPPORTED_ANSYS_VERSIONS
 from ansys.mapdl.core.errors import (
     LockFileException,
     MapdlDidNotStart,
     MapdlRuntimeError,
     VersionError,
 )
@@ -35,21 +34,20 @@
 from ansys.mapdl.core.mapdl import _MapdlCore
 from ansys.mapdl.core.mapdl_grpc import MAX_MESSAGE_LENGTH, MapdlGrpc
 from ansys.mapdl.core.misc import (
     check_valid_ip,
     check_valid_port,
     check_valid_start_instance,
     create_temp_dir,
-    is_float,
     random_string,
     threaded,
 )
 
 # settings directory
-SETTINGS_DIR = appdirs.user_data_dir("ansys_mapdl_core")
+SETTINGS_DIR = pymapdl.USER_DATA_PATH
 if not os.path.isdir(SETTINGS_DIR):
     try:
         os.makedirs(SETTINGS_DIR)
         LOG.debug(f"Created settings directory: {SETTINGS_DIR}")
     except:
         warnings.warn(
             "Unable to create settings directory.\n"
@@ -116,44 +114,14 @@
         if lsb_release.get_distro_information()["ID"].lower() == "ubuntu":
             return True
     except ImportError:
         # finally, check platform
         return "ubuntu" in platform.platform().lower()
 
 
-def _version_from_path(path):
-    """Extract ansys version from a path.  Generally, the version of
-    ANSYS is contained in the path:
-
-    C:/Program Files/ANSYS Inc/v202/ansys/bin/winx64/ANSYS202.exe
-
-    /usr/ansys_inc/v211/ansys/bin/mapdl
-
-    Note that if the MAPDL executable, you have to rely on the version
-    in the path.
-
-    Parameters
-    ----------
-    path : str
-        Path to the MAPDL executable
-
-    Returns
-    -------
-    int
-        Integer version number (e.g. 211).
-
-    """
-    # expect v<ver>/ansys
-    # replace \\ with / to account for possible windows path
-    matches = re.findall(r"v(\d\d\d).ansys", path.replace("\\", "/"), re.IGNORECASE)
-    if not matches:
-        raise MapdlRuntimeError(f"Unable to extract Ansys version from {path}")
-    return int(matches[-1])
-
-
 def close_all_local_instances(port_range=None):
     """Close all MAPDL instances within a port_range.
 
     This function can be used when cleaning up from a failed pool or
     batch run.
 
     Parameters
@@ -430,15 +398,15 @@
         os.mkdir(run_location)
         LOG.debug(f"Creating directory for MAPDL run location: {run_location}")
 
     if not os.access(run_location, os.W_OK):
         raise IOError('Unable to write to ``run_location`` "%s"' % run_location)
 
     # verify version
-    if _version_from_path(exec_file) < 202:
+    if version_from_path("mapdl", exec_file) < 202:
         raise VersionError("The MAPDL gRPC interface requires MAPDL 20.2 or later")
 
     # verify lock file does not exist
     check_lock_file(run_location, jobname, override)
 
     # get the next available port
     if port is None:
@@ -747,210 +715,14 @@
 
     LOG.debug(
         f"PYMAPDL_START_INSTANCE is unset, using default value {start_instance_default}"
     )
     return start_instance_default
 
 
-def _get_available_base_ansys():
-    """Return a dictionary of available Ansys versions with their base paths.
-
-    Returns
-    -------
-    dict[int: str]
-        Return all installed Ansys paths in Windows.
-
-    Notes
-    -----
-
-    On Windows, It uses the environment variable ``AWP_ROOTXXX``.
-
-    The student versions are returned at the end of the dict and with negative value for the version.
-
-    Examples
-    --------
-
-    >>> from ansys.mapdl.core import _get_available_base_ansys
-    >>> _get_available_base_ansys()
-    {222: 'C:\\Program Files\\ANSYS Inc\\v222',
-     212: 'C:\\Program Files\\ANSYS Inc\\v212',
-     -222: 'C:\\Program Files\\ANSYS Inc\\ANSYS Student\\v222'}
-
-    Return all installed Ansys paths in Linux.
-
-    >>> _get_available_base_ansys()
-    {194: '/usr/ansys_inc/v194',
-     202: '/usr/ansys_inc/v202',
-     211: '/usr/ansys_inc/v211'}
-    """
-    base_path = None
-    if os.name == "nt":  # pragma: no cover
-        supported_versions = SUPPORTED_ANSYS_VERSIONS
-        # The student version overwrites the AWP_ROOT env var (if it is installed later)
-        # However the priority should be given to the non-student version.
-        awp_roots = []
-        awp_roots_student = []
-
-        for ver in supported_versions:
-            path_ = os.environ.get(f"AWP_ROOT{ver}", "")
-            path_non_student = path_.replace("\\ANSYS Student", "")
-
-            if "student" in path_.lower() and os.path.exists(path_non_student):
-                # Check if also exist a non-student version
-                awp_roots.append([ver, path_non_student])
-                awp_roots_student.insert(0, [-1 * ver, path_])
-
-            else:
-                awp_roots.append([ver, path_])
-
-        awp_roots.extend(awp_roots_student)
-        installed_versions = {
-            ver: path for ver, path in awp_roots if path and os.path.isdir(path)
-        }
-
-        if installed_versions:
-            LOG.debug(
-                f"Found the following installed Ansys versions: {installed_versions}"
-            )
-            return installed_versions
-        else:  # pragma: no cover
-            LOG.debug(
-                "No installed ANSYS found using 'AWP_ROOT' environments. Let's suppose a base path."
-            )
-            base_path = os.path.join(os.environ["PROGRAMFILES"], "ANSYS INC")
-            if not os.path.exists(base_path):
-                LOG.debug(
-                    f"The supposed 'base_path'{base_path} does not exist. No available ansys found."
-                )
-                return {}
-    elif os.name == "posix":
-        for path in LINUX_DEFAULT_DIRS:
-            if os.path.isdir(path):
-                base_path = path
-    else:  # pragma: no cover
-        raise OSError(f"Unsupported OS {os.name}")
-
-    if base_path is None:
-        return {}
-
-    paths = glob(os.path.join(base_path, "v*"))
-
-    # Testing for ANSYS STUDENT version
-    if not paths:  # pragma: no cover
-        paths = glob(os.path.join(base_path, "ANSYS*"))
-
-    if not paths:
-        return {}
-
-    ansys_paths = {}
-    for path in paths:
-        ver_str = path[-3:]
-        if is_float(ver_str):
-            ansys_paths[int(ver_str)] = path
-
-    return ansys_paths
-
-
-def get_available_ansys_installations():
-    """Return a dictionary of available Ansys versions with their base paths.
-
-    Returns
-    -------
-    dict[int: str]
-        Return all installed Ansys paths in Windows.
-
-    Notes
-    -----
-
-    On Windows, It uses the environment variable ``AWP_ROOTXXX``.
-
-    The student versions are returned at the end of the dict and with negative value for the version.
-
-    Examples
-    --------
-
-    >>> from ansys.mapdl.core import get_available_ansys_installations
-    >>> get_available_ansys_installations()
-    {222: 'C:\\Program Files\\ANSYS Inc\\v222',
-     212: 'C:\\Program Files\\ANSYS Inc\\v212',
-     -222: 'C:\\Program Files\\ANSYS Inc\\ANSYS Student\\v222'}
-
-    Return all installed Ansys paths in Linux.
-
-    >>> get_available_ansys_installations()
-    {194: '/usr/ansys_inc/v194',
-     202: '/usr/ansys_inc/v202',
-     211: '/usr/ansys_inc/v211'}
-    """
-    return _get_available_base_ansys()
-
-
-def find_ansys(version=None):
-    """Searches for ansys path within the standard install location
-    and returns the path of the latest version.
-
-    Parameters
-    ----------
-    version : int, float, optional
-        Version of ANSYS to search for.
-        If using ``int``, it should follow the convention ``XXY``, where ``XX`` is the major version,
-        and ``Y`` is the minor.
-        If using ``float``, it should follow the convention ``XX.Y``, where ``XX`` is the major version,
-        and ``Y`` is the minor.
-        If ``None``, use latest available version on the machine.
-
-    Returns
-    -------
-    ansys_path : str
-        Full path to ANSYS executable.
-
-    version : float
-        Version float.  For example, 21.1 corresponds to 2021R1.
-
-    Examples
-    --------
-    Within Windows
-
-    >>> from ansys.mapdl.core.launcher import find_ansys
-    >>> find_ansys()
-    'C:/Program Files/ANSYS Inc/v211/ANSYS/bin/winx64/ansys211.exe', 21.1
-
-    Within Linux
-
-    >>> find_ansys()
-    (/usr/ansys_inc/v211/ansys/bin/ansys211, 21.1)
-    """
-    versions = _get_available_base_ansys()
-    if not versions:
-        return "", ""
-
-    if not version:
-        version = max(versions.keys())
-
-    elif isinstance(version, float):
-        # Using floats, converting to int.
-        version = int(version * 10)
-
-    try:
-        ans_path = versions[version]
-    except KeyError as e:
-        raise ValueError(
-            f"Version {version} not found. Available versions are {list(versions.keys())}"
-        ) from e
-
-    version = abs(version)
-    if os.name == "nt":
-        ansys_bin = os.path.join(
-            ans_path, "ansys", "bin", "winx64", f"ansys{version}.exe"
-        )
-    else:
-        ansys_bin = os.path.join(ans_path, "ansys", "bin", f"ansys{version}")
-    return ansys_bin, version / 10
-
-
 def get_default_ansys():
     """Searches for ansys path within the standard install location
     and returns the path and version of the latest MAPDL version installed.
 
     Returns
     -------
     ansys_path : str
@@ -968,15 +740,15 @@
     'C:/Program Files/ANSYS Inc/v211/ANSYS/bin/winx64/ansys211.exe', 21.1
 
     Within Linux
 
     >>> get_default_ansys()
     (/usr/ansys_inc/v211/ansys/bin/ansys211, 21.1)
     """
-    return find_ansys()
+    return find_ansys(supported_versions=SUPPORTED_ANSYS_VERSIONS)
 
 
 def get_default_ansys_path():
     """Searches for ansys path within the standard install location
     and returns the path of the latest MAPDL version installed.
 
     Returns
@@ -1021,209 +793,23 @@
 
     >>> get_default_ansys_version()
     21.1
     """
     return get_default_ansys()[1]
 
 
-def get_ansys_path(allow_input=True, version=None):
-    """Acquires ANSYS Path from a cached file or user input
-
-    Parameters
-    ----------
-    allow_input : bool, optional
-        Allow user input to find ANSYS path.  The default is ``True``.
-
-    version : float, optional
-        Version of ANSYS to search for. For example ``version=22.2``.
-        If ``None``, use latest.
-
-    """
-    exe_loc = None
-    if not version and os.path.isfile(CONFIG_FILE):
-        with open(CONFIG_FILE) as f:
-            exe_loc = f.read()
-        # verify
-        if not os.path.isfile(exe_loc) and allow_input:
-            exe_loc = save_ansys_path()
-    elif not version and allow_input:  # create configuration file
-        exe_loc = save_ansys_path()
-
-    if exe_loc is None:
-        exe_loc = find_ansys(version=version)[0]
-        if not exe_loc:
-            exe_loc = None
-
-    return exe_loc
-
-
 def check_valid_ansys():
     """Checks if a valid version of ANSYS is installed and preconfigured"""
     ansys_bin = get_ansys_path(allow_input=False)
     if ansys_bin is not None:
-        version = _version_from_path(ansys_bin)
+        version = version_from_path("mapdl", ansys_bin)
         return not (version < 170 and os.name != "posix")
     return False
 
 
-def change_default_ansys_path(exe_loc):
-    """Change your default ansys path.
-
-    Parameters
-    ----------
-    exe_loc : str
-        Ansys executable path.  Must be a full path.
-
-    Examples
-    --------
-    Change default Ansys location on Linux
-
-    >>> from ansys.mapdl.core import launcher
-    >>> launcher.change_default_ansys_path('/ansys_inc/v201/ansys/bin/ansys201')
-    >>> launcher.get_ansys_path()
-    '/ansys_inc/v201/ansys/bin/ansys201'
-
-    Change default Ansys location on Windows
-
-    >>> ans_pth = 'C:/Program Files/ANSYS Inc/v193/ansys/bin/winx64/ANSYS193.exe'
-    >>> launcher.change_default_ansys_path(ans_pth)
-    >>> launcher.check_valid_ansys()
-    True
-
-    """
-    if os.path.isfile(exe_loc):
-        with open(CONFIG_FILE, "w") as f:
-            f.write(exe_loc)
-    else:
-        raise FileNotFoundError("File %s is invalid or does not exist" % exe_loc)
-
-
-def save_ansys_path(exe_loc=None):  # pragma: no cover
-    """Find MAPDL's path or query user.
-
-    If no ``exe_loc`` argument is supplied, this function attempt
-    to obtain the MAPDL executable from (and in order):
-
-    - The default ansys paths (i.e. ``'C:/Program Files/Ansys Inc/vXXX/ansys/bin/ansysXXX'``)
-    - The configuration file
-    - User input
-
-    If ``exe_loc`` is supplied, this function does some checks.
-    If successful, it will write that ``exe_loc`` into the config file.
-
-    Parameters
-    ----------
-    exe_loc : str, optional
-        Path of the MAPDL executable ('ansysXXX'), by default ``None``.
-
-    Returns
-    -------
-    str
-        Path of the MAPDL executable.
-
-    Notes
-    -----
-    The configuration file location (``config.txt``) can be found in
-    ``appdirs.user_data_dir("ansys_mapdl_core")``. For example:
-
-    .. code:: pycon
-
-        >>> import appdirs
-        >>> import os
-        >>> print(os.path.join(appdirs.user_data_dir("ansys_mapdl_core"), "config.txt"))
-        C:/Users/user/AppData/Local/ansys_mapdl_core/ansys_mapdl_core/config.txt
-
-    Examples
-    --------
-    You can change the default ``exe_loc`` either by modifying the mentioned
-    ``config.txt`` file or by executing:
-
-    >>> from ansys.mapdl.core import save_ansys_path
-    >>> save_ansys_path('/new/path/to/executable')
-
-    """
-    if exe_loc is None:
-        exe_loc, _ = find_ansys()
-
-    if is_valid_executable_path(exe_loc):  # pragma: not cover
-        if not is_common_executable_path(exe_loc):
-            warn_uncommon_executable_path(exe_loc)
-
-        change_default_ansys_path(exe_loc)
-        return exe_loc
-
-    if exe_loc is not None:
-        if is_valid_executable_path(exe_loc):
-            return exe_loc  # pragma: no cover
-
-    # otherwise, query user for the location
-    print("Cached ANSYS executable not found")
-    print(
-        "You are about to enter manually the path of the ANSYS MAPDL executable (ansysXXX, where XXX is the version"
-        "This file is very likely to contained in path ending in 'vXXX/ansys/bin/ansysXXX', but it is not required.\n"
-        "\nIf you experience problems with the input path you can overwrite the configuration file by typing:\n"
-        ">>> from ansys.mapdl.core.launcher import save_ansys_path\n"
-        ">>> save_ansys_path('/new/path/to/executable/')\n"
-    )
-    need_path = True
-    while need_path:  # pragma: no cover
-        exe_loc = input("Enter the location of an ANSYS executable (ansysXXX):")
-
-        if is_valid_executable_path(exe_loc):
-            if not is_common_executable_path(exe_loc):
-                warn_uncommon_executable_path(exe_loc)
-            with open(CONFIG_FILE, "w") as f:
-                f.write(exe_loc)
-            need_path = False
-        else:
-            print(
-                "The supplied path is either: not a valid file path, or does not match 'ansysXXX' name."
-            )
-
-    return exe_loc
-
-
-def is_valid_executable_path(exe_loc):  # pragma: no cover
-    return (
-        os.path.isfile(exe_loc)
-        and re.search("ansys\d\d\d", os.path.basename(os.path.normpath(exe_loc)))
-        is not None
-    )
-
-
-def is_common_executable_path(exe_loc):  # pragma: no cover
-    path = os.path.normpath(exe_loc)
-    path = path.split(os.sep)
-    if (
-        re.search("v(\d\d\d)", exe_loc) is not None
-        and re.search("ansys(\d\d\d)", exe_loc) is not None
-    ):
-        equal_version = (
-            re.search("v(\d\d\d)", exe_loc)[1] == re.search("ansys(\d\d\d)", exe_loc)[1]
-        )
-    else:
-        equal_version = False
-
-    return (
-        is_valid_executable_path(exe_loc)
-        and re.search("v\d\d\d", exe_loc)
-        and "ansys" in path
-        and "bin" in path
-        and equal_version
-    )
-
-
-def warn_uncommon_executable_path(exe_loc):  # pragma: no cover
-    warnings.warn(
-        f"The supplied path ('{exe_loc}') does not match the usual ansys executable path style"
-        "('directory/vXXX/ansys/bin/ansysXXX'). "
-        "You might have problems at later use."
-    )
-
-
 def check_lock_file(path, jobname, override):
     LOG.debug("Checking for lock file")
     # Check for lock file
     lockfile = os.path.join(path, jobname + ".lock")
     if os.path.isfile(lockfile):
         if not override:
             raise LockFileException(
@@ -1274,15 +860,15 @@
         if _is_ubuntu():
             LOG.debug("Ubuntu system detected. Adding 'I_MPI_SHM_LMT' env var.")
             os.environ["I_MPI_SHM_LMT"] = "shm"
 
         if (
             os.name == "nt"
             and not force_intel
-            and (222 > _version_from_path(exec_path) >= 210)
+            and (222 > version_from_path("mapdl", exec_path) >= 210)
         ):
             # Workaround to fix a problem when launching ansys in 'dmp' mode in the
             # recent windows version and using VPN.
             # This is due to the intel compiler, and only afects versions between
             # 210 and 222.
             #
             # There doesn't appear to be an easy way to check if we
@@ -1372,15 +958,15 @@
         variable is set.
 
         .. note::
 
            The executable path can be also set through the environment variable
            ``PYMAPDL_MAPDL_EXEC``. For example:
 
-           .. code:: bash
+           .. code:: console
 
               export PYMAPDL_MAPDL_EXEC=/ansys_inc/v211/ansys/bin/mapdl
 
     run_location : str, optional
         MAPDL working directory.  Defaults to a temporary working
         directory.  If directory doesn't exist, one is created.
 
@@ -1535,22 +1121,22 @@
         process, use ``add_env_vars``. Defaults to ``None``.
 
     version : float, optional
         Version of MAPDL to launch. If ``None``, the latest version is used.
         Versions can be provided as integers (i.e. ``version=222``) or
         floats (i.e. ``version=22.2``).
         To retrieve the available installed versions, use the function
-        :meth:`ansys.mapdl.core.get_available_ansys_installations`.
+        :meth:`ansys.tools.path.path.get_available_ansys_installations`.
 
         .. note::
 
            The default version can be also set through the environment variable
            ``PYMAPDL_MAPDL_VERSION``. For example:
 
-           .. code:: bash
+           .. code:: console
 
               export PYMAPDL_MAPDL_VERSION=22.2
 
     kwargs : dict, optional
         These keyword arguments are interface specific or for
         development purposes. See Notes for more details.
 
@@ -1733,15 +1319,24 @@
             "The ``verbose_mapdl`` argument is deprecated and will be removed in a future release. "
             "Use a logger instead. See :ref:`api_logging` for more details.",
             DeprecationWarning,
         )
         verbose_mapdl = False
 
     # These parameters are partially used for unit testing
-    set_no_abort = kwargs.get("set_no_abort", True)
+    set_no_abort = kwargs.pop("set_no_abort", True)
+
+    # Extract arguments:
+    force_intel = kwargs.pop("force_intel", False)
+    broadcast = kwargs.pop("log_broadcast", False)
+
+    # Raising error if using non-allowed arguments
+    if kwargs:
+        ms_ = ", ".join([f"'{each}'" for each in kwargs.keys()])
+        raise ValueError(f"The following arguments are not recognaised: {ms_}")
 
     if ip is None:
         ip = os.environ.get("PYMAPDL_IP", LOCALHOST)
     else:  # pragma: no cover
         LOG.debug(
             "Because ``PYMAPDL_IP is not None, an attempt is made to connect to a remote session. ('START_INSTANCE' is set to False.`)"
         )
@@ -1894,23 +1489,23 @@
             remove_temp_dir_on_exit = False
 
     LOG.debug("Using run location at %s", run_location)
 
     # verify no lock file and the mode is valid
     check_lock_file(run_location, jobname, override)
 
-    mode = check_mode(mode, _version_from_path(exec_file))
+    mode = check_mode(mode, version_from_path("mapdl", exec_file))
     LOG.debug("Using mode %s", mode)
 
     # Setting SMP by default if student version is used.
     additional_switches = _force_smp_student_version(additional_switches, exec_file)
 
     #
     additional_switches = _validate_MPI(
-        additional_switches, exec_file, kwargs.pop("force_intel", False)
+        additional_switches, exec_file, force_intel=force_intel
     )
 
     additional_switches = _check_license_argument(license_type, additional_switches)
     LOG.debug(f"Using additional switches {additional_switches}.")
 
     start_parm = {
         "exec_file": exec_file,
@@ -1948,15 +1543,14 @@
                 from ansys.mapdl.core.mapdl_corba import MapdlCorba
             except ModuleNotFoundError:  # pragma: no cover
                 raise ModuleNotFoundError(
                     "To use this feature, install the MAPDL CORBA package"
                     " with:\n\npip install ansys_corba"
                 ) from None
 
-            broadcast = kwargs.get("log_broadcast", False)
             mapdl = MapdlCorba(
                 loglevel=loglevel,
                 log_apdl=log_apdl,
                 log_broadcast=broadcast,
                 verbose=verbose_mapdl,
                 **start_parm,
             )
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/licensing.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/licensing.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,21 +460,21 @@
         licdebug log file complete name.
 
     """
     # Licdebug name convention:
     # - For version 22.1 and above: `licdebug.$hostname.$appname.$version.out`
     # - For version 21.2 and below: `licdebug.$appname.$version.out`
 
-    from ansys.mapdl.core.launcher import _version_from_path, get_ansys_path
+    from ansys.mapdl.core.launcher import get_ansys_path, version_from_path
 
     name = "licdebug"
     hostname = socket.gethostname()
     appname = APP_NAME
     # This is the type of license my client requests (Windows 10, 2021R2)
-    version = _version_from_path(get_ansys_path(allow_input=False))
+    version = version_from_path("mapdl", get_ansys_path(allow_input=False))
     ending = "out"
 
     if version < 221:
         parts = (name, appname, version, ending)
     else:
         parts = (name, hostname, appname, version, ending)
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/logging.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,37 @@
         return setup_logger.log
     else:
         setup_logger.log = logger.add_instance_logger("MAPDL", mapdl_instance)
 
     return setup_logger.log
 
 
+_ALLOWED_START_PARM = [
+    "additional_switches",
+    "exec_file",
+    "ip",
+    "jobname",
+    "local",
+    "nproc",
+    "override",
+    "port",
+    "print_com",
+    "process",
+    "ram",
+    "run_location",
+    "start_timeout" "timeout",
+]
+
+
+def _sanitize_start_parm(start_parm):
+    for each_key in start_parm:
+        if each_key not in _ALLOWED_START_PARM:
+            raise ValueError(f"The argument '{each_key}' is not recognaised.")
+
+
 class _MapdlCore(Commands):
     """Contains methods in common between all Mapdl subclasses"""
 
     def __init__(
         self,
         loglevel="DEBUG",
         use_vtk=None,
@@ -189,26 +212,28 @@
                 )
             else:
                 self._use_vtk = False
 
         self._log_filehandler = None
         self._version = None  # cached version
         self._local = local
-        self._jobname = start_parm.get("jobname", "file")
         self._cleanup = True
         self._vget_arr_counter = 0
-        self._start_parm = start_parm
-        self._path = start_parm.get("run_location", None)
-        self._print_com = print_com  # print the command /COM input.
         self._cached_routine = None
         self._geometry = None
-        self._kylov = None
+        self._krylov = None
         self._on_docker = None
         self._platform = None
 
+        _sanitize_start_parm(start_parm)
+        self._start_parm = start_parm
+        self._jobname = start_parm.get("jobname", "file")
+        self._path = start_parm.get("run_location", None)
+        self._print_com = print_com  # print the command /COM input.
+
         # Setting up loggers
         self._log = logger.add_instance_logger(
             self.name, self, level=loglevel
         )  # instance logger
         # adding a file handler to the logger
         if log_file:
             if not isinstance(log_file, str):
@@ -221,14 +246,18 @@
 
         self._parameters = Parameters(self)
 
         from ansys.mapdl.core.solution import Solution
 
         self._solution = Solution(self)
 
+        from ansys.mapdl.core.xpl import ansXpl
+
+        self._xpl = ansXpl(self)
+
         if log_apdl:
             self.open_apdl_log(log_apdl, mode="w")
 
         self._post = PostProcessing(self)
 
         # Wrapping listing functions for "to_array" methods
         self._wrap_listing_functions()
@@ -458,21 +487,36 @@
             self._query = Query(self)
         return self._query
 
     @property
     def non_interactive(self):
         """Non-interactive context manager.
 
-        Use this when using commands that require user
-        interaction within MAPDL (e.g. :func:`Mapdl.vwrite`).
+        Allow to execute code without user interaction or waiting
+        between PyMAPDL responses.
+        It can also be used to execute some commands which are not
+        supported in interactive mode. For a complete list of commands
+        visit :ref:`ref_unsupported_interactive_commands`.
+
+        View the last response with :attr:`Mapdl.last_response` method.
+
+        Notes
+        -----
+        All the commands executed inside this context manager are not
+        executed until the context manager exits which then execute them
+        all at once in the MAPDL instance.
+
+        This command uses :func:`Mapdl.input() <ansys.mapdl.core.Mapdl.input>`
+        method.
 
         Examples
         --------
-        Use the non-interactive context manager for the VWRITE
-        command.  View the last response with :attr:`Mapdl.last_response`.
+        Use the non-interactive context manager for the VWRITE (
+        :func:`Mapdl.vwrite() <ansys.mapdl.core.Mapdl.vwrite>`)
+        command.
 
         >>> with mapdl.non_interactive:
         ...    mapdl.run("*VWRITE,LABEL(1),VALUE(1,1),VALUE(1,2),VALUE(1,3)")
         ...    mapdl.run("(1X,A8,'   ',F10.1,'  ',F10.1,'   ',1F5.3)")
         >>> mapdl.last_response
 
         """
@@ -632,14 +676,15 @@
         def __enter__(self):
             self._parent()._log.debug("Entering non-interactive mode")
             self._parent()._store_commands = True
 
         def __exit__(self, *args):
             self._parent()._log.debug("Exiting non-interactive mode")
             self._parent()._flush_stored()
+            self._parent()._store_commands = False
 
     class _chain_commands:
         """Store MAPDL commands and send one chained command."""
 
         def __init__(self, parent):
             self._parent = weakref.ref(parent)
 
@@ -1049,15 +1094,15 @@
             raise ValueError(
                 "'inplace' and 'include_result' kwargs are not compatible."
             )
 
         if inplace and include_result is None:
             include_result = False
 
-        elif not include_result:
+        if include_result is None:
             include_result = True
 
         if not inplace:
             inplace = False
 
         name = self.jobname
 
@@ -1988,15 +2033,15 @@
 
         # otherwise, use the legacy plotter
         self._enable_interactive_plotting()
         return super().kplot(np1=np1, np2=np2, ninc=ninc, lab=lab, **kwargs)
 
     @property
     @requires_package("ansys.mapdl.reader", softerror=True)
-    def result(self) -> "ansys.mapdl.reader.rst.Result":
+    def result(self):
         """Binary interface to the result file using :class:`ansys.mapdl.reader.rst.Result`.
 
         Returns
         -------
         :class:`ansys.mapdl.reader.rst.Result`.
             Result reader class.  See `Legacy PyMAPDL Reader <https://readerdocs.pyansys.com/>`.
 
@@ -2028,15 +2073,15 @@
         RF  : Nodal reaction forces
         """
         from ansys.mapdl.reader import read_binary
         from ansys.mapdl.reader.rst import Result
 
         if not self._local:
             # download to temporary directory
-            save_path = os.path.join(tempfile.gettempdir(), "ansys_tmp")
+            save_path = os.path.join(tempfile.gettempdir())
             result_path = self.download_result(save_path)
         else:
             if self._distributed_result_file and self._result_file:
                 result_path = self._distributed_result_file
                 result = Result(result_path, read_mesh=False)
                 if result._is_cyclic:
                     result_path = self._result_file
@@ -2232,14 +2277,18 @@
         self,
         entity="",
         entnum="",
         item1="",
         it1num="",
         item2="",
         it2num="",
+        item3="",
+        it3num="",
+        item4="",
+        it4num="",
         **kwargs,
     ):
         """Runs the MAPDL GET command and returns a Python value.
 
         This method uses :func:`Mapdl.get`.
 
         See the full MADPL command documentation at `*GET
@@ -2275,14 +2324,33 @@
             level of information.
 
         it2num : str, int, optional
             The number (or label) for the specified ``item2`` (if
             any). Some ``item2`` labels do not require an ``it2num``
             value.
 
+        item3 : str, optional
+            A third set of item labels and numbers to further qualify the item
+            for which data are to be retrieved. Most items do not require this
+            level of information.
+
+        it3num : str, int, optional
+            The number (or label) for the specified ``item3`` (if
+            any). Some ``item3`` labels do not require an ``it3num``
+            value.
+
+        item4 : str, optional
+            A fourth set of item labels and numbers to further qualify the item
+            for which data are to be retrieved. Most items do not require this level of information.
+
+        it4num : str, int, optional
+            The number (or label) for the specified ``item4`` (if
+            any). Some ``item4`` labels do not require an ``it4num``
+            value.
+
         Returns
         -------
         float
             Floating point value of the parameter.
 
         Examples
         --------
@@ -2301,27 +2369,34 @@
         return self._get(
             entity=entity,
             entnum=entnum,
             item1=item1,
             it1num=it1num,
             item2=item2,
             it2num=it2num,
+            item3=item3,
+            it3num=it3num,
+            item4=item4,
+            it4num=it4num,
             **kwargs,
         )
 
     def get(
         self,
         par="__floatparameter__",
         entity="",
         entnum="",
         item1="",
         it1num="",
         item2="",
         it2num="",
         item3="",
+        it3num="",
+        item4="",
+        it4num="",
         **kwargs,
     ):
         """Retrieves a value and stores it as a scalar parameter or part of an array parameter.
 
         APDL Command: ``*GET``
 
         See the full MADPL command at `*GET
@@ -2392,14 +2467,33 @@
             not require this level of information.
 
         item3
             A third set of item labels to further qualify
             the item for which data are to be retrieved. Almost all items do
             not require this level of information.
 
+        item3 : str, optional
+            A third set of item labels and numbers to further qualify the item
+            for which data are to be retrieved. Most items do not require this
+            level of information.
+
+        it3num : str, int, optional
+            The number (or label) for the specified ``item3`` (if
+            any). Some ``item3`` labels do not require an ``it3num``
+            value.
+
+        item4 : str, optional
+            A fourth set of item labels and numbers to further qualify the item
+            for which data are to be retrieved. Most items do not require this level of information.
+
+        it4num : str, int, optional
+            The number (or label) for the specified ``item4`` (if
+            any). Some ``item4`` labels do not require an ``it4num``
+            value.
+
         Returns
         -------
         float
             Floating point value of the parameter.
 
         Examples
         --------
@@ -2416,17 +2510,15 @@
         >>> value
         3003
 
         """
 
         self._check_parameter_name(par)
 
-        command = (
-            f"*GET,{par},{entity},{entnum},{item1},{it1num},{item2},{it2num},{item3}"
-        )
+        command = f"*GET,{par},{entity},{entnum},{item1},{it1num},{item2},{it2num},{item3},{it3num},{item4},{it4num}"
         kwargs["mute"] = False
 
         # Checking printout is not suppressed by checking "wrinqr" flag.
         with self.force_output:
             response = self.run(command, **kwargs)
 
         value = response.split("=")[-1].strip()
@@ -2754,17 +2846,20 @@
          KEYOPT( 7-12)=        0      0      0        0      0      0
          KEYOPT(13-18)=        0      0      0        0      0      0
 
         """
         if isinstance(commands, str):
             commands = commands.splitlines()
 
-        self._stored_commands = commands
-        self._flush_stored()
-        return self._response
+        self._stored_commands.extend(commands)
+        if self._store_commands:
+            return None
+        else:
+            self._flush_stored()
+            return self._response
 
     def run(self, command, write_to_log=True, mute=None, **kwargs) -> str:
         """
         Run single APDL command.
 
         For multiple commands, use :func:`Mapdl.input_strings()
         <ansys.mapdl.core.Mapdl.input_strings>`.
@@ -3817,14 +3912,31 @@
         @allow_pickable_points()
         @wrap_point_SEL(entity="node")
         def wrapped(self, *args, **kwargs):
             return sel_func(*args, **kwargs)
 
         return wrapped(self, *args, **kwargs)
 
+    @wraps(Commands.esel)
+    def esel(self, *args, **kwargs):
+        """Wraps previons ESEL to allow to use a list/tuple/array for vmin.
+
+        It will raise an error in case vmax or vinc are used too.
+        """
+        sel_func = (
+            super().esel
+        )  # using super() inside the wrapped function confuses the references
+
+        # @allow_pickable_points()
+        @wrap_point_SEL(entity="elem")
+        def wrapped(self, *args, **kwargs):
+            return sel_func(*args, **kwargs)
+
+        return wrapped(self, *args, **kwargs)
+
     @wraps(Commands.ksel)
     def ksel(self, *args, **kwargs):
         """Wraps superclassed KSEL to allow to use a list/tuple/array for vmin.
 
         It will raise an error in case vmax or vinc are used too.
         """
         sel_func = (
@@ -3834,14 +3946,65 @@
         @allow_pickable_points(entity="kp", plot_function="kplot")
         @wrap_point_SEL(entity="kp")
         def wrapped(self, *args, **kwargs):
             return sel_func(*args, **kwargs)
 
         return wrapped(self, *args, **kwargs)
 
+    @wraps(Commands.lsel)
+    def lsel(self, *args, **kwargs):
+        """Wraps superclassed LSEL to allow to use a list/tuple/array for vmin.
+
+        It will raise an error in case vmax or vinc are used too.
+        """
+        sel_func = (
+            super().lsel
+        )  # using super() inside the wrapped function confuses the references
+
+        # @allow_pickable_points(entity="line", plot_function="lplot")
+        @wrap_point_SEL(entity="line")
+        def wrapped(self, *args, **kwargs):
+            return sel_func(*args, **kwargs)
+
+        return wrapped(self, *args, **kwargs)
+
+    @wraps(Commands.asel)
+    def asel(self, *args, **kwargs):
+        """Wraps superclassed ASEL to allow to use a list/tuple/array for vmin.
+
+        It will raise an error in case vmax or vinc are used too.
+        """
+        sel_func = (
+            super().asel
+        )  # using super() inside the wrapped function confuses the references
+
+        # @allow_pickable_points(entity="area", plot_function="aplot")
+        @wrap_point_SEL(entity="area")
+        def wrapped(self, *args, **kwargs):
+            return sel_func(*args, **kwargs)
+
+        return wrapped(self, *args, **kwargs)
+
+    @wraps(Commands.vsel)
+    def vsel(self, *args, **kwargs):
+        """Wraps superclassed VSEL to allow to use a list/tuple/array for vmin.
+
+        It will raise an error in case vmax or vinc are used too.
+        """
+        sel_func = (
+            super().vsel
+        )  # using super() inside the wrapped function confuses the references
+
+        # @allow_pickable_points(entity="volume", plot_function="vplot")
+        @wrap_point_SEL(entity="volume")
+        def wrapped(self, *args, **kwargs):
+            return sel_func(*args, **kwargs)
+
+        return wrapped(self, *args, **kwargs)
+
     def _raise_errors(self, text):
         # to make sure the following error messages are caught even if a breakline is in between.
         flat_text = " ".join([each.strip() for each in text.splitlines()])
 
         if "is not a recognized" in flat_text:
             text = text.replace("This command will be ignored.", "")
             text += "\n\nIgnore these messages by setting 'ignore_errors'=True"
@@ -4155,7 +4318,41 @@
             self._previous_mute, self._parent()._mute = self._parent()._mute, False
 
         def __exit__(self, *args):
             self._parent()._log.debug("Exiting force-output mode")
             if self._in_nopr:
                 self._parent()._run("/nopr")
             self._parent()._mute = self._previous_mute
+
+    def _parse_rlist(self):
+        # mapdl.rmore(*list)
+        with self.force_output:
+            rlist = self.rlist()
+
+        # removing ueless part
+        rlist = rlist.replace(
+            """   *****MAPDL VERIFICATION RUN ONLY*****
+     DO NOT USE RESULTS FOR PRODUCTION
+""",
+            "",
+        )
+        constants_ = re.findall(
+            r"REAL CONSTANT SET.*?\n\n", rlist + "\n\n", flags=re.DOTALL
+        )
+
+        const_ = {}
+        for each in constants_:
+            values = [0 for i in range(18)]
+            set_ = int(re.match(r"REAL CONSTANT SET\s+(\d+)\s+", each).groups()[0])
+            limits = (
+                int(re.match(r".*ITEMS\s+(\d+)\s+", each).groups()[0]),
+                int(re.match(r".*TO\s+(\d+)\s*", each).groups()[0]),
+            )
+            values_ = [float(i) for i in each.strip().splitlines()[1].split()]
+
+            if not set_ in const_.keys():
+                const_[set_] = values
+
+            for i, jlimit in enumerate(range(limits[0] - 1, limits[1])):
+                const_[set_][jlimit] = values_[i]
+
+        return const_
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_console.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_console.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_corba.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_corba.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_geometry.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     """
 
     def __init__(self, mapdl):
         from ansys.mapdl.core.mapdl import _MapdlCore
 
         if not isinstance(mapdl, _MapdlCore):
-            raise TypeError("Must be initialized using a MAPDL class")
+            raise TypeError("Must be initialized using a gRPC MAPDL class")
 
         self._mapdl = mapdl
         self._keypoints_cache = None
         self._lines_cache = None
         self._log = self._mapdl._log
 
     def _set_log_level(self, level):
@@ -886,38 +886,22 @@
 
         # convert to a flat array as it's easier for type checking
         items = np.asarray(items)
         if not np.issubdtype(items.dtype, np.number):
             raise TypeError("Item numbers must be a numeric type")
         items = items.ravel().astype(np.int_, copy=False)
 
-        # consider logic for negative values to support ranges.  This
-        # is the 'ORDER' option
-
-        # ordered items
-        # FLST,5,76,4,ORDE,74
-        # FITEM,5,2
-        # LSEL, , , ,P51X
-
-        # unordered option
-        with self._mapdl.non_interactive:
-            self._mapdl.flst(5, items.size, FLST_LOOKUP[item_type])
-            for item in items:
-                self._mapdl.fitem(5, item)
-
-            # Using 'return_mapdl_output' avoid querying MAPDL in a non-interactive
-            # environment. Otherwise a *get command is issued to MAPDL which will return
-            # none in this non_interactive environment.
-            if item_type == "NODE":
-                self._mapdl.nsel(sel_type, vmin="P51X", return_mapdl_output=True)
-            elif item_type == "ELEM":
-                self._mapdl.esel(sel_type, vmin="P51X", return_mapdl_output=True)
-            elif item_type == "KP":
-                self._mapdl.ksel(sel_type, vmin="P51X", return_mapdl_output=True)
-            elif item_type == "LINE":
-                self._mapdl.lsel(sel_type, vmin="P51X", return_mapdl_output=True)
-            elif item_type == "AREA":
-                self._mapdl.asel(sel_type, vmin="P51X", return_mapdl_output=True)
-            elif item_type == "VOLU":
-                self._mapdl.vsel(sel_type, vmin="P51X", return_mapdl_output=True)
-            else:
-                raise ValueError(f'Unable to select "{item_type}"')
+        # We can use list or arrays for vmin
+        if item_type == "NODE":
+            self._mapdl.nsel(sel_type, vmin=items, return_mapdl_output=True)
+        elif item_type == "ELEM":
+            self._mapdl.esel(sel_type, vmin=items, return_mapdl_output=True)
+        elif item_type == "KP":
+            self._mapdl.ksel(sel_type, vmin=items, return_mapdl_output=True)
+        elif item_type == "LINE":
+            self._mapdl.lsel(sel_type, vmin=items, return_mapdl_output=True)
+        elif item_type == "AREA":
+            self._mapdl.asel(sel_type, vmin=items, return_mapdl_output=True)
+        elif item_type == "VOLU":
+            self._mapdl.vsel(sel_type, vmin=items, return_mapdl_output=True)
+        else:
+            raise ValueError(f'Unable to select "{item_type}"')
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mapdl_grpc.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,31 +27,21 @@
 Please make sure you have the latest updated version using:
 
 'pip install ansys-api-mapdl' or 'pip install --upgrade ansys-api-mapdl'
 
 If this does not solve it, please reinstall 'ansys.mapdl.core'
 or contact Technical Support at 'https://github.com/pyansys/pymapdl'."""
 
-MSG_MODULE = """ANSYS API module `ansys.api.mapdl` could not be found.
-This might be due to a faulty installation or obsolete API module version.
-Please make sure you have the latest updated version using:
-
-'pip install ansys-api-mapdl' or 'pip install --upgrade ansys-api-mapdl'
-
-If this does not solve it, please reinstall 'ansys.mapdl.core'.
-or contact Technical Support at 'https://github.com/pyansys/pymapdl'."""
 
 try:
     from ansys.api.mapdl.v0 import ansys_kernel_pb2 as anskernel
     from ansys.api.mapdl.v0 import mapdl_pb2 as pb_types
     from ansys.api.mapdl.v0 import mapdl_pb2_grpc as mapdl_grpc
 except ImportError:  # pragma: no cover
     raise ImportError(MSG_IMPORT)
-except ModuleNotFoundError:  # pragma: no cover
-    raise ImportError(MSG_MODULE)
 
 from ansys.mapdl.core import _LOCAL_PORTS, __version__
 from ansys.mapdl.core.common_grpc import (
     ANSYS_VALUE_TYPE,
     DEFAULT_CHUNKSIZE,
     DEFAULT_FILE_CHUNK_SIZE,
     parse_chunks,
@@ -68,15 +58,14 @@
     check_valid_ip,
     last_created,
     random_string,
     requires_package,
     run_as_prep7,
     supress_logging,
 )
-from ansys.mapdl.core.post import PostProcessing
 
 # Checking if tqdm is installed.
 # If it is, the default value for progress_bar is true.
 try:
     from tqdm import tqdm
 
     _HAS_TQDM = True
@@ -198,18 +187,18 @@
 class MapdlGrpc(_MapdlCore):
     """This class connects to a GRPC MAPDL server and allows commands
     to be passed to a persistent session.
 
     Parameters
     ----------
     ip : str, optional
-        IP address to connect to the server.  Defaults to 'localhost'.
+        IP address to connect to the server.  The default is 'localhost'.
 
     port : int, optional
-        Port to connect to the mapdl server.  Defaults to 50052.
+        Port to connect to the MAPDL server.  The default is ``50052``.
 
     timeout : float
         Maximum allowable time to connect to the MAPDL server.
 
     loglevel : str, optional
         Sets which messages are printed to the console.  Default
         'INFO' prints out all ANSYS messages, 'WARNING` prints only
@@ -218,28 +207,28 @@
 
     cleanup_on_exit : bool, optional
         Exit MAPDL when Python exits or when this instance is garbage
         collected.
 
     set_no_abort : bool, optional
         Sets MAPDL to not abort at the first error within /BATCH mode.
-        Default ``True``.
+        The default is ``True``.
 
     remove_temp_dir : bool, optional
         When this parameter is ``True``, the MAPDL working directory will be
         deleted when MAPDL is exited provided that it is within the temporary
-        user directory. Default ``False``.
+        user directory. The default is ``False``.
 
     log_file : bool, optional
         Copy the log to a file called `logs.log` located where the
-        python script is executed. Default ``True``.
+        python script is executed. The default is ``True``.
 
     print_com : bool, optional
         Print the command ``/COM`` arguments to the standard output.
-        Default ``False``.
+        The default is ``False``.
 
     channel : grpc.Channel, optional
         gRPC channel to use for the connection. Can be used as an
         alternative to the ``ip`` and ``port`` parameters.
 
     remote_instance : ansys.platform.instancemanagement.Instance
         The corresponding remote instance when MAPDL is launched through
@@ -313,20 +302,23 @@
         self._remote_instance = remote_instance
 
         if channel is not None:
             if ip is not None or port is not None:
                 raise ValueError(
                     "If `channel` is specified, neither `port` nor `ip` can be specified."
                 )
-        elif ip is None:
+        if ip is None:
             ip = "127.0.0.1"
 
         # port and ip are needed to setup the log
         self._port = port
+
+        check_valid_ip(ip)
         self._ip = ip
+
         super().__init__(
             loglevel=loglevel,
             log_apdl=log_apdl,
             log_file=log_file,
             print_com=print_com,
             **start_parm,
         )
@@ -372,23 +364,22 @@
             self._log.debug("Creating channel to %s:%s", ip, port)
             self._channel = self._create_channel(ip, port)
         else:
             self._log.debug("Using provided channel")
             self._channel = channel
 
         # connect and validate to the channel
-        process = start_parm.pop("process", None)
-        self._mapdl_process = process
+        self._mapdl_process = start_parm.pop("process", None)
 
         # Queueing the stds
         if self._mapdl_process:
             self._create_process_stds_queue()
 
         try:
-            self._multi_connect(timeout=timeout, set_no_abort=set_no_abort)
+            self._multi_connect(timeout=timeout)
         except MapdlConnectionError as err:  # pragma: no cover
             self._post_mortem_checks()
             self._log.debug(
                 "The error wasn't catch by the post-mortem checks.\nThe stdout is printed now:"
             )
             self._log.debug(self._stdout)
 
@@ -396,14 +387,32 @@
         else:
             self._log.debug("Connection established")
 
         # Avoiding muting when connecting to the session
         # It might trigger some errors later on if not.
         self._run("/gopr")
 
+        # initialize mesh, post processing, and file explorer interfaces
+        try:
+            from ansys.mapdl.core.mesh_grpc import MeshGrpc
+
+            self._mesh_rep = MeshGrpc(self)
+        except ModuleNotFoundError:  # pragma: no cover
+            self._mesh_rep = None
+
+        # Run at connect
+        self._run_at_connect()
+
+        # HOUSEKEEPING:
+        # Set to not abort after encountering errors.  Otherwise, many
+        # failures in a row will cause MAPDL to exit without returning
+        # anything useful.  Also avoids abort in batch mode if set.
+        if set_no_abort:
+            self._set_no_abort()
+
         # double check we have access to the local path if not
         # explicitly specified
         if "local" not in start_parm:
             self._verify_local()
 
         # only cache process IDs if launched locally
         if self._local and "exec_file" in start_parm:
@@ -418,51 +427,45 @@
             process = self._mapdl_process
 
         self._stdout_queue, self._stdout_thread = _create_queue_for_std(process.stdout)
         self._stderr_queue, self._stderr_thread = _create_queue_for_std(process.stderr)
 
     def _create_channel(self, ip, port):
         """Create an insecured grpc channel."""
-        check_valid_ip(ip)
 
         # open the channel
         channel_str = f"{ip}:{port}"
         self._log.debug("Opening insecure channel at %s", channel_str)
         return grpc.insecure_channel(
             channel_str,
             options=[
                 ("grpc.max_receive_message_length", MAX_MESSAGE_LENGTH),
             ],
         )
 
-    def _multi_connect(self, n_attempts=5, timeout=15, set_no_abort=True):
+    def _multi_connect(self, n_attempts=5, timeout=15):
         """Try to connect over a series of attempts to the channel.
 
         Parameters
         ----------
         n_attempts : int, optional
             Number of connection attempts.
         timeout : float, optional
             Total timeout.
-        set_no_abort : bool, optional
-            Sets MAPDL to not abort at the first error within /BATCH mode.
-            Default ``True``.
 
         """
         # This prevents a single failed connection from blocking other attempts
         connected = False
         attempt_timeout = int(timeout / n_attempts)
 
         max_time = time.time() + timeout
         i = 0
         while time.time() < max_time and i <= n_attempts:
             self._log.debug("Connection attempt %d", i + 1)
-            connected = self._connect(
-                timeout=attempt_timeout, set_no_abort=set_no_abort
-            )
+            connected = self._connect(timeout=attempt_timeout)
             i += 1
             if connected:
                 self._log.debug("Connected")
                 break
         else:  # pragma: no cover
             # Check if mapdl process is alive
             msg = (
@@ -675,15 +678,15 @@
     def mute(self, value):
         self._mute = value
 
     def __repr__(self):
         info = super().__repr__()
         return info
 
-    def _connect(self, timeout=5, set_no_abort=True, enable_health_check=False):
+    def _connect(self, timeout=5, enable_health_check=False):
         """Establish a gRPC channel to a remote or local MAPDL instance.
 
         Parameters
         ----------
         timeout : float
             Time in seconds to wait until the connection has been established
         """
@@ -708,39 +711,18 @@
             self._timer = threading.Thread(
                 target=MapdlGrpc._threaded_heartbeat,
                 args=(weakref.proxy(self),),
             )
             self._timer.daemon = True
             self._timer.start()
 
-        # initialize mesh, post processing, and file explorer interfaces
-        try:
-            from ansys.mapdl.core.mesh_grpc import MeshGrpc
-
-            self._mesh_rep = MeshGrpc(self)
-        except ModuleNotFoundError:  # pragma: no cover
-            self._mesh_rep = None
-
-        from ansys.mapdl.core.xpl import ansXpl
-
-        self._post = PostProcessing(self)
-        self._xpl = ansXpl(self)
-
         # enable health check
         if enable_health_check:
             self._enable_health_check()
 
-        # HOUSEKEEPING:
-        # Set to not abort after encountering errors.  Otherwise, many
-        # failures in a row will cause MAPDL to exit without returning
-        # anything useful.  Also avoids abort in batch mode if set.
-        if set_no_abort:
-            self._set_no_abort()
-
-        self._run_at_connect()
         return True
 
     @property
     def _server_version(self):
         """Return the server version.
 
         Examples
@@ -845,30 +827,14 @@
                 break
             except:
                 pass
 
         if not success:
             raise MapdlConnectionError("Unable to reconnect to MAPDL")
 
-    @property
-    def post_processing(self):
-        """Post-process in an active MAPDL session.
-
-        Examples
-        --------
-        Get the nodal displacement in the X direction for the first
-        result set.
-
-        >>> mapdl.set(1, 1)
-        >>> disp_x = mapdl.post_processing.nodal_displacement('X')
-        array([1.07512979e-04, 8.59137773e-05, 5.70690047e-05, ...,
-               5.70333124e-05, 8.58600402e-05, 1.07445726e-04])
-        """
-        return self._post
-
     @supress_logging
     def _set_no_abort(self):
         """Do not abort MAPDL."""
         self.nerr(abort=-1, mute=True)
 
     def _run_at_connect(self):
         """Run house-keeping commands when initially connecting to MAPDL."""
@@ -897,17 +863,17 @@
         cmd : str
             Valid MAPDL command.
 
         verbose : bool, optional
             Print the response of a command while it is being run.
 
         mute : bool, optional
-            Request that no output be sent from the gRPC server.
-            Defaults to the global setting as specified with
-            ``mapdl.mute = <bool>``.  Default ``False``
+            Whether output is to be sent from the gRPC server. The default
+            is ``None``, in which case the global setting specified by
+            ``mapdl.mute = <bool>`` is used, which is ``False`` by default.
 
         Examples
         --------
         Run a basic command.
 
         >>> mapdl.run('/PREP7')
 
@@ -996,15 +962,15 @@
 
     def exit(self, save=False, force=False):  # pragma: no cover
         """Exit MAPDL.
 
         Parameters
         ----------
         save : bool, optional
-            Save the database on exit.  Default ``False``.
+            Save the database on exit.  The default is ``False``.
         force : bool, optional
             Override any environment variables that may inhibit exiting MAPDL.
 
         Notes
         -----
         If ``PYMAPDL_START_INSTANCE`` is set to ``False`` (generally set in
         remote testing or documentation build), then this will be
@@ -1024,14 +990,18 @@
             # See issue #1796
         elif self._exited:
             # Already exited.
             return
         else:
             mapdl_path = self.directory
 
+        if save:
+            self._log.debug("Saving MAPDL database")
+            self.save()
+
         if not force:
             # lazy import here to avoid circular import
             from ansys.mapdl.core.launcher import get_start_instance
 
             # ignore this method if PYMAPDL_START_INSTANCE=False
             if not get_start_instance():
                 self._log.info("Ignoring exit due to PYMAPDL_START_INSTANCE=False")
@@ -1039,21 +1009,14 @@
             # or building the gallery
             from ansys.mapdl import core as pymapdl
 
             if pymapdl.BUILDING_GALLERY:
                 self._log.info("Ignoring exit due as BUILDING_GALLERY=True")
                 return
 
-        if save:
-            try:
-                self._log.debug("Saving MAPDL database")
-                self.save()
-            except:
-                pass
-
         self._exiting = True
         self._log.debug("Exiting MAPDL")
 
         if self._local:
             self._cache_pids()  # Recache processes
 
             if os.name == "nt":
@@ -1359,16 +1322,17 @@
           Path where the files are downloaded, by default the current
           python path (``os.getcwd()``)
 
         progress_bar : bool, optional
           Show the progress bar or not, default to False.
 
         preference : str
-          Specify the preferred result file, either ``rst`` or ``rth``.
-          Only required when both files are present. Defaults to 'rst'.
+          Preferred type for the result file, which is either ``rst`` or ``rth``.
+          This parameter is only required when both files are present. The default is ```None``,
+          in which case ``"rst"`` is used.
 
         Examples
         --------
         Download remote result files into the current working directory
 
         >>> import os
         >>> mapdl.download_result(os.getcwd())
@@ -1538,33 +1502,38 @@
         option4="",
         option5="",
         option6="",
         option7="",
         **kwargs,
     ):
         """Wraps ``_MapdlCore.tbft``."""
+        extra_info = ""
         if oper.lower() == "eadd":
             # Option 2 is a file and option 4 is the directory.
             # Option 3 is be extension
             option3 = option3.replace(".", "")
             fname = option2 if not option3 else option2 + "." + option3
             filename = os.path.join(option4, fname)
 
-            if self._local:
-                if not os.path.exists(filename) and filename not in self.list_files():
-                    raise FileNotFoundError(f"File '{filename}' could not be found.")
-            else:
-                if os.path.exists(filename):
-                    self.upload(filename)
-                    option4 = ""  # You don't need the directory if you upload it.
-                elif filename in self.list_files():
-                    option4 = ""  # You don't need the directory if the file is in WDIR
-                    pass
-                else:
-                    raise FileNotFoundError(f"File '{filename}' could not be found.")
+            fname = self._get_file_name(fname=option2, ext=option3)
+            if option4:  # if directory is supplied
+                fname = os.path.join(option4, fname)
+
+            filename = self._get_file_path(fname, progress_bar=False)
+
+            # since we upload the file, we dont need the full path: not in option2 nor option4.
+            if not self._local:
+                extra_info = f"PyMAPDL has upload the file {option2} to the MAPDL instance, hence the options for 'TBFT' command have changed."
+                option2 = filename
+                option3 = ""  # the extension is now included in filename
+                option4 = ""
+
+        if extra_info:
+            self.com("")
+            self._log.debug(extra_info)
 
         return super().tbft(
             oper,
             id_,
             option1,
             option2,
             option3,
@@ -1600,42 +1569,42 @@
             in within this command.
             However, the gRPC implementation does *not* uses the APDL ``/INPUT`` command,
             rather the gRPC input method with the appropriate configuration to replicate
             ``/INPUT`` behaviour.
 
         Parameters
         ----------
-        fname : str
-            MAPDL input file to stream to the MAPDL grpc server.
+        fname : str, optional
+            MAPDL input file to stream to the MAPDL gRPC server.
             File name and directory path.
             An unspecified directory path defaults to the Python working
             directory; in this case, you can use all 248 characters for the file name.
             The file name defaults to the current ``Jobname`` if ``Ext`` is specified.
 
-        ext : str
+        ext : str, optional
             Filename extension (eight-character maximum).
 
-        dir : str
-            Directory path. Defaults to current directory.
+        dir : str, optional
+            Directory path. The default is the current working directory.
 
-        line : int
+        line : int, optional
             A value indicating either a line number in the file from which to
             begin reading the input file. The first line is the zero line (Python
             convention).
 
             (blank), or 0
-                Begins reading from the top of the file (default).
+                Begins reading from the top of the file. Default.
 
             LINE_NUMBER
                 Begins reading from the specified line number in the file.
 
-        log
+        log : optional
             Not supported in the gRPC implementation.
 
-        time_step_stream : int
+        time_step_stream : int, optional
             Time to wait between streaming updates to send back chunks
             from the listener file.  Larger values mean more data per
             chunk and less chunks, but if the command is short, will
             wait until time_step_stream is finished leading to a long
             execution time.
 
             Due to stability issues, the default time_step_stream is
@@ -1643,15 +1612,15 @@
 
             - ``verbose=True``: ``time_step_stream=500``
             - ``verbose=False``: ``time_step_stream=50``
 
             These defaults will be ignored if ``time_step_stream`` is
             manually set.
 
-        orig_cmd : str
+        orig_cmd : str, optional
             Original command. There are some cases, were input is
             used to send the file to the grpc server but then we want
             to run something different than ``/INPUT``, for example
             ``CDREAD``.
 
         Returns
         -------
@@ -1813,14 +1782,19 @@
             tmp_dat = f"/OUT,{tmp_out}\n{orig_cmd},'{filename}'\n"
             delete_uploaded_files = True
 
         if write_to_log and self._apdl_log is not None:
             if not self._apdl_log.closed:
                 self._apdl_log.write(tmp_dat)
 
+        # Escaping early if inside non_interactive context
+        if self._store_commands:
+            self._stored_commands.append(tmp_dat.splitlines()[1])
+            return None
+
         if self._local:
             local_path = self.directory
             tmp_name_path = os.path.join(local_path, tmp_name)
             with open(tmp_name_path, "w") as f:
                 f.write(tmp_dat)
         else:
             self._upload_raw(tmp_dat.encode(), tmp_name)
@@ -1924,21 +1898,29 @@
 
         fname can be the full path.
 
         Parameters
         ----------
         fname : str
             File name (with our with extension). It can be a full path.
+
         ext : str, optional
-            File extension, by default None
+            File extension. The default is None.
+
+        default_extension : str
+            Default filename extension. The default is None.
         """
 
         # the old behaviour is to supplied the name and the extension separately.
         # to make it easier let's going to allow names with extensions
 
+        # Sanitizing ext
+        while ext and ext[0] == ".":
+            ext = ext[1:]
+
         if ext:
             fname = fname + "." + ext
         else:
             basename = os.path.basename(fname)
 
             if len(basename.split(".")) == 1:
                 # there is no extension in the main name.
@@ -1995,28 +1977,30 @@
         # try/except here because MAPDL might have not closed the temp file
         try:
             os.remove(tmp_filename)
         except:
             self._log.warning("Unable to remove temporary file %s", tmp_filename)
 
     @protect_grpc
-    def _get(self, entity, entnum, item1, it1num, item2, it2num):
+    def _get(
+        self, entity, entnum, item1, it1num, item2, it2num, item3, it3num, item4, it4num
+    ):
         """Sends gRPC *Get request.
 
         .. warning::
            Not thread safe.  Uses ``_get_lock`` to ensure multiple
            request are not evaluated simultaneously.
         """
         if self._store_commands:
             raise MapdlRuntimeError(
                 "Cannot use gRPC enabled ``GET`` when in non_interactive mode. "
                 "Exit non_interactive mode before using this method."
             )
 
-        cmd = f"{entity},{entnum},{item1},{it1num},{item2},{it2num}"
+        cmd = f"{entity},{entnum},{item1},{it1num},{item2},{it2num},{item3}, {it3num}, {item4}, {it4num}"
 
         # not threadsafe; don't allow multiple get commands
         while self._get_lock:
             time.sleep(0.001)
 
         self._get_lock = True
         try:
@@ -2047,25 +2031,25 @@
         )
 
     def download_project(self, extensions=None, target_dir=None, progress_bar=False):
         """Download all the project files located in the MAPDL working directory.
 
         Parameters
         ----------
-        extensions : List[Str], Tuple[Str], optional
+        extensions : list[str], tuple[str], optional
             List of extensions to filter the files before downloading,
             by default None.
 
-        target_dir : Str, optional
-            Path where the downloaded files will be located, by default None.
+        target_dir : str, optional
+            Path to downloaded the files will to. The default is ``None``.
 
         progress_bar : bool, optional
             Display a progress bar using
             ``tqdm`` when ``True``.  Helpful for showing download
-            progress. Default to ``False``.
+            progress. The default is ``False``.
 
         Returns
         -------
         List[Str]
             List of downloaded files.
         """
         if not extensions:
@@ -2101,30 +2085,33 @@
 
         Parameters
         ----------
         files : str or List[str] or Tuple(str)
             Name of the file on the server. File must be in the same
             directory as the mapdl instance. A list of string names or
             tuples of string names can also be used.
-            List current files with :func:`Mapdl.directory <ansys.mapdl.core.Mapdl.list_files>`.
+            List current files with :meth:`Mapdl.list_files <MapdlGrpc.list_files>`.
 
             Alternatively, you can also specify **glob expressions** to
             match file names. For example: `'file*'` to match every file whose
             name starts with `'file'`.
 
+        target_dir : str, optional
+            Path where the downloaded files will be located. The default is the current
+            working directory.
+
         chunk_size : int, optional
-            Chunk size in bytes.  Must be less than 4MB.  Defaults to 256 kB.
+            Chunk size in bytes.  Must be less than 4MB. The default is 256 kB.
 
         progress_bar : bool, optional
-            Display a progress bar using
-            ``tqdm`` when ``True``.  Helpful for showing download
-            progress.
+            Display a progress bar using ``tqdm`` when ``True``.
+            Helpful for showing download progress.
 
-        recursive : bool
-            Use recursion when using glob pattern.
+        recursive : bool, optional
+            Whether to use recursion when using glob pattern. The default is ``False``.
 
         Notes
         -----
         There are some considerations to keep in mind when using this command:
 
         * The glob pattern search does not search recursively in remote instances.
         * In a remote instance, it is not possible to list or download files in different
@@ -2248,15 +2235,15 @@
 
     @protect_grpc
     def _download(
         self,
         target_name,
         out_file_name=None,
         chunk_size=DEFAULT_CHUNKSIZE,
-        progress_bar=None,
+        progress_bar=False,
     ):
         """Download a file from the gRPC instance.
 
         Parameters
         ----------
         target_name : str
             Target file on the server.  File must be in the same
@@ -2264,19 +2251,20 @@
             ``mapdl.list_files()``
 
         out_file_name : str, optional
             Save the filename as a different name other than the
             ``target_name``.
 
         chunk_size : int, optional
-            Chunk size in bytes.  Must be less than 4MB.  Defaults to 256 kB.
+            Chunk size in bytes.  Must be less than 4MB.  The default is 256 kB.
 
-        progress_bar : bool, optional Display a progress bar using
-            ``tqdm`` when ``True``.  Helpful for showing download
-            progress.
+        progress_bar : bool, optional
+            Display a progress bar using ``tqdm`` when ``True``.
+            Helpful for showing download progress. The default is
+            ``False`` to avoid excessive command printout.
 
         Examples
         --------
         Download the remote result file "file.rst" as "my_result.rst"
 
         >>> mapdl.download('file.rst', 'my_result.rst')
         """
@@ -2306,17 +2294,17 @@
     @protect_grpc
     def upload(self, file_name, progress_bar=True):
         """Upload a file to the grpc instance
 
         file_name : str
             Local file to upload.
 
-        progress_bar : bool, optional Display a progress bar using
-            ``tqdm`` when ``True``.  Helpful for showing download
-            progress.
+        progress_bar : bool, optional
+            Whether to display a progress bar using ``tqdm``. The default is ``True``.
+            This parameter is helpful for showing download progress.
 
         Returns
         -------
         str
             Base name of the file uploaded.  File can be accessed
             relative to the mapdl instance with this file name.
 
@@ -2508,20 +2496,20 @@
         For more information, see the :class:`KrylovSolver <ansys.mapdl.core.krylov.KrylovSolver>`
 
         Returns
         -------
         :class:`Krylov class <ansys.mapdl.core.krylov.KrylovSolver>`
 
         """
-        if self._kylov is None:
+        if self._krylov is None:
             from ansys.mapdl.core.krylov import KrylovSolver
 
-            self._kylov = KrylovSolver(self)
+            self._krylov = KrylovSolver(self)
 
-        return self._kylov
+        return self._krylov
 
     @property
     def db(self):
         """
         MAPDL database interface.
 
         Returns
@@ -2715,109 +2703,38 @@
         elif self._exited:
             raise MapdlExitedError(
                 "Cannot list error file when MAPDL Service has " "exited"
             )
 
         return self._download_as_raw(error_file).decode("latin-1")
 
-    @property
-    @requires_package("ansys.mapdl.reader", softerror=True)
-    def result(self):
-        """Binary interface to the result file using ``pyansys.Result``
+    @wraps(_MapdlCore.igesin)
+    def igesin(self, fname="", ext="", **kwargs):
+        """Wrap the IGESIN command to handle the remote case."""
 
-        Examples
-        --------
-        >>> mapdl.solve()
-        >>> mapdl.finish()
-        >>> result = mapdl.result
-        >>> print(result)
-        PyANSYS MAPDL Result file object
-        Units       : User Defined
-        Version     : 18.2
-        Cyclic      : False
-        Result Sets : 1
-        Nodes       : 3083
-        Elements    : 977
-
-        Available Results:
-        EMS : Miscellaneous summable items (normally includes face pressures)
-        ENF : Nodal forces
-        ENS : Nodal stresses
-        ENG : Element energies and volume
-        EEL : Nodal elastic strains
-        ETH : Nodal thermal strains (includes swelling strains)
-        EUL : Element euler angles
-        EMN : Miscellaneous nonsummable items
-        EPT : Nodal temperatures
-        NSL : Nodal displacements
-        RF  : Nodal reaction forces
-        """
-        from ansys.mapdl.reader import read_binary
-        from ansys.mapdl.reader.rst import Result
+        fname = self._get_file_name(fname=fname, ext=ext)
+        filename = self._get_file_path(fname, progress_bar=False)
 
-        if not self._local:
-            # download to temporary directory
-            save_path = os.path.join(tempfile.gettempdir())
-            result_path = self.download_result(save_path)
-        else:
-            if self._distributed_result_file and self._result_file:
-                result_path = self._distributed_result_file
-                result = Result(result_path, read_mesh=False)
-                if result._is_cyclic:
-                    result_path = self._result_file
-                else:  # pragma: no cover
-                    # return the file with the last access time
-                    filenames = [
-                        self._distributed_result_file,
-                        self._result_file,
-                    ]
-                    result_path = last_created(filenames)
-                    if result_path is None:  # if same return result_file
-                        result_path = self._result_file
-
-            elif self._distributed_result_file:
-                result_path = self._distributed_result_file
-                result = Result(result_path, read_mesh=False)
-                if result._is_cyclic:
-                    if not os.path.isfile(self._result_file):
-                        raise MapdlRuntimeError(
-                            "Distributed Cyclic result not supported"
-                        )
-                    result_path = self._result_file
-            else:
-                result_path = self._result_file
+        if " " in fname:
+            # Bug in reading file paths with whitespaces.
+            # https://github.com/pyansys/pymapdl/issues/1601
 
-        if result_path is None:
-            raise FileNotFoundError("No result file(s) at %s" % self.directory)
-        if not os.path.isfile(result_path):
-            raise FileNotFoundError("No results found at %s" % result_path)
+            msg_ = f"Applying \\IGESIN whitespace patch.\nSee #1601 issue in PyMAPDL repository.\nReading file {fname}"
+            self.input_strings("\n".join([f"! {each}" for each in msg_.splitlines()]))
+            self._log.debug(msg_)
 
-        return read_binary(result_path)
+            cmd = f"*dim,__iges_file__,string,248\n*set,__iges_file__(1), '{filename}'"
+            self.input_strings(cmd)
 
-    @wraps(_MapdlCore.igesin)
-    def igesin(self, fname="", ext="", **kwargs):
-        """Wrap the IGESIN command to handle the remote case."""
-        if self._local:
-            out = super().igesin(fname, ext, **kwargs)
-        elif not fname:
-            out = super().igesin(**kwargs)
-        elif fname in self.list_files():
-            # check if this file is already remote
-            out = super().igesin(fname, ext, **kwargs)
+            out = super().igesin(fname="__iges_file__(1)", **kwargs)
+            self.run("__iges_file__ =")  # cleaning array.
+            self.run("! Ending \\IGESIN whitespace patch.")
+            return out
         else:
-            if not os.path.isfile(fname):
-                raise FileNotFoundError(
-                    f"Unable to find {fname}.  You may need to "
-                    "input the full path to the file."
-                )
-
-            basename = self.upload(fname, progress_bar=False)
-            out = super().igesin(basename, **kwargs)
-
-        return out
+            return super().igesin(fname=filename, **kwargs)
 
     @wraps(_MapdlCore.cmatrix)
     def cmatrix(
         self,
         symfac="",
         condname="",
         numcond="",
@@ -3072,31 +2989,31 @@
 
     def get_nsol(self, node, item, comp, name="", sector="", **kwargs):
         """
         Get NSOL solutions
 
         Parameters
         ----------
-        node
-            Node for which data are to be stored.
+        node : int
+            Node for which data is to be stored.
 
-        item
+        item : str
             Label identifying the item.  Valid item labels are shown in the
-            table below.  Some items also require a component label.
+            table below. Some items also require a component label.
 
-        comp
+        comp : str
             Component of the item (if required).  Valid component labels are
             shown in the table below.
 
-        name
+        name : str, optional
             Thirty-two character name identifying the item on printouts and
-            displays.  Defaults to a label formed by concatenating the first
-            four characters of the Item and Comp labels.
+            displays.  The default is a label formed by concatenating the first
+            four characters of the ``item`` and ``comp`` labels.
 
-        sector
+        sector : int, optional
             For a full harmonic cyclic symmetry solution, the sector number for
             which the results from NODE are to be stored.
 
         Returns
         -------
         np.array
             Variable values
@@ -3145,38 +3062,38 @@
     ):
         """Get ESOL data.
 
         /POST26 APDL Command: ESOL
 
         Parameters
         ----------
-        elem
+        elem : int
             Element for which data are to be stored.
 
-        node
+        node : int
             Node number on this element for which data are to be
             stored. If blank, store the average element value (except
             for FMAG values, which are summed instead of averaged).
 
-        item
+        item : str
             Label identifying the item. General item labels are shown
             in Table 134: ESOL - General Item and Component Labels
             below. Some items also require a component label.
 
-        comp
+        comp : str
             Component of the item (if required). General component
             labels are shown in Table 134: ESOL - General Item and
             Component Labels below.  If Comp is a sequence number (n),
             the NODE field will be ignored.
 
-        name
+        name : str, optional
             Thirty-two character name for identifying the item on the
-            printout and displays.  Defaults to a label formed by
-            concatenating the first four characters of the Item and
-            Comp labels.
+            printout and displays.  The default is a label formed by
+            concatenating the first four characters of the ``item`` and
+           ``comp`` labels.
 
         tstrt : str, optional
             Time (or frequency) corresponding to start of IR data.  If between
             values, the nearer value is used. By default it is the first value.
 
         kcplx : str, optional
             Complex number key:
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/math.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -898,15 +898,26 @@
         thresh : float, optional
             Numerical threshold value used to sparsify. The default
             value is 1E-16.
         """
         kwargs.setdefault("mute", True)
         self._mapdl.run(f"*COMP,{mat.id},SPARSE,{thresh}", **kwargs)
 
-    def eigs(self, nev, k, m=None, c=None, phi=None, algo=None, fmin=None, fmax=None):
+    def eigs(
+        self,
+        nev,
+        k,
+        m=None,
+        c=None,
+        phi=None,
+        algo=None,
+        fmin=None,
+        fmax=None,
+        cpxmod=None,
+    ):
         """Solve an eigenproblem.
 
         Parameters
         ----------
         nev : int
             Number of eigenvalues to compute.
         k : ansys.AnsMat
@@ -929,29 +940,31 @@
         >>> a = mm.mat(k.nrow, nev)
         >>> ev = mm.eigs(nev, k, m, phi=a)
         """
         if not fmin:
             fmin = ""
         if not fmax:
             fmax = ""
+        if not cpxmod:
+            cpxmod = ""
 
         cid = ""
         if not c:
             if k.sym() and m.sym():
                 if not algo:
                     algo = "LANB"
             else:
                 algo = "UNSYM"
         else:
             cid = c.id
             algo = "DAMP"
 
         self._mapdl.run("/SOLU", mute=True)
         self._mapdl.run("antype,modal", mute=True)
-        self._mapdl.run(f"modopt,{algo},{nev},{fmin},{fmax}", mute=True)
+        self._mapdl.run(f"modopt,{algo},{nev},{fmin},{fmax},{cpxmod}", mute=True)
         ev = self.vec()
 
         phistr = "" if not phi else phi.id
         self._mapdl.run(f"*EIG,{k.id},{m.id},{cid},{ev.id},{phistr}", mute=True)
         return ev
 
     def dot(self, vec_a, vec_b):
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mesh/mesh.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh/mesh.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Module for common class between Archive, and result mesh."""
 from ansys.mapdl.reader import _reader, _relaxmidside
 from ansys.mapdl.reader.elements import ETYPE_MAP
 from ansys.mapdl.reader.misc import unique_rows
 import numpy as np
 import pyvista as pv
-from pyvista._vtk import VTK9
 
 INVALID_ALLOWABLE_TYPES = TypeError(
     "`allowable_types` must be an array " "of ANSYS element types from 1 and 300"
 )
 
 # map MESH200 elements to a pymapdl_reader/VTK element type (see elements.py)
 MESH200_MAP = {
@@ -129,40 +128,43 @@
                     continue
                 tshape_num = mesh.tshape_key[etype_ind]
                 if tshape_num >= 19:  # weird bug when 'PILO' can be 99 instead of 19.
                     tshape_num = 19
                 tshape_label = SHAPE_MAP[tshape_num]
                 type_ref[etype_ind] = TARGE170_MAP.get(tshape_label, 0)
 
+    nodes, angles, nnum = mesh.nodes, mesh.node_angles, mesh.nnum
+
     offset, celltypes, cells = _reader.ans_vtk_convert(
-        mesh._elem, mesh._elem_off, type_ref, mesh.nnum, True
+        mesh._elem, mesh._elem_off, type_ref, nnum, True
     )  # for reset_midside
 
-    nodes, angles, nnum = mesh.nodes, mesh.node_angles, mesh.nnum
-
     # fix missing midside
     if np.any(cells == -1):
         if fix_midside:
             nodes, angles, nnum = fix_missing_midside(
                 cells, nodes, celltypes, offset, angles, nnum
             )
         else:
             cells[cells == -1] = 0
 
     if additional_checking:
         cells[cells < 0] = 0
         # cells[cells >= nodes.shape[0]] = 0  # fails when n_nodes < 20
 
-    if VTK9:
-        grid = pv.UnstructuredGrid(cells, celltypes, nodes, deep=True)
-    else:
-        grid = pv.UnstructuredGrid(offset, cells, celltypes, nodes, deep=True)
+    grid = pv.UnstructuredGrid(cells, celltypes, nodes, deep=True)
 
     # Store original ANSYS element and node information
-    grid.point_data["ansys_node_num"] = nnum
+    try:
+        grid.point_data["ansys_node_num"] = nnum
+    except ValueError:
+        grid.point_data["ansys_node_num"] = (
+            mesh._mapdl.nlist(kinternal="internal").to_array()[:, 0].astype(np.int32)
+        )
+
     grid.cell_data["ansys_elem_num"] = mesh.enum
     grid.cell_data["ansys_real_constant"] = mesh.elem_real_constant
     grid.cell_data["ansys_material_type"] = mesh.material_type
     grid.cell_data["ansys_etype"] = mesh._ans_etype
     grid.cell_data["ansys_elem_type_num"] = mesh.etype
 
     # add components
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/mesh_grpc.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -359,26 +359,20 @@
 
         """
         return self._ekey
 
     @property
     def rlblock(self):
         """Real constant data from the RLBLOCK."""
-        # if not self._rdat:
-        #     pass # todo: fix this
-        # return self._rdat
-        raise NotImplementedError()
+        return self._mapdl._parse_rlist()
 
     @property
     def rlblock_num(self):
         """Indices from the real constant data"""
-        # if not self._rnum:
-        #     pass # todo: to fix
-        # return self._rnum
-        raise NotImplementedError()
+        return list(self._mapdl._parse_rlist().keys())
 
     @property
     def nnum(self) -> np.ndarray:
         """Array of currently selected node numbers.
 
         Examples
         --------
@@ -496,15 +490,15 @@
                 ans_keyopt = np.vstack((np.nonzero(keyopt)[0] + 1, valid_keyopt))
                 key_opt[einfo[0]] = ans_keyopt.T.tolist()
 
         return key_opt
 
     @property
     def nodes(self) -> np.ndarray:
-        """Array of nodes.
+        """Array of nodes in Global Cartesian coordinate system.
 
         Examples
         --------
         >>> mapdl.mesh.nodes
         array([[0.   0.   0.  ]
                [1.   0.   0.  ]
                [0.25 0.   0.  ]
@@ -514,14 +508,34 @@
                [0.75 0.5  4.5 ]]
         """
         self._update_node_coord().join()
         if self._node_coord is None:
             return np.empty(0)
         return self._node_coord
 
+    @property
+    def nodes_in_current_CS(self) -> np.ndarray:
+        """Returns the nodes array in the current coordinate system."""
+        CS_id = self._mapdl.get_value("active", 0, "CSYS")
+        return self.nodes_in_coordinate_system(CS_id=CS_id)
+
+    def nodes_in_coordinate_system(self, CS_id):
+        """Return nodes in the desired coordinate system."""
+        if CS_id == 0:
+            return self.nodes
+        else:
+            self._mapdl.parameters["__node_loc__"] = self.nodes
+            self._mapdl.vfun("__node_loc_cs__", "local", "__node_loc__", CS_id)
+            return self._mapdl.parameters["__node_loc_cs__"]
+
+    @property
+    def nodes_rotation(self):
+        """Returns an array of node rotations"""
+        return self._mapdl.nlist(kinternal="").to_array()[:, 4:]
+
     def _load_nodes(self, chunk_size=DEFAULT_CHUNKSIZE):
         """Loads nodes from server.
 
         Parameters
         ----------
         chunk_size : int
             Size of the chunks to request from the server.  Default
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/misc.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Module for miscellaneous functions and methods"""
 from enum import Enum
 from functools import wraps
 import importlib
 import inspect
 import os
+from pathlib import Path
 import platform
 import random
 import re
 import socket
 import string
 import sys
 import tempfile
 from threading import Thread
 from warnings import warn
 import weakref
 
+from ansys.tools.path import get_available_ansys_installations
 import numpy as np
 
 from ansys.mapdl import core as pymapdl
-from ansys.mapdl.core import _HAS_PYVISTA, LINUX_DEFAULT_DIRS, LOG
-from ansys.mapdl.core.errors import MapdlExitedError
+from ansys.mapdl.core import _HAS_PYVISTA, LOG
+from ansys.mapdl.core.errors import MapdlExitedError, MapdlRuntimeError
 
 try:
     import ansys.tools.report as pyansys_report
 
     _HAS_PYANSYS_REPORT = True
 except ModuleNotFoundError:  # pragma: no cover
     LOG.debug("The package 'pyansys-tools-report' is not installed.")
@@ -79,65 +81,14 @@
         valid_routines_str = "\n".join([f'\t- "{item}"' for item in valid_routines])
         raise ValueError(
             f"Invalid routine {routine}. Should be one of:\n{valid_routines_str}"
         )
     return True
 
 
-def get_linux_default_ansys_bin(rver):
-    """Find the MAPDL executable file using standard Linux installation paths,
-
-    Raises:
-        FileNotFoundError: When no binary is found.
-
-    Returns:
-        str: Path to MAPDL executable.
-    """
-    for each_path in LINUX_DEFAULT_DIRS:
-        for each_file in [f"ansys{rver}", "mapdl"]:
-            ans_root = os.getenv(f"AWP_ROOT{rver}", each_path)
-            mapdlbin = os.path.join(ans_root, f"v{rver}", "ansys", "bin", each_file)
-
-            # rare case where the versioned binary doesn't exist
-            if os.path.isfile(mapdlbin):
-                LOG.debug(f"Found ANSYS binary at {mapdlbin}")
-                return mapdlbin
-            else:
-                LOG.debug(f"NOT found Ansys binary at {mapdlbin}")
-
-    # We could not find a binary, returning a default one
-    return os.path.join(
-        LINUX_DEFAULT_DIRS[0], f"v{rver}", "ansys", "bin", f"ansys{rver}"
-    )
-
-
-def get_windows_default_ansys_bin(rver):
-    """Find the MAPDL executable using standard Windows installation paths"""
-    program_files = os.getenv("PROGRAMFILES", os.path.join("c:\\", "Program Files"))
-    ans_root = os.getenv(
-        f"AWP_ROOT{rver}", os.path.join(program_files, "ANSYS Inc", f"v{rver}")
-    )
-    return os.path.join(ans_root, "ansys", "bin", "winx64", f"ANSYS{rver}.exe")
-
-
-def get_ansys_bin(rver):
-    """Identify the ansys executable based on the release version (e.g. "201")"""
-    if os.getenv(f"AWP_ROOT{rver}") is not None:
-        LOG.debug(
-            f"Found 'AWP_ROOT{rver}' environment variable and it has value {os.getenv(f'AWP_ROOT{rver}')}"
-        )
-
-    if os.name == "nt":  # pragma: no cover
-        mapdlbin = get_windows_default_ansys_bin(rver)
-    else:
-        mapdlbin = get_linux_default_ansys_bin(rver)
-
-    return mapdlbin
-
-
 class Plain_Report:
     def __init__(self, core, optional=None, additional=None, **kwargs):
         """
         Base class for a plain report.
 
 
         Based on `scooby <https://github.com/banesullivan/scooby>`_ package.
@@ -231,20 +182,19 @@
             additional = [""]
 
         return "\n".join(header + core + optional + additional) + self.mapdl_info()
 
     def mapdl_info(self):
         """Return information regarding the ansys environment and installation."""
         # this is here to avoid circular imports
-        from ansys.mapdl.core.launcher import _get_available_base_ansys
 
         # List installed Ansys
         lines = ["", "Ansys Environment Report", "-" * 79]
         lines = ["\n", "Ansys Installation", "******************"]
-        mapdl_install = _get_available_base_ansys()
+        mapdl_install = get_available_ansys_installations()
         if not mapdl_install:
             lines.append("Unable to locate any Ansys installations")
         else:  # pragma: no cover
             lines.append("Version   Location")
             lines.append("------------------")
             for key in sorted(mapdl_install.keys()):
                 lines.append(f"{abs(key)}       {mapdl_install[key]}")
@@ -595,22 +545,22 @@
     If the file is local, it will be uploaded.
 
     """
 
     base_fname = os.path.basename(fname)
     if not os.path.exists(fname) and base_fname not in mapdl.list_files():
         raise FileNotFoundError(
-            f"The file {fname} could not be found in the Python working directory ('{os.getcwd()}')"
+            f"The file {fname} could not be found in the Python working directory ('{os.getcwd()}') "
             f"nor in the MAPDL working directory ('{mapdl.directory}')."
         )
 
     elif os.path.exists(fname) and base_fname in mapdl.list_files():  # pragma: no cover
         if priority_mapdl_file is None:
             warn(
-                f"The file '{base_fname}' is present in both, the python working directory ('{os.getcwd()}')"
+                f"The file '{base_fname}' is present in both, the python working directory ('{os.getcwd()}') "
                 f"and in the MAPDL working directory ('{mapdl.directory}'). "
                 "Using the one already in the MAPDL directory.\n"
                 "If you prefer to use the file in the Python directory, you shall remove the file in the MAPDL directory."
             )
             priority_mapdl_file = True
 
         if not priority_mapdl_file:
@@ -733,14 +683,15 @@
     >>> info = mapdl.info
     >>> info.mapdl_version
     'RELEASE  2021 R2           BUILD 21.2      UPDATE 20210601'
 
     """
 
     def __init__(self, mapdl):
+        """Class Initializer"""
         from ansys.mapdl.core.mapdl import _MapdlCore  # lazy import to avoid circular
 
         if not isinstance(mapdl, _MapdlCore):  # pragma: no cover
             raise TypeError("Must be implemented from MAPDL class")
 
         self._mapdl_weakref = weakref.ref(mapdl)
         self._stats = None
@@ -976,14 +927,15 @@
     @update_information_first(True)
     def load_step_options(self):
         """Retrieve the load step options from the MAPDL instance."""
         return self._get_load_step_options()
 
     def _get_between(self, init_string, end_string=None, string=None):
         if not string:
+            self._update()
             string = self._stats
 
         st = string.find(init_string) + len(init_string)
 
         if not end_string:
             en = None
         else:
@@ -1006,16 +958,17 @@
         match = re.match(r"TITLE=(.*)$", self._get_titles())
         if match:
             return match.groups(1)[0].strip()
 
     def _get_stitles(self):
         return [
             re.search(f"SUBTITLE  {i}=(.*)", self._get_titles()).groups(1)[0].strip()
-            for i in range(1, 5)
             if re.search(f"SUBTITLE  {i}=(.*)", self._get_titles())
+            else ""
+            for i in range(1, 5)
         ]
 
     def _get_products(self):
         init_ = "*** Products ***"
         end_string = "*** PreProcessing Capabilities ***"
         return self._get_between(init_, end_string)
 
@@ -1250,16 +1203,16 @@
 
                 self.run(
                     f"/com, Selecting {entity}s from an iterable (i.e. set, list, tuple, or array)"
                 )  # To have a clue in the apdl log file
 
                 if vmax or vinc:
                     raise ValueError(
-                        "If an iterable is used as 'vmin' argument,"
-                        " it is not allowed to use 'vmax' or 'vinc' arguments."
+                        "If an iterable is used as 'vmin' argument, "
+                        "it is not allowed to use 'vmax' or 'vinc' arguments."
                     )
 
                 if len(vmin) == 0 and type_ == "S":
                     # assuming you want to select nothing because you supplied an empty list/tuple/array
                     return original_sel_func(self, "none")
 
                 self._perform_entity_list_selection(
@@ -1268,12 +1221,42 @@
 
                 if kwargs.pop("Used_P", False):
                     # we want to return the
                     return np.array(vmin)
                 else:
                     return
             else:
-                return original_sel_func(self, *args, **kwargs)
+                return original_sel_func(
+                    self,
+                    type_=type_,
+                    item=item,
+                    comp=comp,
+                    vmin=vmin,
+                    vmax=vmax,
+                    vinc=vinc,
+                    kabs=kabs,
+                    **kwargs,
+                )
 
         return wrapper
 
     return decorator
+
+
+def get_active_branch_name():
+    head_dir = Path(".") / ".git" / "HEAD"
+
+    if os.path.exists(head_dir):
+        with head_dir.open("r") as f:
+            content = f.read().splitlines()
+
+        for line in content:
+            if line[0:4] == "ref:":
+                return line.partition("refs/heads/")[2]
+
+    # In case the previous statements return None
+    if "dev" in pymapdl.__version__:
+        kind = "main"
+    else:  # pragma: no cover
+        kind = f"release/{'.'.join(pymapdl.__version__.split('.')[:2])}"
+
+    return kind
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/parameters.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/parameters.py`

 * *Files 9% similar despite different names*

```diff
@@ -351,19 +351,90 @@
         # parameters = self._parm  # check parameter exists
         if isinstance(value, (np.ndarray, list)):
             self._set_parameter_array(key, value)
         else:
             self._set_parameter(key, value)
 
     def __contains__(self, key):
-        return key in self._parm.keys()
+        """
+        Check if a given key is present in the dictionary.
+
+        Parameters
+        ----------
+        key : hashable
+            The key to search for in the dictionary.
+
+        Returns
+        -------
+        bool
+            True if the key is in the dictionary, False otherwise.
+
+        """
+        return key.upper() in self._parm.keys()
 
     def __iter__(self):
+        """
+        Return an iterator over the keys in the dictionary.
+
+        Returns
+        -------
+        iterator
+            An iterator over the keys in the dictionary.
+
+        """
         yield from self._parm.keys()
 
+    def keys(self):
+        """
+        Return a view object that contains the keys in the dictionary.
+
+        Returns
+        -------
+        dict_keys
+            A view object that contains the keys in the dictionary.
+
+        """
+        return self._parm.keys()
+
+    def values(self):
+        """
+        Return a view object that contains the values in the dictionary.
+
+        Returns
+        -------
+        dict_values
+            A view object that contains the values in the dictionary.
+
+        """
+        return self._parm.values()
+
+    def copy(self):
+        """
+        Return a shallow copy of the dictionary.
+
+        Returns
+        -------
+        dict
+            A shallow copy of the dictionary.
+
+        """
+        return self._parm.copy()
+
+    def items(self):
+        """
+        Return a view object that contains the key-value pairs in the dictionary.
+
+        Returns
+        -------
+        dict_items
+            A view object that contains the key-value pairs in the dictionary.
+
+        """
+        return self._parm.items()
+
     @supress_logging
     def _set_parameter(self, name, value):
         """Set a single parameter within MAPDL
 
         Parameters
         ----------
         name : str
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/plotting.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/plotting.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/pool.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,15 @@
 import os
 import shutil
 import time
 import warnings
 
 from ansys.mapdl.core import LOG, get_ansys_path, launch_mapdl
 from ansys.mapdl.core.errors import VersionError
-from ansys.mapdl.core.launcher import (
-    MAPDL_DEFAULT_PORT,
-    _version_from_path,
-    port_in_use,
-)
+from ansys.mapdl.core.launcher import MAPDL_DEFAULT_PORT, port_in_use, version_from_path
 from ansys.mapdl.core.mapdl_grpc import _HAS_TQDM
 from ansys.mapdl.core.misc import create_temp_dir, threaded, threaded_daemon
 
 if _HAS_TQDM:
     from tqdm import tqdm
 
 
@@ -137,15 +133,15 @@
             if exec_file is None:
                 raise FileNotFoundError(
                     "Invalid exec_file path or cannot load cached "
                     "ansys path.  Enter one manually using "
                     "exec_file=<path to executable>"
                 )
 
-        if _version_from_path(exec_file) < 211:
+        if version_from_path("mapdl", exec_file) < 211:
             raise VersionError("LocalMapdlPool requires MAPDL 2021R1 or later.")
 
         # grab available ports
         ports = available_ports(n_instances, port)
 
         if self._root_dir is not None:
             if not os.path.isdir(self._root_dir):
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/post.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,15 @@
         Plot the contact status for the selected elements.
 
         >>> mapdl.post_processing.plot_nodal_values(
         ...     "CONT", "STAT", scalar_bar_args={"title": "Contact status"}
         ... )
         """
 
-        values = self.nodal_values(self, item, comp="")
+        values = self.nodal_values(item=item, comp=comp)
         kwargs.setdefault(
             "scalar_bar_args", {"title": f"item: {item}\nComponent: {comp}"}
         )
         return self._plot_point_scalars(
             values, show_node_numbering=show_node_numbering, **kwargs
         )
```

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/solution.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/solution.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/theme.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/theme.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/src/ansys/mapdl/core/xpl.py` & `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/xpl.py`

 * *Files identical despite different names*

### Comparing `ansys-mapdl-core-0.64.1/PKG-INFO` & `ansys_mapdl_core-0.65.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mapdl-core
-Version: 0.64.1
+Version: 0.65.0
 Summary: A Python wrapper for Ansys MAPDL.
 Author-email: "Ansys, Inc." <pyansys.maintainers@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -19,64 +19,66 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ansys-api-mapdl==0.5.1
 Requires-Dist: ansys-corba; python_version < '3.9'
 Requires-Dist: ansys-mapdl-reader>=0.51.7
 Requires-Dist: ansys-platform-instancemanagement~=1.0
 Requires-Dist: appdirs>=1.4.0
+Requires-Dist: click>=8.1.3
 Requires-Dist: grpcio>=1.30.0
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: matplotlib>=3.0.0
 Requires-Dist: numpy>=1.14.0
 Requires-Dist: pexpect>=4.8.0 ; platform_system=='Linux'
 Requires-Dist: protobuf>=3.12.2
-Requires-Dist: pyiges>=0.1.4
+Requires-Dist: psutil>=5.9.4
 Requires-Dist: pyansys-tools-versioning>=0.3.3
+Requires-Dist: ansys-tools-path>=0.2.4
+Requires-Dist: pyiges>=0.1.4
 Requires-Dist: pyvista>=0.33.0
 Requires-Dist: scipy>=1.3.0
 Requires-Dist: tqdm>=4.45.0
-Requires-Dist: click>=8.1.3
-Requires-Dist: psutil>=5.9.4
-Requires-Dist: sphinx==5.3.0 ; extra == "doc"
-Requires-Dist: ansys-dpf-core==0.8.0 ; extra == "doc"
-Requires-Dist: ansys-mapdl-reader==0.52.11 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.6 ; extra == "doc"
+Requires-Dist: vtk>=9.0.0
+Requires-Dist: sphinx==6.2.1 ; extra == "doc"
+Requires-Dist: ansys-dpf-core==0.8.1 ; extra == "doc"
+Requires-Dist: ansys-mapdl-reader==0.52.13 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: grpcio==1.51.1 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
-Requires-Dist: imageio==2.27.0 ; extra == "doc"
+Requires-Dist: imageio==2.30.0 ; extra == "doc"
 Requires-Dist: jupyter_sphinx==0.4.0 ; extra == "doc"
 Requires-Dist: jupyterlab>=3.2.8 ; extra == "doc"
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: pandas==2.0.0 ; extra == "doc"
-Requires-Dist: plotly==5.14.0 ; extra == "doc"
+Requires-Dist: pandas==2.0.1 ; extra == "doc"
+Requires-Dist: plotly==5.14.1 ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pythreejs==2.4.2 ; extra == "doc"
-Requires-Dist: pyvista==0.38.5 ; extra == "doc"
+Requires-Dist: pyvista==0.39.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.22 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.12.2 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: sphinxemoji==0.2.0 ; extra == "doc"
 Requires-Dist: vtk==9.2.6 ; extra == "doc"
-Requires-Dist: ansys-dpf-core==0.8.0 ; extra == "tests"
+Requires-Dist: ansys-dpf-core==0.8.1 ; extra == "tests"
 Requires-Dist: autopep8==2.0.2 ; extra == "tests"
 Requires-Dist: matplotlib==3.7.1 ; extra == "tests"
 Requires-Dist: scipy==1.10.1 ; extra == "tests"
-Requires-Dist: pandas==2.0.0 ; extra == "tests"
-Requires-Dist: pytest==7.2.2 ; extra == "tests"
-Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
-Requires-Dist: pyvista==0.38.5 ; extra == "tests"
+Requires-Dist: pandas==2.0.1 ; extra == "tests"
+Requires-Dist: pytest==7.3.1 ; extra == "tests"
+Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
+Requires-Dist: pyvista==0.39.1 ; extra == "tests"
 Requires-Dist: pyansys-tools-report==0.5.0 ; extra == "tests"
 Requires-Dist: vtk==9.2.6 ; extra == "tests"
 Requires-Dist: pytest-rerunfailures==11.1.2 ; extra == "tests"
-Project-URL: Source, https://github.com/pyansys/pymapdl
+Project-URL: Source, https://github.com/ansys/pymapdl
 Provides-Extra: doc
 Provides-Extra: tests
 
 PyMAPDL
 =======
 |pyansys| |pypi| |PyPIact| |GH-CI| |codecov| |zenodo| |MIT| |black| |pre-commit|
 
@@ -252,15 +254,15 @@
 (either locally the LAN or through the internet), first ensure you
 have MAPDL started in gRPC server mode.  This example assumes that you
 are launching an instance locally from Windows, but it can be easily
 adapted to run from Linux, or the LAN provided the necessary ports are
 open. This example specifies the port with ``-port 50052``, but this
 option can be left out if you plan on using the default port 50052.
 
-.. code:: pwsh
+.. code:: pwsh-session
 
     start "MAPDL" "%ANSYS211_DIR%\bin\winx64\ANSYS211.exe" -port 50052 -grpc
 
 Next, connect to the instance of MAPDL from python with:
 
 .. code:: pycon
```

