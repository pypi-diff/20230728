# Comparing `tmp/ansys_mapdl_core-0.65.0.tar.gz` & `tmp/ansys_mapdl_core-0.65.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_mapdl_core-0.65.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_mapdl_core-0.65.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_mapdl_core-0.65.0.tar` & `ansys_mapdl_core-0.65.1.tar`

### file list

```diff
@@ -1,521 +1,521 @@
--rw-r--r--   0        0        0     1089 2023-06-02 09:30:43.135172 ansys_mapdl_core-0.65.0/LICENSE
--rw-r--r--   0        0        0    10472 2023-06-02 09:30:43.135172 ansys_mapdl_core-0.65.0/README.rst
--rw-r--r--   0        0        0     4553 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/pyproject.toml
--rw-r--r--   0        0        0     2341 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/__init__.py
--rw-r--r--   0        0        0      134 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/__init__.py
--rw-r--r--   0        0        0     7083 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/abbreviations.py
--rw-r--r--   0        0        0    65022 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/array_param.py
--rw-r--r--   0        0        0    24293 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/macro_files.py
--rw-r--r--   0        0        0    33278 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/matrix_op.py
--rw-r--r--   0        0        0    49087 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/parameter_definition.py
--rw-r--r--   0        0        0      877 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/process_controls.py
--rw-r--r--   0        0        0       65 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/__init__.py
--rw-r--r--   0        0        0     1800 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/general_radiation.py
--rw-r--r--   0        0        0     4381 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/radiation_mat.py
--rw-r--r--   0        0        0    15390 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/radiosity_solver.py
--rw-r--r--   0        0        0     5782 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux15_.py
--rw-r--r--   0        0        0       34 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/__init__.py
--rw-r--r--   0        0        0     2783 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/bin_dump.py
--rw-r--r--   0        0        0    13843 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/bin_manip.py
--rw-r--r--   0        0        0     4949 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux3_.py
--rw-r--r--   0        0        0    11323 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/conn.py
--rw-r--r--   0        0        0       78 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/__init__.py
--rw-r--r--   0        0        0    22459 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/components.py
--rw-r--r--   0        0        0    17248 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/coord_sys.py
--rw-r--r--   0        0        0     4715 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/picking.py
--rw-r--r--   0        0        0    53650 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/selecting.py
--rw-r--r--   0        0        0    13775 2023-06-02 09:30:43.347172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/setup.py
--rw-r--r--   0        0        0    16923 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/working_plane.py
--rw-r--r--   0        0        0       20 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/display_/__init__.py
--rw-r--r--   0        0        0     9516 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/display_/setup.py
--rw-r--r--   0        0        0       73 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/__init__.py
--rw-r--r--   0        0        0    21774 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/annotation.py
--rw-r--r--   0        0        0    11407 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/graphs.py
--rw-r--r--   0        0        0    42963 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/labeling.py
--rw-r--r--   0        0        0    10248 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/scaling.py
--rw-r--r--   0        0        0    53850 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/setup.py
--rw-r--r--   0        0        0    22511 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/style.py
--rw-r--r--   0        0        0    18352 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/views.py
--rw-r--r--   0        0        0     3162 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/hidden.py
--rw-r--r--   0        0        0    50786 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/inq_func.py
--rw-r--r--   0        0        0    10067 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/map_cmd.py
--rw-r--r--   0        0        0       19 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/misc/__init__.py
--rw-r--r--   0        0        0      992 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/misc/misc.py
--rw-r--r--   0        0        0     2975 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/parse.py
--rw-r--r--   0        0        0      248 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/__init__.py
--rw-r--r--   0        0        0    26912 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/animation.py
--rw-r--r--   0        0        0    21848 2023-06-02 09:30:43.351173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/controls.py
--rw-r--r--   0        0        0    31418 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/element_table.py
--rw-r--r--   0        0        0     7015 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/failure_criteria.py
--rw-r--r--   0        0        0    11070 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/listing.py
--rw-r--r--   0        0        0    15600 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/load_case.py
--rw-r--r--   0        0        0    11457 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/magnetics_calc.py
--rw-r--r--   0        0        0    36235 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/path_operations.py
--rw-r--r--   0        0        0    38181 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/results.py
--rw-r--r--   0        0        0    32317 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/setup.py
--rw-r--r--   0        0        0    96414 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/special.py
--rw-r--r--   0        0        0     4431 2023-06-02 09:30:43.355172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/status.py
--rw-r--r--   0        0        0    16032 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/surface_operations.py
--rw-r--r--   0        0        0     8201 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/trace_points.py
--rw-r--r--   0        0        0       77 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/__init__.py
--rw-r--r--   0        0        0     9792 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/controls.py
--rw-r--r--   0        0        0     5716 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/display.py
--rw-r--r--   0        0        0     4351 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/listing.py
--rw-r--r--   0        0        0    22683 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/operations.py
--rw-r--r--   0        0        0    33525 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/setup.py
--rw-r--r--   0        0        0    20246 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/special.py
--rw-r--r--   0        0        0     2904 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/status.py
--rw-r--r--   0        0        0      441 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/__init__.py
--rw-r--r--   0        0        0    42817 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/areas.py
--rw-r--r--   0        0        0     4341 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/artificially_matched_layers.py
--rw-r--r--   0        0        0    62005 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/booleans.py
--rw-r--r--   0        0        0    22650 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/constraint_equations.py
--rw-r--r--   0        0        0    15817 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/coupled_dof.py
--rw-r--r--   0        0        0    38580 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/database.py
--rw-r--r--   0        0        0     4096 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/digitizing.py
--rw-r--r--   0        0        0    16260 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/element_type.py
--rw-r--r--   0        0        0   102587 2023-06-02 09:30:43.359172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/elements.py
--rw-r--r--   0        0        0   158286 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/explicit_dynamics.py
--rw-r--r--   0        0        0     3745 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/hard_points.py
--rw-r--r--   0        0        0    32528 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/keypoints.py
--rw-r--r--   0        0        0    52765 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/lines.py
--rw-r--r--   0        0        0    26805 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/material_data_tables.py
--rw-r--r--   0        0        0    38458 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/materials.py
--rw-r--r--   0        0        0   136306 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/meshing.py
--rw-r--r--   0        0        0    12362 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/morphing.py
--rw-r--r--   0        0        0    43541 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/nodes.py
--rw-r--r--   0        0        0    35522 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/primitives.py
--rw-r--r--   0        0        0     9440 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/real_constants.py
--rw-r--r--   0        0        0    59811 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/sections.py
--rw-r--r--   0        0        0    43269 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/special_purpose.py
--rw-r--r--   0        0        0    15604 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/status.py
--rw-r--r--   0        0        0     9685 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/superelements.py
--rw-r--r--   0        0        0    44600 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/volumes.py
--rw-r--r--   0        0        0       55 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/__init__.py
--rw-r--r--   0        0        0    15305 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/generation.py
--rw-r--r--   0        0        0     3067 2023-06-02 09:30:43.363173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/preparation.py
--rw-r--r--   0        0        0     1154 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/setup.py
--rw-r--r--   0        0        0     4692 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/use_pass.py
--rw-r--r--   0        0        0       66 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/__init__.py
--rw-r--r--   0        0        0    26143 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/files.py
--rw-r--r--   0        0        0     3481 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/list_controls.py
--rw-r--r--   0        0        0     5122 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/processor_entry.py
--rw-r--r--   0        0        0    25874 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/run_controls.py
--rw-r--r--   0        0        0      763 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/all_others.py
--rw-r--r--   0        0        0   157108 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/analysis_options.py
--rw-r--r--   0        0        0     3320 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/birth_and_death.py
--rw-r--r--   0        0        0    56005 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/dynamic_options.py
--rw-r--r--   0        0        0    34700 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_body_loads.py
--rw-r--r--   0        0        0    29784 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_constraints.py
--rw-r--r--   0        0        0    15694 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_forces.py
--rw-r--r--   0        0        0    23544 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_surface_loads.py
--rw-r--r--   0        0        0     8378 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/gap_conditions.py
--rw-r--r--   0        0        0    33877 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/inertia.py
--rw-r--r--   0        0        0     8882 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/load_step_operations.py
--rw-r--r--   0        0        0    36881 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/load_step_options.py
--rw-r--r--   0        0        0     6753 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/master_dof.py
--rw-r--r--   0        0        0    55158 2023-06-02 09:30:43.367173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/miscellaneous_loads.py
--rw-r--r--   0        0        0     4065 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_convergence_controls.py
--rw-r--r--   0        0        0     6518 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_definition_commands.py
--rw-r--r--   0        0        0    12413 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_global_controls.py
--rw-r--r--   0        0        0     7669 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_interface_mapping.py
--rw-r--r--   0        0        0     9429 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_load_transfer.py
--rw-r--r--   0        0        0     7905 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_time_controls.py
--rw-r--r--   0        0        0    58898 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/nonlinear_options.py
--rw-r--r--   0        0        0    15629 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/ocean.py
--rw-r--r--   0        0        0    10287 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/radiosity.py
--rw-r--r--   0        0        0    12029 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/rezoning.py
--rw-r--r--   0        0        0    18965 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_body_loads.py
--rw-r--r--   0        0        0    18072 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_constraints.py
--rw-r--r--   0        0        0     4405 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_forces.py
--rw-r--r--   0        0        0    10519 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_surface_loads.py
--rw-r--r--   0        0        0    12380 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solution_status.py
--rw-r--r--   0        0        0    61309 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/spectrum_options.py
--rw-r--r--   0        0        0     2435 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/twod_to_3d_analysis.py
--rw-r--r--   0        0        0      720 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_version.py
--rw-r--r--   0        0        0    24307 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/commands.py
--rw-r--r--   0        0        0     4583 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/common_grpc.py
--rw-r--r--   0        0        0    36769 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/convert.py
--rw-r--r--   0        0        0      209 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/__init__.py
--rw-r--r--   0        0        0    14261 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/database.py
--rw-r--r--   0        0        0    10848 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/elems.py
--rw-r--r--   0        0        0    16557 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/nodes.py
--rw-r--r--   0        0        0     4532 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/docs.py
--rw-r--r--   0        0        0     5900 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/errors.py
--rw-r--r--   0        0        0      171 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/__init__.py
--rw-r--r--   0        0        0     5342 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/downloads.py
--rw-r--r--   0        0        0     1001 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/examples.py
--rwxr-xr-x   0        0        0     1294 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm1.dat
--rwxr-xr-x   0        0        0     1143 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm10.dat
--rwxr-xr-x   0        0        0     2429 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm100.dat
--rwxr-xr-x   0        0        0     2341 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm101.dat
--rwxr-xr-x   0        0        0     2354 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm102.dat
--rwxr-xr-x   0        0        0     3467 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm103.dat
--rwxr-xr-x   0        0        0     2193 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm104.dat
--rwxr-xr-x   0        0        0     1941 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm105.dat
--rwxr-xr-x   0        0        0     1165 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm106.dat
--rwxr-xr-x   0        0        0     1374 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm107.dat
--rwxr-xr-x   0        0        0     1365 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm108.dat
--rwxr-xr-x   0        0        0     1713 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm109.dat
--rwxr-xr-x   0        0        0     1782 2023-06-02 09:30:43.371173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm11.dat
--rwxr-xr-x   0        0        0     2110 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm110.dat
--rwxr-xr-x   0        0        0     1533 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm111.dat
--rwxr-xr-x   0        0        0     1662 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm112.dat
--rwxr-xr-x   0        0        0     1913 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm113.dat
--rwxr-xr-x   0        0        0     2232 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm114.dat
--rwxr-xr-x   0        0        0     1740 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm115.dat
--rwxr-xr-x   0        0        0     2338 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm116.dat
--rwxr-xr-x   0        0        0     4303 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm117.dat
--rwxr-xr-x   0        0        0     3349 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm118.dat
--rwxr-xr-x   0        0        0     4277 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm119.dat
--rwxr-xr-x   0        0        0     2152 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm12.dat
--rwxr-xr-x   0        0        0     2354 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm120.dat
--rwxr-xr-x   0        0        0     5119 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm121.dat
--rwxr-xr-x   0        0        0     1164 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm122.dat
--rwxr-xr-x   0        0        0     1278 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm123.dat
--rwxr-xr-x   0        0        0     1871 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm124.dat
--rwxr-xr-x   0        0        0     2200 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm125.dat
--rwxr-xr-x   0        0        0     2246 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm126.dat
--rwxr-xr-x   0        0        0     2732 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm127.dat
--rwxr-xr-x   0        0        0     1620 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm128.dat
--rwxr-xr-x   0        0        0     2150 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm129.dat
--rwxr-xr-x   0        0        0     1311 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm13.dat
--rwxr-xr-x   0        0        0     2688 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm130.dat
--rwxr-xr-x   0        0        0     1323 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm131.dat
--rwxr-xr-x   0        0        0     1862 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm132.dat
--rwxr-xr-x   0        0        0     1926 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm133.dat
--rwxr-xr-x   0        0        0     4300 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm134.dat
--rwxr-xr-x   0        0        0     1292 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm135.dat
--rwxr-xr-x   0        0        0     4141 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm136.dat
--rwxr-xr-x   0        0        0     1613 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm137.dat
--rwxr-xr-x   0        0        0     1213 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm138.dat
--rwxr-xr-x   0        0        0     5140 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm139.dat
--rwxr-xr-x   0        0        0     1373 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm14.dat
--rwxr-xr-x   0        0        0     2090 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm140.dat
--rwxr-xr-x   0        0        0     9580 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm141.dat
--rwxr-xr-x   0        0        0     3499 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm142.dat
--rwxr-xr-x   0        0        0    14726 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm143.dat
--rwxr-xr-x   0        0        0     7109 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm144.dat
--rwxr-xr-x   0        0        0     1604 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm145.dat
--rwxr-xr-x   0        0        0     2719 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm146.dat
--rwxr-xr-x   0        0        0     2211 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm147.dat
--rwxr-xr-x   0        0        0     2434 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm148.dat
--rwxr-xr-x   0        0        0     9444 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm149.dat
--rwxr-xr-x   0        0        0     3253 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm15.dat
--rwxr-xr-x   0        0        0     3079 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm150.dat
--rwxr-xr-x   0        0        0     1851 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm151.dat
--rwxr-xr-x   0        0        0     2218 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm152.dat
--rwxr-xr-x   0        0        0     3525 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm153.dat
--rwxr-xr-x   0        0        0     1304 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm154.dat
--rwxr-xr-x   0        0        0     2623 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm155.dat
--rwxr-xr-x   0        0        0     2111 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm156.dat
--rwxr-xr-x   0        0        0     2361 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm157.dat
--rwxr-xr-x   0        0        0     1738 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm158.dat
--rwxr-xr-x   0        0        0     1782 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm159.dat
--rwxr-xr-x   0        0        0     3798 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm16.dat
--rwxr-xr-x   0        0        0     1996 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm160.dat
--rwxr-xr-x   0        0        0     1330 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm161.dat
--rwxr-xr-x   0        0        0     1296 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm162.dat
--rwxr-xr-x   0        0        0     1864 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm163.dat
--rwxr-xr-x   0        0        0     1334 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm164.dat
--rwxr-xr-x   0        0        0     2675 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm165.dat
--rwxr-xr-x   0        0        0     5313 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm166.dat
--rwxr-xr-x   0        0        0     6989 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm167.dat
--rwxr-xr-x   0        0        0     3254 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm168.dat
--rwxr-xr-x   0        0        0     3067 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm169.dat
--rwxr-xr-x   0        0        0     4418 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm17.dat
--rwxr-xr-x   0        0        0     1871 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm170.dat
--rwxr-xr-x   0        0        0     6145 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm171.dat
--rwxr-xr-x   0        0        0     3494 2023-06-02 09:30:43.375172 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm172.dat
--rwxr-xr-x   0        0        0     2335 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm173.dat
--rwxr-xr-x   0        0        0     3230 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm174.dat
--rwxr-xr-x   0        0        0     7199 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm175.dat
--rwxr-xr-x   0        0        0    10669 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm176.dat
--rwxr-xr-x   0        0        0    13041 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm177.dat
--rwxr-xr-x   0        0        0     2406 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm178.dat
--rwxr-xr-x   0        0        0     3603 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm179.dat
--rwxr-xr-x   0        0        0     2570 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm18.dat
--rwxr-xr-x   0        0        0     1741 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm180.dat
--rwxr-xr-x   0        0        0     1315 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm181.dat
--rwxr-xr-x   0        0        0     2478 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm182.dat
--rwxr-xr-x   0        0        0     2117 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm183.dat
--rwxr-xr-x   0        0        0     8768 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm184.dat
--rwxr-xr-x   0        0        0     7867 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm185.dat
--rwxr-xr-x   0        0        0     7761 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm186.dat
--rwxr-xr-x   0        0        0     4075 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm187.dat
--rwxr-xr-x   0        0        0     3640 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm188.dat
--rwxr-xr-x   0        0        0     2788 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm189.dat
--rwxr-xr-x   0        0        0     2363 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm19.dat
--rwxr-xr-x   0        0        0     4207 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm190.dat
--rwxr-xr-x   0        0        0     8521 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm191.dat
--rwxr-xr-x   0        0        0     1997 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm192.dat
--rwxr-xr-x   0        0        0    19768 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm193.dat
--rwxr-xr-x   0        0        0     1806 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm194.dat
--rwxr-xr-x   0        0        0     2059 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm195.dat
--rwxr-xr-x   0        0        0     4882 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm196.dat
--rwxr-xr-x   0        0        0    10456 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm197.dat
--rwxr-xr-x   0        0        0    11449 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm198.dat
--rwxr-xr-x   0        0        0    16406 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm199.dat
--rwxr-xr-x   0        0        0     1628 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm2.dat
--rwxr-xr-x   0        0        0     1695 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm20.dat
--rwxr-xr-x   0        0        0     5739 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm200.dat
--rwxr-xr-x   0        0        0     6398 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm201.dat
--rwxr-xr-x   0        0        0     2541 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm202.dat
--rwxr-xr-x   0        0        0     2650 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm203.dat
--rwxr-xr-x   0        0        0     3666 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm204.dat
--rwxr-xr-x   0        0        0     4965 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm205.dat
--rwxr-xr-x   0        0        0     2601 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm206.dat
--rwxr-xr-x   0        0        0     3280 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm207.dat
--rwxr-xr-x   0        0        0     1940 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm208.dat
--rwxr-xr-x   0        0        0    12271 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm209.dat
--rwxr-xr-x   0        0        0     2721 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm21.dat
--rwxr-xr-x   0        0        0     9391 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm210.dat
--rwxr-xr-x   0        0        0    10266 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm211.dat
--rwxr-xr-x   0        0        0     6116 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm212.dat
--rwxr-xr-x   0        0        0     7793 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm213.dat
--rwxr-xr-x   0        0        0     2080 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm214.dat
--rwxr-xr-x   0        0        0     1755 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm215.dat
--rwxr-xr-x   0        0        0     2988 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm216.dat
--rwxr-xr-x   0        0        0     2041 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm217.dat
--rwxr-xr-x   0        0        0    11642 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm218.dat
--rwxr-xr-x   0        0        0     3857 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm219.dat
--rwxr-xr-x   0        0        0     1133 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm22.dat
--rwxr-xr-x   0        0        0     5191 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm220.dat
--rwxr-xr-x   0        0        0     2040 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm221.dat
--rwxr-xr-x   0        0        0     2660 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm222.dat
--rwxr-xr-x   0        0        0     5776 2023-06-02 09:30:43.379173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm223.dat
--rwxr-xr-x   0        0        0     3557 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm224.dat
--rwxr-xr-x   0        0        0     3076 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm225.dat
--rwxr-xr-x   0        0        0     3045 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm226.dat
--rwxr-xr-x   0        0        0     2644 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm227.dat
--rwxr-xr-x   0        0        0     6215 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm228.dat
--rwxr-xr-x   0        0        0     6354 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm229.dat
--rwxr-xr-x   0        0        0     6500 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm23.dat
--rwxr-xr-x   0        0        0    13140 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm230.dat
--rwxr-xr-x   0        0        0     7508 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm231.dat
--rwxr-xr-x   0        0        0    12245 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm232.dat
--rwxr-xr-x   0        0        0     3641 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm233.dat
--rwxr-xr-x   0        0        0     2512 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm234.dat
--rwxr-xr-x   0        0        0     3682 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm235.dat
--rwxr-xr-x   0        0        0     5976 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm236.dat
--rwxr-xr-x   0        0        0     6546 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm237.dat
--rwxr-xr-x   0        0        0     3577 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm238.dat
--rwxr-xr-x   0        0        0     7798 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm239.dat
--rwxr-xr-x   0        0        0     1321 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm24.dat
--rwxr-xr-x   0        0        0     2365 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm240.dat
--rwxr-xr-x   0        0        0     8657 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm241.dat
--rwxr-xr-x   0        0        0     3161 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm242.dat
--rwxr-xr-x   0        0        0     2539 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm243.dat
--rwxr-xr-x   0        0        0     2902 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm244.dat
--rwxr-xr-x   0        0        0     3393 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm245.dat
--rwxr-xr-x   0        0        0     6795 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm246.dat
--rwxr-xr-x   0        0        0     7914 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm247.dat
--rwxr-xr-x   0        0        0    21905 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm248.dat
--rwxr-xr-x   0        0        0     7788 2023-06-02 09:30:43.383173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm249.dat
--rwxr-xr-x   0        0        0     3963 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm25.dat
--rwxr-xr-x   0        0        0     7596 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm250.dat
--rwxr-xr-x   0        0        0     8087 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm251.dat
--rwxr-xr-x   0        0        0     4136 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm252.dat
--rwxr-xr-x   0        0        0     3729 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm253.dat
--rwxr-xr-x   0        0        0     8515 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm254.dat
--rwxr-xr-x   0        0        0     4234 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm255.dat
--rwxr-xr-x   0        0        0    13336 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm256.dat
--rwxr-xr-x   0        0        0     8703 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm257.dat
--rwxr-xr-x   0        0        0     7160 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm258.dat
--rwxr-xr-x   0        0        0    20687 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm259.dat
--rwxr-xr-x   0        0        0     5148 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm26.dat
--rwxr-xr-x   0        0        0     8199 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm260.dat
--rwxr-xr-x   0        0        0     5024 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm261.dat
--rwxr-xr-x   0        0        0     3065 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm262.dat
--rwxr-xr-x   0        0        0    26501 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm263.dat
--rwxr-xr-x   0        0        0     7906 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm264.dat
--rwxr-xr-x   0        0        0     5972 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm265.dat
--rwxr-xr-x   0        0        0    10185 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm266.dat
--rwxr-xr-x   0        0        0     5657 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm267.dat
--rwxr-xr-x   0        0        0     3299 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm268.dat
--rwxr-xr-x   0        0        0     2805 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm269.dat
--rwxr-xr-x   0        0        0     1755 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm27.dat
--rwxr-xr-x   0        0        0     4557 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm270.dat
--rwxr-xr-x   0        0        0    15604 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm271.dat
--rwxr-xr-x   0        0        0    20113 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm272.dat
--rwxr-xr-x   0        0        0     5455 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm273.dat
--rwxr-xr-x   0        0        0     3861 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm274.dat
--rwxr-xr-x   0        0        0     8112 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm275.dat
--rwxr-xr-x   0        0        0     3493 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm276.dat
--rwxr-xr-x   0        0        0     2927 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm277.dat
--rwxr-xr-x   0        0        0     3941 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm278.dat
--rwxr-xr-x   0        0        0     8873 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm279.dat
--rwxr-xr-x   0        0        0     2146 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm28.dat
--rwxr-xr-x   0        0        0     5670 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm280.dat
--rwxr-xr-x   0        0        0    11199 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm281.dat
--rwxr-xr-x   0        0        0     5507 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm282.dat
--rwxr-xr-x   0        0        0     4643 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm283.dat
--rw-r--r--   0        0        0     8968 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm284.dat
--rw-r--r--   0        0        0     3246 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm285.dat
--rw-r--r--   0        0        0     6386 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm286.dat
--rw-r--r--   0        0        0     4820 2023-06-02 09:30:43.387173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm287.dat
--rw-r--r--   0        0        0     6538 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm288.dat
--rw-r--r--   0        0        0     4181 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm289.dat
--rwxr-xr-x   0        0        0     4831 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm29.dat
--rw-r--r--   0        0        0     3166 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm290.dat
--rw-r--r--   0        0        0    10932 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm291.dat
--rw-r--r--   0        0        0     3336 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm292.dat
--rw-r--r--   0        0        0     4870 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm293.dat
--rw-r--r--   0        0        0     9804 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm294.dat
--rw-r--r--   0        0        0     4039 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm295.dat
--rw-r--r--   0        0        0    13015 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm296.dat
--rw-r--r--   0        0        0     3945 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm297.dat
--rw-r--r--   0        0        0     7921 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm298.dat
--rw-r--r--   0        0        0     2525 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm299.dat
--rwxr-xr-x   0        0        0     1686 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm3.dat
--rwxr-xr-x   0        0        0     2541 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm30.dat
--rw-r--r--   0        0        0     2728 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm300.dat
--rw-r--r--   0        0        0     3680 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm301.dat
--rw-r--r--   0        0        0    14358 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm302.dat
--rw-r--r--   0        0        0     7826 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm303.dat
--rw-r--r--   0        0        0     3600 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm304.dat
--rw-r--r--   0        0        0     2644 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm305.dat
--rw-r--r--   0        0        0     2156 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm306.dat
--rw-r--r--   0        0        0     1561 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm307.dat
--rw-r--r--   0        0        0     3832 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm308.dat
--rw-r--r--   0        0        0     2255 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm309.dat
--rwxr-xr-x   0        0        0     3036 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm31.dat
--rw-r--r--   0        0        0     7310 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm310.dat
--rw-r--r--   0        0        0     8882 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm311.dat
--rw-r--r--   0        0        0     8654 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm312.dat
--rw-r--r--   0        0        0     4303 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm313.dat
--rw-r--r--   0        0        0     2738 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm314.dat
--rw-r--r--   0        0        0     4253 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm315.dat
--rw-r--r--   0        0        0     9789 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm316.dat
--rw-r--r--   0        0        0     6697 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm317.dat
--rw-r--r--   0        0        0     3273 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm318.dat
--rwxr-xr-x   0        0        0     2889 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm32.dat
--rwxr-xr-x   0        0        0     5950 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm33.dat
--rwxr-xr-x   0        0        0     6416 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm34.dat
--rwxr-xr-x   0        0        0     2157 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm35.dat
--rwxr-xr-x   0        0        0     4291 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm36.dat
--rwxr-xr-x   0        0        0     3955 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm37.dat
--rwxr-xr-x   0        0        0     4674 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm38.dat
--rwxr-xr-x   0        0        0     5136 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm39.dat
--rwxr-xr-x   0        0        0     1464 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm4.dat
--rwxr-xr-x   0        0        0     2954 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm40.dat
--rwxr-xr-x   0        0        0     5122 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm41.dat
--rwxr-xr-x   0        0        0     3012 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm42.dat
--rwxr-xr-x   0        0        0     2779 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm43.dat
--rwxr-xr-x   0        0        0     2891 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm44.dat
--rwxr-xr-x   0        0        0     1052 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm45.dat
--rwxr-xr-x   0        0        0     3393 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm46.dat
--rwxr-xr-x   0        0        0     1498 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm47.dat
--rwxr-xr-x   0        0        0     1543 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm48.dat
--rwxr-xr-x   0        0        0     3279 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm49.dat
--rwxr-xr-x   0        0        0     2882 2023-06-02 09:30:43.391173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm5.dat
--rwxr-xr-x   0        0        0     1463 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm50.dat
--rwxr-xr-x   0        0        0    13711 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm51.dat
--rwxr-xr-x   0        0        0     1871 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm52.dat
--rwxr-xr-x   0        0        0     2275 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm53.dat
--rwxr-xr-x   0        0        0     5974 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm54.dat
--rwxr-xr-x   0        0        0     1747 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm55.dat
--rwxr-xr-x   0        0        0     5942 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm56.dat
--rwxr-xr-x   0        0        0     5808 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm57.dat
--rwxr-xr-x   0        0        0     1876 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm58.dat
--rwxr-xr-x   0        0        0     2136 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm59.dat
--rwxr-xr-x   0        0        0     2369 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm6.dat
--rwxr-xr-x   0        0        0     1679 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm60.dat
--rwxr-xr-x   0        0        0     1312 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm61.dat
--rwxr-xr-x   0        0        0     4605 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm62.dat
--rwxr-xr-x   0        0        0     3642 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm63.dat
--rwxr-xr-x   0        0        0     1708 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm64.dat
--rwxr-xr-x   0        0        0     3090 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm65.dat
--rwxr-xr-x   0        0        0     4459 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm66.dat
--rwxr-xr-x   0        0        0     1560 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm67.dat
--rwxr-xr-x   0        0        0     2510 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm68.dat
--rwxr-xr-x   0        0        0     1823 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm69.dat
--rwxr-xr-x   0        0        0     6368 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm7.dat
--rwxr-xr-x   0        0        0     2172 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm70.dat
--rwxr-xr-x   0        0        0     2366 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm71.dat
--rwxr-xr-x   0        0        0     2805 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm72.dat
--rwxr-xr-x   0        0        0     2047 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm73.dat
--rwxr-xr-x   0        0        0     2647 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm74.dat
--rwxr-xr-x   0        0        0     2391 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm75.dat
--rwxr-xr-x   0        0        0     2401 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm76.dat
--rwxr-xr-x   0        0        0     2703 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm77.dat
--rwxr-xr-x   0        0        0     2157 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm78.dat
--rwxr-xr-x   0        0        0     2369 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm79.dat
--rwxr-xr-x   0        0        0     3521 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm8.dat
--rwxr-xr-x   0        0        0     2436 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm80.dat
--rwxr-xr-x   0        0        0     4016 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm81.dat
--rwxr-xr-x   0        0        0    10303 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm82.dat
--rwxr-xr-x   0        0        0     2368 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm83.dat
--rwxr-xr-x   0        0        0     2250 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm84.dat
--rwxr-xr-x   0        0        0     2867 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm85.dat
--rwxr-xr-x   0        0        0     1441 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm86.dat
--rwxr-xr-x   0        0        0     1568 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm87.dat
--rwxr-xr-x   0        0        0     1627 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm88.dat
--rwxr-xr-x   0        0        0     2123 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm89.dat
--rwxr-xr-x   0        0        0     2471 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm9.dat
--rwxr-xr-x   0        0        0     2604 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm90.dat
--rwxr-xr-x   0        0        0     2837 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm91.dat
--rwxr-xr-x   0        0        0     1402 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm92.dat
--rwxr-xr-x   0        0        0     1115 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm93.dat
--rwxr-xr-x   0        0        0     1549 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm94.dat
--rwxr-xr-x   0        0        0     3501 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm95.dat
--rwxr-xr-x   0        0        0     3033 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm96.dat
--rwxr-xr-x   0        0        0     2585 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm97.dat
--rwxr-xr-x   0        0        0     2041 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm98.dat
--rwxr-xr-x   0        0        0     1614 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm99.dat
--rwxr-xr-x   0        0        0    11868 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc1.dat
--rwxr-xr-x   0        0        0     9617 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc2.dat
--rwxr-xr-x   0        0        0     4766 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc3.dat
--rwxr-xr-x   0        0        0     6787 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc4.dat
--rwxr-xr-x   0        0        0     5775 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc5.dat
--rwxr-xr-x   0        0        0     6120 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc6.dat
--rwxr-xr-x   0        0        0     4152 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc7.dat
--rwxr-xr-x   0        0        0     4320 2023-06-02 09:30:43.395173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc8.dat
--rwxr-xr-x   0        0        0    11304 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd1.dat
--rwxr-xr-x   0        0        0     4372 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd2.dat
--rwxr-xr-x   0        0        0    11914 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd3.dat
--rwxr-xr-x   0        0        0     2600 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme1.dat
--rwxr-xr-x   0        0        0     1771 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme2.dat
--rwxr-xr-x   0        0        0     3360 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme3.dat
--rwxr-xr-x   0        0        0     3447 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme4.dat
--rwxr-xr-x   0        0        0     2452 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme5.dat
--rwxr-xr-x   0        0        0     3670 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme6.dat
--rwxr-xr-x   0        0        0      639 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif_files.py
--rw-r--r--   0        0        0     1455 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/wing.dat
--rw-r--r--   0        0        0       70 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/__init__.py
--rw-r--r--   0        0        0    20036 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/component_queries.py
--rw-r--r--   0        0        0     2523 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/connectivity_queries.py
--rw-r--r--   0        0        0     2973 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/core.py
--rw-r--r--   0        0        0     5878 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/geometry_queries.py
--rw-r--r--   0        0        0     4495 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/inline_functions.py
--rw-r--r--   0        0        0     7220 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/line_queries.py
--rw-r--r--   0        0        0     3021 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/nearest_queries.py
--rw-r--r--   0        0        0     7010 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/normals_queries.py
--rw-r--r--   0        0        0     4285 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/scalar_queries.py
--rw-r--r--   0        0        0    16111 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/selection_queries.py
--rw-r--r--   0        0        0     3999 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/jupyter.py
--rw-r--r--   0        0        0    25522 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/krylov.py
--rw-r--r--   0        0        0    61926 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/launcher.py
--rw-r--r--   0        0        0    17789 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/licensing.py
--rw-r--r--   0        0        0    20215 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/logging.py
--rw-r--r--   0        0        0   149074 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl.py
--rw-r--r--   0        0        0     7620 2023-06-02 09:30:43.399173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_console.py
--rw-r--r--   0        0        0    13258 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_corba.py
--rw-r--r--   0        0        0    28656 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_geometry.py
--rw-r--r--   0        0        0   107281 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_grpc.py
--rw-r--r--   0        0        0      258 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_types.py
--rwxr-xr-x   0        0        0    61110 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/math.py
--rw-r--r--   0        0        0        0 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh/__init__.py
--rw-r--r--   0        0        0     7707 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh/mesh.py
--rw-r--r--   0        0        0    24709 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh_grpc.py
--rw-r--r--   0        0        0    39484 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/misc.py
--rw-r--r--   0        0        0    24772 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/parameters.py
--rw-r--r--   0        0        0    37509 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/plotting.py
--rwxr-xr-x   0        0        0    20586 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/pool.py
--rw-r--r--   0        0        0   130584 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/post.py
--rw-r--r--   0        0        0     8039 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/solution.py
--rw-r--r--   0        0        0     1267 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/theme.py
--rw-r--r--   0        0        0    16086 2023-06-02 09:30:43.403173 ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/xpl.py
--rw-r--r--   0        0        0    14064 1970-01-01 00:00:00.000000 ansys_mapdl_core-0.65.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-28 07:27:27.647816 ansys_mapdl_core-0.65.1/LICENSE
+-rw-r--r--   0        0        0    10472 2023-07-28 07:27:27.647816 ansys_mapdl_core-0.65.1/README.rst
+-rw-r--r--   0        0        0     4714 2023-07-28 07:27:27.855819 ansys_mapdl_core-0.65.1/pyproject.toml
+-rw-r--r--   0        0        0     2341 2023-07-28 07:27:27.855819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 07:27:27.855819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/__init__.py
+-rw-r--r--   0        0        0      134 2023-07-28 07:27:27.855819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/__init__.py
+-rw-r--r--   0        0        0     7083 2023-07-28 07:27:27.855819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/abbreviations.py
+-rw-r--r--   0        0        0    65022 2023-07-28 07:27:27.855819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/array_param.py
+-rw-r--r--   0        0        0    24293 2023-07-28 07:27:27.855819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/macro_files.py
+-rw-r--r--   0        0        0    33278 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/matrix_op.py
+-rw-r--r--   0        0        0    49087 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/parameter_definition.py
+-rw-r--r--   0        0        0      877 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/process_controls.py
+-rw-r--r--   0        0        0       65 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux12_/__init__.py
+-rw-r--r--   0        0        0     1800 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux12_/general_radiation.py
+-rw-r--r--   0        0        0     4381 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux12_/radiation_mat.py
+-rw-r--r--   0        0        0    15390 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux12_/radiosity_solver.py
+-rw-r--r--   0        0        0     5782 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux15_.py
+-rw-r--r--   0        0        0       34 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux2_/__init__.py
+-rw-r--r--   0        0        0     2783 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux2_/bin_dump.py
+-rw-r--r--   0        0        0    13843 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux2_/bin_manip.py
+-rw-r--r--   0        0        0     4949 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux3_.py
+-rw-r--r--   0        0        0    11323 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/conn.py
+-rw-r--r--   0        0        0       78 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/__init__.py
+-rw-r--r--   0        0        0    22459 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/components.py
+-rw-r--r--   0        0        0    17248 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/coord_sys.py
+-rw-r--r--   0        0        0     4715 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/picking.py
+-rw-r--r--   0        0        0    53650 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/selecting.py
+-rw-r--r--   0        0        0    13775 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/setup.py
+-rw-r--r--   0        0        0    16923 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/working_plane.py
+-rw-r--r--   0        0        0       20 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/display_/__init__.py
+-rw-r--r--   0        0        0     9516 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/display_/setup.py
+-rw-r--r--   0        0        0       73 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/__init__.py
+-rw-r--r--   0        0        0    21774 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/annotation.py
+-rw-r--r--   0        0        0    11407 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/graphs.py
+-rw-r--r--   0        0        0    42963 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/labeling.py
+-rw-r--r--   0        0        0    10248 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/scaling.py
+-rw-r--r--   0        0        0    53850 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/setup.py
+-rw-r--r--   0        0        0    22511 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/style.py
+-rw-r--r--   0        0        0    18352 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/views.py
+-rw-r--r--   0        0        0     3162 2023-07-28 07:27:27.859819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/hidden.py
+-rw-r--r--   0        0        0    50786 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/inq_func.py
+-rw-r--r--   0        0        0    10067 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/map_cmd.py
+-rw-r--r--   0        0        0       19 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/misc/__init__.py
+-rw-r--r--   0        0        0      992 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/misc/misc.py
+-rw-r--r--   0        0        0     2975 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/parse.py
+-rw-r--r--   0        0        0      248 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/__init__.py
+-rw-r--r--   0        0        0    26912 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/animation.py
+-rw-r--r--   0        0        0    21848 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/controls.py
+-rw-r--r--   0        0        0    31418 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/element_table.py
+-rw-r--r--   0        0        0     7015 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/failure_criteria.py
+-rw-r--r--   0        0        0    11070 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/listing.py
+-rw-r--r--   0        0        0    15600 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/load_case.py
+-rw-r--r--   0        0        0    11457 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/magnetics_calc.py
+-rw-r--r--   0        0        0    36235 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/path_operations.py
+-rw-r--r--   0        0        0    38181 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/results.py
+-rw-r--r--   0        0        0    32317 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/setup.py
+-rw-r--r--   0        0        0    96414 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/special.py
+-rw-r--r--   0        0        0     4431 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/status.py
+-rw-r--r--   0        0        0    16032 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/surface_operations.py
+-rw-r--r--   0        0        0     8201 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/trace_points.py
+-rw-r--r--   0        0        0       77 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/__init__.py
+-rw-r--r--   0        0        0     9792 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/controls.py
+-rw-r--r--   0        0        0     5716 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/display.py
+-rw-r--r--   0        0        0     4351 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/listing.py
+-rw-r--r--   0        0        0    22683 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/operations.py
+-rw-r--r--   0        0        0    33525 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/setup.py
+-rw-r--r--   0        0        0    20246 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/special.py
+-rw-r--r--   0        0        0     2904 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/status.py
+-rw-r--r--   0        0        0      441 2023-07-28 07:27:27.863819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/__init__.py
+-rw-r--r--   0        0        0    42817 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/areas.py
+-rw-r--r--   0        0        0     4341 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/artificially_matched_layers.py
+-rw-r--r--   0        0        0    62005 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/booleans.py
+-rw-r--r--   0        0        0    22650 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/constraint_equations.py
+-rw-r--r--   0        0        0    15817 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/coupled_dof.py
+-rw-r--r--   0        0        0    38580 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/database.py
+-rw-r--r--   0        0        0     4096 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/digitizing.py
+-rw-r--r--   0        0        0    16260 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/element_type.py
+-rw-r--r--   0        0        0   102587 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/elements.py
+-rw-r--r--   0        0        0   158286 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/explicit_dynamics.py
+-rw-r--r--   0        0        0     3745 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/hard_points.py
+-rw-r--r--   0        0        0    32528 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/keypoints.py
+-rw-r--r--   0        0        0    52765 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/lines.py
+-rw-r--r--   0        0        0    26805 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/material_data_tables.py
+-rw-r--r--   0        0        0    38458 2023-07-28 07:27:27.867819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/materials.py
+-rw-r--r--   0        0        0   136306 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/meshing.py
+-rw-r--r--   0        0        0    12362 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/morphing.py
+-rw-r--r--   0        0        0    43541 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/nodes.py
+-rw-r--r--   0        0        0    35522 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/primitives.py
+-rw-r--r--   0        0        0     9440 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/real_constants.py
+-rw-r--r--   0        0        0    59811 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/sections.py
+-rw-r--r--   0        0        0    43269 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/special_purpose.py
+-rw-r--r--   0        0        0    15604 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/status.py
+-rw-r--r--   0        0        0     9685 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/superelements.py
+-rw-r--r--   0        0        0    44600 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/volumes.py
+-rw-r--r--   0        0        0       55 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/__init__.py
+-rw-r--r--   0        0        0    15305 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/generation.py
+-rw-r--r--   0        0        0     3067 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/preparation.py
+-rw-r--r--   0        0        0     1154 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/setup.py
+-rw-r--r--   0        0        0     4692 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/use_pass.py
+-rw-r--r--   0        0        0       66 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/__init__.py
+-rw-r--r--   0        0        0    26143 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/files.py
+-rw-r--r--   0        0        0     3481 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/list_controls.py
+-rw-r--r--   0        0        0     5122 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/processor_entry.py
+-rw-r--r--   0        0        0    25874 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/run_controls.py
+-rw-r--r--   0        0        0      763 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/all_others.py
+-rw-r--r--   0        0        0   157108 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/analysis_options.py
+-rw-r--r--   0        0        0     3320 2023-07-28 07:27:27.871819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/birth_and_death.py
+-rw-r--r--   0        0        0    56005 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/dynamic_options.py
+-rw-r--r--   0        0        0    34700 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/fe_body_loads.py
+-rw-r--r--   0        0        0    29784 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/fe_constraints.py
+-rw-r--r--   0        0        0    15694 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/fe_forces.py
+-rw-r--r--   0        0        0    23544 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/fe_surface_loads.py
+-rw-r--r--   0        0        0     8378 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/gap_conditions.py
+-rw-r--r--   0        0        0    33877 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/inertia.py
+-rw-r--r--   0        0        0     8882 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/load_step_operations.py
+-rw-r--r--   0        0        0    36881 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/load_step_options.py
+-rw-r--r--   0        0        0     6753 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/master_dof.py
+-rw-r--r--   0        0        0    55158 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/miscellaneous_loads.py
+-rw-r--r--   0        0        0     4065 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_convergence_controls.py
+-rw-r--r--   0        0        0     6518 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_definition_commands.py
+-rw-r--r--   0        0        0    12413 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_global_controls.py
+-rw-r--r--   0        0        0     7669 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_interface_mapping.py
+-rw-r--r--   0        0        0     9429 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_load_transfer.py
+-rw-r--r--   0        0        0     7905 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_time_controls.py
+-rw-r--r--   0        0        0    58898 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/nonlinear_options.py
+-rw-r--r--   0        0        0    15629 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/ocean.py
+-rw-r--r--   0        0        0    10287 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/radiosity.py
+-rw-r--r--   0        0        0    12029 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/rezoning.py
+-rw-r--r--   0        0        0    18965 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solid_body_loads.py
+-rw-r--r--   0        0        0    18072 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solid_constraints.py
+-rw-r--r--   0        0        0     4405 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solid_forces.py
+-rw-r--r--   0        0        0    10519 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solid_surface_loads.py
+-rw-r--r--   0        0        0    12380 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solution_status.py
+-rw-r--r--   0        0        0    61309 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/spectrum_options.py
+-rw-r--r--   0        0        0     2435 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/twod_to_3d_analysis.py
+-rw-r--r--   0        0        0      720 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_version.py
+-rw-r--r--   0        0        0    24307 2023-07-28 07:27:27.875819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/commands.py
+-rw-r--r--   0        0        0     4583 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/common_grpc.py
+-rw-r--r--   0        0        0    36769 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/convert.py
+-rw-r--r--   0        0        0      209 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/database/__init__.py
+-rw-r--r--   0        0        0    14261 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/database/database.py
+-rw-r--r--   0        0        0    10848 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/database/elems.py
+-rw-r--r--   0        0        0    16557 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/database/nodes.py
+-rw-r--r--   0        0        0     4532 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/docs.py
+-rw-r--r--   0        0        0     5900 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/errors.py
+-rw-r--r--   0        0        0      171 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/__init__.py
+-rw-r--r--   0        0        0     5342 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/downloads.py
+-rw-r--r--   0        0        0     1001 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/examples.py
+-rwxr-xr-x   0        0        0     1294 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm1.dat
+-rwxr-xr-x   0        0        0     1143 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm10.dat
+-rwxr-xr-x   0        0        0     2429 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm100.dat
+-rwxr-xr-x   0        0        0     2341 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm101.dat
+-rwxr-xr-x   0        0        0     2354 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm102.dat
+-rwxr-xr-x   0        0        0     3467 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm103.dat
+-rwxr-xr-x   0        0        0     2193 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm104.dat
+-rwxr-xr-x   0        0        0     1941 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm105.dat
+-rwxr-xr-x   0        0        0     1165 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm106.dat
+-rwxr-xr-x   0        0        0     1374 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm107.dat
+-rwxr-xr-x   0        0        0     1365 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm108.dat
+-rwxr-xr-x   0        0        0     1713 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm109.dat
+-rwxr-xr-x   0        0        0     1782 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm11.dat
+-rwxr-xr-x   0        0        0     2110 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm110.dat
+-rwxr-xr-x   0        0        0     1533 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm111.dat
+-rwxr-xr-x   0        0        0     1662 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm112.dat
+-rwxr-xr-x   0        0        0     1913 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm113.dat
+-rwxr-xr-x   0        0        0     2232 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm114.dat
+-rwxr-xr-x   0        0        0     1740 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm115.dat
+-rwxr-xr-x   0        0        0     2338 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm116.dat
+-rwxr-xr-x   0        0        0     4303 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm117.dat
+-rwxr-xr-x   0        0        0     3349 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm118.dat
+-rwxr-xr-x   0        0        0     4277 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm119.dat
+-rwxr-xr-x   0        0        0     2152 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm12.dat
+-rwxr-xr-x   0        0        0     2354 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm120.dat
+-rwxr-xr-x   0        0        0     5119 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm121.dat
+-rwxr-xr-x   0        0        0     1164 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm122.dat
+-rwxr-xr-x   0        0        0     1278 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm123.dat
+-rwxr-xr-x   0        0        0     1871 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm124.dat
+-rwxr-xr-x   0        0        0     2200 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm125.dat
+-rwxr-xr-x   0        0        0     2246 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm126.dat
+-rwxr-xr-x   0        0        0     2732 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm127.dat
+-rwxr-xr-x   0        0        0     1620 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm128.dat
+-rwxr-xr-x   0        0        0     2150 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm129.dat
+-rwxr-xr-x   0        0        0     1311 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm13.dat
+-rwxr-xr-x   0        0        0     2688 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm130.dat
+-rwxr-xr-x   0        0        0     1323 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm131.dat
+-rwxr-xr-x   0        0        0     1862 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm132.dat
+-rwxr-xr-x   0        0        0     1926 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm133.dat
+-rwxr-xr-x   0        0        0     4300 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm134.dat
+-rwxr-xr-x   0        0        0     1292 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm135.dat
+-rwxr-xr-x   0        0        0     4141 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm136.dat
+-rwxr-xr-x   0        0        0     1613 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm137.dat
+-rwxr-xr-x   0        0        0     1213 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm138.dat
+-rwxr-xr-x   0        0        0     5140 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm139.dat
+-rwxr-xr-x   0        0        0     1373 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm14.dat
+-rwxr-xr-x   0        0        0     2090 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm140.dat
+-rwxr-xr-x   0        0        0     9580 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm141.dat
+-rwxr-xr-x   0        0        0     3499 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm142.dat
+-rwxr-xr-x   0        0        0    14726 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm143.dat
+-rwxr-xr-x   0        0        0     7109 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm144.dat
+-rwxr-xr-x   0        0        0     1604 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm145.dat
+-rwxr-xr-x   0        0        0     2719 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm146.dat
+-rwxr-xr-x   0        0        0     2211 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm147.dat
+-rwxr-xr-x   0        0        0     2434 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm148.dat
+-rwxr-xr-x   0        0        0     9444 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm149.dat
+-rwxr-xr-x   0        0        0     3253 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm15.dat
+-rwxr-xr-x   0        0        0     3079 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm150.dat
+-rwxr-xr-x   0        0        0     1851 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm151.dat
+-rwxr-xr-x   0        0        0     2218 2023-07-28 07:27:27.879819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm152.dat
+-rwxr-xr-x   0        0        0     3525 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm153.dat
+-rwxr-xr-x   0        0        0     1304 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm154.dat
+-rwxr-xr-x   0        0        0     2623 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm155.dat
+-rwxr-xr-x   0        0        0     2111 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm156.dat
+-rwxr-xr-x   0        0        0     2361 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm157.dat
+-rwxr-xr-x   0        0        0     1738 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm158.dat
+-rwxr-xr-x   0        0        0     1782 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm159.dat
+-rwxr-xr-x   0        0        0     3798 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm16.dat
+-rwxr-xr-x   0        0        0     1996 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm160.dat
+-rwxr-xr-x   0        0        0     1330 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm161.dat
+-rwxr-xr-x   0        0        0     1296 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm162.dat
+-rwxr-xr-x   0        0        0     1864 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm163.dat
+-rwxr-xr-x   0        0        0     1334 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm164.dat
+-rwxr-xr-x   0        0        0     2675 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm165.dat
+-rwxr-xr-x   0        0        0     5313 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm166.dat
+-rwxr-xr-x   0        0        0     6989 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm167.dat
+-rwxr-xr-x   0        0        0     3254 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm168.dat
+-rwxr-xr-x   0        0        0     3067 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm169.dat
+-rwxr-xr-x   0        0        0     4418 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm17.dat
+-rwxr-xr-x   0        0        0     1871 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm170.dat
+-rwxr-xr-x   0        0        0     6145 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm171.dat
+-rwxr-xr-x   0        0        0     3494 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm172.dat
+-rwxr-xr-x   0        0        0     2335 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm173.dat
+-rwxr-xr-x   0        0        0     3230 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm174.dat
+-rwxr-xr-x   0        0        0     7199 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm175.dat
+-rwxr-xr-x   0        0        0    10669 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm176.dat
+-rwxr-xr-x   0        0        0    13041 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm177.dat
+-rwxr-xr-x   0        0        0     2406 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm178.dat
+-rwxr-xr-x   0        0        0     3603 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm179.dat
+-rwxr-xr-x   0        0        0     2570 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm18.dat
+-rwxr-xr-x   0        0        0     1741 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm180.dat
+-rwxr-xr-x   0        0        0     1315 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm181.dat
+-rwxr-xr-x   0        0        0     2478 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm182.dat
+-rwxr-xr-x   0        0        0     2117 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm183.dat
+-rwxr-xr-x   0        0        0     8768 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm184.dat
+-rwxr-xr-x   0        0        0     7867 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm185.dat
+-rwxr-xr-x   0        0        0     7761 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm186.dat
+-rwxr-xr-x   0        0        0     4075 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm187.dat
+-rwxr-xr-x   0        0        0     3640 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm188.dat
+-rwxr-xr-x   0        0        0     2788 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm189.dat
+-rwxr-xr-x   0        0        0     2363 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm19.dat
+-rwxr-xr-x   0        0        0     4207 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm190.dat
+-rwxr-xr-x   0        0        0     8521 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm191.dat
+-rwxr-xr-x   0        0        0     1997 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm192.dat
+-rwxr-xr-x   0        0        0    19768 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm193.dat
+-rwxr-xr-x   0        0        0     1806 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm194.dat
+-rwxr-xr-x   0        0        0     2059 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm195.dat
+-rwxr-xr-x   0        0        0     4882 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm196.dat
+-rwxr-xr-x   0        0        0    10456 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm197.dat
+-rwxr-xr-x   0        0        0    11449 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm198.dat
+-rwxr-xr-x   0        0        0    16406 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm199.dat
+-rwxr-xr-x   0        0        0     1628 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm2.dat
+-rwxr-xr-x   0        0        0     1695 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm20.dat
+-rwxr-xr-x   0        0        0     5739 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm200.dat
+-rwxr-xr-x   0        0        0     6398 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm201.dat
+-rwxr-xr-x   0        0        0     2541 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm202.dat
+-rwxr-xr-x   0        0        0     2650 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm203.dat
+-rwxr-xr-x   0        0        0     3666 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm204.dat
+-rwxr-xr-x   0        0        0     4965 2023-07-28 07:27:27.883819 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm205.dat
+-rwxr-xr-x   0        0        0     2601 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm206.dat
+-rwxr-xr-x   0        0        0     3280 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm207.dat
+-rwxr-xr-x   0        0        0     1940 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm208.dat
+-rwxr-xr-x   0        0        0    12271 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm209.dat
+-rwxr-xr-x   0        0        0     2721 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm21.dat
+-rwxr-xr-x   0        0        0     9391 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm210.dat
+-rwxr-xr-x   0        0        0    10266 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm211.dat
+-rwxr-xr-x   0        0        0     6116 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm212.dat
+-rwxr-xr-x   0        0        0     7793 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm213.dat
+-rwxr-xr-x   0        0        0     2080 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm214.dat
+-rwxr-xr-x   0        0        0     1755 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm215.dat
+-rwxr-xr-x   0        0        0     2988 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm216.dat
+-rwxr-xr-x   0        0        0     2041 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm217.dat
+-rwxr-xr-x   0        0        0    11642 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm218.dat
+-rwxr-xr-x   0        0        0     3857 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm219.dat
+-rwxr-xr-x   0        0        0     1133 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm22.dat
+-rwxr-xr-x   0        0        0     5191 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm220.dat
+-rwxr-xr-x   0        0        0     2040 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm221.dat
+-rwxr-xr-x   0        0        0     2660 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm222.dat
+-rwxr-xr-x   0        0        0     5776 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm223.dat
+-rwxr-xr-x   0        0        0     3557 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm224.dat
+-rwxr-xr-x   0        0        0     3076 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm225.dat
+-rwxr-xr-x   0        0        0     3045 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm226.dat
+-rwxr-xr-x   0        0        0     2644 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm227.dat
+-rwxr-xr-x   0        0        0     6215 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm228.dat
+-rwxr-xr-x   0        0        0     6354 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm229.dat
+-rwxr-xr-x   0        0        0     6500 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm23.dat
+-rwxr-xr-x   0        0        0    13140 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm230.dat
+-rwxr-xr-x   0        0        0     7508 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm231.dat
+-rwxr-xr-x   0        0        0    12245 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm232.dat
+-rwxr-xr-x   0        0        0     3641 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm233.dat
+-rwxr-xr-x   0        0        0     2512 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm234.dat
+-rwxr-xr-x   0        0        0     3682 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm235.dat
+-rwxr-xr-x   0        0        0     5976 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm236.dat
+-rwxr-xr-x   0        0        0     6546 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm237.dat
+-rwxr-xr-x   0        0        0     3577 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm238.dat
+-rwxr-xr-x   0        0        0     7798 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm239.dat
+-rwxr-xr-x   0        0        0     1321 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm24.dat
+-rwxr-xr-x   0        0        0     2365 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm240.dat
+-rwxr-xr-x   0        0        0     8657 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm241.dat
+-rwxr-xr-x   0        0        0     3161 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm242.dat
+-rwxr-xr-x   0        0        0     2539 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm243.dat
+-rwxr-xr-x   0        0        0     2902 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm244.dat
+-rwxr-xr-x   0        0        0     3393 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm245.dat
+-rwxr-xr-x   0        0        0     6795 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm246.dat
+-rwxr-xr-x   0        0        0     7914 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm247.dat
+-rwxr-xr-x   0        0        0    21905 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm248.dat
+-rwxr-xr-x   0        0        0     7788 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm249.dat
+-rwxr-xr-x   0        0        0     3963 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm25.dat
+-rwxr-xr-x   0        0        0     7596 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm250.dat
+-rwxr-xr-x   0        0        0     8087 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm251.dat
+-rwxr-xr-x   0        0        0     4136 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm252.dat
+-rwxr-xr-x   0        0        0     3729 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm253.dat
+-rwxr-xr-x   0        0        0     8515 2023-07-28 07:27:27.887820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm254.dat
+-rwxr-xr-x   0        0        0     4234 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm255.dat
+-rwxr-xr-x   0        0        0    13336 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm256.dat
+-rwxr-xr-x   0        0        0     8703 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm257.dat
+-rwxr-xr-x   0        0        0     7160 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm258.dat
+-rwxr-xr-x   0        0        0    20687 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm259.dat
+-rwxr-xr-x   0        0        0     5148 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm26.dat
+-rwxr-xr-x   0        0        0     8199 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm260.dat
+-rwxr-xr-x   0        0        0     5024 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm261.dat
+-rwxr-xr-x   0        0        0     3065 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm262.dat
+-rwxr-xr-x   0        0        0    26501 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm263.dat
+-rwxr-xr-x   0        0        0     7906 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm264.dat
+-rwxr-xr-x   0        0        0     5972 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm265.dat
+-rwxr-xr-x   0        0        0    10185 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm266.dat
+-rwxr-xr-x   0        0        0     5657 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm267.dat
+-rwxr-xr-x   0        0        0     3299 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm268.dat
+-rwxr-xr-x   0        0        0     2805 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm269.dat
+-rwxr-xr-x   0        0        0     1755 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm27.dat
+-rwxr-xr-x   0        0        0     4557 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm270.dat
+-rwxr-xr-x   0        0        0    15604 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm271.dat
+-rwxr-xr-x   0        0        0    20113 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm272.dat
+-rwxr-xr-x   0        0        0     5455 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm273.dat
+-rwxr-xr-x   0        0        0     3861 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm274.dat
+-rwxr-xr-x   0        0        0     8112 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm275.dat
+-rwxr-xr-x   0        0        0     3493 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm276.dat
+-rwxr-xr-x   0        0        0     2927 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm277.dat
+-rwxr-xr-x   0        0        0     3941 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm278.dat
+-rwxr-xr-x   0        0        0     8873 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm279.dat
+-rwxr-xr-x   0        0        0     2146 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm28.dat
+-rwxr-xr-x   0        0        0     5670 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm280.dat
+-rwxr-xr-x   0        0        0    11199 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm281.dat
+-rwxr-xr-x   0        0        0     5507 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm282.dat
+-rwxr-xr-x   0        0        0     4643 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm283.dat
+-rw-r--r--   0        0        0     8968 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm284.dat
+-rw-r--r--   0        0        0     3246 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm285.dat
+-rw-r--r--   0        0        0     6386 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm286.dat
+-rw-r--r--   0        0        0     4820 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm287.dat
+-rw-r--r--   0        0        0     6538 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm288.dat
+-rw-r--r--   0        0        0     4181 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm289.dat
+-rwxr-xr-x   0        0        0     4831 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm29.dat
+-rw-r--r--   0        0        0     3166 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm290.dat
+-rw-r--r--   0        0        0    10932 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm291.dat
+-rw-r--r--   0        0        0     3336 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm292.dat
+-rw-r--r--   0        0        0     4870 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm293.dat
+-rw-r--r--   0        0        0     9804 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm294.dat
+-rw-r--r--   0        0        0     4039 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm295.dat
+-rw-r--r--   0        0        0    13015 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm296.dat
+-rw-r--r--   0        0        0     3945 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm297.dat
+-rw-r--r--   0        0        0     7921 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm298.dat
+-rw-r--r--   0        0        0     2525 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm299.dat
+-rwxr-xr-x   0        0        0     1686 2023-07-28 07:27:27.891820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm3.dat
+-rwxr-xr-x   0        0        0     2541 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm30.dat
+-rw-r--r--   0        0        0     2728 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm300.dat
+-rw-r--r--   0        0        0     3680 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm301.dat
+-rw-r--r--   0        0        0    14358 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm302.dat
+-rw-r--r--   0        0        0     7826 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm303.dat
+-rw-r--r--   0        0        0     3600 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm304.dat
+-rw-r--r--   0        0        0     2644 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm305.dat
+-rw-r--r--   0        0        0     2156 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm306.dat
+-rw-r--r--   0        0        0     1561 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm307.dat
+-rw-r--r--   0        0        0     3832 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm308.dat
+-rw-r--r--   0        0        0     2255 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm309.dat
+-rwxr-xr-x   0        0        0     3036 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm31.dat
+-rw-r--r--   0        0        0     7310 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm310.dat
+-rw-r--r--   0        0        0     8882 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm311.dat
+-rw-r--r--   0        0        0     8654 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm312.dat
+-rw-r--r--   0        0        0     4303 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm313.dat
+-rw-r--r--   0        0        0     2738 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm314.dat
+-rw-r--r--   0        0        0     4253 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm315.dat
+-rw-r--r--   0        0        0     9789 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm316.dat
+-rw-r--r--   0        0        0     6697 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm317.dat
+-rw-r--r--   0        0        0     3273 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm318.dat
+-rwxr-xr-x   0        0        0     2889 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm32.dat
+-rwxr-xr-x   0        0        0     5950 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm33.dat
+-rwxr-xr-x   0        0        0     6416 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm34.dat
+-rwxr-xr-x   0        0        0     2157 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm35.dat
+-rwxr-xr-x   0        0        0     4291 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm36.dat
+-rwxr-xr-x   0        0        0     3955 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm37.dat
+-rwxr-xr-x   0        0        0     4674 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm38.dat
+-rwxr-xr-x   0        0        0     5136 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm39.dat
+-rwxr-xr-x   0        0        0     1464 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm4.dat
+-rwxr-xr-x   0        0        0     2954 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm40.dat
+-rwxr-xr-x   0        0        0     5122 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm41.dat
+-rwxr-xr-x   0        0        0     3012 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm42.dat
+-rwxr-xr-x   0        0        0     2779 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm43.dat
+-rwxr-xr-x   0        0        0     2891 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm44.dat
+-rwxr-xr-x   0        0        0     1052 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm45.dat
+-rwxr-xr-x   0        0        0     3393 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm46.dat
+-rwxr-xr-x   0        0        0     1498 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm47.dat
+-rwxr-xr-x   0        0        0     1543 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm48.dat
+-rwxr-xr-x   0        0        0     3279 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm49.dat
+-rwxr-xr-x   0        0        0     2882 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm5.dat
+-rwxr-xr-x   0        0        0     1463 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm50.dat
+-rwxr-xr-x   0        0        0    13711 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm51.dat
+-rwxr-xr-x   0        0        0     1871 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm52.dat
+-rwxr-xr-x   0        0        0     2275 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm53.dat
+-rwxr-xr-x   0        0        0     5974 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm54.dat
+-rwxr-xr-x   0        0        0     1747 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm55.dat
+-rwxr-xr-x   0        0        0     5942 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm56.dat
+-rwxr-xr-x   0        0        0     5808 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm57.dat
+-rwxr-xr-x   0        0        0     1876 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm58.dat
+-rwxr-xr-x   0        0        0     2136 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm59.dat
+-rwxr-xr-x   0        0        0     2369 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm6.dat
+-rwxr-xr-x   0        0        0     1679 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm60.dat
+-rwxr-xr-x   0        0        0     1312 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm61.dat
+-rwxr-xr-x   0        0        0     4605 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm62.dat
+-rwxr-xr-x   0        0        0     3642 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm63.dat
+-rwxr-xr-x   0        0        0     1708 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm64.dat
+-rwxr-xr-x   0        0        0     3090 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm65.dat
+-rwxr-xr-x   0        0        0     4459 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm66.dat
+-rwxr-xr-x   0        0        0     1560 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm67.dat
+-rwxr-xr-x   0        0        0     2510 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm68.dat
+-rwxr-xr-x   0        0        0     1823 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm69.dat
+-rwxr-xr-x   0        0        0     6368 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm7.dat
+-rwxr-xr-x   0        0        0     2172 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm70.dat
+-rwxr-xr-x   0        0        0     2366 2023-07-28 07:27:27.895820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm71.dat
+-rwxr-xr-x   0        0        0     2805 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm72.dat
+-rwxr-xr-x   0        0        0     2047 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm73.dat
+-rwxr-xr-x   0        0        0     2647 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm74.dat
+-rwxr-xr-x   0        0        0     2391 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm75.dat
+-rwxr-xr-x   0        0        0     2401 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm76.dat
+-rwxr-xr-x   0        0        0     2703 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm77.dat
+-rwxr-xr-x   0        0        0     2157 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm78.dat
+-rwxr-xr-x   0        0        0     2369 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm79.dat
+-rwxr-xr-x   0        0        0     3521 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm8.dat
+-rwxr-xr-x   0        0        0     2436 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm80.dat
+-rwxr-xr-x   0        0        0     4016 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm81.dat
+-rwxr-xr-x   0        0        0    10303 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm82.dat
+-rwxr-xr-x   0        0        0     2368 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm83.dat
+-rwxr-xr-x   0        0        0     2250 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm84.dat
+-rwxr-xr-x   0        0        0     2867 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm85.dat
+-rwxr-xr-x   0        0        0     1441 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm86.dat
+-rwxr-xr-x   0        0        0     1568 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm87.dat
+-rwxr-xr-x   0        0        0     1627 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm88.dat
+-rwxr-xr-x   0        0        0     2123 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm89.dat
+-rwxr-xr-x   0        0        0     2471 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm9.dat
+-rwxr-xr-x   0        0        0     2604 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm90.dat
+-rwxr-xr-x   0        0        0     2837 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm91.dat
+-rwxr-xr-x   0        0        0     1402 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm92.dat
+-rwxr-xr-x   0        0        0     1115 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm93.dat
+-rwxr-xr-x   0        0        0     1549 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm94.dat
+-rwxr-xr-x   0        0        0     3501 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm95.dat
+-rwxr-xr-x   0        0        0     3033 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm96.dat
+-rwxr-xr-x   0        0        0     2585 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm97.dat
+-rwxr-xr-x   0        0        0     2041 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm98.dat
+-rwxr-xr-x   0        0        0     1614 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm99.dat
+-rwxr-xr-x   0        0        0    11868 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc1.dat
+-rwxr-xr-x   0        0        0     9617 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc2.dat
+-rwxr-xr-x   0        0        0     4766 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc3.dat
+-rwxr-xr-x   0        0        0     6787 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc4.dat
+-rwxr-xr-x   0        0        0     5775 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc5.dat
+-rwxr-xr-x   0        0        0     6120 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc6.dat
+-rwxr-xr-x   0        0        0     4152 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc7.dat
+-rwxr-xr-x   0        0        0     4320 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc8.dat
+-rwxr-xr-x   0        0        0    11304 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmd1.dat
+-rwxr-xr-x   0        0        0     4372 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmd2.dat
+-rwxr-xr-x   0        0        0    11914 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmd3.dat
+-rwxr-xr-x   0        0        0     2600 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme1.dat
+-rwxr-xr-x   0        0        0     1771 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme2.dat
+-rwxr-xr-x   0        0        0     3360 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme3.dat
+-rwxr-xr-x   0        0        0     3447 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme4.dat
+-rwxr-xr-x   0        0        0     2452 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme5.dat
+-rwxr-xr-x   0        0        0     3670 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme6.dat
+-rwxr-xr-x   0        0        0      639 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif_files.py
+-rw-r--r--   0        0        0     1455 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/wing.dat
+-rw-r--r--   0        0        0       70 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/__init__.py
+-rw-r--r--   0        0        0    20036 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/component_queries.py
+-rw-r--r--   0        0        0     2523 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/connectivity_queries.py
+-rw-r--r--   0        0        0     2973 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/core.py
+-rw-r--r--   0        0        0     5878 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/geometry_queries.py
+-rw-r--r--   0        0        0     4495 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/inline_functions.py
+-rw-r--r--   0        0        0     7220 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/line_queries.py
+-rw-r--r--   0        0        0     3021 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/nearest_queries.py
+-rw-r--r--   0        0        0     7010 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/normals_queries.py
+-rw-r--r--   0        0        0     4285 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/scalar_queries.py
+-rw-r--r--   0        0        0    16111 2023-07-28 07:27:27.899820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/selection_queries.py
+-rw-r--r--   0        0        0     3999 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/jupyter.py
+-rw-r--r--   0        0        0    25522 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/krylov.py
+-rw-r--r--   0        0        0    61926 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/launcher.py
+-rw-r--r--   0        0        0    17789 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/licensing.py
+-rw-r--r--   0        0        0    20215 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/logging.py
+-rw-r--r--   0        0        0   149074 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl.py
+-rw-r--r--   0        0        0     7620 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_console.py
+-rw-r--r--   0        0        0    13258 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_corba.py
+-rw-r--r--   0        0        0    28656 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_geometry.py
+-rw-r--r--   0        0        0   107281 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_grpc.py
+-rw-r--r--   0        0        0      258 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_types.py
+-rwxr-xr-x   0        0        0    61110 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/math.py
+-rw-r--r--   0        0        0        0 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mesh/__init__.py
+-rw-r--r--   0        0        0     7707 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mesh/mesh.py
+-rw-r--r--   0        0        0    24709 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mesh_grpc.py
+-rw-r--r--   0        0        0    39484 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/misc.py
+-rw-r--r--   0        0        0    24772 2023-07-28 07:27:27.903820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/parameters.py
+-rw-r--r--   0        0        0    37509 2023-07-28 07:27:27.907820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/plotting.py
+-rwxr-xr-x   0        0        0    20586 2023-07-28 07:27:27.907820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/pool.py
+-rw-r--r--   0        0        0   130584 2023-07-28 07:27:27.907820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/post.py
+-rw-r--r--   0        0        0     8039 2023-07-28 07:27:27.907820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/solution.py
+-rw-r--r--   0        0        0     1267 2023-07-28 07:27:27.907820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/theme.py
+-rw-r--r--   0        0        0    16086 2023-07-28 07:27:27.907820 ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/xpl.py
+-rw-r--r--   0        0        0    14162 1970-01-01 00:00:00.000000 ansys_mapdl_core-0.65.1/PKG-INFO
```

### Comparing `ansys_mapdl_core-0.65.0/LICENSE` & `ansys_mapdl_core-0.65.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/README.rst` & `ansys_mapdl_core-0.65.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/pyproject.toml` & `ansys_mapdl_core-0.65.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-mapdl-core"
-version = "0.65.0"
+version = "0.65.1"
 description = "A Python wrapper for Ansys MAPDL."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ansys, Inc.", email = "pyansys.maintainers@ansys.com"},
 ]
@@ -22,22 +22,23 @@
     "ansys-mapdl-reader>=0.51.7",
     "ansys-platform-instancemanagement~=1.0",
     "appdirs>=1.4.0",
     "click>=8.1.3", # for CLI interface
     "grpcio>=1.30.0",  # tested up to grpcio==1.35
     "importlib-metadata>=4.0",
     "matplotlib>=3.0.0",  # for colormaps for pyvista
-    "numpy>=1.14.0",
+    "numpy>=1.14.0,<1.25.0; python_version < '3.9'",
+    "numpy>=1.14.0; python_version >= '3.9'",
     "pexpect>=4.8.0 ; platform_system=='Linux'",
     "protobuf>=3.12.2",  # minimum required based on latest ansys-grpc-mapdl
     "psutil>=5.9.4",
     "pyansys-tools-versioning>=0.3.3",
     "ansys-tools-path>=0.2.4",
-    "pyiges>=0.1.4",
-    "pyvista>=0.33.0",
+    "pyiges[full]>=0.3.1", # Since v0.3.0, the 'full' flag is needed in order to install 'geomdl'
+    "pyvista>=0.33.0,<0.41",
     "scipy>=1.3.0",  # for sparse (consider optional?)
     "tqdm>=4.45.0",
     "vtk>=9.0.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
```

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/__init__.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/abbreviations.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/abbreviations.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/array_param.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/array_param.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/macro_files.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/macro_files.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/matrix_op.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/matrix_op.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/parameter_definition.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/apdl/process_controls.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/apdl/process_controls.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/general_radiation.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux12_/general_radiation.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/radiation_mat.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux12_/radiation_mat.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux12_/radiosity_solver.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux12_/radiosity_solver.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux15_.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux15_.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/bin_dump.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux2_/bin_dump.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux2_/bin_manip.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux2_/bin_manip.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/aux3_.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/aux3_.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/conn.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/conn.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/components.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/components.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/coord_sys.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/coord_sys.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/picking.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/picking.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/selecting.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/selecting.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/setup.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/database/working_plane.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/database/working_plane.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/display_/setup.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/display_/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/annotation.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/annotation.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/graphs.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/graphs.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/labeling.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/labeling.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/scaling.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/scaling.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/setup.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/style.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/style.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/graphics_/views.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/graphics_/views.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/hidden.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/hidden.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/inq_func.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/inq_func.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/map_cmd.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/map_cmd.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/misc/misc.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/misc/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/parse.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/parse.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/animation.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/animation.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/controls.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/controls.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/element_table.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/element_table.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/failure_criteria.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/failure_criteria.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/listing.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/listing.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/load_case.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/load_case.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/magnetics_calc.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/magnetics_calc.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/path_operations.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/path_operations.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/results.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/results.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/setup.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/special.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/special.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/status.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/status.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/surface_operations.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/surface_operations.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post1_/trace_points.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post1_/trace_points.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/controls.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/controls.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/display.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/display.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/listing.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/listing.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/operations.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/operations.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/setup.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/special.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/special.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/post26_/status.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/post26_/status.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/areas.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/areas.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/artificially_matched_layers.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/artificially_matched_layers.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/booleans.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/booleans.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/constraint_equations.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/constraint_equations.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/coupled_dof.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/coupled_dof.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/database.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/database.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/digitizing.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/digitizing.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/element_type.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/element_type.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/elements.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/elements.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/explicit_dynamics.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/explicit_dynamics.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/hard_points.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/hard_points.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/keypoints.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/keypoints.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/lines.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/lines.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/material_data_tables.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/material_data_tables.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/materials.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/materials.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/meshing.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/meshing.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/morphing.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/morphing.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/nodes.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/primitives.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/primitives.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/real_constants.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/real_constants.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/sections.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/sections.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/special_purpose.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/special_purpose.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/status.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/status.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/superelements.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/superelements.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/preproc/volumes.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/preproc/volumes.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/generation.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/generation.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/preparation.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/preparation.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/setup.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/reduced/use_pass.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/reduced/use_pass.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/files.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/files.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/list_controls.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/list_controls.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/processor_entry.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/processor_entry.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/session/run_controls.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/session/run_controls.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/__init__.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/analysis_options.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/analysis_options.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/birth_and_death.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/birth_and_death.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/dynamic_options.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/dynamic_options.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_body_loads.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/fe_body_loads.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_constraints.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/fe_constraints.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_forces.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/fe_forces.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/fe_surface_loads.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/fe_surface_loads.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/gap_conditions.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/gap_conditions.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/inertia.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/inertia.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/load_step_operations.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/load_step_operations.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/load_step_options.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/load_step_options.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/master_dof.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/master_dof.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/miscellaneous_loads.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/miscellaneous_loads.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_convergence_controls.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_convergence_controls.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_definition_commands.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_definition_commands.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_global_controls.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_global_controls.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_interface_mapping.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_interface_mapping.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_load_transfer.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_load_transfer.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/multi_field_solver_time_controls.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/multi_field_solver_time_controls.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/nonlinear_options.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/nonlinear_options.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/ocean.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/ocean.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/radiosity.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/radiosity.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/rezoning.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/rezoning.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_body_loads.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solid_body_loads.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_constraints.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solid_constraints.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_forces.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solid_forces.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solid_surface_loads.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solid_surface_loads.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/solution_status.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/solution_status.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/spectrum_options.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/spectrum_options.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_commands/solution/twod_to_3d_analysis.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_commands/solution/twod_to_3d_analysis.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/_version.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/_version.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/commands.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/commands.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/common_grpc.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/common_grpc.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/convert.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/convert.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/database.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/database/database.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/elems.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/database/elems.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/database/nodes.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/database/nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/docs.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/docs.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/errors.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/downloads.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/examples.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/examples.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm1.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm1.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm10.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm10.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm100.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm100.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm101.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm101.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm102.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm102.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm103.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm103.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm104.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm104.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm105.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm105.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm106.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm106.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm107.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm107.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm108.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm108.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm109.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm109.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm11.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm11.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm110.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm110.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm111.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm111.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm112.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm112.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm113.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm113.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm114.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm114.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm115.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm115.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm116.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm116.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm117.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm117.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm118.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm118.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm119.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm119.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm12.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm12.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm120.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm120.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm121.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm121.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm122.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm122.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm123.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm123.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm124.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm124.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm125.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm125.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm126.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm126.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm127.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm127.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm128.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm128.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm129.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm129.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm13.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm13.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm130.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm130.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm131.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm131.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm132.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm132.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm133.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm133.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm134.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm134.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm135.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm135.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm136.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm136.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm137.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm137.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm138.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm138.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm139.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm139.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm14.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm14.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm140.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm140.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm141.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm141.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm142.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm142.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm143.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm143.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm144.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm144.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm145.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm145.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm146.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm146.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm147.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm147.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm148.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm148.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm149.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm149.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm15.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm15.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm150.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm150.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm151.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm151.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm152.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm152.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm153.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm153.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm154.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm154.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm155.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm155.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm156.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm156.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm157.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm157.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm158.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm158.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm159.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm159.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm16.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm16.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm160.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm160.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm161.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm161.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm162.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm162.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm163.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm163.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm164.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm164.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm165.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm165.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm166.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm166.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm167.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm167.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm168.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm168.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm169.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm169.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm17.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm17.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm170.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm170.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm171.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm171.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm172.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm172.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm173.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm173.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm174.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm174.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm175.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm175.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm176.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm176.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm177.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm177.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm178.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm178.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm179.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm179.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm18.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm18.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm180.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm180.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm181.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm181.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm182.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm182.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm183.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm183.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm184.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm184.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm185.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm185.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm186.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm186.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm187.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm187.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm188.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm188.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm189.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm189.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm19.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm19.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm190.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm190.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm191.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm191.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm192.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm192.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm193.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm193.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm194.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm194.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm195.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm195.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm196.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm196.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm197.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm197.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm198.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm198.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm199.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm199.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm2.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm2.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm20.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm20.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm200.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm200.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm201.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm201.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm202.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm202.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm203.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm203.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm204.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm204.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm205.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm205.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm206.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm206.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm207.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm207.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm208.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm208.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm209.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm209.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm21.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm21.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm210.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm210.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm211.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm211.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm212.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm212.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm213.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm213.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm214.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm214.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm215.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm215.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm216.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm216.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm217.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm217.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm218.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm218.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm219.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm219.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm22.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm22.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm220.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm220.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm221.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm221.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm222.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm222.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm223.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm223.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm224.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm224.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm225.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm225.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm226.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm226.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm227.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm227.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm228.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm228.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm229.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm229.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm23.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm23.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm230.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm230.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm231.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm231.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm232.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm232.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm233.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm233.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm234.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm234.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm235.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm235.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm236.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm236.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm237.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm237.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm238.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm238.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm239.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm239.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm24.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm24.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm240.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm240.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm241.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm241.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm242.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm242.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm243.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm243.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm244.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm244.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm245.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm245.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm246.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm246.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm247.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm247.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm248.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm248.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm249.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm249.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm25.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm25.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm250.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm250.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm251.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm251.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm252.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm252.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm253.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm253.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm254.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm254.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm255.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm255.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm256.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm256.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm257.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm257.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm258.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm258.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm259.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm259.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm26.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm26.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm260.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm260.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm261.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm261.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm262.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm262.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm263.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm263.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm264.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm264.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm265.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm265.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm266.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm266.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm267.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm267.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm268.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm268.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm269.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm269.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm27.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm27.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm270.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm270.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm271.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm271.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm272.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm272.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm273.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm273.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm274.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm274.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm275.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm275.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm276.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm276.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm277.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm277.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm278.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm278.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm279.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm279.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm28.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm28.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm280.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm280.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm281.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm281.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm282.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm282.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm283.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm283.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm284.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm284.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm285.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm285.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm286.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm286.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm287.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm287.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm288.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm288.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm289.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm289.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm29.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm29.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm290.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm290.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm291.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm291.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm292.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm292.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm293.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm293.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm294.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm294.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm295.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm295.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm296.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm296.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm297.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm297.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm298.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm298.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm299.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm299.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm3.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm3.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm30.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm30.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm300.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm300.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm301.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm301.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm302.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm302.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm303.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm303.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm304.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm304.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm305.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm305.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm306.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm306.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm307.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm307.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm308.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm308.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm309.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm309.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm31.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm31.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm310.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm310.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm311.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm311.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm312.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm312.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm313.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm313.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm314.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm314.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm315.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm315.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm316.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm316.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm317.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm317.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm318.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm318.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm32.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm32.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm33.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm33.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm34.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm34.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm35.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm35.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm36.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm36.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm37.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm37.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm38.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm38.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm39.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm39.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm4.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm4.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm40.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm40.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm41.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm41.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm42.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm42.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm43.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm43.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm44.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm44.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm45.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm45.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm46.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm46.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm47.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm47.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm48.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm48.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm49.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm49.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm5.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm5.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm50.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm50.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm51.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm51.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm52.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm52.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm53.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm53.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm54.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm54.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm55.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm55.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm56.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm56.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm57.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm57.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm58.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm58.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm59.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm59.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm6.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm6.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm60.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm60.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm61.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm61.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm62.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm62.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm63.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm63.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm64.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm64.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm65.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm65.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm66.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm66.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm67.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm67.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm68.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm68.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm69.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm69.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm7.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm7.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm70.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm70.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm71.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm71.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm72.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm72.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm73.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm73.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm74.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm74.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm75.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm75.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm76.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm76.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm77.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm77.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm78.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm78.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm79.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm79.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm8.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm8.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm80.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm80.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm81.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm81.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm82.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm82.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm83.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm83.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm84.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm84.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm85.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm85.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm86.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm86.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm87.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm87.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm88.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm88.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm89.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm89.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm9.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm9.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm90.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm90.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm91.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm91.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm92.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm92.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm93.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm93.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm94.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm94.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm95.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm95.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm96.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm96.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm97.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm97.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm98.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm98.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vm99.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vm99.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc1.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc1.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc2.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc2.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc3.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc3.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc4.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc4.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc5.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc5.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc6.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc6.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc7.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc7.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmc8.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmc8.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd1.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmd1.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd2.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmd2.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vmd3.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vmd3.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme1.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme1.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme2.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme2.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme3.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme3.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme4.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme4.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme5.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme5.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif/vme6.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif/vme6.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/verif_files.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/verif_files.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/examples/wing.dat` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/examples/wing.dat`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/component_queries.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/component_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/connectivity_queries.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/connectivity_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/core.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/core.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/geometry_queries.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/geometry_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/inline_functions.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/inline_functions.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/line_queries.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/line_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/nearest_queries.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/nearest_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/normals_queries.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/normals_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/scalar_queries.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/scalar_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/inline_functions/selection_queries.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/inline_functions/selection_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/jupyter.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/jupyter.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/krylov.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/krylov.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/launcher.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/licensing.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/licensing.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/logging.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_console.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_console.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_corba.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_corba.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_geometry.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_geometry.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mapdl_grpc.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mapdl_grpc.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/math.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/math.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh/mesh.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/mesh_grpc.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/mesh_grpc.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/misc.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/misc.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/parameters.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/parameters.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/plotting.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/plotting.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/pool.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/pool.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/post.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/post.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/solution.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/solution.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/theme.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/theme.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/src/ansys/mapdl/core/xpl.py` & `ansys_mapdl_core-0.65.1/src/ansys/mapdl/core/xpl.py`

 * *Files identical despite different names*

### Comparing `ansys_mapdl_core-0.65.0/PKG-INFO` & `ansys_mapdl_core-0.65.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-mapdl-core
-Version: 0.65.0
+Version: 0.65.1
 Summary: A Python wrapper for Ansys MAPDL.
 Author-email: "Ansys, Inc." <pyansys.maintainers@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -23,22 +23,23 @@
 Requires-Dist: ansys-mapdl-reader>=0.51.7
 Requires-Dist: ansys-platform-instancemanagement~=1.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: click>=8.1.3
 Requires-Dist: grpcio>=1.30.0
 Requires-Dist: importlib-metadata>=4.0
 Requires-Dist: matplotlib>=3.0.0
-Requires-Dist: numpy>=1.14.0
+Requires-Dist: numpy>=1.14.0,<1.25.0; python_version < '3.9'
+Requires-Dist: numpy>=1.14.0; python_version >= '3.9'
 Requires-Dist: pexpect>=4.8.0 ; platform_system=='Linux'
 Requires-Dist: protobuf>=3.12.2
 Requires-Dist: psutil>=5.9.4
 Requires-Dist: pyansys-tools-versioning>=0.3.3
 Requires-Dist: ansys-tools-path>=0.2.4
-Requires-Dist: pyiges>=0.1.4
-Requires-Dist: pyvista>=0.33.0
+Requires-Dist: pyiges[full]>=0.3.1
+Requires-Dist: pyvista>=0.33.0,<0.41
 Requires-Dist: scipy>=1.3.0
 Requires-Dist: tqdm>=4.45.0
 Requires-Dist: vtk>=9.0.0
 Requires-Dist: sphinx==6.2.1 ; extra == "doc"
 Requires-Dist: ansys-dpf-core==0.8.1 ; extra == "doc"
 Requires-Dist: ansys-mapdl-reader==0.52.13 ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
```

