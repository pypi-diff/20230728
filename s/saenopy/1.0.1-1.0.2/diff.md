# Comparing `tmp/saenopy-1.0.1.tar.gz` & `tmp/saenopy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saenopy-1.0.1.tar", max compression
+gzip compressed data, was "saenopy-1.0.2.tar", max compression
```

## Comparing `saenopy-1.0.1.tar` & `saenopy-1.0.2.tar`

### file list

```diff
@@ -1,101 +1,115 @@
--rw-r--r--   0        0        0     1065 2023-06-08 19:47:54.157571 saenopy-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2183 2023-06-08 19:47:54.157571 saenopy-1.0.1/README.md
--rw-r--r--   0        0        0     1307 2023-06-08 19:47:54.261573 saenopy-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      348 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/__init__.py
--rw-r--r--   0        0        0     1347 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/build_beams.py
--rw-r--r--   0        0        0     1279 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/conjugate_gradient.py
--rw-r--r--   0        0        0     7716 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/examples.py
--rw-r--r--   0        0        0    15307 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/get_deformations.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/__init__.py
--rw-r--r--   0        0        0     3918 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/code_editor.py
--rw-r--r--   0        0        0     7389 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/gui_code.py
--rw-r--r--   0        0        0     4605 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/script_file.py
--rw-r--r--   0        0        0     7099 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/code/syntax.py
--rw-r--r--   0        0        0    19372 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/QExtendedGraphicsView.py
--rw-r--r--   0        0        0    46067 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/QtShortCuts.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/__init__.py
--rw-r--r--   0        0        0    21886 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/gui_classes.py
--rw-r--r--   0        0        0    33357 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/lif_reader.py
--rw-r--r--   0        0        0     6027 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/patch_lifreader.py
--rw-r--r--   0        0        0      282 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/resources.py
--rw-r--r--   0        0        0    15449 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/sigmoid_widget.py
--rw-r--r--   0        0        0     6583 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_preview.py
--rw-r--r--   0        0        0     3848 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_selector.py
--rw-r--r--   0        0        0     9342 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_selector_crop.py
--rw-r--r--   0        0        0     3096 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_selector_leica.py
--rw-r--r--   0        0        0    12078 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/common/stack_selector_tif.py
--rw-r--r--   0        0        0     7192 2023-06-08 19:47:54.261573 saenopy-1.0.1/saenopy/gui/gui_master.py
--rw-r--r--   0        0        0    16079 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/material_fit/gui_fit.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/orientation/__init__.py
--rw-r--r--   0        0        0    51650 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/orientation/gui_orientation.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/analyze/__init__.py
--rw-r--r--   0        0        0    20715 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/analyze/plot_window.py
--rw-r--r--   0        0        0     1575 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/gui_solver.py
--rw-r--r--   0        0        0    16165 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/BatchEvaluate.py
--rw-r--r--   0        0        0    11795 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/DeformationDetector.py
--rw-r--r--   0        0        0     4203 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/FittedMesh.py
--rw-r--r--   0        0        0    11660 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/MeshCreator.py
--rw-r--r--   0        0        0    10563 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/PipelineModule.py
--rw-r--r--   0        0        0     1103 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/QTimeSlider.py
--rw-r--r--   0        0        0    14384 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/Regularizer.py
--rw-r--r--   0        0        0    11278 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/ResultView.py
--rw-r--r--   0        0        0    20033 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/StackDisplay.py
--rw-r--r--   0        0        0    12999 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/VTK_Toolbar.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/__init__.py
--rw-r--r--   0        0        0      541 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/code_export.py
--rw-r--r--   0        0        0     6645 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
--rw-r--r--   0        0        0    48390 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/Exporter.py
--rw-r--r--   0        0        0    13704 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
--rw-r--r--   0        0        0    17357 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
--rw-r--r--   0        0        0    18697 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/FiberViewer.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/exporter/__init__.py
--rw-r--r--   0        0        0    11681 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/load_measurement_dialog.py
--rw-r--r--   0        0        0     3868 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/path_editor.py
--rw-r--r--   0        0        0    12003 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/solver/modules/showVectorField.py
--rw-r--r--   0        0        0        0 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/spheroid/__init__.py
--rw-r--r--   0        0        0    93350 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/gui/spheroid/gui_deformation_spheroid.py
--rw-r--r--   0        0        0    53944 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/Icon.ico
--rw-r--r--   0        0        0    42003 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/Logo.png
--rw-r--r--   0        0        0    77561 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/Logo.svg
--rw-r--r--   0        0        0    37691 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/Logo_black.png
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/arrowscale.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/autoscale0.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/autoscale1.ico
--rw-r--r--   0        0        0    48947 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/buttons.svg
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/center0.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.265573 saenopy-1.0.1/saenopy/img/center1.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/contrast0.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/contrast1.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/grid.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/grid2.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/grid3.ico
--rw-r--r--   0        0        0    38885 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/logo_splash.png
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/nan0.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/nan1.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/show_image.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/show_image2.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/show_image3.ico
--rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/slice0.ico
--rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/slice1.ico
--rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/slice2.ico
--rw-r--r--   0        0        0     1150 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/slice_all.ico
--rw-r--r--   0        0        0   121664 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/BFTFM.png
--rw-r--r--   0        0        0   132449 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/BFTFM_2.png
--rw-r--r--   0        0        0   180081 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/Bead_example_icon.png
--rw-r--r--   0        0        0   202759 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/Dynamic_icon.png
--rw-r--r--   0        0        0   554429 2023-06-08 19:47:54.269573 saenopy-1.0.1/saenopy/img/thumbnails/StainedOrganoid_icon.png
--rw-r--r--   0        0        0   263760 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/img/thumbnails/liver_fibroblast_icon.png
--rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/img/view_single.ico
--rw-r--r--   0        0        0     3606 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/img/view_two.ico
--rw-r--r--   0        0        0    12316 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/macro.py
--rw-r--r--   0        0        0    12253 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/materials.py
--rw-r--r--   0        0        0     3701 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/mesh.py
--rw-r--r--   0        0        0     5635 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/multigrid_helper.py
--rw-r--r--   0        0        0    22760 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/result_file.py
--rw-r--r--   0        0        0     7754 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/saveable.py
--rw-r--r--   0        0        0    46114 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/solver.py
--rw-r--r--   0        0        0    11130 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/stack.py
--rw-r--r--   0        0        0    17259 2023-06-08 19:47:54.273573 saenopy-1.0.1/saenopy/unused/macro.py
--rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 saenopy-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-28 17:42:27.967829 saenopy-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2183 2023-07-28 17:42:27.967829 saenopy-1.0.2/README.md
+-rw-r--r--   0        0        0     1307 2023-07-28 17:42:28.087828 saenopy-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      348 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/build_beams.py
+-rw-r--r--   0        0        0     1279 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/conjugate_gradient.py
+-rw-r--r--   0        0        0     7716 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/examples.py
+-rw-r--r--   0        0        0    15307 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/get_deformations.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/__init__.py
+-rw-r--r--   0        0        0     3918 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/code_editor.py
+-rw-r--r--   0        0        0     7389 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/gui_code.py
+-rw-r--r--   0        0        0     4605 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/script_file.py
+-rw-r--r--   0        0        0     7099 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/code/syntax.py
+-rw-r--r--   0        0        0    19372 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/QExtendedGraphicsView.py
+-rw-r--r--   0        0        0    46067 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/QtShortCuts.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/__init__.py
+-rw-r--r--   0        0        0    21886 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/gui_classes.py
+-rw-r--r--   0        0        0    33357 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/lif_reader.py
+-rw-r--r--   0        0        0     6027 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/patch_lifreader.py
+-rw-r--r--   0        0        0      282 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/resources.py
+-rw-r--r--   0        0        0    15449 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/sigmoid_widget.py
+-rw-r--r--   0        0        0     6583 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_preview.py
+-rw-r--r--   0        0        0     3848 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_selector.py
+-rw-r--r--   0        0        0    10884 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_selector_crop.py
+-rw-r--r--   0        0        0     3096 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_selector_leica.py
+-rw-r--r--   0        0        0    12184 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/common/stack_selector_tif.py
+-rw-r--r--   0        0        0     7932 2023-07-28 17:42:28.087828 saenopy-1.0.2/saenopy/gui/gui_master.py
+-rw-r--r--   0        0        0    16079 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/material_fit/gui_fit.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/orientation/__init__.py
+-rw-r--r--   0        0        0    51650 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/orientation/gui_orientation.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/analyze/__init__.py
+-rw-r--r--   0        0        0    20715 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/analyze/plot_window.py
+-rw-r--r--   0        0        0     1575 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/gui_solver.py
+-rw-r--r--   0        0        0    16215 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/BatchEvaluate.py
+-rw-r--r--   0        0        0    11801 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/DeformationDetector.py
+-rw-r--r--   0        0        0     4203 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/FittedMesh.py
+-rw-r--r--   0        0        0    11660 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/MeshCreator.py
+-rw-r--r--   0        0        0    10563 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/PipelineModule.py
+-rw-r--r--   0        0        0     1103 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/QTimeSlider.py
+-rw-r--r--   0        0        0    15201 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/Regularizer.py
+-rw-r--r--   0        0        0    11278 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/ResultView.py
+-rw-r--r--   0        0        0    20076 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/StackDisplay.py
+-rw-r--r--   0        0        0    12999 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/VTK_Toolbar.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/__init__.py
+-rw-r--r--   0        0        0      541 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/code_export.py
+-rw-r--r--   0        0        0     6645 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py
+-rw-r--r--   0        0        0    48390 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/Exporter.py
+-rw-r--r--   0        0        0    13704 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExporterRender2D.py
+-rw-r--r--   0        0        0    17357 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExporterRender3D.py
+-rw-r--r--   0        0        0    18697 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/FiberViewer.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/exporter/__init__.py
+-rw-r--r--   0        0        0    11704 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/load_measurement_dialog.py
+-rw-r--r--   0        0        0     3868 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/path_editor.py
+-rw-r--r--   0        0        0    12328 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/solver/modules/showVectorField.py
+-rw-r--r--   0        0        0        0 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/spheroid/__init__.py
+-rw-r--r--   0        0        0    93350 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/gui/spheroid/gui_deformation_spheroid.py
+-rw-r--r--   0        0        0    53944 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/img/Icon.ico
+-rw-r--r--   0        0        0    42217 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/img/Logo.png
+-rw-r--r--   0        0        0    88874 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/img/Logo.svg
+-rw-r--r--   0        0        0    37691 2023-07-28 17:42:28.091828 saenopy-1.0.2/saenopy/img/Logo_black.png
+-rw-r--r--   0        0        0    19301 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame00.png
+-rw-r--r--   0        0        0    19413 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame01.png
+-rw-r--r--   0        0        0    19360 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame02.png
+-rw-r--r--   0        0        0    19344 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame03.png
+-rw-r--r--   0        0        0    19267 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame04.png
+-rw-r--r--   0        0        0    18999 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame05.png
+-rw-r--r--   0        0        0    31030 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame06.png
+-rw-r--r--   0        0        0    32933 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame07.png
+-rw-r--r--   0        0        0    34748 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame08.png
+-rw-r--r--   0        0        0    35475 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame09.png
+-rw-r--r--   0        0        0    37528 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame10.png
+-rw-r--r--   0        0        0    39777 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame11.png
+-rw-r--r--   0        0        0    41902 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame12.png
+-rw-r--r--   0        0        0    41897 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/animation/frame13.png
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/arrowscale.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/autoscale0.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/autoscale1.ico
+-rw-r--r--   0        0        0    48947 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/buttons.svg
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/center0.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/center1.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/contrast0.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/contrast1.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/grid.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/grid2.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/grid3.ico
+-rw-r--r--   0        0        0    38885 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/logo_splash.png
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/nan0.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/nan1.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/show_image.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/show_image2.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/show_image3.ico
+-rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/slice0.ico
+-rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/slice1.ico
+-rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/slice2.ico
+-rw-r--r--   0        0        0     1150 2023-07-28 17:42:28.095828 saenopy-1.0.2/saenopy/img/slice_all.ico
+-rw-r--r--   0        0        0   121664 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/BFTFM.png
+-rw-r--r--   0        0        0   132449 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/BFTFM_2.png
+-rw-r--r--   0        0        0   180081 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/Bead_example_icon.png
+-rw-r--r--   0        0        0   202759 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/Dynamic_icon.png
+-rw-r--r--   0        0        0   554429 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/StainedOrganoid_icon.png
+-rw-r--r--   0        0        0   263760 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/thumbnails/liver_fibroblast_icon.png
+-rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/view_single.ico
+-rw-r--r--   0        0        0     3606 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/img/view_two.ico
+-rw-r--r--   0        0        0    12316 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/macro.py
+-rw-r--r--   0        0        0    12253 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/materials.py
+-rw-r--r--   0        0        0     3701 2023-07-28 17:42:28.099828 saenopy-1.0.2/saenopy/mesh.py
+-rw-r--r--   0        0        0     5635 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/multigrid_helper.py
+-rw-r--r--   0        0        0    24079 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/result_file.py
+-rw-r--r--   0        0        0     7754 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/saveable.py
+-rw-r--r--   0        0        0    47872 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/solver.py
+-rw-r--r--   0        0        0    11130 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/stack.py
+-rw-r--r--   0        0        0    17259 2023-07-28 17:42:28.103828 saenopy-1.0.2/saenopy/unused/macro.py
+-rw-r--r--   0        0        0     3710 1970-01-01 00:00:00.000000 saenopy-1.0.2/PKG-INFO
```

### Comparing `saenopy-1.0.1/LICENSE.txt` & `saenopy-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/README.md` & `saenopy-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 ## Installation
 
 ### Standalone
 To use saenopy without a complicated installation you can use our standalone binaries to get started right away on Windows or Linux.
 
 Windows
-https://github.com/rgerum/saenopy/releases/download/v1.0.1/saenopy.exe
+https://github.com/rgerum/saenopy/releases/download/v1.0.2/saenopy.exe
 
 Linux
-https://github.com/rgerum/saenopy/releases/download/v1.0.1/saenopy
+https://github.com/rgerum/saenopy/releases/download/v1.0.2/saenopy
 
 ### Using Python
 
 If you are experienced with python or even want to use our Python API, you need to install saenopy as a python package.
 Saenopy can be installed directly using pip:
 
     ``pip install saenopy``
```

### Comparing `saenopy-1.0.1/pyproject.toml` & `saenopy-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saenopy"
-version = "1.0.1"
+version = "1.0.2"
 description = "Semi-elastic fiber optimisation in python."
 authors = ["rgerum <14153051+rgerum@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "saenopy"}]
```

### Comparing `saenopy-1.0.1/saenopy/build_beams.py` & `saenopy-1.0.2/saenopy/build_beams.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/conjugate_gradient.py` & `saenopy-1.0.2/saenopy/conjugate_gradient.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/examples.py` & `saenopy-1.0.2/saenopy/examples.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/get_deformations.py` & `saenopy-1.0.2/saenopy/get_deformations.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/code/code_editor.py` & `saenopy-1.0.2/saenopy/gui/code/code_editor.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/code/gui_code.py` & `saenopy-1.0.2/saenopy/gui/code/gui_code.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/code/script_file.py` & `saenopy-1.0.2/saenopy/gui/code/script_file.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/code/syntax.py` & `saenopy-1.0.2/saenopy/gui/code/syntax.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/QExtendedGraphicsView.py` & `saenopy-1.0.2/saenopy/gui/common/QExtendedGraphicsView.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/QtShortCuts.py` & `saenopy-1.0.2/saenopy/gui/common/QtShortCuts.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/gui_classes.py` & `saenopy-1.0.2/saenopy/gui/common/gui_classes.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/lif_reader.py` & `saenopy-1.0.2/saenopy/gui/common/lif_reader.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/patch_lifreader.py` & `saenopy-1.0.2/saenopy/gui/common/patch_lifreader.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/sigmoid_widget.py` & `saenopy-1.0.2/saenopy/gui/common/sigmoid_widget.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/stack_preview.py` & `saenopy-1.0.2/saenopy/gui/common/stack_preview.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/stack_selector.py` & `saenopy-1.0.2/saenopy/gui/common/stack_selector.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/stack_selector_crop.py` & `saenopy-1.0.2/saenopy/gui/common/stack_selector_crop.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,17 +57,18 @@
             fp.write(s)
             fp.write("\n")
 
 
 class StackSelectorCrop(QtWidgets.QWidget):
     set_voxel_size = None
 
-    def __init__(self, parent: "StackSelector", parent2: "StackSelector", use_time=False):
+    def __init__(self, parent: "StackSelector", reference_choice, parent2: "StackSelector", use_time=False):
         super().__init__()
         self.parent_selector = parent
+        self.reference_choice = reference_choice
 
         with QtShortCuts.QHBoxLayout(self) as main_layout:
             main_layout.setContentsMargins(0, 0, 0, 0)
             with QtShortCuts.QVBoxLayout():
                 self.input_voxel_size = QtShortCuts.QInputString(None, "Voxel size (xyz) (µm)", "0, 0, 0", validator=self.validator)
                 self.input_voxel_size.valueChanged.connect(self.input_voxel_size_changed)
                 self.completer = QtWidgets.QCompleter(get_last_voxel_sizes(), self)
@@ -91,23 +92,26 @@
 
                 QtShortCuts.current_layout.addStretch()
 
             with QtShortCuts.QVBoxLayout():
                 with QtShortCuts.QHBoxLayout():
                     self.input_time_dt = QtShortCuts.QInputString(None, "Time Delta", "0",
                                                                      validator=self.validator_time, type=float)
+                    self.input_time_dt.setEnabled(False)
+                    self.input_time_dt.emitValueChanged()
                     self.input_tbar_unit = QtShortCuts.QInputChoice(self.input_time_dt.layout(), None, "s",
                                                                     ["s", "min", "h"])
                     self.completer2 = QtWidgets.QCompleter(get_last_time_deltas(), self)
                     self.input_time_dt.line_edit.setCompleter(self.completer2)
 
                 self.input_cropt = QtShortCuts.QRangeSlider(None, "crop t", 0, 200)
                 self.input_cropt.setRange(0, 1)
                 self.input_cropt.setValue((0, 1))
                 self.input_cropt.valueChanged.connect(self.z_moved)
+                self.input_t_label = QtWidgets.QLabel().addToLayout()
                 QtShortCuts.current_layout.addStretch()
 
                 self.input_cropt.setDisabled(True)
                 self.input_tbar_unit.setDisabled(True)
                 self.input_time_dt.setDisabled(True)
 
         self.parent_selector.stack_changed.connect(self.update_ranges)
@@ -160,24 +164,35 @@
                 self.input_voxel_size.setValue(", ".join([f"{x:.3f}" for x in voxel_size]))
             self.set_voxel_size = voxel_size
 
             if t_max == 1:
                 self.input_time_dt.setDisabled(True)
                 self.input_tbar_unit.setDisabled(True)
                 self.input_cropt.setDisabled(True)
+                if self.parent2.get_t_count():
+                    self.input_t_label.setText(f"1 time step - 1 reference state\n1 differences")
+                else:
+                    self.input_t_label.setText(f"1 time step - no reference state\ninvalid")
             else:
                 self.input_time_dt.setDisabled(False)
                 self.input_tbar_unit.setDisabled(False)
                 self.input_cropt.setDisabled(False)
+                if self.parent2.get_t_count():
+                    self.input_t_label.setText(f"{t_max} time steps - 1 reference state\n{t_max} differences")
+                else:
+                    self.input_t_label.setText(f"{t_max} time steps - no reference state\n{t_max-1} differences")
+            self.input_time_dt.emitValueChanged()
 
             self.label.setText(f"Stack: ({x_max}, {y_max}, {z_max})px")
+        self.update_timesteps_text()
+        self.reference_choice.valueChanged.connect(self.update_timesteps_text)
 
     def validator_time(self, value=None):
         if getattr(self, "input_time_dt", None) and not self.input_time_dt.isEnabled():
-            True
+            return True
         try:
             if value is None:
                 value = self.input_time_dt.value()
             size = float(value)
 
             if size <= 1e-10:
                 return False
@@ -212,16 +227,26 @@
                 continue
             a, b = value(widget, 0), value(widget, 1)
             if a != None or b != None:
                 crop[name] = (a, b)
 
         return crop
 
+    def update_timesteps_text(self):
+        if self.reference_choice.value():
+            t_max_ref = min(self.parent2.get_t_count(), 1)
+        else:
+            t_max_ref = 0
+        t_max = self.input_cropt.value()[1] - self.input_cropt.value()[0]
+        num_diff = t_max + t_max_ref - 1
+        self.input_t_label.setText(f"{t_max_ref if t_max_ref else 'no'} reference state, {t_max} time step{'s' if t_max != 1 else ''}\n→ {num_diff} difference{'s' if num_diff != 1 else ''} {'(invalid)' if num_diff == 0 else ''}")
+
     def z_moved(self):
         self.parent_selector.stack_changed.emit()
+        self.update_timesteps_text()
         return
 
     def input_voxel_size_changed(self):
         if not self.validator(None):
             return
         voxel_size = self.getVoxelSize()
         shape = (self.input_cropx.range()[1], self.input_cropy.range()[1], self.input_cropz.range()[1])
```

### Comparing `saenopy-1.0.1/saenopy/gui/common/stack_selector_leica.py` & `saenopy-1.0.2/saenopy/gui/common/stack_selector_leica.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/common/stack_selector_tif.py` & `saenopy-1.0.2/saenopy/gui/common/stack_selector_tif.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 import re
+import natsort
 from pathlib import Path
 import imageio
 import tifffile
 from qtpy import QtWidgets
 from saenopy.gui.common import QtShortCuts
 import appdirs
 from saenopy.stack import read_tiff
@@ -190,15 +191,15 @@
         t_name = None
         names = []
         for col in df.columns:
             if col == "filename":
                 continue
             names.append(col)
 
-            prop = QtShortCuts.QInputChoice(self.property_layout, col, str(selected_prop[col]), [str(i) for i in df[col].unique()])
+            prop = QtShortCuts.QInputChoice(self.property_layout, col, str(selected_prop[col]), natsort.natsorted([str(i) for i in df[col].unique()]))
             prop.valueChanged.connect(self.propertiesChanged)
             prop.name = col
             prop.check = QtShortCuts.QInputBool(prop.layout(), "all", False)
             prop.check.valueChanged.connect(self.propertiesChanged)
             self.property_selectors.append(prop)
             properties.append(col)
             if col == "z":
@@ -249,21 +250,21 @@
                 selected_props_dict[prop.name] = "*"
             else:
                 selected_props_dict[prop.name] = str(prop.value())
 
         self.stack_obj = []
         from saenopy.stack import Stack
         if not self.use_time or t_prop_name == "None":
-            d = d.sort_values(z_prop_name)
+            d = d.sort_values(z_prop_name, key=natsort.natsort_keygen())
             self.stack_obj = [Stack("", (1, 1, 1), {}, image_filenames=[[str(f)] for f in d.filename])]
             self.stack_obj[0].image_filenames = [[str(f)] for f in d.filename]
         else:
-            d = d.sort_values([t_prop_name, z_prop_name])
+            d = d.sort_values([t_prop_name, z_prop_name], key=natsort.natsort_keygen())
             self.stack_obj = []
-            for t, dd in d.groupby(t_prop_name):
+            for t, dd in d.groupby(t_prop_name, sort=False):
                 s = Stack("", (1, 1, 1), {}, image_filenames=[[str(f)] for f in dd.filename])
                 self.stack_obj.append(s)
 
         self.target_glob = self.format_template.format(**selected_props_dict)
         if z_prop_name == "tiff pages":
             self.target_glob += "[z]"
         elif z_prop_name == "tiff pages":
```

### Comparing `saenopy-1.0.1/saenopy/gui/gui_master.py` & `saenopy-1.0.2/saenopy/gui/gui_master.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,28 @@
                 self.tabs.currentChanged.connect(self.changedTab)
                 self.tabs.setTabPosition(QtWidgets.QTabWidget.West)
                 with self.tabs.createTab("Home") as layout:
                     layout.addStretch()
                     with QtShortCuts.QHBoxLayout() as layout2:
                         layout.addStretch()
                         self.image = QtWidgets.QLabel("x").addToLayout()
-                        self.image.setPixmap(QtGui.QPixmap(resource_path("Logo.png")))
+                        self.image_timer = QtCore.QTimer()
+                        timer_index = 0
+                        def timer():
+                            nonlocal timer_index
+                            if timer_index == 14:
+                                #self.image.setPixmap(QtGui.QPixmap(resource_path("Logo.png")))
+                                self.image_timer.stop()
+                                return
+                            self.image.setPixmap(QtGui.QPixmap(resource_path(f"animation/frame{timer_index:02d}.png")))
+                            timer_index += 1
+                        self.image_timer.timeout.connect(timer)
+                        self.image_timer.start(100)
+                        timer()
+                        #self.image.setPixmap(QtGui.QPixmap(resource_path("Logo.png")))
                         self.image.setScaledContents(True)
                         self.image.setMaximumWidth(400)
                         self.image.setMaximumHeight(200)
                         layout.addStretch()
                     with QtShortCuts.QHBoxLayout() as layout2:
                         layout2.addStretch()
                         InfoBox("Solver", lambda: self.setTab(2)).addToLayout()
```

### Comparing `saenopy-1.0.1/saenopy/gui/material_fit/gui_fit.py` & `saenopy-1.0.2/saenopy/gui/material_fit/gui_fit.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/orientation/gui_orientation.py` & `saenopy-1.0.2/saenopy/gui/orientation/gui_orientation.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/analyze/plot_window.py` & `saenopy-1.0.2/saenopy/gui/solver/analyze/plot_window.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/gui_solver.py` & `saenopy-1.0.2/saenopy/gui/solver/gui_solver.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/BatchEvaluate.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/BatchEvaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from qtpy import QtCore, QtWidgets, QtGui
 import numpy as np
 import glob
 import threading
 from pathlib import Path
 import matplotlib as mpl
 
+import traceback
+
 from saenopy import get_stacks
 from saenopy import Result
 from saenopy.gui.common import QtShortCuts
 from saenopy.gui.common.gui_classes import ListWidget
 from saenopy.gui.common.stack_selector_tif import add_last_voxel_size, add_last_time_delta
 
 from .DeformationDetector import DeformationDetector
@@ -274,15 +276,15 @@
             # glob over the path (or just use the path if it does not contain a *)
             for p in sorted(glob.glob(str(path), recursive=True)):
                 print(p)
                 try:
                     self.add_data(Result.load(p))
                 except Exception as err:
                     QtWidgets.QMessageBox.critical(self, "Open Files", f"File {p} is not a valid Saenopy file.")
-                    raise
+                    traceback.print_exc()
         self.update_icons()
 
     def add_data(self, data):
         self.list.addData(data.output, True, data, mpl.colors.to_hex(f"gray"))
 
     def update_icons(self):
         for j in range(self.list.count( ) -1):
@@ -349,15 +351,15 @@
                     time_delta=time_delta,
                     crop=dialog.stack_data.get_crop(),
                     exist_overwrite_callback=do_overwrite,
                 )
             except Exception as err:
                 # notify the user if errors occured
                 QtWidgets.QMessageBox.critical(self, "Load Stacks", str(err))
-                raise
+                traceback.print_exc()
             else:
                 # store the last voxel size
                 add_last_voxel_size(dialog.stack_data.getVoxelSize())
                 # add the loaded measruement objects
                 for data in results:
                     self.add_data(data)
```

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/DeformationDetector.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/DeformationDetector.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,23 +181,23 @@
                 result.mesh_piv[i] = return_value
 
         result.solvers = None
 
     def get_code(self) -> Tuple[str, str]:
         import_code = ""
 
-        results = None
+        results = []
         def code(my_piv_params):  # pragma: no cover
             # define the parameters for the piv deformation detection
             piv_parameters = my_piv_params
 
             # iterate over all the results objects
             for result in results:
                 # set the parameters
-                result.piv_parameters = params
+                result.piv_parameters = piv_parameters
                 # get count
                 count = len(result.stacks)
                 if result.stack_reference is None:
                     count -= 1
                 # iterate over all stack pairs
                 for i in range(count):
                     # get two consecutive stacks
```

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/FittedMesh.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/FittedMesh.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/MeshCreator.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/MeshCreator.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/PipelineModule.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/PipelineModule.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,17 @@
     tab: QtWidgets.QTabWidget = None
 
     parameter_mappings: List[ParameterMapping] = None
     params_name: None
 
     def __init__(self, parent: "BatchEvaluate", layout):
         super().__init__()
+        self.parameter_mappings = []
+        self.params_name = None
+
         if layout is not None:
             layout.addWidget(self)
         if parent is None:
             return
         self.parent = parent
         self.settings = self.parent.settings
 
@@ -86,17 +89,14 @@
 
         self.parent.result_changed.connect(self.resultChanged)
         self.parent.set_current_result.connect(self.setResult)
         self.parent.tab_changed.connect(self.tabChanged)
 
         self.processing_progress.connect(self.parent.progress)
 
-        self.parameter_mappings = []
-        self.params_name = None
-
     def setParameterMapping(self, params_name: str = None, parameter_dict: dict=None):
         self.params_name = params_name
         if params_name is None:
             return
         self.parameter_mappings.append(ParameterMapping(params_name, parameter_dict))
 
     current_result_plotted = False
```

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/QTimeSlider.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/QTimeSlider.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/Regularizer.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/Regularizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,16 @@
                         with QtShortCuts.QHBoxLayout() as layout2:
                             self.input_k = QtShortCuts.QInputString(None, "k", "1645", type=float, tooltip="the stiffness of the material's fibers")
                             self.input_d_0 = QtShortCuts.QInputString(None, "d_0", "0.0008", type=float, tooltip="the bluckling strength of the material's fibers")
                             self.input_lamda_s = QtShortCuts.QInputString(None, "λ_s", "0.0075", type=float, tooltip="the length at which strain stiffening of the material's fibers starts")
                             self.input_d_s = QtShortCuts.QInputString(None, "d_s", "0.033", type=float, tooltip="the strain stiffening strength of the material's fibers")
 
                     with QtShortCuts.QGroupBox(None, "Regularisation Parameters") as self.material_parameters:
+                        self.input_previous_t_as_start = QtShortCuts.QInputBool(None, "use previous time steps deformation field", True,
+                                                                tooltip="wether to use the previous time steps deformation field as a starting value for the next regularisation")
                         with QtShortCuts.QHBoxLayout(None) as layout:
                             self.input_alpha = QtShortCuts.QInputString(None, "alpha", "1e10", type="exp", tooltip="the strength of the regularisation (higher values mean weaker forces)")
                             self.input_step_size = QtShortCuts.QInputString(None, "step size", "0.33", type=float, tooltip="the step with of the iteration algorithm")
                         with QtShortCuts.QHBoxLayout(None) as layout:
                             self.input_imax = QtShortCuts.QInputNumber(None, "max iterations", 100, float=False, tooltip="the maximum number of iterations after which to abort the iteration algorithm")
                             self.input_conv_crit = QtShortCuts.QInputString(None, "rel. conv. crit.", 0.01, type=float, tooltip="the convergence criterion of the iteration algorithm")
 
@@ -82,14 +84,15 @@
             "d_s": self.input_d_s,
         })
         self.setParameterMapping("solve_parameters", {
             "alpha": self.input_alpha,
             "step_size": self.input_step_size,
             "max_iterations": self.input_imax,
             "rel_conv_crit": self.input_conv_crit,
+            "prev_t_as_start": self.input_previous_t_as_start,
         })
 
         self.iteration_finished.connect(self.iteration_callback)
         self.iteration_finished.emit(None, np.ones([10, 3]), 0, None)
 
     def z_slider_value_changed(self):
         self.update_display()
@@ -148,14 +151,17 @@
                 self.iteration_finished.emit(result, result.solver_relrec_demo[:i], i, imax)
             result.solvers[0].regularisation_results = result.solver_relrec_demo
             return
 
         for i in range(len(result.solvers)):
             M = result.solvers[i]
 
+            if i > 0 and solve_parameters["prev_t_as_start"]:
+                M.mesh.displacements[:] = result.solvers[i-1].mesh.displacements.copy()
+
             def callback(M, relrec, i, imax):
                 self.iteration_finished.emit(result, relrec, i, imax)
 
             M.set_material_model(saenopy.materials.SemiAffineFiberMaterial(
                                material_parameters["k"],
                                material_parameters["d_0"] if material_parameters["d_0"] != "None" else None,
                                material_parameters["lambda_s"] if material_parameters["lambda_s"] != "None" else None,
@@ -238,20 +244,24 @@
             solve_parameters = my_reg_params2
 
             # iterate over all the results objects
             for result in results:
                 result.mesh_parameters = material_parameters
                 result.solve_parameters = solve_parameters
                 for index, M in enumerate(result.solvers):
+                    # optionally copy the displacement field from the previous time step as a starting value
+                    if index > 0 and solve_parameters["prev_t_as_start"]:
+                        M.mesh.displacements[:] = result.solvers[index - 1].mesh.displacements.copy()
+
                     # set the material model
                     M.set_material_model(saenopy.materials.SemiAffineFiberMaterial(
                         material_parameters["k"],
                         material_parameters["d_0"],
                         material_parameters["lambda_s"],
-                        material_parameters["ds"],
+                        material_parameters["d_s"],
                     ))
                     # find the regularized force solution
                     M.solve_regularized(alpha=solve_parameters["alpha"], step_size=solve_parameters["step_size"],
                                         max_iterations=solve_parameters["max_iterations"], rel_conv_crit=solve_parameters["rel_conv_crit"],
                                         verbose=True)
                     # save the forces
                     result.save()
```

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/ResultView.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/ResultView.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/StackDisplay.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/StackDisplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,16 +282,16 @@
                         crop=crop1,
                         load_existing=True)
                     # or if you want to explicitly load existing results files
                     # use * to load multiple result files for batch processing
                     # results = saenopy.load_results(result_file)
 
                 data = dict(
-                    filename=self.result.template,
-                    reference_stack1=self.result.stack_reference.template,
+                    filename=self.result.get_absolute_path(),
+                    reference_stack1=self.result.get_absolute_path_reference(),
                     output1=str(Path(self.result.output).parent),
                     voxel_size1=self.result.stacks[0].voxel_size,
                     crop1=self.result.stacks[0].crop,
                     result_file=str(self.result.output),
                 )
         else:
             if self.result.stack_reference is not None:
@@ -311,16 +311,16 @@
                         crop=crop1,
                         load_existing=True)
                     # or if you want to explicitly load existing results files
                     # use * to load multiple result files for batch processing
                     # results = saenopy.load_results(result_file)
 
                 data = dict(
-                    filename=self.result.template,
-                    reference_stack1=self.result.stack_reference.template,
+                    filename=self.result.get_absolute_path(),
+                    reference_stack1=self.result.get_absolute_path_reference(),
                     output1=str(Path(self.result.output).parent),
                     result_file=str(self.result.output),
                     voxel_size1=self.result.stacks[0].voxel_size,
                     crop1=self.result.stacks[0].crop,
                     time_delta1=self.result.time_delta,
                 )
             else:
@@ -339,15 +339,15 @@
                         crop=crop1,
                         load_existing=True)
                     # or if you want to explicitly load existing results files
                     # use * to load multiple result files for batch processing
                     # results = saenopy.load_results(result_file)
 
                 data = dict(
-                    filename=self.result.template,
+                    filename=self.result.get_absolute_path(),
                     output1=str(Path(self.result.output).parent),
                     voxel_size1=self.result.stacks[0].voxel_size,
                     time_delta1=self.result.time_delta,
                     crop1=self.result.stacks[0].crop,
                     result_file=str(self.result.output),
                 )
```

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/VTK_Toolbar.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/VTK_Toolbar.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/code_export.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/code_export.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExportRenderCommon.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/Exporter.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/Exporter.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExporterRender2D.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExporterRender2D.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/ExporterRender3D.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/ExporterRender3D.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/exporter/FiberViewer.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/exporter/FiberViewer.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/load_measurement_dialog.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/load_measurement_dialog.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                                                                         self.stack_reference, use_time=True)
                                         self.stack_data.setMinimumWidth(300)
                                         self.stack_reference.setMinimumWidth(300)
                                         self.place_holder_widget.setMinimumWidth(300)
                                         self.stack_data.glob_string_changed.connect(
                                             lambda x, y: self.stack_data_input.setText(y))
                                         self.stack_data_input = QtWidgets.QLineEdit().addToLayout()
-                            self.stack_crop = StackSelectorCrop(self.stack_data, self.stack_reference).addToLayout()
+                            self.stack_crop = StackSelectorCrop(self.stack_data, self.reference_choice, self.stack_reference).addToLayout()
                             self.stack_data.stack_crop = self.stack_crop
                         self.stack_preview = StackPreview(QtShortCuts.current_layout, self.reference_choice,
                                                           self.stack_reference, self.stack_data)
                     self.outputText = QtShortCuts.QInputFolder(None, "output", settings=settings,
                                                                settings_key="batch/wildcard2", allow_edit=True)
                     with QtShortCuts.QHBoxLayout():
                         # self.button_clear = QtShortCuts.QPushButton(None, "clear list", self.clear_files)
```

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/path_editor.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/path_editor.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/gui/solver/modules/showVectorField.py` & `saenopy-1.0.2/saenopy/gui/solver/modules/showVectorField.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,20 @@
             point_cloud.point_data[name + "_mag2"][nan_values] = 0
             # show nans
             if not show_all_points and show_nan:
                 R = obj_R[nan_values]
                 if R.shape[0]:
                     point_cloud2 = pv.PolyData(R)
                     point_cloud2.point_data["nan"] = obj_R[nan_values, 0] * np.nan
+            R = obj_R[nan_values]
+            if name == "forces" and getattr(obj, "cell_boundary_mask", None) is not None:
+                R = obj_R[obj.cell_boundary_mask]
+                if R.shape[0]:
+                    point_cloud2 = pv.PolyData(R)
+                    point_cloud2.point_data["nan"] = R[:, 0] * np.nan
 
             # scalebar scaling factor
             norm_stack_size = np.abs(np.max(obj_R) - np.min(obj_R))
             if scalebar_max is None:
                 factor = factor * norm_stack_size / np.nanmax(point_cloud[name + "_mag2"])#np.nanpercentile(point_cloud[name + "_mag2"], 99.9)
             else:
                 factor = factor * norm_stack_size / scalebar_max
```

### Comparing `saenopy-1.0.1/saenopy/gui/spheroid/gui_deformation_spheroid.py` & `saenopy-1.0.2/saenopy/gui/spheroid/gui_deformation_spheroid.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/Icon.ico` & `saenopy-1.0.2/saenopy/img/Icon.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/Logo.svg` & `saenopy-1.0.2/saenopy/img/Logo.svg`

 * *Files 7% similar despite different names*

```diff
@@ -46,4803 +46,5510 @@
 000002d0: 7262 6f61 7264 3d22 6661 6c73 6522 0a20  rboard="false". 
 000002e0: 2020 2020 696e 6b73 6361 7065 3a64 6573      inkscape:des
 000002f0: 6b63 6f6c 6f72 3d22 2364 3164 3164 3122  kcolor="#d1d1d1"
 00000300: 0a20 2020 2020 696e 6b73 6361 7065 3a64  .     inkscape:d
 00000310: 6f63 756d 656e 742d 756e 6974 733d 2270  ocument-units="p
 00000320: 7822 0a20 2020 2020 7368 6f77 6772 6964  x".     showgrid
 00000330: 3d22 6661 6c73 6522 0a20 2020 2020 696e  ="false".     in
-00000340: 6b73 6361 7065 3a7a 6f6f 6d3d 2230 2e37  kscape:zoom="0.7
-00000350: 3732 3437 3733 3522 0a20 2020 2020 696e  7247735".     in
-00000360: 6b73 6361 7065 3a63 783d 2234 3236 2e35  kscape:cx="426.5
-00000370: 3439 3733 220a 2020 2020 2069 6e6b 7363  4973".     inksc
-00000380: 6170 653a 6379 3d22 3237 322e 3439 3939  ape:cy="272.4999
+00000340: 6b73 6361 7065 3a7a 6f6f 6d3d 2232 2e31  kscape:zoom="2.1
+00000350: 3834 3839 3539 220a 2020 2020 2069 6e6b  848959".     ink
+00000360: 7363 6170 653a 6378 3d22 3136 332e 3632  scape:cx="163.62
+00000370: 3333 3622 0a20 2020 2020 696e 6b73 6361  336".     inksca
+00000380: 7065 3a63 793d 2237 362e 3636 3236 3932  pe:cy="76.662692
 00000390: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
 000003a0: 7769 6e64 6f77 2d77 6964 7468 3d22 3138  window-width="18
 000003b0: 3436 220a 2020 2020 2069 6e6b 7363 6170  46".     inkscap
 000003c0: 653a 7769 6e64 6f77 2d68 6569 6768 743d  e:window-height=
 000003d0: 2231 3031 3622 0a20 2020 2020 696e 6b73  "1016".     inks
 000003e0: 6361 7065 3a77 696e 646f 772d 783d 2237  cape:window-x="7
 000003f0: 3422 0a20 2020 2020 696e 6b73 6361 7065  4".     inkscape
 00000400: 3a77 696e 646f 772d 793d 2232 3722 0a20  :window-y="27". 
 00000410: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
 00000420: 646f 772d 6d61 7869 6d69 7a65 643d 2231  dow-maximized="1
 00000430: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
 00000440: 6375 7272 656e 742d 6c61 7965 723d 226c  current-layer="l
-00000450: 6179 6572 3122 3e0a 2020 2020 3c69 6e6b  ayer1">.    <ink
-00000460: 7363 6170 653a 7061 6765 0a20 2020 2020  scape:page.     
-00000470: 2020 783d 2230 220a 2020 2020 2020 2079    x="0".       y
-00000480: 3d22 3022 0a20 2020 2020 2020 7769 6474  ="0".       widt
-00000490: 683d 2234 3030 220a 2020 2020 2020 2068  h="400".       h
-000004a0: 6569 6768 743d 2232 3030 220a 2020 2020  eight="200".    
-000004b0: 2020 2069 643d 2270 6167 6533 3236 220a     id="page326".
-000004c0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000004d0: 6c61 6265 6c3d 224c 6f67 6f22 202f 3e0a  label="Logo" />.
-000004e0: 2020 2020 3c69 6e6b 7363 6170 653a 7061      <inkscape:pa
-000004f0: 6765 0a20 2020 2020 2020 783d 222d 302e  ge.       x="-0.
-00000500: 3638 3031 3539 3633 220a 2020 2020 2020  68015963".      
-00000510: 2079 3d22 3235 302e 3632 3835 3422 0a20   y="250.62854". 
-00000520: 2020 2020 2020 7769 6474 683d 2232 3536        width="256
-00000530: 220a 2020 2020 2020 2068 6569 6768 743d  ".       height=
-00000540: 2232 3536 220a 2020 2020 2020 2069 643d  "256".       id=
-00000550: 2270 6167 6533 3238 220a 2020 2020 2020  "page328".      
-00000560: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
-00000570: 2249 636f 6e32 3536 2220 2f3e 0a20 2020  "Icon256" />.   
-00000580: 203c 696e 6b73 6361 7065 3a70 6167 650a   <inkscape:page.
-00000590: 2020 2020 2020 2078 3d22 3331 312e 3635         x="311.65
-000005a0: 3437 3222 0a20 2020 2020 2020 793d 2232  472".       y="2
-000005b0: 3539 2e34 3130 3433 220a 2020 2020 2020  59.41043".      
-000005c0: 2077 6964 7468 3d22 3132 3822 0a20 2020   width="128".   
-000005d0: 2020 2020 6865 6967 6874 3d22 3132 3822      height="128"
-000005e0: 0a20 2020 2020 2020 6964 3d22 7061 6765  .       id="page
-000005f0: 3338 3122 0a20 2020 2020 2020 696e 6b73  381".       inks
-00000600: 6361 7065 3a6c 6162 656c 3d22 4963 6f6e  cape:label="Icon
-00000610: 3132 3822 202f 3e0a 2020 2020 3c69 6e6b  128" />.    <ink
-00000620: 7363 6170 653a 7061 6765 0a20 2020 2020  scape:page.     
-00000630: 2020 783d 2233 3136 2e32 3732 3634 220a    x="316.27264".
-00000640: 2020 2020 2020 2079 3d22 3431 382e 3937         y="418.97
-00000650: 3837 3622 0a20 2020 2020 2020 7769 6474  876".       widt
-00000660: 683d 2236 3422 0a20 2020 2020 2020 6865  h="64".       he
-00000670: 6967 6874 3d22 3634 220a 2020 2020 2020  ight="64".      
-00000680: 2069 643d 2270 6167 6533 3833 220a 2020   id="page383".  
-00000690: 2020 2020 2069 6e6b 7363 6170 653a 6c61       inkscape:la
-000006a0: 6265 6c3d 2249 636f 6e36 3422 0a20 2020  bel="Icon64".   
-000006b0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-000006c0: 6f72 742d 6669 6c65 6e61 6d65 3d22 2e2f  ort-filename="./
-000006d0: 4963 6f6e 3634 2e70 6e67 220a 2020 2020  Icon64.png".    
-000006e0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-000006f0: 7274 2d78 6470 693d 2239 3622 0a20 2020  rt-xdpi="96".   
-00000700: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00000710: 6f72 742d 7964 7069 3d22 3936 2220 2f3e  ort-ydpi="96" />
-00000720: 0a20 2020 203c 696e 6b73 6361 7065 3a70  .    <inkscape:p
-00000730: 6167 650a 2020 2020 2020 2078 3d22 3436  age.       x="46
-00000740: 382e 3832 3332 3422 0a20 2020 2020 2020  8.82324".       
-00000750: 793d 2232 3631 2e33 3132 3431 220a 2020  y="261.31241".  
-00000760: 2020 2020 2077 6964 7468 3d22 3332 220a       width="32".
-00000770: 2020 2020 2020 2068 6569 6768 743d 2233         height="3
-00000780: 3222 0a20 2020 2020 2020 6964 3d22 7061  2".       id="pa
-00000790: 6765 3338 3522 0a20 2020 2020 2020 696e  ge385".       in
-000007a0: 6b73 6361 7065 3a6c 6162 656c 3d22 4963  kscape:label="Ic
-000007b0: 6f6e 3332 2220 2f3e 0a20 2020 203c 696e  on32" />.    <in
-000007c0: 6b73 6361 7065 3a70 6167 650a 2020 2020  kscape:page.    
-000007d0: 2020 2078 3d22 3437 302e 3931 3434 3322     x="470.91443"
-000007e0: 0a20 2020 2020 2020 793d 2233 3236 2e30  .       y="326.0
-000007f0: 3831 3032 220a 2020 2020 2020 2077 6964  8102".       wid
-00000800: 7468 3d22 3136 220a 2020 2020 2020 2068  th="16".       h
-00000810: 6569 6768 743d 2231 3622 0a20 2020 2020  eight="16".     
-00000820: 2020 6964 3d22 7061 6765 3338 3722 0a20    id="page387". 
-00000830: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
-00000840: 6162 656c 3d22 4963 6f6e 3136 2220 2f3e  abel="Icon16" />
-00000850: 0a20 2020 203c 696e 6b73 6361 7065 3a70  .    <inkscape:p
-00000860: 6167 650a 2020 2020 2020 2078 3d22 3430  age.       x="40
-00000870: 352e 3639 3738 3122 0a20 2020 2020 2020  5.69781".       
-00000880: 793d 2234 3236 2e31 3333 3234 220a 2020  y="426.13324".  
-00000890: 2020 2020 2077 6964 7468 3d22 3438 220a       width="48".
-000008a0: 2020 2020 2020 2068 6569 6768 743d 2234         height="4
-000008b0: 3822 0a20 2020 2020 2020 6964 3d22 7061  8".       id="pa
-000008c0: 6765 3738 3032 220a 2020 2020 2020 2069  ge7802".       i
-000008d0: 6e6b 7363 6170 653a 6c61 6265 6c3d 2249  nkscape:label="I
-000008e0: 636f 6e34 3822 0a20 2020 2020 2020 696e  con48".       in
-000008f0: 6b73 6361 7065 3a65 7870 6f72 742d 6669  kscape:export-fi
-00000900: 6c65 6e61 6d65 3d22 2e2f 4963 6f6e 3438  lename="./Icon48
-00000910: 2e70 6e67 220a 2020 2020 2020 2069 6e6b  .png".       ink
-00000920: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-00000930: 693d 2239 3622 0a20 2020 2020 2020 696e  i="96".       in
-00000940: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00000950: 7069 3d22 3936 2220 2f3e 0a20 2020 203c  pi="96" />.    <
-00000960: 696e 6b73 6361 7065 3a70 6167 650a 2020  inkscape:page.  
-00000970: 2020 2020 2078 3d22 3435 3022 0a20 2020       x="450".   
-00000980: 2020 2020 793d 222d 312e 3835 3230 3631      y="-1.852061
-00000990: 3165 2d30 3622 0a20 2020 2020 2020 7769  1e-06".       wi
-000009a0: 6474 683d 2234 3030 220a 2020 2020 2020  dth="400".      
-000009b0: 2068 6569 6768 743d 2232 3030 220a 2020   height="200".  
-000009c0: 2020 2020 2069 643d 2270 6167 6536 3532       id="page652
-000009d0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-000009e0: 653a 6c61 6265 6c3d 224c 6f67 6f5f 626c  e:label="Logo_bl
-000009f0: 6163 6b22 0a20 2020 2020 2020 696e 6b73  ack".       inks
-00000a00: 6361 7065 3a65 7870 6f72 742d 6669 6c65  cape:export-file
-00000a10: 6e61 6d65 3d22 2e2e 2f62 6237 6635 3866  name="../bb7f58f
-00000a20: 352f 4c6f 676f 5f62 6c61 636b 2e70 6e67  5/Logo_black.png
-00000a30: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00000a40: 653a 6578 706f 7274 2d78 6470 693d 2239  e:export-xdpi="9
-00000a50: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
-00000a60: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-00000a70: 3936 2220 2f3e 0a20 2020 203c 696e 6b73  96" />.    <inks
-00000a80: 6361 7065 3a70 6167 650a 2020 2020 2020  cape:page.      
-00000a90: 2078 3d22 3930 3022 0a20 2020 2020 2020   x="900".       
-00000aa0: 793d 222d 312e 3835 3230 3631 3165 2d30  y="-1.8520611e-0
-00000ab0: 3622 0a20 2020 2020 2020 7769 6474 683d  6".       width=
-00000ac0: 2234 3030 220a 2020 2020 2020 2068 6569  "400".       hei
-00000ad0: 6768 743d 2232 3030 220a 2020 2020 2020  ght="200".      
-00000ae0: 2069 643d 2270 6167 6532 3031 3422 202f   id="page2014" /
-00000af0: 3e0a 2020 3c2f 736f 6469 706f 6469 3a6e  >.  </sodipodi:n
-00000b00: 616d 6564 7669 6577 3e0a 2020 3c64 6566  amedview>.  <def
-00000b10: 730a 2020 2020 2069 643d 2264 6566 7332  s.     id="defs2
-00000b20: 223e 0a20 2020 203c 6669 6c74 6572 0a20  ">.    <filter. 
-00000b30: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00000b40: 6f6c 6c65 6374 3d22 616c 7761 7973 220a  ollect="always".
-00000b50: 2020 2020 2020 2073 7479 6c65 3d22 636f         style="co
-00000b60: 6c6f 722d 696e 7465 7270 6f6c 6174 696f  lor-interpolatio
-00000b70: 6e2d 6669 6c74 6572 733a 7352 4742 220a  n-filters:sRGB".
-00000b80: 2020 2020 2020 2069 643d 2266 696c 7465         id="filte
-00000b90: 7231 3530 3531 220a 2020 2020 2020 2078  r15051".       x
-00000ba0: 3d22 2d30 2e31 3637 3333 3430 3622 0a20  ="-0.16733406". 
-00000bb0: 2020 2020 2020 7769 6474 683d 2231 2e33        width="1.3
-00000bc0: 3334 3636 3831 220a 2020 2020 2020 2079  346681".       y
-00000bd0: 3d22 2d30 2e36 3532 3938 3433 3522 0a20  ="-0.65298435". 
-00000be0: 2020 2020 2020 6865 6967 6874 3d22 322e        height="2.
-00000bf0: 3330 3539 3638 3722 3e0a 2020 2020 2020  3059687">.      
-00000c00: 3c66 6547 6175 7373 6961 6e42 6c75 720a  <feGaussianBlur.
-00000c10: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-00000c20: 653a 636f 6c6c 6563 743d 2261 6c77 6179  e:collect="alway
-00000c30: 7322 0a20 2020 2020 2020 2020 7374 6444  s".         stdD
-00000c40: 6576 6961 7469 6f6e 3d22 352e 3232 3630  eviation="5.2260
-00000c50: 3230 3922 0a20 2020 2020 2020 2020 6964  209".         id
-00000c60: 3d22 6665 4761 7573 7369 616e 426c 7572  ="feGaussianBlur
-00000c70: 3135 3035 3322 202f 3e0a 2020 2020 3c2f  15053" />.    </
-00000c80: 6669 6c74 6572 3e0a 2020 2020 3c66 696c  filter>.    <fil
-00000c90: 7465 720a 2020 2020 2020 2069 6e6b 7363  ter.       inksc
-00000ca0: 6170 653a 636f 6c6c 6563 743d 2261 6c77  ape:collect="alw
-00000cb0: 6179 7322 0a20 2020 2020 2020 7374 796c  ays".       styl
-00000cc0: 653d 2263 6f6c 6f72 2d69 6e74 6572 706f  e="color-interpo
-00000cd0: 6c61 7469 6f6e 2d66 696c 7465 7273 3a73  lation-filters:s
-00000ce0: 5247 4222 0a20 2020 2020 2020 6964 3d22  RGB".       id="
-00000cf0: 6669 6c74 6572 3135 3035 312d 3322 0a20  filter15051-3". 
-00000d00: 2020 2020 2020 783d 222d 302e 3136 3733        x="-0.1673
-00000d10: 3334 3036 220a 2020 2020 2020 2077 6964  3406".       wid
-00000d20: 7468 3d22 312e 3333 3436 3638 3122 0a20  th="1.3346681". 
-00000d30: 2020 2020 2020 793d 222d 302e 3635 3239        y="-0.6529
-00000d40: 3834 3335 220a 2020 2020 2020 2068 6569  8435".       hei
-00000d50: 6768 743d 2232 2e33 3035 3936 3837 223e  ght="2.3059687">
-00000d60: 0a20 2020 2020 203c 6665 4761 7573 7369  .      <feGaussi
-00000d70: 616e 426c 7572 0a20 2020 2020 2020 2020  anBlur.         
-00000d80: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
-00000d90: 3d22 616c 7761 7973 220a 2020 2020 2020  ="always".      
-00000da0: 2020 2073 7464 4465 7669 6174 696f 6e3d     stdDeviation=
-00000db0: 2235 2e32 3236 3032 3039 220a 2020 2020  "5.2260209".    
-00000dc0: 2020 2020 2069 643d 2266 6547 6175 7373       id="feGauss
-00000dd0: 6961 6e42 6c75 7231 3530 3533 2d36 2220  ianBlur15053-6" 
-00000de0: 2f3e 0a20 2020 203c 2f66 696c 7465 723e  />.    </filter>
-00000df0: 0a20 2020 203c 6669 6c74 6572 0a20 2020  .    <filter.   
-00000e00: 2020 2020 696e 6b73 6361 7065 3a63 6f6c      inkscape:col
-00000e10: 6c65 6374 3d22 616c 7761 7973 220a 2020  lect="always".  
-00000e20: 2020 2020 2073 7479 6c65 3d22 636f 6c6f       style="colo
-00000e30: 722d 696e 7465 7270 6f6c 6174 696f 6e2d  r-interpolation-
-00000e40: 6669 6c74 6572 733a 7352 4742 220a 2020  filters:sRGB".  
-00000e50: 2020 2020 2069 643d 2266 696c 7465 7231       id="filter1
-00000e60: 3530 3531 2d33 2d32 220a 2020 2020 2020  5051-3-2".      
-00000e70: 2078 3d22 2d30 2e31 3637 3333 3430 3622   x="-0.16733406"
-00000e80: 0a20 2020 2020 2020 7769 6474 683d 2231  .       width="1
-00000e90: 2e33 3334 3636 3831 220a 2020 2020 2020  .3346681".      
-00000ea0: 2079 3d22 2d30 2e36 3532 3938 3433 3522   y="-0.65298435"
-00000eb0: 0a20 2020 2020 2020 6865 6967 6874 3d22  .       height="
-00000ec0: 322e 3330 3539 3638 3722 3e0a 2020 2020  2.3059687">.    
-00000ed0: 2020 3c66 6547 6175 7373 6961 6e42 6c75    <feGaussianBlu
-00000ee0: 720a 2020 2020 2020 2020 2069 6e6b 7363  r.         inksc
-00000ef0: 6170 653a 636f 6c6c 6563 743d 2261 6c77  ape:collect="alw
-00000f00: 6179 7322 0a20 2020 2020 2020 2020 7374  ays".         st
-00000f10: 6444 6576 6961 7469 6f6e 3d22 352e 3232  dDeviation="5.22
-00000f20: 3630 3230 3922 0a20 2020 2020 2020 2020  60209".         
-00000f30: 6964 3d22 6665 4761 7573 7369 616e 426c  id="feGaussianBl
-00000f40: 7572 3135 3035 332d 362d 3222 202f 3e0a  ur15053-6-2" />.
-00000f50: 2020 2020 3c2f 6669 6c74 6572 3e0a 2020      </filter>.  
-00000f60: 3c2f 6465 6673 3e0a 2020 3c67 0a20 2020  </defs>.  <g.   
-00000f70: 2020 696e 6b73 6361 7065 3a6c 6162 656c    inkscape:label
-00000f80: 3d22 4c61 7965 7220 3122 0a20 2020 2020  ="Layer 1".     
-00000f90: 696e 6b73 6361 7065 3a67 726f 7570 6d6f  inkscape:groupmo
-00000fa0: 6465 3d22 6c61 7965 7222 0a20 2020 2020  de="layer".     
-00000fb0: 6964 3d22 6c61 7965 7231 223e 0a20 2020  id="layer1">.   
-00000fc0: 203c 7265 6374 0a20 2020 2020 2020 7374   <rect.       st
-00000fd0: 796c 653d 2266 696c 6c3a 2366 6666 6666  yle="fill:#fffff
-00000fe0: 663b 7374 726f 6b65 3a6e 6f6e 653b 7374  f;stroke:none;st
-00000ff0: 726f 6b65 2d77 6964 7468 3a35 2e30 3834  roke-width:5.084
-00001000: 3736 3b73 7472 6f6b 652d 6c69 6e65 6361  76;stroke-lineca
-00001010: 703a 726f 756e 643b 7374 726f 6b65 2d6c  p:round;stroke-l
-00001020: 696e 656a 6f69 6e3a 726f 756e 643b 6669  inejoin:round;fi
-00001030: 6c6c 2d6f 7061 6369 7479 3a30 2e30 3230  ll-opacity:0.020
-00001040: 3039 3730 3622 0a20 2020 2020 2020 6964  09706".       id
-00001050: 3d22 7265 6374 3730 3622 0a20 2020 2020  ="rect706".     
-00001060: 2020 7769 6474 683d 2234 3030 220a 2020    width="400".  
-00001070: 2020 2020 2068 6569 6768 743d 2232 3030       height="200
-00001080: 220a 2020 2020 2020 2078 3d22 2d36 2e36  ".       x="-6.6
-00001090: 3936 3531 3331 652d 3036 220a 2020 2020  965131e-06".    
-000010a0: 2020 2079 3d22 2d31 2e38 3532 3036 3131     y="-1.8520611
-000010b0: 652d 3036 220a 2020 2020 2020 2072 793d  e-06".       ry=
-000010c0: 2230 2220 2f3e 0a20 2020 203c 7061 7468  "0" />.    <path
-000010d0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-000010e0: 696c 6c3a 2330 3030 3030 303b 6669 6c6c  ill:#000000;fill
-000010f0: 2d6f 7061 6369 7479 3a30 2e39 3938 3430  -opacity:0.99840
-00001100: 383b 7374 726f 6b65 3a23 3030 3030 3030  8;stroke:#000000
-00001110: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00001120: 3530 3030 3232 7078 3b73 7472 6f6b 652d  500022px;stroke-
-00001130: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00001140: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00001150: 6572 3b73 7472 6f6b 652d 6f70 6163 6974  er;stroke-opacit
-00001160: 793a 3122 0a20 2020 2020 2020 643d 224d  y:1".       d="M
-00001170: 2031 3733 2e38 3438 3131 2c38 392e 3036   173.84811,89.06
-00001180: 3935 3120 3333 372e 3635 3039 362c 3634  951 337.65096,64
-00001190: 2e39 3439 3731 2031 3731 2e38 3734 3435  .94971 171.87445
-000011a0: 2c38 302e 3731 3433 3620 5a22 0a20 2020  ,80.71436 Z".   
-000011b0: 2020 2020 6964 3d22 7061 7468 3134 3635      id="path1465
-000011c0: 3722 0a20 2020 2020 2020 696e 6b73 6361  7".       inksca
-000011d0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-000011e0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-000011f0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-00001200: 7970 6573 3d22 6363 6363 2220 2f3e 0a20  ypes="cccc" />. 
-00001210: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00001220: 7374 796c 653d 2266 696c 6c3a 2333 6534  style="fill:#3e4
-00001230: 6237 373b 6669 6c6c 2d6f 7061 6369 7479  b77;fill-opacity
-00001240: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-00001250: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
-00001260: 2e30 3530 3035 3b73 7472 6f6b 652d 6c69  .05005;stroke-li
-00001270: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00001280: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00001290: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-000012a0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-000012b0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-000012c0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000012d0: 2020 2020 643d 224d 2031 392e 3630 3330      d="M 19.6030
-000012e0: 372c 3637 2e36 3536 3920 3830 2e38 3538  7,67.6569 80.858
-000012f0: 3032 382c 3634 2e38 3835 3132 2031 3231  028,64.88512 121
-00001300: 2e31 3034 3035 2c32 302e 3238 3435 3420  .10405,20.28454 
-00001310: 4320 3730 2e34 3032 3538 372c 3534 2e32  C 70.402587,54.2
-00001320: 3238 3733 2034 362e 3137 3936 3035 2c35  2873 46.179605,5
-00001330: 392e 3637 3633 3720 3139 2e36 3033 3037  9.67637 19.60307
-00001340: 2c36 372e 3635 3639 205a 220a 2020 2020  ,67.6569 Z".    
-00001350: 2020 2069 643d 2270 6174 6831 3435 3437     id="path14547
-00001360: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00001370: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00001380: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
-00001390: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-000013a0: 7065 733d 2263 6363 6322 202f 3e0a 2020  pes="cccc" />.  
-000013b0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-000013c0: 7479 6c65 3d22 6669 6c6c 3a23 3163 3263  tyle="fill:#1c2c
-000013d0: 3638 3b66 696c 6c2d 6f70 6163 6974 793a  68;fill-opacity:
-000013e0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-000013f0: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
-00001400: 3035 3030 353b 7374 726f 6b65 2d6c 696e  05005;stroke-lin
-00001410: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-00001420: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-00001430: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00001440: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00001450: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00001460: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00001470: 2020 2064 3d22 6d20 3830 2e38 3538 3032     d="m 80.85802
-00001480: 382c 3634 2e38 3835 3132 2032 362e 3537  8,64.88512 26.57
-00001490: 3735 3632 2c36 2e30 3437 3534 2031 332e  7562,6.04754 13.
-000014a0: 3636 3834 362c 2d35 302e 3634 3831 3220  66846,-50.64812 
-000014b0: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
-000014c0: 7468 3134 3534 3922 0a20 2020 2020 2020  th14549".       
-000014d0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-000014e0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-000014f0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
-00001500: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00001510: 3a23 3036 3035 3038 3b66 696c 6c2d 6f70  :#060508;fill-op
-00001520: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-00001530: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-00001540: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
-00001550: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-00001560: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-00001570: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-00001580: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00001590: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-000015a0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-000015b0: 220a 2020 2020 2020 2064 3d22 4d20 3130  ".       d="M 10
-000015c0: 372e 3433 3535 392c 3730 2e39 3332 3636  7.43559,70.93266
-000015d0: 2031 3738 2e35 3632 3233 2c38 332e 3533   178.56223,83.53
-000015e0: 3137 2043 2031 3530 2e38 3435 3431 2c36  17 C 150.84541,6
-000015f0: 382e 3934 3439 3720 3133 342e 3739 3530  8.94497 134.7950
-00001600: 312c 3435 2e35 3039 3535 2031 3231 2e31  1,45.50955 121.1
-00001610: 3034 3035 2c32 302e 3238 3435 3420 5a22  0405,20.28454 Z"
-00001620: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00001630: 3134 3535 3122 0a20 2020 2020 2020 696e  14551".       in
-00001640: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00001650: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00001660: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00001670: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
-00001680: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00001690: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-000016a0: 2332 3733 3737 333b 6669 6c6c 2d6f 7061  #273773;fill-opa
-000016b0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-000016c0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-000016d0: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
-000016e0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-000016f0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00001700: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00001710: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00001720: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00001730: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00001740: 0a20 2020 2020 2020 643d 226d 2031 392e  .       d="m 19.
-00001750: 3630 3330 372c 3637 2e36 3536 3920 6320  60307,67.6569 c 
-00001760: 3133 2e34 3739 3331 322c 372e 3639 3738  13.479312,7.6978
-00001770: 2032 382e 3334 3131 3037 2c31 342e 3333   28.341107,14.33
-00001780: 3639 3520 3333 2e34 3131 3739 362c 3238  695 33.411796,28
-00001790: 2e34 3733 3832 206c 2032 372e 3834 3331  .47382 l 27.8431
-000017a0: 3632 2c2d 3331 2e32 3435 3620 7a22 0a20  62,-31.2456 z". 
-000017b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-000017c0: 3535 3322 0a20 2020 2020 2020 696e 6b73  553".       inks
-000017d0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-000017e0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-000017f0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-00001800: 6574 7970 6573 3d22 6363 6363 2220 2f3e  etypes="cccc" />
-00001810: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-00001820: 2020 7374 796c 653d 2266 696c 6c3a 2331    style="fill:#1
-00001830: 3432 3637 323b 6669 6c6c 2d6f 7061 6369  42672;fill-opaci
-00001840: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-00001850: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00001860: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
-00001870: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00001880: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00001890: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-000018a0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-000018b0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-000018c0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-000018d0: 2020 2020 2020 643d 224d 2035 332e 3031        d="M 53.01
-000018e0: 3438 3636 2c39 362e 3133 3037 3220 3137  4866,96.13072 17
-000018f0: 382e 3536 3232 332c 3833 2e35 3331 3720  8.56223,83.5317 
-00001900: 3830 2e38 3538 3032 382c 3634 2e38 3835  80.858028,64.885
-00001910: 3132 205a 220a 2020 2020 2020 2069 643d  12 Z".       id=
-00001920: 2270 6174 6831 3435 3535 220a 2020 2020  "path14555".    
-00001930: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00001940: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00001950: 2230 2220 2f3e 0a20 2020 203c 7061 7468  "0" />.    <path
-00001960: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00001970: 696c 6c3a 2335 3436 3638 633b 6669 6c6c  ill:#54668c;fill
-00001980: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00001990: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-000019a0: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
-000019b0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-000019c0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-000019d0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-000019e0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-000019f0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00001a00: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00001a10: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00001a20: 2035 332e 3031 3438 3636 2c39 362e 3133   53.014866,96.13
-00001a30: 3037 3220 3732 2e33 3932 3232 342c 372e  072 72.392224,7.
-00001a40: 3535 3934 3420 3533 2e31 3535 3134 2c2d  55944 53.15514,-
-00001a50: 3230 2e31 3538 3436 207a 220a 2020 2020  20.15846 z".    
-00001a60: 2020 2069 643d 2270 6174 6831 3435 3537     id="path14557
-00001a70: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00001a80: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00001a90: 6174 7572 653d 2230 2220 2f3e 0a20 2020  ature="0" />.   
-00001aa0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-00001ab0: 796c 653d 2266 696c 6c3a 2332 3233 3437  yle="fill:#22347
-00001ac0: 653b 6669 6c6c 2d6f 7061 6369 7479 3a31  e;fill-opacity:1
-00001ad0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-00001ae0: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
-00001af0: 3530 3035 3b73 7472 6f6b 652d 6c69 6e65  5005;stroke-line
-00001b00: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00001b10: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00001b20: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00001b30: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00001b40: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00001b50: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00001b60: 2020 643d 226d 2035 332e 3031 3438 3636    d="m 53.014866
-00001b70: 2c39 362e 3133 3037 3220 6320 312e 3632  ,96.13072 c 1.62
-00001b80: 3738 3235 2c31 332e 3937 3235 3220 2d34  7825,13.97252 -4
-00001b90: 2e30 3036 3737 322c 3232 2e37 3830 3933  .006772,22.78093
-00001ba0: 202d 362e 3538 3131 3039 2c33 332e 3736   -6.581109,33.76
-00001bb0: 3534 3120 6c20 3738 2e39 3733 3333 332c  541 l 78.973333,
-00001bc0: 2d32 362e 3230 3539 3720 7a22 0a20 2020  -26.20597 z".   
-00001bd0: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
-00001be0: 3922 0a20 2020 2020 2020 696e 6b73 6361  9".       inksca
-00001bf0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-00001c00: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-00001c10: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-00001c20: 7970 6573 3d22 6363 6363 2220 2f3e 0a20  ypes="cccc" />. 
-00001c30: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00001c40: 7374 796c 653d 2266 696c 6c3a 2330 3831  style="fill:#081
-00001c50: 3036 393b 6669 6c6c 2d6f 7061 6369 7479  069;fill-opacity
-00001c60: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-00001c70: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
-00001c80: 2e30 3530 3035 3b73 7472 6f6b 652d 6c69  .05005;stroke-li
-00001c90: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00001ca0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00001cb0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00001cc0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00001cd0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00001ce0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00001cf0: 2020 2020 643d 224d 2034 362e 3433 3337      d="M 46.4337
-00001d00: 3537 2c31 3239 2e38 3936 3133 2031 3031  57,129.89613 101
-00001d10: 2e31 3037 362c 3133 372e 3935 3935 3120  .1076,137.95951 
-00001d20: 3137 382e 3536 3232 332c 3833 2e35 3331  178.56223,83.531
-00001d30: 3720 5a22 0a20 2020 2020 2020 6964 3d22  7 Z".       id="
-00001d40: 7061 7468 3134 3536 3122 0a20 2020 2020  path14561".     
-00001d50: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00001d60: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00001d70: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
-00001d80: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00001d90: 6c6c 3a23 3037 3065 3262 3b66 696c 6c2d  ll:#070e2b;fill-
-00001da0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00001db0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00001dc0: 7769 6474 683a 312e 3035 3030 353b 7374  width:1.05005;st
-00001dd0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00001de0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00001df0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-00001e00: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00001e10: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00001e20: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-00001e30: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
-00001e40: 3130 312e 3130 3736 2c31 3337 2e39 3539  101.1076,137.959
-00001e50: 3531 2033 322e 3134 3631 392c 3432 2e30  51 32.14619,42.0
-00001e60: 3830 3739 202d 3131 2e38 3936 3632 2c2d  8079 -11.89662,-
-00001e70: 3536 2e36 3935 3636 207a 220a 2020 2020  56.69566 z".    
-00001e80: 2020 2069 643d 2270 6174 6831 3435 3633     id="path14563
-00001e90: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00001ea0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00001eb0: 6174 7572 653d 2230 2220 2f3e 0a20 2020  ature="0" />.   
-00001ec0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-00001ed0: 796c 653d 2266 696c 6c3a 2332 3833 6438  yle="fill:#283d8
-00001ee0: 373b 6669 6c6c 2d6f 7061 6369 7479 3a31  7;fill-opacity:1
-00001ef0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-00001f00: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
-00001f10: 3530 3035 3b73 7472 6f6b 652d 6c69 6e65  5005;stroke-line
-00001f20: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-00001f30: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-00001f40: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00001f50: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00001f60: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00001f70: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00001f80: 2020 643d 226d 2031 3231 2e33 3537 3137    d="m 121.35717
-00001f90: 2c31 3233 2e33 3434 3634 2031 312e 3839  ,123.34464 11.89
-00001fa0: 3636 322c 3536 2e36 3935 3636 2063 2036  662,56.69566 c 6
-00001fb0: 2e31 3538 3632 2c2d 3530 2e39 3636 3733  .15862,-50.96673
-00001fc0: 2032 372e 3833 3134 372c 2d36 392e 3332   27.83147,-69.32
-00001fd0: 3836 3120 3435 2e33 3038 3434 2c2d 3936  861 45.30844,-96
-00001fe0: 2e35 3038 3620 7a22 0a20 2020 2020 2020  .5086 z".       
-00001ff0: 6964 3d22 7061 7468 3134 3536 3522 0a20  id="path14565". 
-00002000: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00002010: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00002020: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
-00002030: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00002040: 3d22 6363 6363 2220 2f3e 0a20 2020 203c  ="cccc" />.    <
-00002050: 656c 6c69 7073 650a 2020 2020 2020 2073  ellipse.       s
-00002060: 7479 6c65 3d22 6669 6c6c 3a23 3037 3065  tyle="fill:#070e
-00002070: 3262 3b66 696c 6c2d 6f70 6163 6974 793a  2b;fill-opacity:
-00002080: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
-00002090: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-000020a0: 6964 7468 3a31 2e30 3530 3035 3b73 7472  idth:1.05005;str
-000020b0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-000020c0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000020d0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-000020e0: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-000020f0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00002100: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-00002110: 3722 0a20 2020 2020 2020 6378 3d22 3230  7".       cx="20
-00002120: 2e39 3033 3131 3822 0a20 2020 2020 2020  .903118".       
-00002130: 6379 3d22 3637 2e37 3231 3538 3822 0a20  cy="67.721588". 
-00002140: 2020 2020 2020 7278 3d22 332e 3135 3632        rx="3.1562
-00002150: 3236 3422 0a20 2020 2020 2020 7279 3d22  264".       ry="
-00002160: 332e 3134 3230 3234 2220 2f3e 0a20 2020  3.142024" />.   
-00002170: 203c 656c 6c69 7073 650a 2020 2020 2020   <ellipse.      
-00002180: 2073 7479 6c65 3d22 6669 6c6c 3a23 3235   style="fill:#25
-00002190: 3361 3764 3b66 696c 6c2d 6f70 6163 6974  3a7d;fill-opacit
-000021a0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-000021b0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-000021c0: 312e 3035 3030 353b 7374 726f 6b65 2d6d  1.05005;stroke-m
-000021d0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-000021e0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-000021f0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-00002200: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-00002210: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
-00002220: 643d 2270 6174 6831 3435 3637 2d33 220a  d="path14567-3".
-00002230: 2020 2020 2020 2063 783d 2234 352e 3932         cx="45.92
-00002240: 3538 3436 220a 2020 2020 2020 2063 793d  5846".       cy=
-00002250: 2231 3239 2e32 3235 3838 220a 2020 2020  "129.22588".    
-00002260: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
-00002270: 7366 6f72 6d2d 6365 6e74 6572 2d78 3d22  sform-center-x="
-00002280: 322e 3332 3639 3734 3522 0a20 2020 2020  2.3269745".     
-00002290: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
-000022a0: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
-000022b0: 342e 3937 3830 3136 3322 0a20 2020 2020  4.9780163".     
-000022c0: 2020 7278 3d22 332e 3135 3632 3236 3422    rx="3.1562264"
-000022d0: 0a20 2020 2020 2020 7279 3d22 332e 3134  .       ry="3.14
-000022e0: 3230 3234 2220 2f3e 0a20 2020 203c 656c  2024" />.    <el
-000022f0: 6c69 7073 650a 2020 2020 2020 2073 7479  lipse.       sty
-00002300: 6c65 3d22 6669 6c6c 3a23 3235 3361 3764  le="fill:#253a7d
-00002310: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-00002320: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00002330: 7472 6f6b 652d 7769 6474 683a 312e 3035  troke-width:1.05
-00002340: 3030 353b 7374 726f 6b65 2d6d 6974 6572  005;stroke-miter
-00002350: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00002360: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00002370: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
-00002380: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
-00002390: 3a31 220a 2020 2020 2020 2069 643d 2270  :1".       id="p
-000023a0: 6174 6831 3435 3637 2d33 2d37 220a 2020  ath14567-3-7".  
-000023b0: 2020 2020 2063 783d 2231 3230 2e35 3838       cx="120.588
-000023c0: 3632 220a 2020 2020 2020 2063 793d 2231  62".       cy="1
-000023d0: 3033 2e38 3931 3339 220a 2020 2020 2020  03.89139".      
-000023e0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-000023f0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
-00002400: 3332 3639 3739 3222 0a20 2020 2020 2020  3269792".       
-00002410: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-00002420: 726d 2d63 656e 7465 722d 793d 222d 342e  rm-center-y="-4.
-00002430: 3937 3830 3230 3422 0a20 2020 2020 2020  9780204".       
-00002440: 7278 3d22 332e 3135 3632 3236 3422 0a20  rx="3.1562264". 
-00002450: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
-00002460: 3234 2220 2f3e 0a20 2020 203c 656c 6c69  24" />.    <elli
-00002470: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
-00002480: 3d22 6669 6c6c 3a23 6138 6139 6161 3b66  ="fill:#a8a9aa;f
-00002490: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-000024a0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-000024b0: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
-000024c0: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
-000024d0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-000024e0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-000024f0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-00002500: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00002510: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-00002520: 6831 3435 3637 2d33 2d35 220a 2020 2020  h14567-3-5".    
-00002530: 2020 2063 783d 2231 3231 2e33 3337 3134     cx="121.33714
-00002540: 220a 2020 2020 2020 2063 793d 2231 3232  ".       cy="122
-00002550: 2e38 3932 3234 220a 2020 2020 2020 2069  .89224".       i
-00002560: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-00002570: 6d2d 6365 6e74 6572 2d78 3d22 322e 3332  m-center-x="2.32
-00002580: 3639 3637 220a 2020 2020 2020 2069 6e6b  6967".       ink
-00002590: 7363 6170 653a 7472 616e 7366 6f72 6d2d  scape:transform-
-000025a0: 6365 6e74 6572 2d79 3d22 2d34 2e39 3738  center-y="-4.978
-000025b0: 3030 3539 220a 2020 2020 2020 2072 783d  0059".       rx=
-000025c0: 2233 2e31 3536 3232 3634 220a 2020 2020  "3.1562264".    
-000025d0: 2020 2072 793d 2233 2e31 3432 3032 3422     ry="3.142024"
-000025e0: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
-000025f0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00002600: 696c 6c3a 2361 6261 6139 633b 6669 6c6c  ill:#abaa9c;fill
-00002610: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00002620: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00002630: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
-00002640: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00002650: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00002660: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00002670: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00002680: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00002690: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-000026a0: 3536 372d 332d 3922 0a20 2020 2020 2020  567-3-9".       
-000026b0: 6378 3d22 3130 312e 3837 3631 3422 0a20  cx="101.87614". 
-000026c0: 2020 2020 2020 6379 3d22 3133 372e 3739        cy="137.79
-000026d0: 3438 3522 0a20 2020 2020 2020 696e 6b73  485".       inks
-000026e0: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
-000026f0: 656e 7465 722d 783d 2232 2e33 3236 3937  enter-x="2.32697
-00002700: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
-00002710: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-00002720: 7465 722d 793d 222d 342e 3937 3830 3235  ter-y="-4.978025
-00002730: 3122 0a20 2020 2020 2020 7278 3d22 332e  1".       rx="3.
-00002740: 3135 3632 3236 3422 0a20 2020 2020 2020  1562264".       
-00002750: 7279 3d22 332e 3134 3230 3234 2220 2f3e  ry="3.142024" />
-00002760: 0a20 2020 203c 656c 6c69 7073 650a 2020  .    <ellipse.  
-00002770: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00002780: 3a23 3131 3230 3636 3b66 696c 6c2d 6f70  :#112066;fill-op
-00002790: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-000027a0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-000027b0: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
-000027c0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-000027d0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-000027e0: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-000027f0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-00002800: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00002810: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-00002820: 2d33 2d32 220a 2020 2020 2020 2063 783d  -3-2".       cx=
-00002830: 2238 312e 3239 3234 3139 220a 2020 2020  "81.292419".    
-00002840: 2020 2063 793d 2236 342e 3231 3331 3635     cy="64.213165
-00002850: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00002860: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-00002870: 6572 2d78 3d22 332e 3539 3133 3630 3922  er-x="3.5913609"
-00002880: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00002890: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-000028a0: 722d 793d 222d 372e 3638 3238 3935 3622  r-y="-7.6828956"
-000028b0: 0a20 2020 2020 2020 7278 3d22 342e 3837  .       rx="4.87
-000028c0: 3131 3932 3922 0a20 2020 2020 2020 7279  11929".       ry
-000028d0: 3d22 342e 3834 3932 3733 3722 202f 3e0a  ="4.8492737" />.
-000028e0: 2020 2020 3c65 6c6c 6970 7365 0a20 2020      <ellipse.   
-000028f0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00002900: 2365 6466 3066 633b 6669 6c6c 2d6f 7061  #edf0fc;fill-opa
-00002910: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
-00002920: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00002930: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
-00002940: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
-00002950: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-00002960: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-00002970: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-00002980: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00002990: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-000029a0: 6831 3435 3637 2d32 220a 2020 2020 2020  h14567-2".      
-000029b0: 2063 783d 2231 3037 2e36 3737 3032 220a   cx="107.67702".
-000029c0: 2020 2020 2020 2063 793d 2236 392e 3631         cy="69.61
-000029d0: 3533 3536 220a 2020 2020 2020 2072 783d  5356".       rx=
-000029e0: 2233 2e31 3536 3232 3634 220a 2020 2020  "3.1562264".    
-000029f0: 2020 2072 793d 2233 2e31 3432 3032 3422     ry="3.142024"
-00002a00: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
-00002a10: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00002a20: 696c 6c3a 2365 6466 3066 633b 6669 6c6c  ill:#edf0fc;fill
-00002a30: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
-00002a40: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
-00002a50: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
-00002a60: 3035 3030 353b 7374 726f 6b65 2d6d 6974  05005;stroke-mit
-00002a70: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00002a80: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00002a90: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-00002aa0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-00002ab0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-00002ac0: 2270 6174 6831 3435 3637 2d32 2d38 220a  "path14567-2-8".
-00002ad0: 2020 2020 2020 2063 783d 2235 332e 3033         cx="53.03
-00002ae0: 3635 3735 220a 2020 2020 2020 2063 793d  6575".       cy=
-00002af0: 2239 352e 3639 3439 3737 220a 2020 2020  "95.694977".    
-00002b00: 2020 2072 783d 2233 2e31 3536 3232 3634     rx="3.1562264
-00002b10: 220a 2020 2020 2020 2072 793d 2233 2e31  ".       ry="3.1
-00002b20: 3432 3032 3422 202f 3e0a 2020 2020 3c70  42024" />.    <p
-00002b30: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-00002b40: 3d22 6669 6c6c 3a23 3030 3030 3030 3b66  ="fill:#000000;f
-00002b50: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
-00002b60: 3834 3038 3b73 7472 6f6b 653a 2330 3030  8408;stroke:#000
-00002b70: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
-00002b80: 3a30 2e33 3233 3538 3870 783b 7374 726f  :0.323588px;stro
-00002b90: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-00002ba0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-00002bb0: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
-00002bc0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-00002bd0: 3d22 6d20 3331 382e 3730 3133 332c 3732  ="m 318.70133,72
-00002be0: 2e37 3031 3732 2032 362e 3630 3435 372c  .70172 26.60457,
-00002bf0: 2d38 2e37 3836 3833 202d 3238 2e33 3833  -8.78683 -28.383
-00002c00: 3935 2c2d 312e 3437 3538 3620 6320 3131  95,-1.47586 c 11
-00002c10: 2e30 3035 3236 2c33 2e32 3034 3636 2031  .00526,3.20466 1
-00002c20: 312e 3035 3533 2c33 2e33 3734 3237 2031  1.0553,3.37427 1
-00002c30: 2e37 3739 3338 2c31 302e 3236 3236 3920  .77938,10.26269 
-00002c40: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
-00002c50: 7468 3134 3635 372d 3922 0a20 2020 2020  th14657-9".     
-00002c60: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00002c70: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00002c80: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
-00002c90: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00002ca0: 6363 2220 2f3e 0a20 2020 203c 656c 6c69  cc" />.    <elli
-00002cb0: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
-00002cc0: 3d22 6669 6c6c 3a23 6564 6630 6663 3b66  ="fill:#edf0fc;f
-00002cd0: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
-00002ce0: 3034 3436 3b73 7472 6f6b 653a 2366 6666  0446;stroke:#fff
-00002cf0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00002d00: 3a31 2e39 3935 3938 3b73 7472 6f6b 652d  :1.99598;stroke-
-00002d10: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00002d20: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00002d30: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
-00002d40: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
-00002d50: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00002d60: 6964 3d22 7061 7468 3134 3536 372d 322d  id="path14567-2-
-00002d70: 3722 0a20 2020 2020 2020 6378 3d22 3137  7".       cx="17
-00002d80: 372e 3437 3435 3622 0a20 2020 2020 2020  7.47456".       
-00002d90: 6379 3d22 3834 2e33 3331 3732 3622 0a20  cy="84.331726". 
-00002da0: 2020 2020 2020 7278 3d22 352e 3939 3935        rx="5.9995
-00002db0: 3232 3222 0a20 2020 2020 2020 7279 3d22  222".       ry="
-00002dc0: 352e 3937 3235 3235 3622 202f 3e0a 2020  5.9725256" />.  
-00002dd0: 2020 3c74 6578 740a 2020 2020 2020 2078    <text.       x
-00002de0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
-00002df0: 7665 220a 2020 2020 2020 2073 7479 6c65  ve".       style
-00002e00: 3d22 666f 6e74 2d73 7479 6c65 3a6e 6f72  ="font-style:nor
-00002e10: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
-00002e20: 6e6f 726d 616c 3b66 6f6e 742d 7369 7a65  normal;font-size
-00002e30: 3a35 2e38 3732 3931 7078 3b6c 696e 652d  :5.87291px;line-
-00002e40: 6865 6967 6874 3a31 2e32 353b 666f 6e74  height:1.25;font
-00002e50: 2d66 616d 696c 793a 7361 6e73 2d73 6572  -family:sans-ser
-00002e60: 6966 3b6c 6574 7465 722d 7370 6163 696e  if;letter-spacin
-00002e70: 673a 3070 783b 776f 7264 2d73 7061 6369  g:0px;word-spaci
-00002e80: 6e67 3a30 7078 3b66 696c 6c3a 2366 6666  ng:0px;fill:#fff
-00002e90: 6666 663b 6669 6c6c 2d6f 7061 6369 7479  fff;fill-opacity
-00002ea0: 3a31 3b73 7472 6f6b 653a 6e6f 6e65 3b73  :1;stroke:none;s
-00002eb0: 7472 6f6b 652d 7769 6474 683a 302e 3430  troke-width:0.40
-00002ec0: 3034 3235 3b66 696c 7465 723a 7572 6c28  0425;filter:url(
-00002ed0: 2366 696c 7465 7231 3530 3531 2922 0a20  #filter15051)". 
-00002ee0: 2020 2020 2020 783d 2237 372e 3639 3438        x="77.6948
-00002ef0: 3933 220a 2020 2020 2020 2079 3d22 3931  93".       y="91
-00002f00: 2e39 3838 3434 3922 0a20 2020 2020 2020  .988449".       
-00002f10: 6964 3d22 7465 7874 3134 3639 312d 3622  id="text14691-6"
-00002f20: 0a20 2020 2020 2020 7472 616e 7366 6f72  .       transfor
-00002f30: 6d3d 226d 6174 7269 7828 322e 3735 3131  m="matrix(2.7511
-00002f40: 3931 392c 302c 302c 322e 3733 3838 3132  919,0,0,2.738812
-00002f50: 2c2d 3735 2e39 3736 3639 362c 2d31 3038  ,-75.976696,-108
-00002f60: 2e30 3838 3636 2922 3e3c 7473 7061 6e0a  .08866)"><tspan.
-00002f70: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
-00002f80: 693a 726f 6c65 3d22 6c69 6e65 220a 2020  i:role="line".  
-00002f90: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
-00002fa0: 3134 3638 392d 3222 0a20 2020 2020 2020  14689-2".       
-00002fb0: 2020 783d 2237 372e 3639 3438 3933 220a    x="77.694893".
-00002fc0: 2020 2020 2020 2020 2079 3d22 3931 2e39           y="91.9
-00002fd0: 3838 3434 3922 0a20 2020 2020 2020 2020  88449".         
-00002fe0: 7374 796c 653d 2266 6f6e 742d 7374 796c  style="font-styl
-00002ff0: 653a 6e6f 726d 616c 3b66 6f6e 742d 7661  e:normal;font-va
-00003000: 7269 616e 743a 6e6f 726d 616c 3b66 6f6e  riant:normal;fon
-00003010: 742d 7765 6967 6874 3a6e 6f72 6d61 6c3b  t-weight:normal;
-00003020: 666f 6e74 2d73 7472 6574 6368 3a6e 6f72  font-stretch:nor
-00003030: 6d61 6c3b 666f 6e74 2d73 697a 653a 3231  mal;font-size:21
-00003040: 2e33 3536 7078 3b66 6f6e 742d 6661 6d69  .356px;font-fami
-00003050: 6c79 3a49 6d70 6163 743b 2d69 6e6b 7363  ly:Impact;-inksc
-00003060: 6170 652d 666f 6e74 2d73 7065 6369 6669  ape-font-specifi
-00003070: 6361 7469 6f6e 3a49 6d70 6163 743b 6669  cation:Impact;fi
-00003080: 6c6c 3a23 6666 6666 6666 3b66 696c 6c2d  ll:#ffffff;fill-
-00003090: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-000030a0: 2d77 6964 7468 3a30 2e34 3030 3432 3522  -width:0.400425"
-000030b0: 3e53 6165 6e6f 7079 3c2f 7473 7061 6e3e  >Saenopy</tspan>
-000030c0: 3c2f 7465 7874 3e0a 2020 2020 3c74 6578  </text>.    <tex
-000030d0: 740a 2020 2020 2020 2078 6d6c 3a73 7061  t.       xml:spa
-000030e0: 6365 3d22 7072 6573 6572 7665 220a 2020  ce="preserve".  
-000030f0: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
-00003100: 2d73 7479 6c65 3a6e 6f72 6d61 6c3b 666f  -style:normal;fo
-00003110: 6e74 2d77 6569 6768 743a 6e6f 726d 616c  nt-weight:normal
-00003120: 3b66 6f6e 742d 7369 7a65 3a31 362e 3132  ;font-size:16.12
-00003130: 3131 7078 3b6c 696e 652d 6865 6967 6874  11px;line-height
-00003140: 3a31 2e32 353b 666f 6e74 2d66 616d 696c  :1.25;font-famil
-00003150: 793a 7361 6e73 2d73 6572 6966 3b6c 6574  y:sans-serif;let
-00003160: 7465 722d 7370 6163 696e 673a 3070 783b  ter-spacing:0px;
-00003170: 776f 7264 2d73 7061 6369 6e67 3a30 7078  word-spacing:0px
-00003180: 3b66 696c 6c3a 2330 3030 3030 303b 6669  ;fill:#000000;fi
-00003190: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-000031a0: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
-000031b0: 7769 6474 683a 312e 3039 3931 3722 0a20  width:1.09917". 
-000031c0: 2020 2020 2020 783d 2231 3335 2e34 3739        x="135.479
-000031d0: 3036 220a 2020 2020 2020 2079 3d22 3133  06".       y="13
-000031e0: 362e 3338 3737 220a 2020 2020 2020 2069  6.3877".       i
-000031f0: 643d 2274 6578 7431 3436 3931 220a 2020  d="text14691".  
-00003200: 2020 2020 2074 7261 6e73 666f 726d 3d22       transform="
-00003210: 7363 616c 6528 312e 3030 3232 3537 352c  scale(1.0022575,
-00003220: 302e 3939 3737 3437 3538 2922 3e3c 7473  0.99774758)"><ts
-00003230: 7061 6e0a 2020 2020 2020 2020 2073 6f64  pan.         sod
-00003240: 6970 6f64 693a 726f 6c65 3d22 6c69 6e65  ipodi:role="line
-00003250: 220a 2020 2020 2020 2020 2069 643d 2274  ".         id="t
-00003260: 7370 616e 3134 3638 3922 0a20 2020 2020  span14689".     
-00003270: 2020 2020 783d 2231 3335 2e34 3739 3036      x="135.47906
-00003280: 220a 2020 2020 2020 2020 2079 3d22 3133  ".         y="13
-00003290: 362e 3338 3737 220a 2020 2020 2020 2020  6.3877".        
-000032a0: 2073 7479 6c65 3d22 666f 6e74 2d73 7479   style="font-sty
-000032b0: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d76  le:normal;font-v
-000032c0: 6172 6961 6e74 3a6e 6f72 6d61 6c3b 666f  ariant:normal;fo
-000032d0: 6e74 2d77 6569 6768 743a 6e6f 726d 616c  nt-weight:normal
-000032e0: 3b66 6f6e 742d 7374 7265 7463 683a 6e6f  ;font-stretch:no
-000032f0: 726d 616c 3b66 6f6e 742d 7369 7a65 3a35  rmal;font-size:5
-00003300: 382e 3632 3231 7078 3b66 6f6e 742d 6661  8.6221px;font-fa
-00003310: 6d69 6c79 3a27 546c 7767 2054 7970 6973  mily:'Tlwg Typis
-00003320: 7427 3b2d 696e 6b73 6361 7065 2d66 6f6e  t';-inkscape-fon
-00003330: 742d 7370 6563 6966 6963 6174 696f 6e3a  t-specification:
-00003340: 2754 6c77 6720 5479 7069 7374 273b 7374  'Tlwg Typist';st
-00003350: 726f 6b65 2d77 6964 7468 3a31 2e30 3939  roke-width:1.099
-00003360: 3137 223e 5361 656e 6f70 793c 2f74 7370  17">Saenopy</tsp
-00003370: 616e 3e3c 2f74 6578 743e 0a20 2020 203c  an></text>.    <
-00003380: 7265 6374 0a20 2020 2020 2020 7374 796c  rect.       styl
-00003390: 653d 2266 696c 6c3a 2330 3030 3030 303b  e="fill:#000000;
-000033a0: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
-000033b0: 6b65 2d77 6964 7468 3a35 2e30 3834 3736  ke-width:5.08476
-000033c0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-000033d0: 726f 756e 643b 7374 726f 6b65 2d6c 696e  round;stroke-lin
-000033e0: 656a 6f69 6e3a 726f 756e 643b 6669 6c6c  ejoin:round;fill
-000033f0: 2d6f 7061 6369 7479 3a30 220a 2020 2020  -opacity:0".    
-00003400: 2020 2069 643d 2272 6563 7437 3036 2d35     id="rect706-5
-00003410: 220a 2020 2020 2020 2077 6964 7468 3d22  ".       width="
-00003420: 3430 3022 0a20 2020 2020 2020 6865 6967  400".       heig
-00003430: 6874 3d22 3230 3022 0a20 2020 2020 2020  ht="200".       
-00003440: 783d 2234 3530 220a 2020 2020 2020 2079  x="450".       y
-00003450: 3d22 2d31 2e38 3532 3036 3131 652d 3036  ="-1.8520611e-06
-00003460: 220a 2020 2020 2020 2072 793d 2230 2220  ".       ry="0" 
-00003470: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00003480: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00003490: 2366 6666 6666 663b 6669 6c6c 2d6f 7061  #ffffff;fill-opa
-000034a0: 6369 7479 3a30 2e39 3938 3430 3830 383b  city:0.99840808;
-000034b0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-000034c0: 7472 6f6b 652d 7769 6474 683a 302e 3530  troke-width:0.50
-000034d0: 3030 3232 7078 3b73 7472 6f6b 652d 6c69  0022px;stroke-li
-000034e0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-000034f0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00003500: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00003510: 3122 0a20 2020 2020 2020 643d 224d 2036  1".       d="M 6
-00003520: 3233 2e38 3438 3132 2c38 392e 3036 3935  23.84812,89.0695
-00003530: 3120 3738 372e 3635 3039 372c 3634 2e39  1 787.65097,64.9
-00003540: 3439 3731 2036 3231 2e38 3734 3436 2c38  4971 621.87446,8
-00003550: 302e 3731 3433 3620 5a22 0a20 2020 2020  0.71436 Z".     
-00003560: 2020 6964 3d22 7061 7468 3134 3635 372d    id="path14657-
-00003570: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
-00003580: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-00003590: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-000035a0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-000035b0: 7970 6573 3d22 6363 6363 2220 2f3e 0a20  ypes="cccc" />. 
-000035c0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-000035d0: 7374 796c 653d 2266 696c 6c3a 2333 6534  style="fill:#3e4
-000035e0: 6237 373b 6669 6c6c 2d6f 7061 6369 7479  b77;fill-opacity
-000035f0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-00003600: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
-00003610: 2e30 3530 3035 3b73 7472 6f6b 652d 6c69  .05005;stroke-li
-00003620: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00003630: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00003640: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00003650: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00003660: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00003670: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00003680: 2020 2020 643d 226d 2034 3639 2e36 3033      d="m 469.603
-00003690: 3038 2c36 372e 3635 3639 2036 312e 3235  08,67.6569 61.25
-000036a0: 3439 362c 2d32 2e37 3731 3738 2034 302e  496,-2.77178 40.
-000036b0: 3234 3630 322c 2d34 342e 3630 3035 3820  24602,-44.60058 
-000036c0: 4320 3532 302e 3430 3236 2c35 342e 3232  C 520.4026,54.22
-000036d0: 3837 3320 3439 362e 3137 3936 312c 3539  873 496.17961,59
-000036e0: 2e36 3736 3337 2034 3639 2e36 3033 3038  .67637 469.60308
-000036f0: 2c36 372e 3635 3639 205a 220a 2020 2020  ,67.6569 Z".    
-00003700: 2020 2069 643d 2270 6174 6831 3435 3437     id="path14547
-00003710: 2d35 220a 2020 2020 2020 2069 6e6b 7363  -5".       inksc
-00003720: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00003730: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-00003740: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-00003750: 7479 7065 733d 2263 6363 6322 202f 3e0a  types="cccc" />.
-00003760: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00003770: 2073 7479 6c65 3d22 6669 6c6c 3a23 3163   style="fill:#1c
-00003780: 3263 3638 3b66 696c 6c2d 6f70 6163 6974  2c68;fill-opacit
-00003790: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-000037a0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-000037b0: 312e 3035 3030 353b 7374 726f 6b65 2d6c  1.05005;stroke-l
-000037c0: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
-000037d0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
-000037e0: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
-000037f0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-00003800: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-00003810: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00003820: 2020 2020 2064 3d22 6d20 3533 302e 3835       d="m 530.85
-00003830: 3830 342c 3634 2e38 3835 3132 2032 362e  804,64.88512 26.
-00003840: 3537 3735 362c 362e 3034 3735 3420 3133  57756,6.04754 13
-00003850: 2e36 3638 3436 2c2d 3530 2e36 3438 3132  .66846,-50.64812
-00003860: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
-00003870: 6174 6831 3435 3439 2d36 220a 2020 2020  ath14549-6".    
-00003880: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00003890: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-000038a0: 2230 2220 2f3e 0a20 2020 203c 7061 7468  "0" />.    <path
-000038b0: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-000038c0: 696c 6c3a 2330 3630 3530 383b 6669 6c6c  ill:#060508;fill
-000038d0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-000038e0: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-000038f0: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
-00003900: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00003910: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00003920: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00003930: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00003940: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00003950: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00003960: 793a 3122 0a20 2020 2020 2020 643d 224d  y:1".       d="M
-00003970: 2035 3537 2e34 3335 362c 3730 2e39 3332   557.4356,70.932
-00003980: 3636 2036 3238 2e35 3632 3234 2c38 332e  66 628.56224,83.
-00003990: 3533 3137 2043 2036 3030 2e38 3435 3432  5317 C 600.84542
-000039a0: 2c36 382e 3934 3439 3720 3538 342e 3739  ,68.94497 584.79
-000039b0: 3530 322c 3435 2e35 3039 3535 2035 3731  502,45.50955 571
-000039c0: 2e31 3034 3036 2c32 302e 3238 3435 3420  .10406,20.28454 
-000039d0: 5a22 0a20 2020 2020 2020 6964 3d22 7061  Z".       id="pa
-000039e0: 7468 3134 3535 312d 3222 0a20 2020 2020  th14551-2".     
-000039f0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00003a00: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00003a10: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
-00003a20: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00003a30: 6363 2220 2f3e 0a20 2020 203c 7061 7468  cc" />.    <path
-00003a40: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00003a50: 696c 6c3a 2332 3733 3737 333b 6669 6c6c  ill:#273773;fill
-00003a60: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00003a70: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00003a80: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
-00003a90: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00003aa0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00003ab0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00003ac0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00003ad0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00003ae0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00003af0: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-00003b00: 2034 3639 2e36 3033 3038 2c36 372e 3635   469.60308,67.65
-00003b10: 3639 2063 2031 332e 3437 3933 312c 372e  69 c 13.47931,7.
-00003b20: 3639 3738 2032 382e 3334 3131 312c 3134  6978 28.34111,14
-00003b30: 2e33 3336 3935 2033 332e 3431 3138 2c32  .33695 33.4118,2
-00003b40: 382e 3437 3338 3220 6c20 3237 2e38 3433  8.47382 l 27.843
-00003b50: 3136 2c2d 3331 2e32 3435 3620 7a22 0a20  16,-31.2456 z". 
-00003b60: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00003b70: 3535 332d 3922 0a20 2020 2020 2020 696e  553-9".       in
-00003b80: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00003b90: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00003ba0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00003bb0: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
-00003bc0: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00003bd0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00003be0: 2331 3432 3637 323b 6669 6c6c 2d6f 7061  #142672;fill-opa
-00003bf0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-00003c00: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00003c10: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
-00003c20: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00003c30: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00003c40: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00003c50: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00003c60: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00003c70: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00003c80: 0a20 2020 2020 2020 643d 224d 2035 3033  .       d="M 503
-00003c90: 2e30 3134 3838 2c39 362e 3133 3037 3220  .01488,96.13072 
-00003ca0: 3632 382e 3536 3232 342c 3833 2e35 3331  628.56224,83.531
-00003cb0: 3720 3533 302e 3835 3830 342c 3634 2e38  7 530.85804,64.8
-00003cc0: 3835 3132 205a 220a 2020 2020 2020 2069  8512 Z".       i
-00003cd0: 643d 2270 6174 6831 3435 3535 2d31 220a  d="path14555-1".
-00003ce0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00003cf0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00003d00: 7572 653d 2230 2220 2f3e 0a20 2020 203c  ure="0" />.    <
-00003d10: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-00003d20: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
-00003d30: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-00003d40: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00003d50: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
-00003d60: 3035 3b73 7472 6f6b 652d 6c69 6e65 6361  05;stroke-lineca
-00003d70: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00003d80: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00003d90: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00003da0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00003db0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-00003dc0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00003dd0: 643d 226d 2035 3033 2e30 3134 3838 2c39  d="m 503.01488,9
-00003de0: 362e 3133 3037 3220 3732 2e33 3932 3232  6.13072 72.39222
-00003df0: 2c37 2e35 3539 3434 2035 332e 3135 3531  ,7.55944 53.1551
-00003e00: 342c 2d32 302e 3135 3834 3620 7a22 0a20  4,-20.15846 z". 
-00003e10: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00003e20: 3535 372d 3222 0a20 2020 2020 2020 696e  557-2".       in
-00003e30: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00003e40: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
-00003e50: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
-00003e60: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00003e70: 3232 3334 3765 3b66 696c 6c2d 6f70 6163  22347e;fill-opac
-00003e80: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-00003e90: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-00003ea0: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
-00003eb0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-00003ec0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-00003ed0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
-00003ee0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00003ef0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00003f00: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00003f10: 2020 2020 2020 2064 3d22 6d20 3530 332e         d="m 503.
-00003f20: 3031 3438 382c 3936 2e31 3330 3732 2063  01488,96.13072 c
-00003f30: 2031 2e36 3237 3832 2c31 332e 3937 3235   1.62782,13.9725
-00003f40: 3220 2d34 2e30 3036 3738 2c32 322e 3738  2 -4.00678,22.78
-00003f50: 3039 3320 2d36 2e35 3831 3131 2c33 332e  093 -6.58111,33.
-00003f60: 3736 3534 3120 6c20 3738 2e39 3733 3333  76541 l 78.97333
-00003f70: 2c2d 3236 2e32 3035 3937 207a 220a 2020  ,-26.20597 z".  
-00003f80: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00003f90: 3539 2d37 220a 2020 2020 2020 2069 6e6b  59-7".       ink
-00003fa0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-00003fb0: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-00003fc0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-00003fd0: 6465 7479 7065 733d 2263 6363 6322 202f  detypes="cccc" /
-00003fe0: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
-00003ff0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00004000: 3038 3130 3639 3b66 696c 6c2d 6f70 6163  081069;fill-opac
-00004010: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-00004020: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-00004030: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
-00004040: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-00004050: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-00004060: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
-00004070: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-00004080: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-00004090: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-000040a0: 2020 2020 2020 2064 3d22 6d20 3439 362e         d="m 496.
-000040b0: 3433 3337 372c 3132 392e 3839 3631 3320  43377,129.89613 
-000040c0: 3534 2e36 3733 3834 2c38 2e30 3633 3338  54.67384,8.06338
-000040d0: 2037 372e 3435 3436 332c 2d35 342e 3432   77.45463,-54.42
-000040e0: 3738 3120 7a22 0a20 2020 2020 2020 6964  781 z".       id
-000040f0: 3d22 7061 7468 3134 3536 312d 3022 0a20  ="path14561-0". 
-00004100: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00004110: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00004120: 7265 3d22 3022 202f 3e0a 2020 2020 3c70  re="0" />.    <p
-00004130: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-00004140: 3d22 6669 6c6c 3a23 3037 3065 3262 3b66  ="fill:#070e2b;f
-00004150: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00004160: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00004170: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
-00004180: 353b 7374 726f 6b65 2d6c 696e 6563 6170  5;stroke-linecap
-00004190: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-000041a0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-000041b0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-000041c0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-000041d0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-000041e0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-000041f0: 3d22 4d20 3535 312e 3130 3736 312c 3133  ="M 551.10761,13
-00004200: 372e 3935 3935 3120 3538 332e 3235 3338  7.95951 583.2538
-00004210: 2c31 3830 2e30 3430 3320 3537 312e 3335  ,180.0403 571.35
-00004220: 3731 382c 3132 332e 3334 3436 3420 5a22  718,123.34464 Z"
-00004230: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00004240: 3134 3536 332d 3922 0a20 2020 2020 2020  14563-9".       
-00004250: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-00004260: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-00004270: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
-00004280: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00004290: 3a23 3238 3364 3837 3b66 696c 6c2d 6f70  :#283d87;fill-op
-000042a0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-000042b0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-000042c0: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
-000042d0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-000042e0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-000042f0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-00004300: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00004310: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00004320: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00004330: 220a 2020 2020 2020 2064 3d22 6d20 3537  ".       d="m 57
-00004340: 312e 3335 3731 382c 3132 332e 3334 3436  1.35718,123.3446
-00004350: 3420 3131 2e38 3936 3632 2c35 362e 3639  4 11.89662,56.69
-00004360: 3536 3620 6320 362e 3135 3836 322c 2d35  566 c 6.15862,-5
-00004370: 302e 3936 3637 3320 3237 2e38 3331 3437  0.96673 27.83147
-00004380: 2c2d 3639 2e33 3238 3631 2034 352e 3330  ,-69.32861 45.30
-00004390: 3834 342c 2d39 362e 3530 3836 207a 220a  844,-96.5086 z".
-000043a0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-000043b0: 3435 3635 2d33 220a 2020 2020 2020 2069  4565-3".       i
-000043c0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
-000043d0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
-000043e0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-000043f0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
-00004400: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
-00004410: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00004420: 696c 6c3a 2330 3730 6532 623b 6669 6c6c  ill:#070e2b;fill
-00004430: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
-00004440: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
-00004450: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
-00004460: 3035 3030 353b 7374 726f 6b65 2d6d 6974  05005;stroke-mit
-00004470: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00004480: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00004490: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-000044a0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-000044b0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-000044c0: 2270 6174 6831 3435 3637 2d36 3022 0a20  "path14567-60". 
-000044d0: 2020 2020 2020 6378 3d22 3437 302e 3930        cx="470.90
-000044e0: 3331 3422 0a20 2020 2020 2020 6379 3d22  314".       cy="
-000044f0: 3637 2e37 3231 3538 3822 0a20 2020 2020  67.721588".     
-00004500: 2020 7278 3d22 332e 3135 3632 3236 3422    rx="3.1562264"
-00004510: 0a20 2020 2020 2020 7279 3d22 332e 3134  .       ry="3.14
-00004520: 3230 3234 2220 2f3e 0a20 2020 203c 656c  2024" />.    <el
-00004530: 6c69 7073 650a 2020 2020 2020 2073 7479  lipse.       sty
-00004540: 6c65 3d22 6669 6c6c 3a23 3235 3361 3764  le="fill:#253a7d
-00004550: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-00004560: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00004570: 7472 6f6b 652d 7769 6474 683a 312e 3035  troke-width:1.05
-00004580: 3030 353b 7374 726f 6b65 2d6d 6974 6572  005;stroke-miter
-00004590: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-000045a0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-000045b0: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
-000045c0: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
-000045d0: 3a31 220a 2020 2020 2020 2069 643d 2270  :1".       id="p
-000045e0: 6174 6831 3435 3637 2d33 2d36 220a 2020  ath14567-3-6".  
-000045f0: 2020 2020 2063 783d 2234 3935 2e39 3235       cx="495.925
-00004600: 3834 220a 2020 2020 2020 2063 793d 2231  84".       cy="1
-00004610: 3239 2e32 3235 3838 220a 2020 2020 2020  29.22588".      
-00004620: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-00004630: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
-00004640: 3332 3639 3734 3522 0a20 2020 2020 2020  3269745".       
-00004650: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-00004660: 726d 2d63 656e 7465 722d 793d 222d 342e  rm-center-y="-4.
-00004670: 3937 3830 3136 3322 0a20 2020 2020 2020  9780163".       
-00004680: 7278 3d22 332e 3135 3632 3236 3422 0a20  rx="3.1562264". 
-00004690: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
-000046a0: 3234 2220 2f3e 0a20 2020 203c 656c 6c69  24" />.    <elli
-000046b0: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
-000046c0: 3d22 6669 6c6c 3a23 3235 3361 3764 3b66  ="fill:#253a7d;f
-000046d0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-000046e0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-000046f0: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
-00004700: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
-00004710: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-00004720: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-00004730: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-00004740: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00004750: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-00004760: 6831 3435 3637 2d33 2d37 2d32 220a 2020  h14567-3-7-2".  
-00004770: 2020 2020 2063 783d 2235 3730 2e35 3838       cx="570.588
-00004780: 3632 220a 2020 2020 2020 2063 793d 2231  62".       cy="1
-00004790: 3033 2e38 3931 3339 220a 2020 2020 2020  03.89139".      
-000047a0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-000047b0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
-000047c0: 3332 3639 3739 3222 0a20 2020 2020 2020  3269792".       
-000047d0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-000047e0: 726d 2d63 656e 7465 722d 793d 222d 342e  rm-center-y="-4.
-000047f0: 3937 3830 3230 3422 0a20 2020 2020 2020  9780204".       
-00004800: 7278 3d22 332e 3135 3632 3236 3422 0a20  rx="3.1562264". 
-00004810: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
-00004820: 3234 2220 2f3e 0a20 2020 203c 656c 6c69  24" />.    <elli
-00004830: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
-00004840: 3d22 6669 6c6c 3a23 6138 6139 6161 3b66  ="fill:#a8a9aa;f
-00004850: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00004860: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00004870: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
-00004880: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
-00004890: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-000048a0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-000048b0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-000048c0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-000048d0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-000048e0: 6831 3435 3637 2d33 2d35 2d36 220a 2020  h14567-3-5-6".  
-000048f0: 2020 2020 2063 783d 2235 3731 2e33 3337       cx="571.337
-00004900: 3136 220a 2020 2020 2020 2063 793d 2231  16".       cy="1
-00004910: 3232 2e38 3932 3234 220a 2020 2020 2020  22.89224".      
-00004920: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-00004930: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
-00004940: 3332 3639 3637 220a 2020 2020 2020 2069  326967".       i
-00004950: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-00004960: 6d2d 6365 6e74 6572 2d79 3d22 2d34 2e39  m-center-y="-4.9
-00004970: 3738 3030 3539 220a 2020 2020 2020 2072  780059".       r
-00004980: 783d 2233 2e31 3536 3232 3634 220a 2020  x="3.1562264".  
-00004990: 2020 2020 2072 793d 2233 2e31 3432 3032       ry="3.14202
-000049a0: 3422 202f 3e0a 2020 2020 3c65 6c6c 6970  4" />.    <ellip
-000049b0: 7365 0a20 2020 2020 2020 7374 796c 653d  se.       style=
-000049c0: 2266 696c 6c3a 2361 6261 6139 633b 6669  "fill:#abaa9c;fi
-000049d0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-000049e0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-000049f0: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
-00004a00: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00004a10: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00004a20: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00004a30: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-00004a40: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00004a50: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-00004a60: 3134 3536 372d 332d 392d 3122 0a20 2020  14567-3-9-1".   
-00004a70: 2020 2020 6378 3d22 3535 312e 3837 3631      cx="551.8761
-00004a80: 3622 0a20 2020 2020 2020 6379 3d22 3133  6".       cy="13
-00004a90: 372e 3739 3438 3522 0a20 2020 2020 2020  7.79485".       
-00004aa0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-00004ab0: 726d 2d63 656e 7465 722d 783d 2232 2e33  rm-center-x="2.3
-00004ac0: 3236 3937 3322 0a20 2020 2020 2020 696e  26973".       in
-00004ad0: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
-00004ae0: 2d63 656e 7465 722d 793d 222d 342e 3937  -center-y="-4.97
-00004af0: 3830 3235 3122 0a20 2020 2020 2020 7278  80251".       rx
-00004b00: 3d22 332e 3135 3632 3236 3422 0a20 2020  ="3.1562264".   
-00004b10: 2020 2020 7279 3d22 332e 3134 3230 3234      ry="3.142024
-00004b20: 2220 2f3e 0a20 2020 203c 656c 6c69 7073  " />.    <ellips
-00004b30: 650a 2020 2020 2020 2073 7479 6c65 3d22  e.       style="
-00004b40: 6669 6c6c 3a23 3131 3230 3636 3b66 696c  fill:#112066;fil
-00004b50: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00004b60: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00004b70: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
-00004b80: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00004b90: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00004ba0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00004bb0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-00004bc0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00004bd0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00004be0: 3435 3637 2d33 2d32 2d38 220a 2020 2020  4567-3-2-8".    
-00004bf0: 2020 2063 783d 2235 3331 2e32 3932 3432     cx="531.29242
-00004c00: 220a 2020 2020 2020 2063 793d 2236 342e  ".       cy="64.
-00004c10: 3231 3331 3635 220a 2020 2020 2020 2069  213165".       i
-00004c20: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-00004c30: 6d2d 6365 6e74 6572 2d78 3d22 332e 3539  m-center-x="3.59
-00004c40: 3133 3630 3922 0a20 2020 2020 2020 696e  13609".       in
-00004c50: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
-00004c60: 2d63 656e 7465 722d 793d 222d 372e 3638  -center-y="-7.68
-00004c70: 3238 3935 3622 0a20 2020 2020 2020 7278  28956".       rx
-00004c80: 3d22 342e 3837 3131 3932 3922 0a20 2020  ="4.8711929".   
-00004c90: 2020 2020 7279 3d22 342e 3834 3932 3733      ry="4.849273
-00004ca0: 3722 202f 3e0a 2020 2020 3c65 6c6c 6970  7" />.    <ellip
-00004cb0: 7365 0a20 2020 2020 2020 7374 796c 653d  se.       style=
-00004cc0: 2266 696c 6c3a 2365 6466 3066 633b 6669  "fill:#edf0fc;fi
-00004cd0: 6c6c 2d6f 7061 6369 7479 3a30 2e39 3930  ll-opacity:0.990
-00004ce0: 3434 363b 7374 726f 6b65 3a23 6666 6666  446;stroke:#ffff
-00004cf0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00004d00: 312e 3035 3030 353b 7374 726f 6b65 2d6d  1.05005;stroke-m
-00004d10: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00004d20: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00004d30: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-00004d40: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-00004d50: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
-00004d60: 643d 2270 6174 6831 3435 3637 2d32 2d37  d="path14567-2-7
-00004d70: 3922 0a20 2020 2020 2020 6378 3d22 3535  9".       cx="55
-00004d80: 372e 3637 3722 0a20 2020 2020 2020 6379  7.677".       cy
-00004d90: 3d22 3639 2e36 3135 3335 3622 0a20 2020  ="69.615356".   
-00004da0: 2020 2020 7278 3d22 332e 3135 3632 3236      rx="3.156226
-00004db0: 3422 0a20 2020 2020 2020 7279 3d22 332e  4".       ry="3.
-00004dc0: 3134 3230 3234 2220 2f3e 0a20 2020 203c  142024" />.    <
-00004dd0: 656c 6c69 7073 650a 2020 2020 2020 2073  ellipse.       s
-00004de0: 7479 6c65 3d22 6669 6c6c 3a23 6564 6630  tyle="fill:#edf0
-00004df0: 6663 3b66 696c 6c2d 6f70 6163 6974 793a  fc;fill-opacity:
-00004e00: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
-00004e10: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00004e20: 6964 7468 3a31 2e30 3530 3035 3b73 7472  idth:1.05005;str
-00004e30: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00004e40: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00004e50: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-00004e60: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-00004e70: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00004e80: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-00004e90: 372d 322d 382d 3222 0a20 2020 2020 2020  7-2-8-2".       
-00004ea0: 6378 3d22 3530 332e 3033 3635 3922 0a20  cx="503.03659". 
-00004eb0: 2020 2020 2020 6379 3d22 3935 2e36 3934        cy="95.694
-00004ec0: 3937 3722 0a20 2020 2020 2020 7278 3d22  977".       rx="
-00004ed0: 332e 3135 3632 3236 3422 0a20 2020 2020  3.1562264".     
-00004ee0: 2020 7279 3d22 332e 3134 3230 3234 2220    ry="3.142024" 
-00004ef0: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-00004f00: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00004f10: 2366 6666 6666 663b 6669 6c6c 2d6f 7061  #ffffff;fill-opa
-00004f20: 6369 7479 3a30 2e39 3938 3430 3830 383b  city:0.99840808;
-00004f30: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00004f40: 7472 6f6b 652d 7769 6474 683a 302e 3332  troke-width:0.32
-00004f50: 3335 3838 7078 3b73 7472 6f6b 652d 6c69  3588px;stroke-li
-00004f60: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00004f70: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00004f80: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00004f90: 3122 0a20 2020 2020 2020 643d 226d 2037  1".       d="m 7
-00004fa0: 3638 2e37 3031 3334 2c37 322e 3730 3137  68.70134,72.7017
-00004fb0: 3220 3236 2e36 3034 3537 2c2d 382e 3738  2 26.60457,-8.78
-00004fc0: 3638 3320 2d32 382e 3338 3339 352c 2d31  683 -28.38395,-1
-00004fd0: 2e34 3735 3836 2063 2031 312e 3030 3532  .47586 c 11.0052
-00004fe0: 362c 332e 3230 3436 3620 3131 2e30 3535  6,3.20466 11.055
-00004ff0: 332c 332e 3337 3432 3720 312e 3737 3933  3,3.37427 1.7793
-00005000: 382c 3130 2e32 3632 3639 207a 220a 2020  8,10.26269 z".  
-00005010: 2020 2020 2069 643d 2270 6174 6831 3436       id="path146
-00005020: 3537 2d39 2d30 220a 2020 2020 2020 2069  57-9-0".       i
-00005030: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
-00005040: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
-00005050: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00005060: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
-00005070: 202f 3e0a 2020 2020 3c65 6c6c 6970 7365   />.    <ellipse
-00005080: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00005090: 696c 6c3a 2365 6466 3066 633b 6669 6c6c  ill:#edf0fc;fill
-000050a0: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
-000050b0: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
-000050c0: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
-000050d0: 3939 3539 383b 7374 726f 6b65 2d6d 6974  99598;stroke-mit
-000050e0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-000050f0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00005100: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-00005110: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-00005120: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-00005130: 2270 6174 6831 3435 3637 2d32 2d37 2d32  "path14567-2-7-2
-00005140: 220a 2020 2020 2020 2063 783d 2236 3237  ".       cx="627
-00005150: 2e34 3734 3535 220a 2020 2020 2020 2063  .47455".       c
-00005160: 793d 2238 342e 3333 3137 3236 220a 2020  y="84.331726".  
-00005170: 2020 2020 2072 783d 2235 2e39 3939 3532       rx="5.99952
-00005180: 3232 220a 2020 2020 2020 2072 793d 2235  22".       ry="5
-00005190: 2e39 3732 3532 3536 2220 2f3e 0a20 2020  .9725256" />.   
-000051a0: 203c 7465 7874 0a20 2020 2020 2020 786d   <text.       xm
-000051b0: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
-000051c0: 6522 0a20 2020 2020 2020 7374 796c 653d  e".       style=
-000051d0: 2266 6f6e 742d 7374 796c 653a 6e6f 726d  "font-style:norm
-000051e0: 616c 3b66 6f6e 742d 7765 6967 6874 3a6e  al;font-weight:n
-000051f0: 6f72 6d61 6c3b 666f 6e74 2d73 697a 653a  ormal;font-size:
-00005200: 352e 3837 3239 3170 783b 6c69 6e65 2d68  5.87291px;line-h
-00005210: 6569 6768 743a 312e 3235 3b66 6f6e 742d  eight:1.25;font-
-00005220: 6661 6d69 6c79 3a73 616e 732d 7365 7269  family:sans-seri
-00005230: 663b 6c65 7474 6572 2d73 7061 6369 6e67  f;letter-spacing
-00005240: 3a30 7078 3b77 6f72 642d 7370 6163 696e  :0px;word-spacin
-00005250: 673a 3070 783b 6669 6c6c 3a23 3534 3534  g:0px;fill:#5454
-00005260: 3534 3b66 696c 6c2d 6f70 6163 6974 793a  54;fill-opacity:
-00005270: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
-00005280: 726f 6b65 2d77 6964 7468 3a30 2e34 3030  roke-width:0.400
-00005290: 3432 353b 6669 6c74 6572 3a75 726c 2823  425;filter:url(#
-000052a0: 6669 6c74 6572 3135 3035 312d 3329 220a  filter15051-3)".
-000052b0: 2020 2020 2020 2078 3d22 3737 2e36 3934         x="77.694
-000052c0: 3839 3322 0a20 2020 2020 2020 793d 2239  893".       y="9
-000052d0: 312e 3938 3834 3439 220a 2020 2020 2020  1.988449".      
-000052e0: 2069 643d 2274 6578 7431 3436 3931 2d36   id="text14691-6
-000052f0: 2d33 220a 2020 2020 2020 2074 7261 6e73  -3".       trans
-00005300: 666f 726d 3d22 6d61 7472 6978 2832 2e37  form="matrix(2.7
-00005310: 3531 3139 3139 2c30 2c30 2c32 2e37 3338  511919,0,0,2.738
-00005320: 3831 322c 3337 342e 3032 3333 312c 2d31  812,374.02331,-1
-00005330: 3038 2e30 3838 3636 2922 3e3c 7473 7061  08.08866)"><tspa
-00005340: 6e0a 2020 2020 2020 2020 2073 6f64 6970  n.         sodip
-00005350: 6f64 693a 726f 6c65 3d22 6c69 6e65 220a  odi:role="line".
-00005360: 2020 2020 2020 2020 2069 643d 2274 7370           id="tsp
-00005370: 616e 3134 3638 392d 322d 3722 0a20 2020  an14689-2-7".   
-00005380: 2020 2020 2020 783d 2237 372e 3639 3438        x="77.6948
-00005390: 3933 220a 2020 2020 2020 2020 2079 3d22  93".         y="
-000053a0: 3931 2e39 3838 3434 3922 0a20 2020 2020  91.988449".     
-000053b0: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
-000053c0: 7374 796c 653a 6e6f 726d 616c 3b66 6f6e  style:normal;fon
-000053d0: 742d 7661 7269 616e 743a 6e6f 726d 616c  t-variant:normal
-000053e0: 3b66 6f6e 742d 7765 6967 6874 3a6e 6f72  ;font-weight:nor
-000053f0: 6d61 6c3b 666f 6e74 2d73 7472 6574 6368  mal;font-stretch
-00005400: 3a6e 6f72 6d61 6c3b 666f 6e74 2d73 697a  :normal;font-siz
-00005410: 653a 3231 2e33 3536 7078 3b66 6f6e 742d  e:21.356px;font-
-00005420: 6661 6d69 6c79 3a49 6d70 6163 743b 2d69  family:Impact;-i
-00005430: 6e6b 7363 6170 652d 666f 6e74 2d73 7065  nkscape-font-spe
-00005440: 6369 6669 6361 7469 6f6e 3a49 6d70 6163  cification:Impac
-00005450: 743b 6669 6c6c 3a23 3534 3534 3534 3b66  t;fill:#545454;f
-00005460: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00005470: 726f 6b65 2d77 6964 7468 3a30 2e34 3030  roke-width:0.400
-00005480: 3432 3522 3e53 6165 6e6f 7079 3c2f 7473  425">Saenopy</ts
-00005490: 7061 6e3e 3c2f 7465 7874 3e0a 2020 2020  pan></text>.    
-000054a0: 3c74 6578 740a 2020 2020 2020 2078 6d6c  <text.       xml
-000054b0: 3a73 7061 6365 3d22 7072 6573 6572 7665  :space="preserve
-000054c0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-000054d0: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
-000054e0: 6c3b 666f 6e74 2d77 6569 6768 743a 6e6f  l;font-weight:no
-000054f0: 726d 616c 3b66 6f6e 742d 7369 7a65 3a31  rmal;font-size:1
-00005500: 362e 3132 3131 7078 3b6c 696e 652d 6865  6.1211px;line-he
-00005510: 6967 6874 3a31 2e32 353b 666f 6e74 2d66  ight:1.25;font-f
-00005520: 616d 696c 793a 7361 6e73 2d73 6572 6966  amily:sans-serif
-00005530: 3b6c 6574 7465 722d 7370 6163 696e 673a  ;letter-spacing:
-00005540: 3070 783b 776f 7264 2d73 7061 6369 6e67  0px;word-spacing
-00005550: 3a30 7078 3b66 696c 6c3a 2366 6666 6666  :0px;fill:#fffff
-00005560: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
-00005570: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
-00005580: 6f6b 652d 7769 6474 683a 312e 3039 3931  oke-width:1.0991
-00005590: 3722 0a20 2020 2020 2020 783d 2235 3834  7".       x="584
-000055a0: 2e34 3635 3532 220a 2020 2020 2020 2079  .46552".       y
-000055b0: 3d22 3133 362e 3338 3737 220a 2020 2020  ="136.3877".    
-000055c0: 2020 2069 643d 2274 6578 7431 3436 3931     id="text14691
-000055d0: 2d35 220a 2020 2020 2020 2074 7261 6e73  -5".       trans
-000055e0: 666f 726d 3d22 7363 616c 6528 312e 3030  form="scale(1.00
-000055f0: 3232 3537 352c 302e 3939 3737 3437 3538  22575,0.99774758
-00005600: 2922 3e3c 7473 7061 6e0a 2020 2020 2020  )"><tspan.      
-00005610: 2020 2073 6f64 6970 6f64 693a 726f 6c65     sodipodi:role
-00005620: 3d22 6c69 6e65 220a 2020 2020 2020 2020  ="line".        
-00005630: 2069 643d 2274 7370 616e 3134 3638 392d   id="tspan14689-
-00005640: 3922 0a20 2020 2020 2020 2020 783d 2235  9".         x="5
-00005650: 3834 2e34 3635 3532 220a 2020 2020 2020  84.46552".      
-00005660: 2020 2079 3d22 3133 362e 3338 3737 220a     y="136.3877".
-00005670: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00005680: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
-00005690: 6c3b 666f 6e74 2d76 6172 6961 6e74 3a6e  l;font-variant:n
-000056a0: 6f72 6d61 6c3b 666f 6e74 2d77 6569 6768  ormal;font-weigh
-000056b0: 743a 6e6f 726d 616c 3b66 6f6e 742d 7374  t:normal;font-st
-000056c0: 7265 7463 683a 6e6f 726d 616c 3b66 6f6e  retch:normal;fon
-000056d0: 742d 7369 7a65 3a35 382e 3632 3231 7078  t-size:58.6221px
-000056e0: 3b66 6f6e 742d 6661 6d69 6c79 3a27 546c  ;font-family:'Tl
-000056f0: 7767 2054 7970 6973 7427 3b2d 696e 6b73  wg Typist';-inks
-00005700: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
-00005710: 6963 6174 696f 6e3a 2754 6c77 6720 5479  ication:'Tlwg Ty
-00005720: 7069 7374 273b 7374 726f 6b65 2d77 6964  pist';stroke-wid
-00005730: 7468 3a31 2e30 3939 3137 3b66 696c 6c3a  th:1.09917;fill:
-00005740: 2366 6666 6666 663b 6669 6c6c 2d6f 7061  #ffffff;fill-opa
-00005750: 6369 7479 3a31 223e 5361 656e 6f70 793c  city:1">Saenopy<
-00005760: 2f74 7370 616e 3e3c 2f74 6578 743e 0a20  /tspan></text>. 
-00005770: 2020 203c 670a 2020 2020 2020 2069 643d     <g.       id=
-00005780: 2267 3134 3238 2d37 2d38 220a 2020 2020  "g1428-7-8".    
-00005790: 2020 2074 7261 6e73 666f 726d 3d22 7472     transform="tr
-000057a0: 616e 736c 6174 6528 3930 302e 3030 3030  anslate(900.0000
-000057b0: 3129 223e 0a20 2020 2020 203c 7265 6374  1)">.      <rect
-000057c0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-000057d0: 2266 696c 6c3a 2366 6666 6666 663b 7374  "fill:#ffffff;st
-000057e0: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
-000057f0: 2d77 6964 7468 3a35 2e30 3834 3736 3b73  -width:5.08476;s
-00005800: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
-00005810: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
-00005820: 6f69 6e3a 726f 756e 6422 0a20 2020 2020  oin:round".     
-00005830: 2020 2020 6964 3d22 7265 6374 3730 362d      id="rect706-
-00005840: 352d 3922 0a20 2020 2020 2020 2020 7769  5-9".         wi
-00005850: 6474 683d 2234 3030 220a 2020 2020 2020  dth="400".      
-00005860: 2020 2068 6569 6768 743d 2232 3030 220a     height="200".
-00005870: 2020 2020 2020 2020 2078 3d22 2d36 2e36           x="-6.6
-00005880: 3936 3531 3331 652d 3036 220a 2020 2020  965131e-06".    
-00005890: 2020 2020 2079 3d22 2d31 2e38 3532 3036       y="-1.85206
-000058a0: 3131 652d 3036 220a 2020 2020 2020 2020  11e-06".        
-000058b0: 2072 793d 2230 2220 2f3e 0a20 2020 2020   ry="0" />.     
-000058c0: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
-000058d0: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
-000058e0: 3030 303b 6669 6c6c 2d6f 7061 6369 7479  000;fill-opacity
-000058f0: 3a30 2e39 3938 3430 383b 7374 726f 6b65  :0.998408;stroke
-00005900: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
-00005910: 7769 6474 683a 302e 3530 3030 3232 7078  width:0.500022px
-00005920: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00005930: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00005940: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00005950: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00005960: 2020 2020 2020 643d 224d 2031 3733 2e38        d="M 173.8
-00005970: 3438 3131 2c38 392e 3036 3935 3120 3333  4811,89.06951 33
-00005980: 372e 3635 3039 362c 3634 2e39 3439 3731  7.65096,64.94971
-00005990: 2031 3731 2e38 3734 3435 2c38 302e 3731   171.87445,80.71
-000059a0: 3433 3620 5a22 0a20 2020 2020 2020 2020  436 Z".         
-000059b0: 6964 3d22 7061 7468 3134 3635 372d 332d  id="path14657-3-
-000059c0: 3722 0a20 2020 2020 2020 2020 696e 6b73  7".         inks
-000059d0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-000059e0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-000059f0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00005a00: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
-00005a10: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
-00005a20: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00005a30: 696c 6c3a 2333 6534 6237 373b 6669 6c6c  ill:#3e4b77;fill
-00005a40: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00005a50: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00005a60: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
-00005a70: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00005a80: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00005a90: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00005aa0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00005ab0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00005ac0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00005ad0: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
-00005ae0: 224d 2031 392e 3630 3330 372c 3637 2e36  "M 19.60307,67.6
-00005af0: 3536 3920 3830 2e38 3538 3032 382c 3634  569 80.858028,64
-00005b00: 2e38 3835 3132 2031 3231 2e31 3034 3035  .88512 121.10405
-00005b10: 2c32 302e 3238 3435 3420 4320 3730 2e34  ,20.28454 C 70.4
-00005b20: 3032 3538 372c 3534 2e32 3238 3733 2034  02587,54.22873 4
-00005b30: 362e 3137 3936 3035 2c35 392e 3637 3633  6.179605,59.6763
-00005b40: 3720 3139 2e36 3033 3037 2c36 372e 3635  7 19.60307,67.65
-00005b50: 3639 205a 220a 2020 2020 2020 2020 2069  69 Z".         i
-00005b60: 643d 2270 6174 6831 3435 3437 2d35 2d33  d="path14547-5-3
-00005b70: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00005b80: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00005b90: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-00005ba0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-00005bb0: 6465 7479 7065 733d 2263 6363 6322 202f  detypes="cccc" /
-00005bc0: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
-00005bd0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00005be0: 6c6c 3a23 3163 3263 3638 3b66 696c 6c2d  ll:#1c2c68;fill-
-00005bf0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00005c00: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00005c10: 7769 6474 683a 312e 3035 3030 353b 7374  width:1.05005;st
-00005c20: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00005c30: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00005c40: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-00005c50: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00005c60: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00005c70: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-00005c80: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
-00005c90: 6d20 3830 2e38 3538 3032 382c 3634 2e38  m 80.858028,64.8
-00005ca0: 3835 3132 2032 362e 3537 3735 3632 2c36  8512 26.577562,6
-00005cb0: 2e30 3437 3534 2031 332e 3636 3834 362c  .04754 13.66846,
-00005cc0: 2d35 302e 3634 3831 3220 7a22 0a20 2020  -50.64812 z".   
-00005cd0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00005ce0: 3534 392d 362d 3622 0a20 2020 2020 2020  549-6-6".       
-00005cf0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00005d00: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00005d10: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
-00005d20: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
-00005d30: 3d22 6669 6c6c 3a23 3036 3035 3038 3b66  ="fill:#060508;f
-00005d40: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00005d50: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00005d60: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
-00005d70: 353b 7374 726f 6b65 2d6c 696e 6563 6170  5;stroke-linecap
-00005d80: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00005d90: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00005da0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00005db0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00005dc0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-00005dd0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
-00005de0: 2064 3d22 4d20 3130 372e 3433 3535 392c   d="M 107.43559,
-00005df0: 3730 2e39 3332 3636 2031 3738 2e35 3632  70.93266 178.562
-00005e00: 3233 2c38 332e 3533 3137 2043 2031 3530  23,83.5317 C 150
-00005e10: 2e38 3435 3431 2c36 382e 3934 3439 3720  .84541,68.94497 
-00005e20: 3133 342e 3739 3530 312c 3435 2e35 3039  134.79501,45.509
-00005e30: 3535 2031 3231 2e31 3034 3035 2c32 302e  55 121.10405,20.
-00005e40: 3238 3435 3420 5a22 0a20 2020 2020 2020  28454 Z".       
-00005e50: 2020 6964 3d22 7061 7468 3134 3535 312d    id="path14551-
-00005e60: 322d 3122 0a20 2020 2020 2020 2020 696e  2-1".         in
-00005e70: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00005e80: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00005e90: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-00005ea0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-00005eb0: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
-00005ec0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00005ed0: 2266 696c 6c3a 2332 3733 3737 333b 6669  "fill:#273773;fi
-00005ee0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-00005ef0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-00005f00: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
-00005f10: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00005f20: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-00005f30: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-00005f40: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00005f50: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00005f60: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00005f70: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-00005f80: 643d 226d 2031 392e 3630 3330 372c 3637  d="m 19.60307,67
-00005f90: 2e36 3536 3920 6320 3133 2e34 3739 3331  .6569 c 13.47931
-00005fa0: 322c 372e 3639 3738 2032 382e 3334 3131  2,7.6978 28.3411
-00005fb0: 3037 2c31 342e 3333 3639 3520 3333 2e34  07,14.33695 33.4
-00005fc0: 3131 3739 362c 3238 2e34 3733 3832 206c  11796,28.47382 l
-00005fd0: 2032 372e 3834 3331 3632 2c2d 3331 2e32   27.843162,-31.2
-00005fe0: 3435 3620 7a22 0a20 2020 2020 2020 2020  456 z".         
-00005ff0: 6964 3d22 7061 7468 3134 3535 332d 392d  id="path14553-9-
-00006000: 3222 0a20 2020 2020 2020 2020 696e 6b73  2".         inks
-00006010: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-00006020: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-00006030: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00006040: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
-00006050: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
-00006060: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00006070: 696c 6c3a 2331 3432 3637 323b 6669 6c6c  ill:#142672;fill
-00006080: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00006090: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-000060a0: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
-000060b0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-000060c0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-000060d0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-000060e0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-000060f0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00006100: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00006110: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
-00006120: 224d 2035 332e 3031 3438 3636 2c39 362e  "M 53.014866,96.
-00006130: 3133 3037 3220 3137 382e 3536 3232 332c  13072 178.56223,
-00006140: 3833 2e35 3331 3720 3830 2e38 3538 3032  83.5317 80.85802
-00006150: 382c 3634 2e38 3835 3132 205a 220a 2020  8,64.88512 Z".  
-00006160: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00006170: 3435 3535 2d31 2d39 220a 2020 2020 2020  4555-1-9".      
-00006180: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00006190: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-000061a0: 2230 2220 2f3e 0a20 2020 2020 203c 7061  "0" />.      <pa
-000061b0: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
-000061c0: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
-000061d0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-000061e0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-000061f0: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
-00006200: 3035 3b73 7472 6f6b 652d 6c69 6e65 6361  05;stroke-lineca
-00006210: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00006220: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00006230: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00006240: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00006250: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-00006260: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00006270: 2020 643d 226d 2035 332e 3031 3438 3636    d="m 53.014866
-00006280: 2c39 362e 3133 3037 3220 3732 2e33 3932  ,96.13072 72.392
-00006290: 3232 342c 372e 3535 3934 3420 3533 2e31  224,7.55944 53.1
-000062a0: 3535 3134 2c2d 3230 2e31 3538 3436 207a  5514,-20.15846 z
-000062b0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
-000062c0: 6174 6831 3435 3537 2d32 2d33 220a 2020  ath14557-2-3".  
-000062d0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000062e0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-000062f0: 7572 653d 2230 2220 2f3e 0a20 2020 2020  ure="0" />.     
-00006300: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
-00006310: 7374 796c 653d 2266 696c 6c3a 2332 3233  style="fill:#223
-00006320: 3437 653b 6669 6c6c 2d6f 7061 6369 7479  47e;fill-opacity
-00006330: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-00006340: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
-00006350: 2e30 3530 3035 3b73 7472 6f6b 652d 6c69  .05005;stroke-li
-00006360: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00006370: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00006380: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00006390: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-000063a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-000063b0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000063c0: 2020 2020 2020 643d 226d 2035 332e 3031        d="m 53.01
-000063d0: 3438 3636 2c39 362e 3133 3037 3220 6320  4866,96.13072 c 
-000063e0: 312e 3632 3738 3235 2c31 332e 3937 3235  1.627825,13.9725
-000063f0: 3220 2d34 2e30 3036 3737 322c 3232 2e37  2 -4.006772,22.7
-00006400: 3830 3933 202d 362e 3538 3131 3039 2c33  8093 -6.581109,3
-00006410: 332e 3736 3534 3120 6c20 3738 2e39 3733  3.76541 l 78.973
-00006420: 3333 332c 2d32 362e 3230 3539 3720 7a22  333,-26.20597 z"
-00006430: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00006440: 7468 3134 3535 392d 372d 3122 0a20 2020  th14559-7-1".   
-00006450: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00006460: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00006470: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
-00006480: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-00006490: 6573 3d22 6363 6363 2220 2f3e 0a20 2020  es="cccc" />.   
-000064a0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-000064b0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-000064c0: 3831 3036 393b 6669 6c6c 2d6f 7061 6369  81069;fill-opaci
-000064d0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-000064e0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-000064f0: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
-00006500: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00006510: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00006520: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-00006530: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00006540: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00006550: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00006560: 2020 2020 2020 2020 643d 224d 2034 362e          d="M 46.
-00006570: 3433 3337 3537 2c31 3239 2e38 3936 3133  433757,129.89613
-00006580: 2031 3031 2e31 3037 362c 3133 372e 3935   101.1076,137.95
-00006590: 3935 3120 3137 382e 3536 3232 332c 3833  951 178.56223,83
-000065a0: 2e35 3331 3720 5a22 0a20 2020 2020 2020  .5317 Z".       
-000065b0: 2020 6964 3d22 7061 7468 3134 3536 312d    id="path14561-
-000065c0: 302d 3922 0a20 2020 2020 2020 2020 696e  0-9".         in
-000065d0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-000065e0: 2d63 7572 7661 7475 7265 3d22 3022 202f  -curvature="0" /
-000065f0: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
-00006600: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-00006610: 6c6c 3a23 3037 3065 3262 3b66 696c 6c2d  ll:#070e2b;fill-
-00006620: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-00006630: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-00006640: 7769 6474 683a 312e 3035 3030 353b 7374  width:1.05005;st
-00006650: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00006660: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00006670: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-00006680: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00006690: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-000066a0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-000066b0: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
-000066c0: 6d20 3130 312e 3130 3736 2c31 3337 2e39  m 101.1076,137.9
-000066d0: 3539 3531 2033 322e 3134 3631 392c 3432  5951 32.14619,42
-000066e0: 2e30 3830 3739 202d 3131 2e38 3936 3632  .08079 -11.89662
-000066f0: 2c2d 3536 2e36 3935 3636 207a 220a 2020  ,-56.69566 z".  
-00006700: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00006710: 3435 3633 2d39 2d34 220a 2020 2020 2020  4563-9-4".      
-00006720: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-00006730: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-00006740: 2230 2220 2f3e 0a20 2020 2020 203c 7061  "0" />.      <pa
-00006750: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
-00006760: 653d 2266 696c 6c3a 2332 3833 6438 373b  e="fill:#283d87;
-00006770: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-00006780: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00006790: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
-000067a0: 3035 3b73 7472 6f6b 652d 6c69 6e65 6361  05;stroke-lineca
-000067b0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-000067c0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-000067d0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-000067e0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000067f0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-00006800: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00006810: 2020 643d 226d 2031 3231 2e33 3537 3137    d="m 121.35717
-00006820: 2c31 3233 2e33 3434 3634 2031 312e 3839  ,123.34464 11.89
-00006830: 3636 322c 3536 2e36 3935 3636 2063 2036  662,56.69566 c 6
-00006840: 2e31 3538 3632 2c2d 3530 2e39 3636 3733  .15862,-50.96673
-00006850: 2032 372e 3833 3134 372c 2d36 392e 3332   27.83147,-69.32
-00006860: 3836 3120 3435 2e33 3038 3434 2c2d 3936  861 45.30844,-96
-00006870: 2e35 3038 3620 7a22 0a20 2020 2020 2020  .5086 z".       
-00006880: 2020 6964 3d22 7061 7468 3134 3536 352d    id="path14565-
-00006890: 332d 3722 0a20 2020 2020 2020 2020 696e  3-7".         in
-000068a0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-000068b0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-000068c0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
-000068d0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-000068e0: 2220 2f3e 0a20 2020 2020 203c 656c 6c69  " />.      <elli
-000068f0: 7073 650a 2020 2020 2020 2020 2073 7479  pse.         sty
-00006900: 6c65 3d22 6669 6c6c 3a23 3037 3065 3262  le="fill:#070e2b
-00006910: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
-00006920: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
-00006930: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00006940: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
-00006950: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00006960: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00006970: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
-00006980: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
-00006990: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-000069a0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-000069b0: 372d 3630 2d38 220a 2020 2020 2020 2020  7-60-8".        
-000069c0: 2063 783d 2232 302e 3930 3331 3138 220a   cx="20.903118".
-000069d0: 2020 2020 2020 2020 2063 793d 2236 372e           cy="67.
-000069e0: 3732 3135 3838 220a 2020 2020 2020 2020  721588".        
-000069f0: 2072 783d 2233 2e31 3536 3232 3634 220a   rx="3.1562264".
-00006a00: 2020 2020 2020 2020 2072 793d 2233 2e31           ry="3.1
-00006a10: 3432 3032 3422 202f 3e0a 2020 2020 2020  42024" />.      
-00006a20: 3c65 6c6c 6970 7365 0a20 2020 2020 2020  <ellipse.       
-00006a30: 2020 7374 796c 653d 2266 696c 6c3a 2332    style="fill:#2
-00006a40: 3533 6137 643b 6669 6c6c 2d6f 7061 6369  53a7d;fill-opaci
-00006a50: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-00006a60: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00006a70: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
-00006a80: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00006a90: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00006aa0: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
-00006ab0: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
-00006ac0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00006ad0: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
-00006ae0: 332d 362d 3422 0a20 2020 2020 2020 2020  3-6-4".         
-00006af0: 6378 3d22 3435 2e39 3235 3834 3622 0a20  cx="45.925846". 
-00006b00: 2020 2020 2020 2020 6379 3d22 3132 392e          cy="129.
-00006b10: 3232 3538 3822 0a20 2020 2020 2020 2020  22588".         
-00006b20: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-00006b30: 726d 2d63 656e 7465 722d 783d 2232 2e33  rm-center-x="2.3
-00006b40: 3236 3937 3435 220a 2020 2020 2020 2020  269745".        
-00006b50: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-00006b60: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d34  orm-center-y="-4
-00006b70: 2e39 3738 3031 3633 220a 2020 2020 2020  .9780163".      
-00006b80: 2020 2072 783d 2233 2e31 3536 3232 3634     rx="3.1562264
-00006b90: 220a 2020 2020 2020 2020 2072 793d 2233  ".         ry="3
-00006ba0: 2e31 3432 3032 3422 202f 3e0a 2020 2020  .142024" />.    
-00006bb0: 2020 3c65 6c6c 6970 7365 0a20 2020 2020    <ellipse.     
-00006bc0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00006bd0: 2332 3533 6137 643b 6669 6c6c 2d6f 7061  #253a7d;fill-opa
-00006be0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-00006bf0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00006c00: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
-00006c10: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00006c20: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00006c30: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
-00006c40: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
-00006c50: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-00006c60: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-00006c70: 372d 332d 372d 322d 3522 0a20 2020 2020  7-3-7-2-5".     
-00006c80: 2020 2020 6378 3d22 3132 302e 3538 3836      cx="120.5886
-00006c90: 3222 0a20 2020 2020 2020 2020 6379 3d22  2".         cy="
-00006ca0: 3130 332e 3839 3133 3922 0a20 2020 2020  103.89139".     
-00006cb0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-00006cc0: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
-00006cd0: 2232 2e33 3236 3937 3932 220a 2020 2020  "2.3269792".    
-00006ce0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-00006cf0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
-00006d00: 3d22 2d34 2e39 3738 3032 3034 220a 2020  ="-4.9780204".  
-00006d10: 2020 2020 2020 2072 783d 2233 2e31 3536         rx="3.156
-00006d20: 3232 3634 220a 2020 2020 2020 2020 2072  2264".         r
-00006d30: 793d 2233 2e31 3432 3032 3422 202f 3e0a  y="3.142024" />.
-00006d40: 2020 2020 2020 3c65 6c6c 6970 7365 0a20        <ellipse. 
-00006d50: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00006d60: 696c 6c3a 2361 3861 3961 613b 6669 6c6c  ill:#a8a9aa;fill
-00006d70: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00006d80: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00006d90: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
-00006da0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00006db0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-00006dc0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-00006dd0: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-00006de0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00006df0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
-00006e00: 3134 3536 372d 332d 352d 362d 3022 0a20  14567-3-5-6-0". 
-00006e10: 2020 2020 2020 2020 6378 3d22 3132 312e          cx="121.
-00006e20: 3333 3731 3422 0a20 2020 2020 2020 2020  33714".         
-00006e30: 6379 3d22 3132 322e 3839 3232 3422 0a20  cy="122.89224". 
-00006e40: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00006e50: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-00006e60: 722d 783d 2232 2e33 3236 3936 3722 0a20  r-x="2.326967". 
-00006e70: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00006e80: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-00006e90: 722d 793d 222d 342e 3937 3830 3035 3922  r-y="-4.9780059"
-00006ea0: 0a20 2020 2020 2020 2020 7278 3d22 332e  .         rx="3.
-00006eb0: 3135 3632 3236 3422 0a20 2020 2020 2020  1562264".       
-00006ec0: 2020 7279 3d22 332e 3134 3230 3234 2220    ry="3.142024" 
-00006ed0: 2f3e 0a20 2020 2020 203c 656c 6c69 7073  />.      <ellips
-00006ee0: 650a 2020 2020 2020 2020 2073 7479 6c65  e.         style
-00006ef0: 3d22 6669 6c6c 3a23 6162 6161 3963 3b66  ="fill:#abaa9c;f
-00006f00: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00006f10: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00006f20: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
-00006f30: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
-00006f40: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-00006f50: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-00006f60: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-00006f70: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00006f80: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
-00006f90: 6174 6831 3435 3637 2d33 2d39 2d31 2d33  ath14567-3-9-1-3
-00006fa0: 220a 2020 2020 2020 2020 2063 783d 2231  ".         cx="1
-00006fb0: 3031 2e38 3736 3134 220a 2020 2020 2020  01.87614".      
-00006fc0: 2020 2063 793d 2231 3337 2e37 3934 3835     cy="137.79485
-00006fd0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00006fe0: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-00006ff0: 6e74 6572 2d78 3d22 322e 3332 3639 3733  nter-x="2.326973
-00007000: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00007010: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-00007020: 6e74 6572 2d79 3d22 2d34 2e39 3738 3032  nter-y="-4.97802
-00007030: 3531 220a 2020 2020 2020 2020 2072 783d  51".         rx=
-00007040: 2233 2e31 3536 3232 3634 220a 2020 2020  "3.1562264".    
-00007050: 2020 2020 2072 793d 2233 2e31 3432 3032       ry="3.14202
-00007060: 3422 202f 3e0a 2020 2020 2020 3c65 6c6c  4" />.      <ell
-00007070: 6970 7365 0a20 2020 2020 2020 2020 7374  ipse.         st
-00007080: 796c 653d 2266 696c 6c3a 2331 3132 3036  yle="fill:#11206
-00007090: 363b 6669 6c6c 2d6f 7061 6369 7479 3a31  6;fill-opacity:1
-000070a0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-000070b0: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
-000070c0: 3530 3035 3b73 7472 6f6b 652d 6d69 7465  5005;stroke-mite
-000070d0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-000070e0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-000070f0: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-00007100: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
-00007110: 793a 3122 0a20 2020 2020 2020 2020 6964  y:1".         id
-00007120: 3d22 7061 7468 3134 3536 372d 332d 322d  ="path14567-3-2-
-00007130: 382d 3622 0a20 2020 2020 2020 2020 6378  8-6".         cx
-00007140: 3d22 3831 2e32 3932 3431 3922 0a20 2020  ="81.292419".   
-00007150: 2020 2020 2020 6379 3d22 3634 2e32 3133        cy="64.213
-00007160: 3136 3522 0a20 2020 2020 2020 2020 696e  165".         in
-00007170: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
-00007180: 2d63 656e 7465 722d 783d 2233 2e35 3931  -center-x="3.591
-00007190: 3336 3039 220a 2020 2020 2020 2020 2069  3609".         i
-000071a0: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-000071b0: 6d2d 6365 6e74 6572 2d79 3d22 2d37 2e36  m-center-y="-7.6
-000071c0: 3832 3839 3536 220a 2020 2020 2020 2020  828956".        
-000071d0: 2072 783d 2234 2e38 3731 3139 3239 220a   rx="4.8711929".
-000071e0: 2020 2020 2020 2020 2072 793d 2234 2e38           ry="4.8
-000071f0: 3439 3237 3337 2220 2f3e 0a20 2020 2020  492737" />.     
-00007200: 203c 656c 6c69 7073 650a 2020 2020 2020   <ellipse.      
-00007210: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00007220: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
-00007230: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
-00007240: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-00007250: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
-00007260: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00007270: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00007280: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00007290: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-000072a0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-000072b0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-000072c0: 7468 3134 3536 372d 322d 3739 2d31 220a  th14567-2-79-1".
-000072d0: 2020 2020 2020 2020 2063 783d 2231 3037           cx="107
-000072e0: 2e36 3737 3032 220a 2020 2020 2020 2020  .67702".        
-000072f0: 2063 793d 2236 392e 3631 3533 3536 220a   cy="69.615356".
-00007300: 2020 2020 2020 2020 2072 783d 2233 2e31           rx="3.1
-00007310: 3536 3232 3634 220a 2020 2020 2020 2020  562264".        
-00007320: 2072 793d 2233 2e31 3432 3032 3422 202f   ry="3.142024" /
-00007330: 3e0a 2020 2020 2020 3c65 6c6c 6970 7365  >.      <ellipse
-00007340: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00007350: 2266 696c 6c3a 2365 6466 3066 633b 6669  "fill:#edf0fc;fi
-00007360: 6c6c 2d6f 7061 6369 7479 3a30 2e39 3930  ll-opacity:0.990
-00007370: 3434 363b 7374 726f 6b65 3a23 6666 6666  446;stroke:#ffff
-00007380: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00007390: 312e 3035 3030 353b 7374 726f 6b65 2d6d  1.05005;stroke-m
-000073a0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-000073b0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-000073c0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-000073d0: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-000073e0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
-000073f0: 2069 643d 2270 6174 6831 3435 3637 2d32   id="path14567-2
-00007400: 2d38 2d32 2d30 220a 2020 2020 2020 2020  -8-2-0".        
-00007410: 2063 783d 2235 332e 3033 3635 3735 220a   cx="53.036575".
-00007420: 2020 2020 2020 2020 2063 793d 2239 352e           cy="95.
-00007430: 3639 3439 3737 220a 2020 2020 2020 2020  694977".        
-00007440: 2072 783d 2233 2e31 3536 3232 3634 220a   rx="3.1562264".
-00007450: 2020 2020 2020 2020 2072 793d 2233 2e31           ry="3.1
-00007460: 3432 3032 3422 202f 3e0a 2020 2020 2020  42024" />.      
-00007470: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-00007480: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
-00007490: 3030 3b66 696c 6c2d 6f70 6163 6974 793a  00;fill-opacity:
-000074a0: 302e 3939 3834 3038 3b73 7472 6f6b 653a  0.998408;stroke:
-000074b0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
-000074c0: 6964 7468 3a30 2e33 3233 3538 3870 783b  idth:0.323588px;
-000074d0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-000074e0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-000074f0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00007500: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00007510: 2020 2020 2064 3d22 6d20 3331 382e 3730       d="m 318.70
-00007520: 3133 332c 3732 2e37 3031 3732 2032 362e  133,72.70172 26.
-00007530: 3630 3435 372c 2d38 2e37 3836 3833 202d  60457,-8.78683 -
-00007540: 3238 2e33 3833 3935 2c2d 312e 3437 3538  28.38395,-1.4758
-00007550: 3620 6320 3131 2e30 3035 3236 2c33 2e32  6 c 11.00526,3.2
-00007560: 3034 3636 2031 312e 3035 3533 2c33 2e33  0466 11.0553,3.3
-00007570: 3734 3237 2031 2e37 3739 3338 2c31 302e  7427 1.77938,10.
-00007580: 3236 3236 3920 7a22 0a20 2020 2020 2020  26269 z".       
-00007590: 2020 6964 3d22 7061 7468 3134 3635 372d    id="path14657-
-000075a0: 392d 302d 3622 0a20 2020 2020 2020 2020  9-0-6".         
-000075b0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-000075c0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-000075d0: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-000075e0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-000075f0: 6363 2220 2f3e 0a20 2020 2020 203c 656c  cc" />.      <el
-00007600: 6c69 7073 650a 2020 2020 2020 2020 2073  lipse.         s
-00007610: 7479 6c65 3d22 6669 6c6c 3a23 6564 6630  tyle="fill:#edf0
-00007620: 6663 3b66 696c 6c2d 6f70 6163 6974 793a  fc;fill-opacity:
-00007630: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
-00007640: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00007650: 6964 7468 3a31 2e39 3935 3938 3b73 7472  idth:1.99598;str
-00007660: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00007670: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00007680: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-00007690: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-000076a0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000076b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-000076c0: 3536 372d 322d 372d 322d 3322 0a20 2020  567-2-7-2-3".   
-000076d0: 2020 2020 2020 6378 3d22 3137 372e 3437        cx="177.47
-000076e0: 3435 3622 0a20 2020 2020 2020 2020 6379  456".         cy
-000076f0: 3d22 3834 2e33 3331 3732 3622 0a20 2020  ="84.331726".   
-00007700: 2020 2020 2020 7278 3d22 352e 3939 3935        rx="5.9995
-00007710: 3232 3222 0a20 2020 2020 2020 2020 7279  222".         ry
-00007720: 3d22 352e 3937 3235 3235 3622 202f 3e0a  ="5.9725256" />.
-00007730: 2020 2020 2020 3c74 6578 740a 2020 2020        <text.    
-00007740: 2020 2020 2078 6d6c 3a73 7061 6365 3d22       xml:space="
-00007750: 7072 6573 6572 7665 220a 2020 2020 2020  preserve".      
-00007760: 2020 2073 7479 6c65 3d22 666f 6e74 2d73     style="font-s
-00007770: 7479 6c65 3a6e 6f72 6d61 6c3b 666f 6e74  tyle:normal;font
-00007780: 2d77 6569 6768 743a 6e6f 726d 616c 3b66  -weight:normal;f
-00007790: 6f6e 742d 7369 7a65 3a35 2e38 3732 3931  ont-size:5.87291
-000077a0: 7078 3b6c 696e 652d 6865 6967 6874 3a31  px;line-height:1
-000077b0: 2e32 353b 666f 6e74 2d66 616d 696c 793a  .25;font-family:
-000077c0: 7361 6e73 2d73 6572 6966 3b6c 6574 7465  sans-serif;lette
-000077d0: 722d 7370 6163 696e 673a 3070 783b 776f  r-spacing:0px;wo
-000077e0: 7264 2d73 7061 6369 6e67 3a30 7078 3b66  rd-spacing:0px;f
-000077f0: 696c 6c3a 2366 6666 6666 663b 6669 6c6c  ill:#ffffff;fill
-00007800: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00007810: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
-00007820: 6474 683a 302e 3430 3034 3235 3b66 696c  dth:0.400425;fil
-00007830: 7465 723a 7572 6c28 2366 696c 7465 7231  ter:url(#filter1
-00007840: 3530 3531 2d33 2d32 2922 0a20 2020 2020  5051-3-2)".     
-00007850: 2020 2020 783d 2237 372e 3639 3438 3933      x="77.694893
-00007860: 220a 2020 2020 2020 2020 2079 3d22 3931  ".         y="91
-00007870: 2e39 3838 3434 3922 0a20 2020 2020 2020  .988449".       
-00007880: 2020 6964 3d22 7465 7874 3134 3639 312d    id="text14691-
-00007890: 362d 332d 3222 0a20 2020 2020 2020 2020  6-3-2".         
-000078a0: 7472 616e 7366 6f72 6d3d 226d 6174 7269  transform="matri
-000078b0: 7828 322e 3735 3131 3931 392c 302c 302c  x(2.7511919,0,0,
-000078c0: 322e 3733 3838 3132 2c2d 3735 2e39 3736  2.738812,-75.976
-000078d0: 3639 362c 2d31 3038 2e30 3838 3636 2922  696,-108.08866)"
-000078e0: 3e3c 7473 7061 6e0a 2020 2020 2020 2020  ><tspan.        
-000078f0: 2020 2073 6f64 6970 6f64 693a 726f 6c65     sodipodi:role
-00007900: 3d22 6c69 6e65 220a 2020 2020 2020 2020  ="line".        
-00007910: 2020 2069 643d 2274 7370 616e 3134 3638     id="tspan1468
-00007920: 392d 322d 372d 3022 0a20 2020 2020 2020  9-2-7-0".       
-00007930: 2020 2020 783d 2237 372e 3639 3438 3933      x="77.694893
-00007940: 220a 2020 2020 2020 2020 2020 2079 3d22  ".           y="
-00007950: 3931 2e39 3838 3434 3922 0a20 2020 2020  91.988449".     
-00007960: 2020 2020 2020 7374 796c 653d 2266 6f6e        style="fon
-00007970: 742d 7374 796c 653a 6e6f 726d 616c 3b66  t-style:normal;f
-00007980: 6f6e 742d 7661 7269 616e 743a 6e6f 726d  ont-variant:norm
-00007990: 616c 3b66 6f6e 742d 7765 6967 6874 3a6e  al;font-weight:n
-000079a0: 6f72 6d61 6c3b 666f 6e74 2d73 7472 6574  ormal;font-stret
-000079b0: 6368 3a6e 6f72 6d61 6c3b 666f 6e74 2d73  ch:normal;font-s
-000079c0: 697a 653a 3231 2e33 3536 7078 3b66 6f6e  ize:21.356px;fon
-000079d0: 742d 6661 6d69 6c79 3a49 6d70 6163 743b  t-family:Impact;
-000079e0: 2d69 6e6b 7363 6170 652d 666f 6e74 2d73  -inkscape-font-s
-000079f0: 7065 6369 6669 6361 7469 6f6e 3a49 6d70  pecification:Imp
-00007a00: 6163 743b 6669 6c6c 3a23 6666 6666 6666  act;fill:#ffffff
-00007a10: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-00007a20: 7374 726f 6b65 2d77 6964 7468 3a30 2e34  stroke-width:0.4
-00007a30: 3030 3432 3522 3e53 6165 6e6f 7079 3c2f  00425">Saenopy</
-00007a40: 7473 7061 6e3e 3c2f 7465 7874 3e0a 2020  tspan></text>.  
-00007a50: 2020 2020 3c74 6578 740a 2020 2020 2020      <text.      
-00007a60: 2020 2078 6d6c 3a73 7061 6365 3d22 7072     xml:space="pr
-00007a70: 6573 6572 7665 220a 2020 2020 2020 2020  eserve".        
-00007a80: 2073 7479 6c65 3d22 666f 6e74 2d73 7479   style="font-sty
-00007a90: 6c65 3a6e 6f72 6d61 6c3b 666f 6e74 2d77  le:normal;font-w
-00007aa0: 6569 6768 743a 6e6f 726d 616c 3b66 6f6e  eight:normal;fon
-00007ab0: 742d 7369 7a65 3a31 362e 3132 3131 7078  t-size:16.1211px
-00007ac0: 3b6c 696e 652d 6865 6967 6874 3a31 2e32  ;line-height:1.2
-00007ad0: 353b 666f 6e74 2d66 616d 696c 793a 7361  5;font-family:sa
-00007ae0: 6e73 2d73 6572 6966 3b6c 6574 7465 722d  ns-serif;letter-
-00007af0: 7370 6163 696e 673a 3070 783b 776f 7264  spacing:0px;word
-00007b00: 2d73 7061 6369 6e67 3a30 7078 3b66 696c  -spacing:0px;fil
-00007b10: 6c3a 2330 3030 3030 303b 6669 6c6c 2d6f  l:#000000;fill-o
-00007b20: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00007b30: 6e6f 6e65 3b73 7472 6f6b 652d 7769 6474  none;stroke-widt
-00007b40: 683a 312e 3039 3931 3722 0a20 2020 2020  h:1.09917".     
-00007b50: 2020 2020 783d 2231 3335 2e34 3739 3036      x="135.47906
-00007b60: 220a 2020 2020 2020 2020 2079 3d22 3133  ".         y="13
-00007b70: 362e 3338 3737 220a 2020 2020 2020 2020  6.3877".        
-00007b80: 2069 643d 2274 6578 7431 3436 3931 2d35   id="text14691-5
-00007b90: 2d36 220a 2020 2020 2020 2020 2074 7261  -6".         tra
-00007ba0: 6e73 666f 726d 3d22 7363 616c 6528 312e  nsform="scale(1.
-00007bb0: 3030 3232 3537 352c 302e 3939 3737 3437  0022575,0.997747
-00007bc0: 3538 2922 3e3c 7473 7061 6e0a 2020 2020  58)"><tspan.    
-00007bd0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00007be0: 726f 6c65 3d22 6c69 6e65 220a 2020 2020  role="line".    
-00007bf0: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
-00007c00: 3134 3638 392d 392d 3122 0a20 2020 2020  14689-9-1".     
-00007c10: 2020 2020 2020 783d 2231 3335 2e34 3739        x="135.479
-00007c20: 3036 220a 2020 2020 2020 2020 2020 2079  06".           y
-00007c30: 3d22 3133 362e 3338 3737 220a 2020 2020  ="136.3877".    
-00007c40: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
-00007c50: 6e74 2d73 7479 6c65 3a6e 6f72 6d61 6c3b  nt-style:normal;
-00007c60: 666f 6e74 2d76 6172 6961 6e74 3a6e 6f72  font-variant:nor
-00007c70: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
-00007c80: 6e6f 726d 616c 3b66 6f6e 742d 7374 7265  normal;font-stre
-00007c90: 7463 683a 6e6f 726d 616c 3b66 6f6e 742d  tch:normal;font-
-00007ca0: 7369 7a65 3a35 382e 3632 3231 7078 3b66  size:58.6221px;f
-00007cb0: 6f6e 742d 6661 6d69 6c79 3a27 546c 7767  ont-family:'Tlwg
-00007cc0: 2054 7970 6973 7427 3b2d 696e 6b73 6361   Typist';-inksca
-00007cd0: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
-00007ce0: 6174 696f 6e3a 2754 6c77 6720 5479 7069  ation:'Tlwg Typi
-00007cf0: 7374 273b 7374 726f 6b65 2d77 6964 7468  st';stroke-width
-00007d00: 3a31 2e30 3939 3137 223e 5361 656e 6f70  :1.09917">Saenop
-00007d10: 793c 2f74 7370 616e 3e3c 2f74 6578 743e  y</tspan></text>
-00007d20: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
-00007d30: 0a20 2020 2020 2020 6964 3d22 6739 3034  .       id="g904
-00007d40: 220a 2020 2020 2020 2074 7261 6e73 666f  ".       transfo
-00007d50: 726d 3d22 6d61 7472 6978 2832 2e36 3837  rm="matrix(2.687
-00007d60: 3937 3433 2c30 2c30 2c32 2e36 3837 3937  9743,0,0,2.68797
-00007d70: 3433 2c2d 352e 3030 3430 3331 352c 2d39  43,-5.0040315,-9
-00007d80: 392e 3932 3838 3935 2922 3e0a 2020 2020  9.928895)">.    
-00007d90: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00007da0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3365   style="fill:#3e
-00007db0: 3462 3737 3b66 696c 6c2d 6f70 6163 6974  4b77;fill-opacit
-00007dc0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00007dd0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00007de0: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
-00007df0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00007e00: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00007e10: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-00007e20: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00007e30: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00007e40: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00007e50: 2020 2020 2020 2020 643d 226d 2035 2e37          d="m 5.7
-00007e60: 3538 3439 3036 2c31 3631 2e38 3336 3531  584906,161.83651
-00007e70: 2033 322e 3333 3936 3230 342c 2d31 2e34   32.3396204,-1.4
-00007e80: 3639 3938 2032 312e 3234 3739 332c 2d32  6998 21.24793,-2
-00007e90: 332e 3635 3333 3520 6320 2d32 362e 3736  3.65335 c -26.76
-00007ea0: 3738 392c 3138 2e30 3031 3837 202d 3339  789,18.00187 -39
-00007eb0: 2e35 3536 3434 2c32 302e 3839 3039 3520  .55644,20.89095 
-00007ec0: 2d35 332e 3538 3735 3530 342c 3235 2e31  -53.5875504,25.1
-00007ed0: 3233 3333 207a 220a 2020 2020 2020 2020  2333 z".        
-00007ee0: 2069 643d 2270 6174 6831 3435 3437 2d31   id="path14547-1
-00007ef0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00007f00: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00007f10: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-00007f20: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-00007f30: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
-00007f40: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00007f50: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00007f60: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00007f70: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00007f80: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00007f90: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-00007fa0: 7479 6c65 3d22 6669 6c6c 3a23 3163 3263  tyle="fill:#1c2c
-00007fb0: 3638 3b66 696c 6c2d 6f70 6163 6974 793a  68;fill-opacity:
-00007fc0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00007fd0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00007fe0: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
-00007ff0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00008000: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00008010: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00008020: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00008030: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00008040: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00008050: 2020 2020 2020 643d 226d 2033 382e 3039        d="m 38.09
-00008060: 3831 3131 2c31 3630 2e33 3636 3533 2031  8111,160.36653 1
-00008070: 342e 3033 3136 352c 332e 3230 3732 3420  4.03165,3.20724 
-00008080: 372e 3231 3632 382c 2d32 362e 3836 3035  7.21628,-26.8605
-00008090: 3920 7a22 0a20 2020 2020 2020 2020 6964  9 z".         id
-000080a0: 3d22 7061 7468 3134 3534 392d 3122 0a20  ="path14549-1". 
-000080b0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000080c0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-000080d0: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
-000080e0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-000080f0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-00008100: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00008110: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-00008120: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
-00008130: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-00008140: 6669 6c6c 3a23 3036 3035 3038 3b66 696c  fill:#060508;fil
-00008150: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00008160: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00008170: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00008180: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-00008190: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-000081a0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-000081b0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-000081c0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-000081d0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-000081e0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-000081f0: 643d 226d 2035 322e 3132 3937 3631 2c31  d="m 52.129761,1
-00008200: 3633 2e35 3733 3737 2033 372e 3535 3133  63.57377 37.5513
-00008210: 372c 362e 3638 3137 3420 6320 2d31 342e  7,6.68174 c -14.
-00008220: 3633 3331 322c 2d37 2e37 3335 3839 202d  63312,-7.73589 -
-00008230: 3233 2e31 3036 3934 2c2d 3230 2e31 3634  23.10694,-20.164
-00008240: 3536 202d 3330 2e33 3335 3039 2c2d 3333  56 -30.33509,-33
-00008250: 2e35 3432 3333 207a 220a 2020 2020 2020  .54233 z".      
-00008260: 2020 2069 643d 2270 6174 6831 3435 3531     id="path14551
-00008270: 2d30 220a 2020 2020 2020 2020 2069 6e6b  -0".         ink
-00008280: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-00008290: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-000082a0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-000082b0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
-000082c0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000082d0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-000082e0: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-000082f0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00008300: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00008310: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00008320: 2073 7479 6c65 3d22 6669 6c6c 3a23 3237   style="fill:#27
-00008330: 3337 3733 3b66 696c 6c2d 6f70 6163 6974  3773;fill-opacit
-00008340: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00008350: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00008360: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
-00008370: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00008380: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00008390: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-000083a0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-000083b0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-000083c0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-000083d0: 2020 2020 2020 2020 643d 226d 2035 2e37          d="m 5.7
-000083e0: 3538 3439 3036 2c31 3631 2e38 3336 3531  584906,161.83651
-000083f0: 2063 2037 2e31 3136 3432 3034 2c34 2e30   c 7.1164204,4.0
-00008400: 3832 3434 2031 342e 3936 3237 3230 342c  8244 14.9627204,
-00008410: 372e 3630 3334 3320 3137 2e36 3339 3739  7.60343 17.63979
-00008420: 3034 2c31 352e 3130 3037 3420 6c20 3134  04,15.10074 l 14
-00008430: 2e36 3939 3833 2c2d 3136 2e35 3730 3732  .69983,-16.57072
-00008440: 207a 220a 2020 2020 2020 2020 2069 643d   z".         id=
-00008450: 2270 6174 6831 3435 3533 2d33 220a 2020  "path14553-3".  
-00008460: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00008470: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00008480: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
-00008490: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-000084a0: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
-000084b0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-000084c0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-000084d0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000084e0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-000084f0: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
-00008500: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
-00008510: 3d22 6669 6c6c 3a23 3134 3236 3732 3b66  ="fill:#142672;f
-00008520: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00008530: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00008540: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
-00008550: 3235 3b73 7472 6f6b 652d 6c69 6e65 6361  25;stroke-lineca
-00008560: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00008570: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00008580: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00008590: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000085a0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-000085b0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-000085c0: 2020 643d 226d 2032 332e 3339 3832 3831    d="m 23.398281
-000085d0: 2c31 3736 2e39 3337 3235 2036 362e 3238  ,176.93725 66.28
-000085e0: 3238 352c 2d36 2e36 3831 3734 202d 3531  285,-6.68174 -51
-000085f0: 2e35 3833 3032 2c2d 392e 3838 3839 3820  .58302,-9.88898 
-00008600: 7a22 0a20 2020 2020 2020 2020 6964 3d22  z".         id="
-00008610: 7061 7468 3134 3535 352d 3422 0a20 2020  path14555-4".   
-00008620: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00008630: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00008640: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
-00008650: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00008660: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-00008670: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00008680: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-00008690: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
-000086a0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-000086b0: 6c6c 3a23 3534 3636 3863 3b66 696c 6c2d  ll:#54668c;fill-
-000086c0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-000086d0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-000086e0: 7769 6474 683a 302e 3535 3536 3235 3b73  width:0.555625;s
-000086f0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-00008700: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-00008710: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-00008720: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-00008730: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-00008740: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00008750: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
-00008760: 226d 2032 332e 3339 3832 3831 2c31 3736  "m 23.398281,176
-00008770: 2e39 3337 3235 2033 382e 3231 3935 352c  .93725 38.21955,
-00008780: 342e 3030 3930 3420 3238 2e30 3633 332c  4.00904 28.0633,
-00008790: 2d31 302e 3639 3037 3820 7a22 0a20 2020  -10.69078 z".   
-000087a0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-000087b0: 3535 372d 3022 0a20 2020 2020 2020 2020  557-0".         
-000087c0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-000087d0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-000087e0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000087f0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00008800: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00008810: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00008820: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00008830: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00008840: 2073 7479 6c65 3d22 6669 6c6c 3a23 3232   style="fill:#22
-00008850: 3334 3765 3b66 696c 6c2d 6f70 6163 6974  347e;fill-opacit
-00008860: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00008870: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00008880: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
-00008890: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-000088a0: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-000088b0: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-000088c0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-000088d0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-000088e0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-000088f0: 2020 2020 2020 2020 643d 226d 2032 332e          d="m 23.
-00008900: 3339 3832 3831 2c31 3736 2e39 3337 3235  398281,176.93725
-00008910: 2063 2030 2e38 3539 3432 2c37 2e34 3130   c 0.85942,7.410
-00008920: 3134 202d 322e 3131 3533 372c 3132 2e30  14 -2.11537,12.0
-00008930: 3831 3537 202d 332e 3437 3435 2c31 372e  8157 -3.4745,17.
-00008940: 3930 3730 3520 6c20 3431 2e36 3934 3035  90705 l 41.69405
-00008950: 2c2d 3133 2e38 3938 3031 207a 220a 2020  ,-13.89801 z".  
-00008960: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00008970: 3435 3539 2d33 220a 2020 2020 2020 2020  4559-3".        
-00008980: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-00008990: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-000089a0: 220a 2020 2020 2020 2020 2073 6f64 6970  ".         sodip
-000089b0: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
-000089c0: 6363 6322 0a20 2020 2020 2020 2020 696e  ccc".         in
-000089d0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-000089e0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-000089f0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00008a00: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
-00008a10: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
-00008a20: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00008a30: 3a23 3038 3130 3639 3b66 696c 6c2d 6f70  :#081069;fill-op
-00008a40: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-00008a50: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-00008a60: 6474 683a 302e 3535 3536 3235 3b73 7472  dth:0.555625;str
-00008a70: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-00008a80: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00008a90: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-00008aa0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00008ab0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00008ac0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00008ad0: 3122 0a20 2020 2020 2020 2020 643d 226d  1".         d="m
-00008ae0: 2031 392e 3932 3337 3831 2c31 3934 2e38   19.923781,194.8
-00008af0: 3434 3320 3238 2e38 3635 3131 2c34 2e32  443 28.86511,4.2
-00008b00: 3736 3332 2034 302e 3839 3232 342c 2d32  7632 40.89224,-2
-00008b10: 382e 3836 3531 3120 7a22 0a20 2020 2020  8.86511 z".     
-00008b20: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-00008b30: 312d 3922 0a20 2020 2020 2020 2020 696e  1-9".         in
-00008b40: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-00008b50: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-00008b60: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00008b70: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00008b80: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00008b90: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00008ba0: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00008bb0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-00008bc0: 7479 6c65 3d22 6669 6c6c 3a23 3037 3065  tyle="fill:#070e
-00008bd0: 3262 3b66 696c 6c2d 6f70 6163 6974 793a  2b;fill-opacity:
-00008be0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00008bf0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00008c00: 3535 3536 3235 3b73 7472 6f6b 652d 6c69  555625;stroke-li
-00008c10: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-00008c20: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-00008c30: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00008c40: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00008c50: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00008c60: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00008c70: 2020 2020 2020 643d 226d 2034 382e 3738        d="m 48.78
-00008c80: 3838 3931 2c31 3939 2e31 3230 3632 2031  8891,199.12062 1
-00008c90: 362e 3937 3136 312c 3232 2e33 3137 3031  6.97161,22.31701
-00008ca0: 202d 362e 3238 3038 332c 2d33 302e 3036   -6.28083,-30.06
-00008cb0: 3738 3220 7a22 0a20 2020 2020 2020 2020  782 z".         
-00008cc0: 6964 3d22 7061 7468 3134 3536 332d 3122  id="path14563-1"
-00008cd0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00008ce0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-00008cf0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-00008d00: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00008d10: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00008d20: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00008d30: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00008d40: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
-00008d50: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
-00008d60: 3d22 6669 6c6c 3a23 3238 3364 3837 3b66  ="fill:#283d87;f
-00008d70: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00008d80: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00008d90: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
-00008da0: 3235 3b73 7472 6f6b 652d 6c69 6e65 6361  25;stroke-lineca
-00008db0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-00008dc0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-00008dd0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00008de0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00008df0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-00008e00: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00008e10: 2020 643d 226d 2035 392e 3437 3936 3731    d="m 59.479671
-00008e20: 2c31 3931 2e33 3639 3831 2036 2e32 3830  ,191.36981 6.280
-00008e30: 3833 2c33 302e 3036 3738 3220 6320 332e  83,30.06782 c 3.
-00008e40: 3235 3134 352c 2d32 372e 3032 3935 3720  25145,-27.02957 
-00008e50: 3134 2e36 3933 3635 2c2d 3336 2e37 3637  14.69365,-36.767
-00008e60: 3536 2032 332e 3932 3036 332c 2d35 312e  56 23.92063,-51.
-00008e70: 3138 3231 3220 7a22 0a20 2020 2020 2020  18212 z".       
-00008e80: 2020 6964 3d22 7061 7468 3134 3536 352d    id="path14565-
-00008e90: 3922 0a20 2020 2020 2020 2020 696e 6b73  9".         inks
-00008ea0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-00008eb0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-00008ec0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-00008ed0: 6f64 6574 7970 6573 3d22 6363 6363 220a  odetypes="cccc".
-00008ee0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-00008ef0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-00008f00: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
-00008f10: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-00008f20: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
-00008f30: 203c 656c 6c69 7073 650a 2020 2020 2020   <ellipse.      
-00008f40: 2020 2073 7479 6c65 3d22 6f70 6163 6974     style="opacit
-00008f50: 793a 313b 6669 6c6c 3a23 3037 3065 3262  y:1;fill:#070e2b
-00008f60: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
-00008f70: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
-00008f80: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00008f90: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
-00008fa0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00008fb0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00008fc0: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-00008fd0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-00008fe0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00008ff0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00009000: 3637 2d36 220a 2020 2020 2020 2020 2063  67-6".         c
-00009010: 783d 2236 2e34 3434 3836 3238 220a 2020  x="6.4448628".  
-00009020: 2020 2020 2020 2063 793d 2231 3631 2e38         cy="161.8
-00009030: 3730 3832 220a 2020 2020 2020 2020 2072  7082".         r
-00009040: 783d 2231 2e36 3636 3333 3237 220a 2020  x="1.6663327".  
-00009050: 2020 2020 2020 2072 793d 2231 2e36 3636         ry="1.666
-00009060: 3333 3238 220a 2020 2020 2020 2020 2069  3328".         i
-00009070: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00009080: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00009090: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-000090a0: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-000090b0: 0a20 2020 2020 203c 6369 7263 6c65 0a20  .      <circle. 
-000090c0: 2020 2020 2020 2020 723d 2231 2e36 3636          r="1.666
-000090d0: 3333 3238 220a 2020 2020 2020 2020 2073  3328".         s
-000090e0: 7479 6c65 3d22 6f70 6163 6974 793a 313b  tyle="opacity:1;
-000090f0: 6669 6c6c 3a23 3235 3361 3764 3b66 696c  fill:#253a7d;fil
-00009100: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-00009110: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00009120: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00009130: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00009140: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00009150: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00009160: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-00009170: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00009180: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00009190: 7468 3134 3536 372d 332d 3933 220a 2020  th14567-3-93".  
-000091a0: 2020 2020 2020 2063 783d 2231 392e 3635         cx="19.65
-000091b0: 3536 3332 220a 2020 2020 2020 2020 2063  5632".         c
-000091c0: 793d 2231 3934 2e34 3838 3835 220a 2020  y="194.48885".  
-000091d0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-000091e0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-000091f0: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
-00009200: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00009210: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-00009220: 722d 793d 222d 392e 3937 3830 3632 3122  r-y="-9.9780621"
-00009230: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00009240: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00009250: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00009260: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00009270: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00009280: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-00009290: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
-000092a0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-000092b0: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
-000092c0: 2332 3533 6137 643b 6669 6c6c 2d6f 7061  #253a7d;fill-opa
-000092d0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-000092e0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-000092f0: 7468 3a30 2e35 3535 3632 353b 7374 726f  th:0.555625;stro
-00009300: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00009310: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00009320: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-00009330: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-00009340: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00009350: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00009360: 3637 2d33 2d37 2d33 220a 2020 2020 2020  67-3-7-3".      
-00009370: 2020 2063 783d 2235 392e 3037 3339 3231     cx="59.073921
-00009380: 220a 2020 2020 2020 2020 2063 793d 2231  ".         cy="1
-00009390: 3831 2e30 3533 3031 220a 2020 2020 2020  81.05301".      
-000093a0: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
-000093b0: 7366 6f72 6d2d 6365 6e74 6572 2d78 3d22  sform-center-x="
-000093c0: 342e 3634 3332 3536 3622 0a20 2020 2020  4.6432566".     
-000093d0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-000093e0: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
-000093f0: 222d 392e 3937 3830 3632 3122 0a20 2020  "-9.9780621".   
-00009400: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00009410: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-00009420: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00009430: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-00009440: 3330 3022 202f 3e0a 2020 2020 2020 3c63  300" />.      <c
-00009450: 6972 636c 650a 2020 2020 2020 2020 2072  ircle.         r
-00009460: 3d22 312e 3636 3633 3332 3822 0a20 2020  ="1.6663328".   
-00009470: 2020 2020 2020 7374 796c 653d 226f 7061        style="opa
-00009480: 6369 7479 3a31 3b66 696c 6c3a 2361 3861  city:1;fill:#a8a
-00009490: 3961 613b 6669 6c6c 2d6f 7061 6369 7479  9aa;fill-opacity
-000094a0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-000094b0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-000094c0: 2e35 3535 3632 353b 7374 726f 6b65 2d6d  .555625;stroke-m
-000094d0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-000094e0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-000094f0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-00009500: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-00009510: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
-00009520: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
-00009530: 2d35 2d38 220a 2020 2020 2020 2020 2063  -5-8".         c
-00009540: 783d 2235 392e 3436 3930 3933 220a 2020  x="59.469093".  
-00009550: 2020 2020 2020 2063 793d 2231 3931 2e31         cy="191.1
-00009560: 3239 3837 220a 2020 2020 2020 2020 2069  2987".         i
-00009570: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
-00009580: 6d2d 6365 6e74 6572 2d78 3d22 342e 3634  m-center-x="4.64
-00009590: 3332 3536 3622 0a20 2020 2020 2020 2020  32566".         
-000095a0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
-000095b0: 726d 2d63 656e 7465 722d 793d 222d 392e  rm-center-y="-9.
-000095c0: 3937 3830 3632 3122 0a20 2020 2020 2020  9780621".       
-000095d0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-000095e0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-000095f0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00009600: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-00009610: 202f 3e0a 2020 2020 2020 3c63 6972 636c   />.      <circl
-00009620: 650a 2020 2020 2020 2020 2072 3d22 312e  e.         r="1.
-00009630: 3636 3633 3332 3822 0a20 2020 2020 2020  6663328".       
-00009640: 2020 7374 796c 653d 226f 7061 6369 7479    style="opacity
-00009650: 3a31 3b66 696c 6c3a 2361 6261 6139 633b  :1;fill:#abaa9c;
-00009660: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-00009670: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00009680: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
-00009690: 3632 353b 7374 726f 6b65 2d6d 6974 6572  625;stroke-miter
-000096a0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-000096b0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-000096c0: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
-000096d0: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
-000096e0: 3a31 220a 2020 2020 2020 2020 2069 643d  :1".         id=
-000096f0: 2270 6174 6831 3435 3637 2d33 2d39 2d30  "path14567-3-9-0
-00009700: 220a 2020 2020 2020 2020 2063 783d 2234  ".         cx="4
-00009710: 392e 3139 3436 3439 220a 2020 2020 2020  9.194649".      
-00009720: 2020 2063 793d 2231 3939 2e30 3333 3238     cy="199.03328
-00009730: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00009740: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-00009750: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
-00009760: 3622 0a20 2020 2020 2020 2020 696e 6b73  6".         inks
-00009770: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
-00009780: 656e 7465 722d 793d 222d 392e 3937 3830  enter-y="-9.9780
-00009790: 3632 3122 0a20 2020 2020 2020 2020 696e  621".         in
-000097a0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-000097b0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-000097c0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-000097d0: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
-000097e0: 2020 2020 2020 3c63 6972 636c 650a 2020        <circle.  
-000097f0: 2020 2020 2020 2072 3d22 322e 3537 3137         r="2.5717
-00009800: 3531 3122 0a20 2020 2020 2020 2020 7374  511".         st
-00009810: 796c 653d 226f 7061 6369 7479 3a31 3b66  yle="opacity:1;f
-00009820: 696c 6c3a 2331 3132 3036 363b 6669 6c6c  ill:#112066;fill
-00009830: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00009840: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00009850: 2d77 6964 7468 3a30 2e35 3535 3632 353b  -width:0.555625;
-00009860: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00009870: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00009880: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00009890: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-000098a0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-000098b0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-000098c0: 6831 3435 3637 2d33 2d32 2d35 220a 2020  h14567-3-2-5".  
-000098d0: 2020 2020 2020 2063 783d 2233 382e 3332         cx="38.32
-000098e0: 3734 3436 220a 2020 2020 2020 2020 2063  7446".         c
-000098f0: 793d 2231 3630 2e30 3130 3138 220a 2020  y="160.01018".  
-00009900: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00009910: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-00009920: 2d78 3d22 372e 3136 3632 3131 3622 0a20  -x="7.1662116". 
-00009930: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00009940: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-00009950: 722d 793d 222d 3135 2e33 3939 3735 3122  r-y="-15.399751"
-00009960: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00009970: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00009980: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00009990: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-000099a0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-000099b0: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-000099c0: 2020 2072 3d22 312e 3636 3633 3332 3822     r="1.6663328"
-000099d0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-000099e0: 226f 7061 6369 7479 3a31 3b66 696c 6c3a  "opacity:1;fill:
-000099f0: 2365 6466 3066 633b 6669 6c6c 2d6f 7061  #edf0fc;fill-opa
-00009a00: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
-00009a10: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00009a20: 6f6b 652d 7769 6474 683a 302e 3535 3536  oke-width:0.5556
-00009a30: 3235 3b73 7472 6f6b 652d 6d69 7465 726c  25;stroke-miterl
-00009a40: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00009a50: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00009a60: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
-00009a70: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00009a80: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
-00009a90: 7061 7468 3134 3536 372d 322d 3622 0a20  path14567-2-6". 
-00009aa0: 2020 2020 2020 2020 6378 3d22 3532 2e32          cx="52.2
-00009ab0: 3537 3232 3522 0a20 2020 2020 2020 2020  57225".         
-00009ac0: 6379 3d22 3136 322e 3837 3531 3722 0a20  cy="162.87517". 
-00009ad0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00009ae0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00009af0: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00009b00: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00009b10: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00009b20: 3c63 6972 636c 650a 2020 2020 2020 2020  <circle.        
-00009b30: 2072 3d22 312e 3636 3633 3332 3822 0a20   r="1.6663328". 
-00009b40: 2020 2020 2020 2020 7374 796c 653d 226f          style="o
-00009b50: 7061 6369 7479 3a31 3b66 696c 6c3a 2365  pacity:1;fill:#e
-00009b60: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
-00009b70: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
-00009b80: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00009b90: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
-00009ba0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-00009bb0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-00009bc0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-00009bd0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-00009be0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00009bf0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
-00009c00: 7468 3134 3536 372d 322d 382d 3622 0a20  th14567-2-8-6". 
-00009c10: 2020 2020 2020 2020 6378 3d22 3233 2e34          cx="23.4
-00009c20: 3039 3735 3222 0a20 2020 2020 2020 2020  09752".         
-00009c30: 6379 3d22 3137 362e 3730 3631 3522 0a20  cy="176.70615". 
-00009c40: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00009c50: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00009c60: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00009c70: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-00009c80: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-00009c90: 3c63 6972 636c 650a 2020 2020 2020 2020  <circle.        
-00009ca0: 2072 3d22 332e 3136 3734 3533 3822 0a20   r="3.1674538". 
-00009cb0: 2020 2020 2020 2020 7374 796c 653d 226f          style="o
-00009cc0: 7061 6369 7479 3a31 3b66 696c 6c3a 2365  pacity:1;fill:#e
-00009cd0: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
-00009ce0: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
-00009cf0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00009d00: 652d 7769 6474 683a 312e 3035 3631 363b  e-width:1.05616;
-00009d10: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00009d20: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00009d30: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00009d40: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-00009d50: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00009d60: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00009d70: 6831 3435 3637 2d32 2d37 2d30 220a 2020  h14567-2-7-0".  
-00009d80: 2020 2020 2020 2063 783d 2238 392e 3130         cx="89.10
-00009d90: 3638 3935 220a 2020 2020 2020 2020 2063  6895".         c
-00009da0: 793d 2231 3730 2e36 3739 3739 220a 2020  y="170.67979".  
-00009db0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00009dc0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-00009dd0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00009de0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-00009df0: 2233 3030 2220 2f3e 0a20 2020 203c 2f67  "300" />.    </g
-00009e00: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
-00009e10: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-00009e20: 3365 3462 3737 3b66 696c 6c2d 6f70 6163  3e4b77;fill-opac
-00009e30: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-00009e40: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-00009e50: 683a 302e 3939 3939 3939 3b73 7472 6f6b  h:0.999999;strok
-00009e60: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00009e70: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00009e80: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00009e90: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00009ea0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00009eb0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00009ec0: 0a20 2020 2020 2020 643d 226d 2033 3137  .       d="m 317
-00009ed0: 2e30 3239 3335 2c33 3031 2e35 3339 3434  .02935,301.53944
-00009ee0: 2034 332e 3436 3430 332c 2d31 2e39 3735   43.46403,-1.975
-00009ef0: 3634 2032 382e 3535 3639 352c 2d33 312e  64 28.55695,-31.
-00009f00: 3738 3937 3920 6320 2d33 352e 3937 3537  78979 c -35.9757
-00009f10: 2c32 342e 3139 3432 3720 2d35 332e 3136  ,24.19427 -53.16
-00009f20: 3333 352c 3238 2e30 3737 3136 202d 3732  335,28.07716 -72
-00009f30: 2e30 3230 3938 2c33 332e 3736 3534 3320  .02098,33.76543 
-00009f40: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
-00009f50: 7468 3134 3534 372d 312d 3722 0a20 2020  th14547-1-7".   
-00009f60: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-00009f70: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-00009f80: 3d22 3022 0a20 2020 2020 2020 736f 6469  ="0".       sodi
-00009f90: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
-00009fa0: 6363 6363 220a 2020 2020 2020 2069 6e6b  cccc".       ink
-00009fb0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-00009fc0: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
-00009fd0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-00009fe0: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-00009ff0: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
-0000a000: 796c 653d 2266 696c 6c3a 2331 6332 6336  yle="fill:#1c2c6
-0000a010: 383b 6669 6c6c 2d6f 7061 6369 7479 3a31  8;fill-opacity:1
-0000a020: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-0000a030: 7374 726f 6b65 2d77 6964 7468 3a30 2e39  stroke-width:0.9
-0000a040: 3939 3939 393b 7374 726f 6b65 2d6c 696e  99999;stroke-lin
-0000a050: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-0000a060: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-0000a070: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-0000a080: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-0000a090: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-0000a0a0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-0000a0b0: 2020 2064 3d22 6d20 3336 302e 3439 3333     d="m 360.4933
-0000a0c0: 382c 3239 392e 3536 3338 2031 382e 3835  8,299.5638 18.85
-0000a0d0: 3833 362c 342e 3331 3035 3220 392e 3639  836,4.31052 9.69
-0000a0e0: 3835 392c 2d33 362e 3130 3033 3120 7a22  859,-36.10031 z"
-0000a0f0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000a100: 3134 3534 392d 312d 3022 0a20 2020 2020  14549-1-0".     
-0000a110: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000a120: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000a130: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000a140: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000a150: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000a160: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000a170: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
-0000a180: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-0000a190: 3d22 6669 6c6c 3a23 3036 3035 3038 3b66  ="fill:#060508;f
-0000a1a0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000a1b0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000a1c0: 6f6b 652d 7769 6474 683a 302e 3939 3939  oke-width:0.9999
-0000a1d0: 3939 3b73 7472 6f6b 652d 6c69 6e65 6361  99;stroke-lineca
-0000a1e0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-0000a1f0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-0000a200: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-0000a210: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-0000a220: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-0000a230: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000a240: 643d 226d 2033 3739 2e33 3531 3734 2c33  d="m 379.35174,3
-0000a250: 3033 2e38 3734 3332 2035 302e 3436 3835  03.87432 50.4685
-0000a260: 382c 382e 3938 3031 3520 6320 2d31 392e  8,8.98015 c -19.
-0000a270: 3636 3637 342c 2d31 302e 3339 3639 3520  66674,-10.39695 
-0000a280: 2d33 312e 3035 3534 342c 2d32 372e 3130  -31.05544,-27.10
-0000a290: 3039 3120 2d34 302e 3736 3939 392c 2d34  091 -40.76999,-4
-0000a2a0: 352e 3038 3034 3620 7a22 0a20 2020 2020  5.08046 z".     
-0000a2b0: 2020 6964 3d22 7061 7468 3134 3535 312d    id="path14551-
-0000a2c0: 302d 3322 0a20 2020 2020 2020 696e 6b73  0-3".       inks
-0000a2d0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-0000a2e0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-0000a2f0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-0000a300: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
-0000a310: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000a320: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-0000a330: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000a340: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-0000a350: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
-0000a360: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-0000a370: 6c3a 2332 3733 3737 333b 6669 6c6c 2d6f  l:#273773;fill-o
-0000a380: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-0000a390: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-0000a3a0: 6964 7468 3a30 2e39 3939 3939 393b 7374  idth:0.999999;st
-0000a3b0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-0000a3c0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-0000a3d0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-0000a3e0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000a3f0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000a400: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-0000a410: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
-0000a420: 3331 372e 3032 3933 352c 3330 312e 3533  317.02935,301.53
-0000a430: 3934 3420 6320 392e 3536 3433 382c 352e  944 c 9.56438,5.
-0000a440: 3438 3637 3420 3230 2e31 3039 372c 3130  48674 20.1097,10
-0000a450: 2e32 3138 3933 2032 332e 3730 3736 352c  .21893 23.70765,
-0000a460: 3230 2e32 3935 3139 206c 2031 392e 3735  20.29519 l 19.75
-0000a470: 3633 382c 2d32 322e 3237 3038 3320 7a22  638,-22.27083 z"
-0000a480: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000a490: 3134 3535 332d 332d 3222 0a20 2020 2020  14553-3-2".     
-0000a4a0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000a4b0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000a4c0: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
-0000a4d0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-0000a4e0: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
-0000a4f0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000a500: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000a510: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000a520: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000a530: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-0000a540: 653d 2266 696c 6c3a 2331 3432 3637 323b  e="fill:#142672;
-0000a550: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-0000a560: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-0000a570: 726f 6b65 2d77 6964 7468 3a30 2e39 3939  roke-width:0.999
-0000a580: 3939 393b 7374 726f 6b65 2d6c 696e 6563  999;stroke-linec
-0000a590: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-0000a5a0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-0000a5b0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000a5c0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-0000a5d0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-0000a5e0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000a5f0: 2064 3d22 6d20 3334 302e 3733 372c 3332   d="m 340.737,32
-0000a600: 312e 3833 3436 3320 3839 2e30 3833 3332  1.83463 89.08332
-0000a610: 2c2d 382e 3938 3031 3620 2d36 392e 3332  ,-8.98016 -69.32
-0000a620: 3639 342c 2d31 332e 3239 3036 3720 7a22  694,-13.29067 z"
-0000a630: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000a640: 3134 3535 352d 342d 3122 0a20 2020 2020  14555-4-1".     
-0000a650: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000a660: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000a670: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000a680: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000a690: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000a6a0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000a6b0: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
-0000a6c0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-0000a6d0: 3d22 6669 6c6c 3a23 3534 3636 3863 3b66  ="fill:#54668c;f
-0000a6e0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000a6f0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000a700: 6f6b 652d 7769 6474 683a 302e 3939 3939  oke-width:0.9999
-0000a710: 3939 3b73 7472 6f6b 652d 6c69 6e65 6361  99;stroke-lineca
-0000a720: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-0000a730: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-0000a740: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-0000a750: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-0000a760: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-0000a770: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000a780: 643d 226d 2033 3430 2e37 3337 2c33 3231  d="m 340.737,321
-0000a790: 2e38 3334 3633 2035 312e 3336 3635 382c  .83463 51.36658,
-0000a7a0: 352e 3338 3831 2033 372e 3731 3637 342c  5.3881 37.71674,
-0000a7b0: 2d31 342e 3336 3832 3620 7a22 0a20 2020  -14.36826 z".   
-0000a7c0: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
-0000a7d0: 372d 302d 3722 0a20 2020 2020 2020 696e  7-0-7".       in
-0000a7e0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-0000a7f0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-0000a800: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000a810: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-0000a820: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000a830: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-0000a840: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
-0000a850: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
-0000a860: 6c6c 3a23 3232 3334 3765 3b66 696c 6c2d  ll:#22347e;fill-
-0000a870: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
-0000a880: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-0000a890: 7769 6474 683a 302e 3939 3939 3939 3b73  width:0.999999;s
-0000a8a0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-0000a8b0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-0000a8c0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-0000a8d0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000a8e0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000a8f0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-0000a900: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
-0000a910: 2033 3430 2e37 3337 2c33 3231 2e38 3334   340.737,321.834
-0000a920: 3633 2063 2031 2e31 3535 3035 2c39 2e39  63 c 1.15505,9.9
-0000a930: 3539 3133 202d 322e 3834 3330 332c 3136  5913 -2.84303,16
-0000a940: 2e32 3337 3439 202d 342e 3636 3936 382c  .23749 -4.66968,
-0000a950: 3234 2e30 3636 3836 206c 2035 362e 3033  24.06686 l 56.03
-0000a960: 3632 362c 2d31 382e 3637 3837 3620 7a22  626,-18.67876 z"
-0000a970: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000a980: 3134 3535 392d 332d 3422 0a20 2020 2020  14559-3-4".     
-0000a990: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000a9a0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000a9b0: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
-0000a9c0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-0000a9d0: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
-0000a9e0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000a9f0: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000aa00: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000aa10: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000aa20: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-0000aa30: 653d 2266 696c 6c3a 2330 3831 3036 393b  e="fill:#081069;
-0000aa40: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-0000aa50: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-0000aa60: 726f 6b65 2d77 6964 7468 3a30 2e39 3939  roke-width:0.999
-0000aa70: 3939 393b 7374 726f 6b65 2d6c 696e 6563  999;stroke-linec
-0000aa80: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-0000aa90: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-0000aaa0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000aab0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-0000aac0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-0000aad0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000aae0: 2064 3d22 6d20 3333 362e 3036 3733 322c   d="m 336.06732,
-0000aaf0: 3334 352e 3930 3134 3920 3338 2e37 3934  345.90149 38.794
-0000ab00: 3333 2c35 2e37 3437 3320 3534 2e39 3538  33,5.7473 54.958
-0000ab10: 3637 2c2d 3338 2e37 3934 3332 207a 220a  67,-38.79432 z".
-0000ab20: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000ab30: 3435 3631 2d39 2d32 220a 2020 2020 2020  4561-9-2".      
-0000ab40: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-0000ab50: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-0000ab60: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000ab70: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000ab80: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000ab90: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000aba0: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
-0000abb0: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-0000abc0: 2266 696c 6c3a 2330 3730 6532 623b 6669  "fill:#070e2b;fi
-0000abd0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-0000abe0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000abf0: 6b65 2d77 6964 7468 3a30 2e39 3939 3939  ke-width:0.99999
-0000ac00: 393b 7374 726f 6b65 2d6c 696e 6563 6170  9;stroke-linecap
-0000ac10: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-0000ac20: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-0000ac30: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-0000ac40: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000ac50: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-0000ac60: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-0000ac70: 3d22 6d20 3337 342e 3836 3136 352c 3335  ="m 374.86165,35
-0000ac80: 312e 3634 3837 3920 3232 2e38 3039 3633  1.64879 22.80963
-0000ac90: 2c32 392e 3939 3338 202d 382e 3434 3133  ,29.9938 -8.4413
-0000aca0: 352c 2d34 302e 3431 3037 3820 7a22 0a20  5,-40.41078 z". 
-0000acb0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-0000acc0: 3536 332d 312d 3022 0a20 2020 2020 2020  563-1-0".       
-0000acd0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-0000ace0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-0000acf0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000ad00: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000ad10: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000ad20: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000ad30: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
-0000ad40: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-0000ad50: 6669 6c6c 3a23 3238 3364 3837 3b66 696c  fill:#283d87;fil
-0000ad60: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000ad70: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000ad80: 652d 7769 6474 683a 302e 3939 3939 3939  e-width:0.999999
-0000ad90: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-0000ada0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-0000adb0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-0000adc0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000add0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000ade0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-0000adf0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-0000ae00: 226d 2033 3839 2e32 3239 3933 2c33 3431  "m 389.22993,341
-0000ae10: 2e32 3331 3831 2038 2e34 3431 3335 2c34  .23181 8.44135,4
-0000ae20: 302e 3431 3037 3820 6320 342e 3336 3939  0.41078 c 4.3699
-0000ae30: 332c 2d33 362e 3332 3734 3220 3139 2e37  3,-36.32742 19.7
-0000ae40: 3438 3037 2c2d 3439 2e34 3135 3133 2033  4807,-49.41513 3
-0000ae50: 322e 3134 3930 342c 2d36 382e 3738 3831  2.14904,-68.7881
-0000ae60: 3220 7a22 0a20 2020 2020 2020 6964 3d22  2 z".       id="
-0000ae70: 7061 7468 3134 3536 352d 392d 3522 0a20  path14565-9-5". 
-0000ae80: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-0000ae90: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-0000aea0: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
-0000aeb0: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-0000aec0: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
-0000aed0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-0000aee0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-0000aef0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000af00: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-0000af10: 2020 203c 656c 6c69 7073 650a 2020 2020     <ellipse.    
-0000af20: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-0000af30: 3037 3065 3262 3b66 696c 6c2d 6f70 6163  070e2b;fill-opac
-0000af40: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
-0000af50: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000af60: 6b65 2d77 6964 7468 3a30 2e39 3939 3939  ke-width:0.99999
-0000af70: 393b 7374 726f 6b65 2d6d 6974 6572 6c69  9;stroke-miterli
-0000af80: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-0000af90: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-0000afa0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-0000afb0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000afc0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-0000afd0: 6831 3435 3637 2d36 2d31 220a 2020 2020  h14567-6-1".    
-0000afe0: 2020 2063 783d 2233 3137 2e39 3531 3834     cx="317.95184
-0000aff0: 220a 2020 2020 2020 2063 793d 2233 3031  ".       cy="301
-0000b000: 2e35 3835 3537 220a 2020 2020 2020 2072  .58557".       r
-0000b010: 783d 2232 2e32 3339 3532 3936 220a 2020  x="2.2395296".  
-0000b020: 2020 2020 2072 793d 2232 2e32 3339 3532       ry="2.23952
-0000b030: 3938 220a 2020 2020 2020 2069 6e6b 7363  98".       inksc
-0000b040: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000b050: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000b060: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000b070: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000b080: 6369 7263 6c65 0a20 2020 2020 2020 723d  circle.       r=
-0000b090: 2232 2e32 3339 3532 3938 220a 2020 2020  "2.2395298".    
-0000b0a0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-0000b0b0: 3235 3361 3764 3b66 696c 6c2d 6f70 6163  253a7d;fill-opac
-0000b0c0: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-0000b0d0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-0000b0e0: 683a 302e 3939 3939 3939 3b73 7472 6f6b  h:0.999999;strok
-0000b0f0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000b100: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000b110: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
-0000b120: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
-0000b130: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-0000b140: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
-0000b150: 332d 3933 2d31 220a 2020 2020 2020 2063  3-93-1".       c
-0000b160: 783d 2233 3335 2e37 3036 3931 220a 2020  x="335.70691".  
-0000b170: 2020 2020 2063 793d 2233 3435 2e34 3233       cy="345.423
-0000b180: 3737 220a 2020 2020 2020 2069 6e6b 7363  77".       inksc
-0000b190: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-0000b1a0: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
-0000b1b0: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
-0000b1c0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000b1d0: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
-0000b1e0: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
-0000b1f0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000b200: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000b210: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000b220: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
-0000b230: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
-0000b240: 322e 3233 3935 3239 3822 0a20 2020 2020  2.2395298".     
-0000b250: 2020 7374 796c 653d 2266 696c 6c3a 2332    style="fill:#2
-0000b260: 3533 6137 643b 6669 6c6c 2d6f 7061 6369  53a7d;fill-opaci
-0000b270: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-0000b280: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-0000b290: 3a30 2e39 3939 3939 393b 7374 726f 6b65  :0.999999;stroke
-0000b2a0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-0000b2b0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-0000b2c0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
-0000b2d0: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
-0000b2e0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000b2f0: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
-0000b300: 2d37 2d33 2d30 220a 2020 2020 2020 2063  -7-3-0".       c
-0000b310: 783d 2233 3838 2e36 3834 3622 0a20 2020  x="388.6846".   
-0000b320: 2020 2020 6379 3d22 3332 372e 3336 3632      cy="327.3662
-0000b330: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
-0000b340: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000b350: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
-0000b360: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b370: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-0000b380: 6572 2d79 3d22 2d39 2e39 3738 3036 3231  er-y="-9.9780621
-0000b390: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b3a0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000b3b0: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000b3c0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000b3d0: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
-0000b3e0: 7263 6c65 0a20 2020 2020 2020 723d 2232  rcle.       r="2
-0000b3f0: 2e32 3339 3532 3938 220a 2020 2020 2020  .2395298".      
-0000b400: 2073 7479 6c65 3d22 6669 6c6c 3a23 6138   style="fill:#a8
-0000b410: 6139 6161 3b66 696c 6c2d 6f70 6163 6974  a9aa;fill-opacit
-0000b420: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-0000b430: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-0000b440: 302e 3939 3939 3939 3b73 7472 6f6b 652d  0.999999;stroke-
-0000b450: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000b460: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000b470: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
-0000b480: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
-0000b490: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000b4a0: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
-0000b4b0: 352d 382d 3822 0a20 2020 2020 2020 6378  5-8-8".       cx
-0000b4c0: 3d22 3338 392e 3231 3537 3322 0a20 2020  ="389.21573".   
-0000b4d0: 2020 2020 6379 3d22 3334 302e 3930 3933      cy="340.9093
-0000b4e0: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
-0000b4f0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000b500: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
-0000b510: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b520: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-0000b530: 6572 2d79 3d22 2d39 2e39 3738 3036 3231  er-y="-9.9780621
-0000b540: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b550: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000b560: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000b570: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000b580: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
-0000b590: 7263 6c65 0a20 2020 2020 2020 723d 2232  rcle.       r="2
-0000b5a0: 2e32 3339 3532 3938 220a 2020 2020 2020  .2395298".      
-0000b5b0: 2073 7479 6c65 3d22 6669 6c6c 3a23 6162   style="fill:#ab
-0000b5c0: 6161 3963 3b66 696c 6c2d 6f70 6163 6974  aa9c;fill-opacit
-0000b5d0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-0000b5e0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-0000b5f0: 302e 3939 3939 3939 3b73 7472 6f6b 652d  0.999999;stroke-
-0000b600: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000b610: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000b620: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
-0000b630: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
-0000b640: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000b650: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
-0000b660: 392d 302d 3922 0a20 2020 2020 2020 6378  9-0-9".       cx
-0000b670: 3d22 3337 352e 3430 3639 3822 0a20 2020  ="375.40698".   
-0000b680: 2020 2020 6379 3d22 3335 312e 3533 3134      cy="351.5314
-0000b690: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
-0000b6a0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000b6b0: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
-0000b6c0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b6d0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-0000b6e0: 6572 2d79 3d22 2d39 2e39 3738 3036 3231  er-y="-9.9780621
-0000b6f0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b700: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000b710: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000b720: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000b730: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
-0000b740: 7263 6c65 0a20 2020 2020 2020 723d 2233  rcle.       r="3
-0000b750: 2e34 3536 3430 3034 220a 2020 2020 2020  .4564004".      
-0000b760: 2073 7479 6c65 3d22 6669 6c6c 3a23 3131   style="fill:#11
-0000b770: 3230 3636 3b66 696c 6c2d 6f70 6163 6974  2066;fill-opacit
-0000b780: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-0000b790: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-0000b7a0: 302e 3939 3939 3939 3b73 7472 6f6b 652d  0.999999;stroke-
-0000b7b0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000b7c0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000b7d0: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
-0000b7e0: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
-0000b7f0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000b800: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
-0000b810: 322d 352d 3422 0a20 2020 2020 2020 6378  2-5-4".       cx
-0000b820: 3d22 3336 302e 3830 3136 3122 0a20 2020  ="360.80161".   
-0000b830: 2020 2020 6379 3d22 3239 392e 3038 3439      cy="299.0849
-0000b840: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000b850: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-0000b860: 6572 2d78 3d22 372e 3136 3632 3131 3622  er-x="7.1662116"
-0000b870: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000b880: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-0000b890: 722d 793d 222d 3135 2e33 3939 3735 3122  r-y="-15.399751"
-0000b8a0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000b8b0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000b8c0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000b8d0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000b8e0: 3330 3022 202f 3e0a 2020 2020 3c63 6972  300" />.    <cir
-0000b8f0: 636c 650a 2020 2020 2020 2072 3d22 322e  cle.       r="2.
-0000b900: 3233 3935 3239 3822 0a20 2020 2020 2020  2395298".       
-0000b910: 7374 796c 653d 2266 696c 6c3a 2365 6466  style="fill:#edf
-0000b920: 3066 633b 6669 6c6c 2d6f 7061 6369 7479  0fc;fill-opacity
-0000b930: 3a30 2e39 3930 3434 363b 7374 726f 6b65  :0.990446;stroke
-0000b940: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
-0000b950: 7769 6474 683a 302e 3939 3939 3939 3b73  width:0.999999;s
-0000b960: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-0000b970: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-0000b980: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-0000b990: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-0000b9a0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-0000b9b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-0000b9c0: 3536 372d 322d 362d 3022 0a20 2020 2020  567-2-6-0".     
-0000b9d0: 2020 6378 3d22 3337 392e 3532 3330 3422    cx="379.52304"
-0000b9e0: 0a20 2020 2020 2020 6379 3d22 3330 322e  .       cy="302.
-0000b9f0: 3933 3533 3622 0a20 2020 2020 2020 696e  93536".       in
-0000ba00: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-0000ba10: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-0000ba20: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000ba30: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-0000ba40: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
-0000ba50: 2072 3d22 322e 3233 3935 3239 3822 0a20   r="2.2395298". 
-0000ba60: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-0000ba70: 6c3a 2365 6466 3066 633b 6669 6c6c 2d6f  l:#edf0fc;fill-o
-0000ba80: 7061 6369 7479 3a30 2e39 3930 3434 363b  pacity:0.990446;
-0000ba90: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-0000baa0: 7472 6f6b 652d 7769 6474 683a 302e 3939  troke-width:0.99
-0000bab0: 3939 3939 3b73 7472 6f6b 652d 6d69 7465  9999;stroke-mite
-0000bac0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-0000bad0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-0000bae0: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-0000baf0: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
-0000bb00: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
-0000bb10: 7061 7468 3134 3536 372d 322d 382d 362d  path14567-2-8-6-
-0000bb20: 3722 0a20 2020 2020 2020 6378 3d22 3334  7".       cx="34
-0000bb30: 302e 3735 3234 3122 0a20 2020 2020 2020  0.75241".       
-0000bb40: 6379 3d22 3332 312e 3532 3430 3522 0a20  cy="321.52405". 
-0000bb50: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000bb60: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-0000bb70: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000bb80: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-0000bb90: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
-0000bba0: 650a 2020 2020 2020 2072 3d22 342e 3235  e.       r="4.25
-0000bbb0: 3730 3137 3122 0a20 2020 2020 2020 7374  70171".       st
-0000bbc0: 796c 653d 2266 696c 6c3a 2365 6466 3066  yle="fill:#edf0f
-0000bbd0: 633b 6669 6c6c 2d6f 7061 6369 7479 3a30  c;fill-opacity:0
-0000bbe0: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
-0000bbf0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-0000bc00: 6474 683a 302e 3939 3939 3939 3b73 7472  dth:0.999999;str
-0000bc10: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-0000bc20: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-0000bc30: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-0000bc40: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-0000bc50: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-0000bc60: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-0000bc70: 372d 322d 372d 302d 3922 0a20 2020 2020  7-2-7-0-9".     
-0000bc80: 2020 6378 3d22 3432 392e 3034 3835 3522    cx="429.04855"
-0000bc90: 0a20 2020 2020 2020 6379 3d22 3331 332e  .       cy="313.
-0000bca0: 3432 3436 3822 0a20 2020 2020 2020 696e  42468".       in
-0000bcb0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-0000bcc0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-0000bcd0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000bce0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-0000bcf0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-0000bd00: 7479 6c65 3d22 6669 6c6c 3a23 3365 3462  tyle="fill:#3e4b
-0000bd10: 3737 3b66 696c 6c2d 6f70 6163 6974 793a  77;fill-opacity:
-0000bd20: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-0000bd30: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-0000bd40: 3734 3839 3937 3b73 7472 6f6b 652d 6c69  748997;stroke-li
-0000bd50: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-0000bd60: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-0000bd70: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000bd80: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000bd90: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000bda0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-0000bdb0: 2020 2020 643d 226d 2033 3139 2e31 3334      d="m 319.134
-0000bdc0: 3735 2c34 3430 2e31 3139 3734 2032 312e  75,440.11974 21.
-0000bdd0: 3733 3230 322c 2d30 2e39 3837 3832 2031  73202,-0.98782 1
-0000bde0: 342e 3237 3834 372c 2d31 352e 3839 3439  4.27847,-15.8949
-0000bdf0: 2063 202d 3137 2e39 3837 3835 2c31 322e   c -17.98785,12.
-0000be00: 3039 3731 3420 2d32 362e 3538 3136 382c  09714 -26.58168,
-0000be10: 3134 2e30 3338 3538 202d 3336 2e30 3130  14.03858 -36.010
-0000be20: 3439 2c31 362e 3838 3237 3220 7a22 0a20  49,16.88272 z". 
-0000be30: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-0000be40: 3534 372d 312d 372d 3822 0a20 2020 2020  547-1-7-8".     
-0000be50: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000be60: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000be70: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
-0000be80: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-0000be90: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
-0000bea0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000beb0: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000bec0: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000bed0: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000bee0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-0000bef0: 653d 2266 696c 6c3a 2331 6332 6336 383b  e="fill:#1c2c68;
-0000bf00: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-0000bf10: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-0000bf20: 726f 6b65 2d77 6964 7468 3a30 2e37 3438  roke-width:0.748
-0000bf30: 3939 373b 7374 726f 6b65 2d6c 696e 6563  997;stroke-linec
-0000bf40: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-0000bf50: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-0000bf60: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000bf70: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-0000bf80: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-0000bf90: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000bfa0: 2064 3d22 6d20 3334 302e 3836 3637 372c   d="m 340.86677,
-0000bfb0: 3433 392e 3133 3139 3220 392e 3432 3931  439.13192 9.4291
-0000bfc0: 372c 322e 3135 3532 3420 342e 3834 3933  7,2.15524 4.8493
-0000bfd0: 2c2d 3138 2e30 3530 3134 207a 220a 2020  ,-18.05014 z".  
-0000bfe0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-0000bff0: 3439 2d31 2d30 2d31 220a 2020 2020 2020  49-1-0-1".      
-0000c000: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-0000c010: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-0000c020: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000c030: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000c040: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000c050: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000c060: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
-0000c070: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-0000c080: 2266 696c 6c3a 2330 3630 3530 383b 6669  "fill:#060508;fi
-0000c090: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-0000c0a0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000c0b0: 6b65 2d77 6964 7468 3a30 2e37 3438 3939  ke-width:0.74899
-0000c0c0: 373b 7374 726f 6b65 2d6c 696e 6563 6170  7;stroke-linecap
-0000c0d0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-0000c0e0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-0000c0f0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-0000c100: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000c110: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-0000c120: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-0000c130: 3d22 6d20 3335 302e 3239 3539 342c 3434  ="m 350.29594,44
-0000c140: 312e 3238 3731 3620 3235 2e32 3334 3238  1.28716 25.23428
-0000c150: 2c34 2e34 3930 3039 2063 202d 392e 3833  ,4.49009 c -9.83
-0000c160: 3333 362c 2d35 2e31 3938 3437 202d 3135  336,-5.19847 -15
-0000c170: 2e35 3237 3731 2c2d 3133 2e35 3530 3436  .52771,-13.55046
-0000c180: 202d 3230 2e33 3834 3938 2c2d 3232 2e35   -20.38498,-22.5
-0000c190: 3430 3233 207a 220a 2020 2020 2020 2069  4023 z".       i
-0000c1a0: 643d 2270 6174 6831 3435 3531 2d30 2d33  d="path14551-0-3
-0000c1b0: 2d39 220a 2020 2020 2020 2069 6e6b 7363  -9".       inksc
-0000c1c0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-0000c1d0: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-0000c1e0: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-0000c1f0: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
-0000c200: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000c210: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000c220: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000c230: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000c240: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
-0000c250: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-0000c260: 3a23 3237 3337 3733 3b66 696c 6c2d 6f70  :#273773;fill-op
-0000c270: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-0000c280: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-0000c290: 6474 683a 302e 3734 3839 3937 3b73 7472  dth:0.748997;str
-0000c2a0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-0000c2b0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-0000c2c0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-0000c2d0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000c2e0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000c2f0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000c300: 3122 0a20 2020 2020 2020 643d 226d 2033  1".       d="m 3
-0000c310: 3139 2e31 3334 3735 2c34 3430 2e31 3139  19.13475,440.119
-0000c320: 3734 2063 2034 2e37 3832 3139 2c32 2e37  74 c 4.78219,2.7
-0000c330: 3433 3337 2031 302e 3035 3438 352c 352e  4337 10.05485,5.
-0000c340: 3130 3934 3520 3131 2e38 3533 3832 2c31  10945 11.85382,1
-0000c350: 302e 3134 3736 206c 2039 2e38 3738 322c  0.1476 l 9.8782,
-0000c360: 2d31 312e 3133 3534 3220 7a22 0a20 2020  -11.13542 z".   
-0000c370: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
-0000c380: 332d 332d 322d 3222 0a20 2020 2020 2020  3-3-2-2".       
-0000c390: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-0000c3a0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-0000c3b0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
-0000c3c0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-0000c3d0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000c3e0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000c3f0: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000c400: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000c410: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
-0000c420: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-0000c430: 2266 696c 6c3a 2331 3432 3637 323b 6669  "fill:#142672;fi
-0000c440: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-0000c450: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000c460: 6b65 2d77 6964 7468 3a30 2e37 3438 3939  ke-width:0.74899
-0000c470: 373b 7374 726f 6b65 2d6c 696e 6563 6170  7;stroke-linecap
-0000c480: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-0000c490: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-0000c4a0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-0000c4b0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000c4c0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-0000c4d0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-0000c4e0: 3d22 6d20 3333 302e 3938 3835 372c 3435  ="m 330.98857,45
-0000c4f0: 302e 3236 3733 3420 3434 2e35 3431 3635  0.26734 44.54165
-0000c500: 2c2d 342e 3439 3030 3920 2d33 342e 3636  ,-4.49009 -34.66
-0000c510: 3334 352c 2d36 2e36 3435 3333 207a 220a  345,-6.64533 z".
-0000c520: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000c530: 3435 3535 2d34 2d31 2d36 220a 2020 2020  4555-4-1-6".    
-0000c540: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-0000c550: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-0000c560: 2230 220a 2020 2020 2020 2069 6e6b 7363  "0".       inksc
-0000c570: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000c580: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000c590: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000c5a0: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000c5b0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-0000c5c0: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
-0000c5d0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-0000c5e0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-0000c5f0: 726f 6b65 2d77 6964 7468 3a30 2e37 3438  roke-width:0.748
-0000c600: 3939 373b 7374 726f 6b65 2d6c 696e 6563  997;stroke-linec
-0000c610: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-0000c620: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-0000c630: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000c640: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-0000c650: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-0000c660: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000c670: 2064 3d22 6d20 3333 302e 3938 3835 372c   d="m 330.98857,
-0000c680: 3435 302e 3236 3733 3420 3235 2e36 3833  450.26734 25.683
-0000c690: 332c 322e 3639 3430 3520 3138 2e38 3538  3,2.69405 18.858
-0000c6a0: 3335 2c2d 372e 3138 3431 3420 7a22 0a20  35,-7.18414 z". 
-0000c6b0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-0000c6c0: 3535 372d 302d 372d 3322 0a20 2020 2020  557-0-7-3".     
-0000c6d0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-0000c6e0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-0000c6f0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000c700: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000c710: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000c720: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000c730: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
-0000c740: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
-0000c750: 3d22 6669 6c6c 3a23 3232 3334 3765 3b66  ="fill:#22347e;f
-0000c760: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000c770: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000c780: 6f6b 652d 7769 6474 683a 302e 3734 3839  oke-width:0.7489
-0000c790: 3937 3b73 7472 6f6b 652d 6c69 6e65 6361  97;stroke-lineca
-0000c7a0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-0000c7b0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-0000c7c0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-0000c7d0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-0000c7e0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-0000c7f0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000c800: 643d 226d 2033 3330 2e39 3838 3537 2c34  d="m 330.98857,4
-0000c810: 3530 2e32 3637 3334 2063 2030 2e35 3737  50.26734 c 0.577
-0000c820: 3533 2c34 2e39 3739 3536 202d 312e 3432  53,4.97956 -1.42
-0000c830: 3135 312c 382e 3131 3837 3320 2d32 2e33  151,8.11873 -2.3
-0000c840: 3334 3834 2c31 322e 3033 3334 3220 6c20  3484,12.03342 l 
-0000c850: 3238 2e30 3138 3134 2c2d 392e 3333 3933  28.01814,-9.3393
-0000c860: 3720 7a22 0a20 2020 2020 2020 6964 3d22  7 z".       id="
-0000c870: 7061 7468 3134 3535 392d 332d 342d 3222  path14559-3-4-2"
-0000c880: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000c890: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-0000c8a0: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
-0000c8b0: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
-0000c8c0: 6573 3d22 6363 6363 220a 2020 2020 2020  es="cccc".      
-0000c8d0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000c8e0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-0000c8f0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000c900: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-0000c910: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-0000c920: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-0000c930: 3831 3036 393b 6669 6c6c 2d6f 7061 6369  81069;fill-opaci
-0000c940: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-0000c950: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-0000c960: 3a30 2e37 3438 3939 373b 7374 726f 6b65  :0.748997;stroke
-0000c970: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-0000c980: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-0000c990: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
-0000c9a0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-0000c9b0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-0000c9c0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-0000c9d0: 2020 2020 2020 2064 3d22 6d20 3332 382e         d="m 328.
-0000c9e0: 3635 3337 332c 3436 322e 3330 3037 3620  65373,462.30076 
-0000c9f0: 3139 2e33 3937 3137 2c32 2e38 3733 3636  19.39717,2.87366
-0000ca00: 2032 372e 3437 3933 322c 2d31 392e 3339   27.47932,-19.39
-0000ca10: 3731 3720 7a22 0a20 2020 2020 2020 6964  717 z".       id
-0000ca20: 3d22 7061 7468 3134 3536 312d 392d 322d  ="path14561-9-2-
-0000ca30: 3222 0a20 2020 2020 2020 696e 6b73 6361  2".       inksca
-0000ca40: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-0000ca50: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-0000ca60: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-0000ca70: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-0000ca80: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000ca90: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-0000caa0: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
-0000cab0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-0000cac0: 3037 3065 3262 3b66 696c 6c2d 6f70 6163  070e2b;fill-opac
-0000cad0: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
-0000cae0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
-0000caf0: 683a 302e 3734 3839 3937 3b73 7472 6f6b  h:0.748997;strok
-0000cb00: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-0000cb10: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-0000cb20: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-0000cb30: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-0000cb40: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-0000cb50: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000cb60: 0a20 2020 2020 2020 643d 226d 2033 3438  .       d="m 348
-0000cb70: 2e30 3530 392c 3436 352e 3137 3434 3220  .0509,465.17442 
-0000cb80: 3131 2e34 3034 3831 2c31 342e 3939 3638  11.40481,14.9968
-0000cb90: 3920 2d34 2e32 3230 3637 2c2d 3230 2e32  9 -4.22067,-20.2
-0000cba0: 3035 3339 207a 220a 2020 2020 2020 2069  0539 z".       i
-0000cbb0: 643d 2270 6174 6831 3435 3633 2d31 2d30  d="path14563-1-0
-0000cbc0: 2d36 220a 2020 2020 2020 2069 6e6b 7363  -6".       inksc
-0000cbd0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-0000cbe0: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-0000cbf0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000cc00: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
-0000cc10: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000cc20: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
-0000cc30: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-0000cc40: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-0000cc50: 2332 3833 6438 373b 6669 6c6c 2d6f 7061  #283d87;fill-opa
-0000cc60: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-0000cc70: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-0000cc80: 7468 3a30 2e37 3438 3939 373b 7374 726f  th:0.748997;stro
-0000cc90: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-0000cca0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-0000ccb0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-0000ccc0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000ccd0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000cce0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000ccf0: 220a 2020 2020 2020 2064 3d22 6d20 3335  ".       d="m 35
-0000cd00: 352e 3233 3530 342c 3435 392e 3936 3539  5.23504,459.9659
-0000cd10: 3220 342e 3232 3036 372c 3230 2e32 3035  2 4.22067,20.205
-0000cd20: 3339 2063 2032 2e31 3834 3936 2c2d 3138  39 c 2.18496,-18
-0000cd30: 2e31 3633 3720 392e 3837 3430 342c 2d32  .1637 9.87404,-2
-0000cd40: 342e 3730 3735 3720 3136 2e30 3734 3531  4.70757 16.07451
-0000cd50: 2c2d 3334 2e33 3934 3036 207a 220a 2020  ,-34.39406 z".  
-0000cd60: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-0000cd70: 3635 2d39 2d35 2d39 220a 2020 2020 2020  65-9-5-9".      
-0000cd80: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
-0000cd90: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
-0000cda0: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
-0000cdb0: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
-0000cdc0: 6322 0a20 2020 2020 2020 696e 6b73 6361  c".       inksca
-0000cdd0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000cde0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000cdf0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000ce00: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
-0000ce10: 6972 636c 650a 2020 2020 2020 2073 7479  ircle.       sty
-0000ce20: 6c65 3d22 6669 6c6c 3a23 3037 3065 3262  le="fill:#070e2b
-0000ce30: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
-0000ce40: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
-0000ce50: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-0000ce60: 7468 3a30 2e37 3438 3939 373b 7374 726f  th:0.748997;stro
-0000ce70: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-0000ce80: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-0000ce90: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
-0000cea0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
-0000ceb0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-0000cec0: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-0000ced0: 2d36 2d31 2d39 220a 2020 2020 2020 2063  -6-1-9".       c
-0000cee0: 783d 2233 3139 2e35 3935 3938 220a 2020  x="319.59598".  
-0000cef0: 2020 2020 2063 793d 2234 3430 2e31 3432       cy="440.142
-0000cf00: 3739 220a 2020 2020 2020 2069 6e6b 7363  79".       inksc
-0000cf10: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000cf20: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000cf30: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000cf40: 693d 2233 3030 220a 2020 2020 2020 2072  i="300".       r
-0000cf50: 3d22 312e 3131 3937 3634 3922 202f 3e0a  ="1.1197649" />.
-0000cf60: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
-0000cf70: 2020 2072 3d22 312e 3131 3937 3634 3922     r="1.1197649"
-0000cf80: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-0000cf90: 696c 6c3a 2332 3533 6137 643b 6669 6c6c  ill:#253a7d;fill
-0000cfa0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-0000cfb0: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-0000cfc0: 2d77 6964 7468 3a30 2e37 3438 3939 373b  -width:0.748997;
-0000cfd0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-0000cfe0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-0000cff0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-0000d000: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-0000d010: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-0000d020: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000d030: 3435 3637 2d33 2d39 332d 312d 3622 0a20  4567-3-93-1-6". 
-0000d040: 2020 2020 2020 6378 3d22 3332 382e 3437        cx="328.47
-0000d050: 3335 3422 0a20 2020 2020 2020 6379 3d22  354".       cy="
-0000d060: 3436 322e 3036 3138 3922 0a20 2020 2020  462.06189".     
-0000d070: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
-0000d080: 666f 726d 2d63 656e 7465 722d 783d 2234  form-center-x="4
-0000d090: 2e36 3433 3235 3636 220a 2020 2020 2020  .6432566".      
-0000d0a0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-0000d0b0: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d39  orm-center-y="-9
-0000d0c0: 2e39 3738 3036 3231 220a 2020 2020 2020  .9780621".      
-0000d0d0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000d0e0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-0000d0f0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000d100: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-0000d110: 0a20 2020 203c 6369 7263 6c65 0a20 2020  .    <circle.   
-0000d120: 2020 2020 723d 2231 2e31 3139 3736 3439      r="1.1197649
-0000d130: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-0000d140: 6669 6c6c 3a23 3235 3361 3764 3b66 696c  fill:#253a7d;fil
-0000d150: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000d160: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000d170: 652d 7769 6474 683a 302e 3734 3839 3937  e-width:0.748997
-0000d180: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000d190: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000d1a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000d1b0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-0000d1c0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000d1d0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000d1e0: 3134 3536 372d 332d 372d 332d 302d 3922  14567-3-7-3-0-9"
-0000d1f0: 0a20 2020 2020 2020 6378 3d22 3335 342e  .       cx="354.
-0000d200: 3936 3233 3722 0a20 2020 2020 2020 6379  96237".       cy
-0000d210: 3d22 3435 332e 3033 3331 3122 0a20 2020  ="453.03311".   
-0000d220: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-0000d230: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
-0000d240: 2234 2e36 3433 3235 3636 220a 2020 2020  "4.6432566".    
-0000d250: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
-0000d260: 7366 6f72 6d2d 6365 6e74 6572 2d79 3d22  sform-center-y="
-0000d270: 2d39 2e39 3738 3036 3231 220a 2020 2020  -9.9780621".    
-0000d280: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000d290: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
-0000d2a0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000d2b0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
-0000d2c0: 2f3e 0a20 2020 203c 6369 7263 6c65 0a20  />.    <circle. 
-0000d2d0: 2020 2020 2020 723d 2231 2e31 3139 3736        r="1.11976
-0000d2e0: 3439 220a 2020 2020 2020 2073 7479 6c65  49".       style
-0000d2f0: 3d22 6669 6c6c 3a23 6138 6139 6161 3b66  ="fill:#a8a9aa;f
-0000d300: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-0000d310: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-0000d320: 6f6b 652d 7769 6474 683a 302e 3734 3839  oke-width:0.7489
-0000d330: 3937 3b73 7472 6f6b 652d 6d69 7465 726c  97;stroke-miterl
-0000d340: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-0000d350: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-0000d360: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
-0000d370: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000d380: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
-0000d390: 7468 3134 3536 372d 332d 352d 382d 382d  th14567-3-5-8-8-
-0000d3a0: 3522 0a20 2020 2020 2020 6378 3d22 3335  5".       cx="35
-0000d3b0: 352e 3232 3739 3422 0a20 2020 2020 2020  5.22794".       
-0000d3c0: 6379 3d22 3435 392e 3830 3436 3922 0a20  cy="459.80469". 
-0000d3d0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
-0000d3e0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
-0000d3f0: 783d 2234 2e36 3433 3235 3636 220a 2020  x="4.6432566".  
-0000d400: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-0000d410: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
-0000d420: 3d22 2d39 2e39 3738 3036 3231 220a 2020  ="-9.9780621".  
-0000d430: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000d440: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-0000d450: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000d460: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-0000d470: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
-0000d480: 0a20 2020 2020 2020 723d 2231 2e31 3139  .       r="1.119
-0000d490: 3736 3439 220a 2020 2020 2020 2073 7479  7649".       sty
-0000d4a0: 6c65 3d22 6669 6c6c 3a23 6162 6161 3963  le="fill:#abaa9c
-0000d4b0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-0000d4c0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-0000d4d0: 7472 6f6b 652d 7769 6474 683a 302e 3734  troke-width:0.74
-0000d4e0: 3839 3937 3b73 7472 6f6b 652d 6d69 7465  8997;stroke-mite
-0000d4f0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-0000d500: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-0000d510: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-0000d520: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
-0000d530: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
-0000d540: 7061 7468 3134 3536 372d 332d 392d 302d  path14567-3-9-0-
-0000d550: 392d 3822 0a20 2020 2020 2020 6378 3d22  9-8".       cx="
-0000d560: 3334 382e 3332 3335 3822 0a20 2020 2020  348.32358".     
-0000d570: 2020 6379 3d22 3436 352e 3131 3537 3222    cy="465.11572"
-0000d580: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000d590: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-0000d5a0: 722d 783d 2234 2e36 3433 3235 3636 220a  r-x="4.6432566".
-0000d5b0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000d5c0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-0000d5d0: 2d79 3d22 2d39 2e39 3738 3036 3231 220a  -y="-9.9780621".
-0000d5e0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000d5f0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000d600: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000d610: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
-0000d620: 3030 2220 2f3e 0a20 2020 203c 6369 7263  00" />.    <circ
-0000d630: 6c65 0a20 2020 2020 2020 723d 2231 2e37  le.       r="1.7
-0000d640: 3238 3230 3032 220a 2020 2020 2020 2073  282002".       s
-0000d650: 7479 6c65 3d22 6669 6c6c 3a23 3131 3230  tyle="fill:#1120
-0000d660: 3636 3b66 696c 6c2d 6f70 6163 6974 793a  66;fill-opacity:
-0000d670: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-0000d680: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-0000d690: 3734 3839 3937 3b73 7472 6f6b 652d 6d69  748997;stroke-mi
-0000d6a0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000d6b0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000d6c0: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
-0000d6d0: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
-0000d6e0: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
-0000d6f0: 3d22 7061 7468 3134 3536 372d 332d 322d  ="path14567-3-2-
-0000d700: 352d 342d 3322 0a20 2020 2020 2020 6378  5-4-3".       cx
-0000d710: 3d22 3334 312e 3032 3038 3722 0a20 2020  ="341.02087".   
-0000d720: 2020 2020 6379 3d22 3433 382e 3839 3234      cy="438.8924
-0000d730: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
-0000d740: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000d750: 7465 722d 783d 2237 2e31 3636 3231 3136  ter-x="7.1662116
-0000d760: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000d770: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-0000d780: 6572 2d79 3d22 2d31 352e 3339 3937 3531  er-y="-15.399751
-0000d790: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000d7a0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-0000d7b0: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-0000d7c0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000d7d0: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
-0000d7e0: 7263 6c65 0a20 2020 2020 2020 723d 2231  rcle.       r="1
-0000d7f0: 2e31 3139 3736 3439 220a 2020 2020 2020  .1197649".      
-0000d800: 2073 7479 6c65 3d22 6669 6c6c 3a23 6564   style="fill:#ed
-0000d810: 6630 6663 3b66 696c 6c2d 6f70 6163 6974  f0fc;fill-opacit
-0000d820: 793a 302e 3939 3034 3436 3b73 7472 6f6b  y:0.990446;strok
-0000d830: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-0000d840: 2d77 6964 7468 3a30 2e37 3438 3939 373b  -width:0.748997;
-0000d850: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-0000d860: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-0000d870: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-0000d880: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-0000d890: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-0000d8a0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000d8b0: 3435 3637 2d32 2d36 2d30 2d30 220a 2020  4567-2-6-0-0".  
-0000d8c0: 2020 2020 2063 783d 2233 3530 2e33 3831       cx="350.381
-0000d8d0: 3539 220a 2020 2020 2020 2063 793d 2234  59".       cy="4
-0000d8e0: 3430 2e38 3137 3732 220a 2020 2020 2020  40.81772".      
-0000d8f0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000d900: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-0000d910: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000d920: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-0000d930: 0a20 2020 203c 6369 7263 6c65 0a20 2020  .    <circle.   
-0000d940: 2020 2020 723d 2231 2e31 3139 3736 3439      r="1.1197649
-0000d950: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
-0000d960: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
-0000d970: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
-0000d980: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
-0000d990: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-0000d9a0: 2e37 3438 3939 373b 7374 726f 6b65 2d6d  .748997;stroke-m
-0000d9b0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000d9c0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000d9d0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-0000d9e0: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-0000d9f0: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
-0000da00: 643d 2270 6174 6831 3435 3637 2d32 2d38  d="path14567-2-8
-0000da10: 2d36 2d37 2d38 220a 2020 2020 2020 2063  -6-7-8".       c
-0000da20: 783d 2233 3330 2e39 3936 3238 220a 2020  x="330.99628".  
-0000da30: 2020 2020 2063 793d 2234 3530 2e31 3132       cy="450.112
-0000da40: 3033 220a 2020 2020 2020 2069 6e6b 7363  03".       inksc
-0000da50: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000da60: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000da70: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000da80: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000da90: 6369 7263 6c65 0a20 2020 2020 2020 723d  circle.       r=
-0000daa0: 2232 2e31 3238 3530 3836 220a 2020 2020  "2.1285086".    
-0000dab0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-0000dac0: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
-0000dad0: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
-0000dae0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000daf0: 6b65 2d77 6964 7468 3a31 2e34 3233 3733  ke-width:1.42373
-0000db00: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000db10: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000db20: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000db30: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
-0000db40: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-0000db50: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000db60: 3134 3536 372d 322d 372d 302d 392d 3022  14567-2-7-0-9-0"
-0000db70: 0a20 2020 2020 2020 6378 3d22 3337 352e  .       cx="375.
-0000db80: 3134 3433 3522 0a20 2020 2020 2020 6379  14435".       cy
-0000db90: 3d22 3434 362e 3036 3233 3822 0a20 2020  ="446.06238".   
-0000dba0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000dbb0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000dbc0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000dbd0: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000dbe0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
-0000dbf0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-0000dc00: 3a23 3365 3462 3737 3b66 696c 6c2d 6f70  :#3e4b77;fill-op
-0000dc10: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-0000dc20: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-0000dc30: 6474 683a 302e 3834 3530 3235 3b73 7472  dth:0.845025;str
-0000dc40: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-0000dc50: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-0000dc60: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-0000dc70: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-0000dc80: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-0000dc90: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-0000dca0: 3122 0a20 2020 2020 2020 643d 226d 2034  1".       d="m 4
-0000dcb0: 3038 2e31 3636 322c 3434 312e 3631 3733  08.1662,441.6173
-0000dcc0: 2031 362e 3334 3535 2c2d 302e 3734 3239   16.3455,-0.7429
-0000dcd0: 3820 3130 2e37 3339 342c 2d31 312e 3935  8 10.7394,-11.95
-0000dce0: 3531 3820 6320 2d31 332e 3532 3933 372c  518 c -13.52937,
-0000dcf0: 392e 3039 3837 3320 2d31 392e 3939 3331  9.09873 -19.9931
-0000dd00: 322c 3130 2e35 3538 3938 202d 3237 2e30  2,10.55898 -27.0
-0000dd10: 3834 392c 3132 2e36 3938 3136 207a 220a  849,12.69816 z".
-0000dd20: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-0000dd30: 3435 3437 2d31 2d37 2d38 2d33 220a 2020  4547-1-7-8-3".  
-0000dd40: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-0000dd50: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-0000dd60: 653d 2230 220a 2020 2020 2020 2073 6f64  e="0".       sod
-0000dd70: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
-0000dd80: 2263 6363 6322 0a20 2020 2020 2020 696e  "cccc".       in
-0000dd90: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-0000dda0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-0000ddb0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000ddc0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-0000ddd0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-0000dde0: 7479 6c65 3d22 6669 6c6c 3a23 3163 3263  tyle="fill:#1c2c
-0000ddf0: 3638 3b66 696c 6c2d 6f70 6163 6974 793a  68;fill-opacity:
-0000de00: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-0000de10: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-0000de20: 3834 3530 3235 3b73 7472 6f6b 652d 6c69  845025;stroke-li
-0000de30: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-0000de40: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-0000de50: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000de60: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000de70: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000de80: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-0000de90: 2020 2020 643d 226d 2034 3234 2e35 3131      d="m 424.511
-0000dea0: 372c 3434 302e 3837 3433 3220 372e 3039  7,440.87432 7.09
-0000deb0: 3230 352c 312e 3632 3130 3420 332e 3634  205,1.62104 3.64
-0000dec0: 3733 352c 2d31 332e 3537 3632 3220 7a22  735,-13.57622 z"
-0000ded0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
-0000dee0: 3134 3534 392d 312d 302d 312d 3622 0a20  14549-1-0-1-6". 
-0000def0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-0000df00: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-0000df10: 7265 3d22 3022 0a20 2020 2020 2020 696e  re="0".       in
-0000df20: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-0000df30: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-0000df40: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-0000df50: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-0000df60: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-0000df70: 7479 6c65 3d22 6669 6c6c 3a23 3036 3035  tyle="fill:#0605
-0000df80: 3038 3b66 696c 6c2d 6f70 6163 6974 793a  08;fill-opacity:
-0000df90: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-0000dfa0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-0000dfb0: 3834 3530 3235 3b73 7472 6f6b 652d 6c69  845025;stroke-li
-0000dfc0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
-0000dfd0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
-0000dfe0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
-0000dff0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
-0000e000: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-0000e010: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-0000e020: 2020 2020 643d 226d 2034 3331 2e36 3033      d="m 431.603
-0000e030: 3735 2c34 3432 2e34 3935 3336 2031 382e  75,442.49536 18.
-0000e040: 3937 3937 2c33 2e33 3737 3138 2063 202d  9797,3.37718 c -
-0000e050: 372e 3339 3630 372c 2d33 2e39 3039 3938  7.39607,-3.90998
-0000e060: 202d 3131 2e36 3739 2c2d 3130 2e31 3931   -11.679,-10.191
-0000e070: 3833 202d 3135 2e33 3332 3335 2c2d 3136  83 -15.33235,-16
-0000e080: 2e39 3533 3420 7a22 0a20 2020 2020 2020  .9534 z".       
-0000e090: 6964 3d22 7061 7468 3134 3535 312d 302d  id="path14551-0-
-0000e0a0: 332d 392d 3722 0a20 2020 2020 2020 696e  3-9-7".       in
-0000e0b0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
-0000e0c0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
-0000e0d0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
-0000e0e0: 6f64 6574 7970 6573 3d22 6363 6363 220a  odetypes="cccc".
-0000e0f0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000e100: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000e110: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000e120: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
-0000e130: 3030 2220 2f3e 0a20 2020 203c 7061 7468  00" />.    <path
-0000e140: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-0000e150: 696c 6c3a 2332 3733 3737 333b 6669 6c6c  ill:#273773;fill
-0000e160: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-0000e170: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-0000e180: 2d77 6964 7468 3a30 2e38 3435 3032 353b  -width:0.845025;
-0000e190: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-0000e1a0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-0000e1b0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-0000e1c0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-0000e1d0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-0000e1e0: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-0000e1f0: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
-0000e200: 6d20 3430 382e 3136 3632 2c34 3431 2e36  m 408.1662,441.6
-0000e210: 3137 3320 6320 332e 3539 3638 372c 322e  173 c 3.59687,2.
-0000e220: 3036 3334 2037 2e35 3632 3635 2c33 2e38  0634 7.56265,3.8
-0000e230: 3433 3032 2038 2e39 3135 3733 2c37 2e36  4302 8.91573,7.6
-0000e240: 3332 3420 6c20 372e 3432 3937 372c 2d38  324 l 7.42977,-8
-0000e250: 2e33 3735 3338 207a 220a 2020 2020 2020  .37538 z".      
-0000e260: 2069 643d 2270 6174 6831 3435 3533 2d33   id="path14553-3
-0000e270: 2d32 2d32 2d35 220a 2020 2020 2020 2069  -2-2-5".       i
-0000e280: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
-0000e290: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
-0000e2a0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-0000e2b0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
-0000e2c0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000e2d0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000e2e0: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000e2f0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000e300: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
-0000e310: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-0000e320: 6669 6c6c 3a23 3134 3236 3732 3b66 696c  fill:#142672;fil
-0000e330: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000e340: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000e350: 652d 7769 6474 683a 302e 3834 3530 3235  e-width:0.845025
-0000e360: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-0000e370: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-0000e380: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-0000e390: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000e3a0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000e3b0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-0000e3c0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-0000e3d0: 226d 2034 3137 2e30 3831 3933 2c34 3439  "m 417.08193,449
-0000e3e0: 2e32 3439 3720 3333 2e35 3031 3532 2c2d  .2497 33.50152,-
-0000e3f0: 332e 3337 3731 3620 2d32 362e 3037 3137  3.37716 -26.0717
-0000e400: 352c 2d34 2e39 3938 3232 207a 220a 2020  5,-4.99822 z".  
-0000e410: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-0000e420: 3535 2d34 2d31 2d36 2d33 220a 2020 2020  55-4-1-6-3".    
-0000e430: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
-0000e440: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
-0000e450: 2230 220a 2020 2020 2020 2069 6e6b 7363  "0".       inksc
-0000e460: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-0000e470: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-0000e480: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-0000e490: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-0000e4a0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-0000e4b0: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
-0000e4c0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-0000e4d0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-0000e4e0: 726f 6b65 2d77 6964 7468 3a30 2e38 3435  roke-width:0.845
-0000e4f0: 3032 353b 7374 726f 6b65 2d6c 696e 6563  025;stroke-linec
-0000e500: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
-0000e510: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
-0000e520: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000e530: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-0000e540: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
-0000e550: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-0000e560: 2064 3d22 6d20 3431 372e 3038 3139 332c   d="m 417.08193,
-0000e570: 3434 392e 3234 3937 2031 392e 3331 3734  449.2497 19.3174
-0000e580: 312c 322e 3032 3633 3120 3134 2e31 3834  1,2.02631 14.184
-0000e590: 3131 2c2d 352e 3430 3334 3720 7a22 0a20  11,-5.40347 z". 
-0000e5a0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-0000e5b0: 3535 372d 302d 372d 332d 3522 0a20 2020  557-0-7-3-5".   
-0000e5c0: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
-0000e5d0: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
-0000e5e0: 3d22 3022 0a20 2020 2020 2020 696e 6b73  ="0".       inks
-0000e5f0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-0000e600: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
-0000e610: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-0000e620: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-0000e630: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
-0000e640: 6c65 3d22 6669 6c6c 3a23 3232 3334 3765  le="fill:#22347e
-0000e650: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-0000e660: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-0000e670: 7472 6f6b 652d 7769 6474 683a 302e 3834  troke-width:0.84
-0000e680: 3530 3235 3b73 7472 6f6b 652d 6c69 6e65  5025;stroke-line
-0000e690: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
-0000e6a0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
-0000e6b0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-0000e6c0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-0000e6d0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-0000e6e0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
-0000e6f0: 2020 643d 226d 2034 3137 2e30 3831 3933    d="m 417.08193
-0000e700: 2c34 3439 2e32 3439 3720 6320 302e 3433  ,449.2497 c 0.43
-0000e710: 3433 382c 332e 3734 3533 3320 2d31 2e30  438,3.74533 -1.0
-0000e720: 3639 3138 2c36 2e31 3036 3433 202d 312e  6918,6.10643 -1.
-0000e730: 3735 3631 332c 392e 3035 3038 3220 6c20  75613,9.05082 l 
-0000e740: 3231 2e30 3733 3534 2c2d 372e 3032 3435  21.07354,-7.0245
-0000e750: 3120 7a22 0a20 2020 2020 2020 6964 3d22  1 z".       id="
-0000e760: 7061 7468 3134 3535 392d 332d 342d 322d  path14559-3-4-2-
-0000e770: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
-0000e780: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-0000e790: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-0000e7a0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-0000e7b0: 7970 6573 3d22 6363 6363 220a 2020 2020  ypes="cccc".    
-0000e7c0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000e7d0: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
-0000e7e0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000e7f0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
-0000e800: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
-0000e810: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-0000e820: 2330 3831 3036 393b 6669 6c6c 2d6f 7061  #081069;fill-opa
-0000e830: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
-0000e840: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-0000e850: 7468 3a30 2e38 3435 3032 353b 7374 726f  th:0.845025;stro
-0000e860: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-0000e870: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-0000e880: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-0000e890: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000e8a0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000e8b0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000e8c0: 220a 2020 2020 2020 2064 3d22 6d20 3431  ".       d="m 41
-0000e8d0: 352e 3332 3538 2c34 3538 2e33 3030 3532  5.3258,458.30052
-0000e8e0: 2031 342e 3538 3933 372c 322e 3136 3133   14.58937,2.1613
-0000e8f0: 3920 3230 2e36 3638 3238 2c2d 3134 2e35  9 20.66828,-14.5
-0000e900: 3839 3337 207a 220a 2020 2020 2020 2069  8937 z".       i
-0000e910: 643d 2270 6174 6831 3435 3631 2d39 2d32  d="path14561-9-2
-0000e920: 2d32 2d32 220a 2020 2020 2020 2069 6e6b  -2-2".       ink
-0000e930: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-0000e940: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-0000e950: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000e960: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-0000e970: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000e980: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-0000e990: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
-0000e9a0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-0000e9b0: 6c3a 2330 3730 6532 623b 6669 6c6c 2d6f  l:#070e2b;fill-o
-0000e9c0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-0000e9d0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-0000e9e0: 6964 7468 3a30 2e38 3435 3032 353b 7374  idth:0.845025;st
-0000e9f0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-0000ea00: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-0000ea10: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-0000ea20: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000ea30: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000ea40: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-0000ea50: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
-0000ea60: 3432 392e 3931 3531 372c 3436 302e 3436  429.91517,460.46
-0000ea70: 3139 3120 382e 3537 3830 312c 3131 2e32  191 8.57801,11.2
-0000ea80: 3739 3734 202d 332e 3137 3435 342c 2d31  7974 -3.17454,-1
-0000ea90: 352e 3139 3732 3620 7a22 0a20 2020 2020  5.19726 z".     
-0000eaa0: 2020 6964 3d22 7061 7468 3134 3536 332d    id="path14563-
-0000eab0: 312d 302d 362d 3922 0a20 2020 2020 2020  1-0-6-9".       
-0000eac0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
-0000ead0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
-0000eae0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000eaf0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000eb00: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000eb10: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000eb20: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
-0000eb30: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-0000eb40: 6669 6c6c 3a23 3238 3364 3837 3b66 696c  fill:#283d87;fil
-0000eb50: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000eb60: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000eb70: 652d 7769 6474 683a 302e 3834 3530 3235  e-width:0.845025
-0000eb80: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-0000eb90: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-0000eba0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-0000ebb0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-0000ebc0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-0000ebd0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-0000ebe0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-0000ebf0: 226d 2034 3335 2e33 3138 3634 2c34 3536  "m 435.31864,456
-0000ec00: 2e35 3434 3339 2033 2e31 3734 3534 2c31  .54439 3.17454,1
-0000ec10: 352e 3139 3732 3620 6320 312e 3634 3333  5.19726 c 1.6433
-0000ec20: 392c 2d31 332e 3636 3136 3220 372e 3432  9,-13.66162 7.42
-0000ec30: 3636 352c 2d31 382e 3538 3335 3320 3132  665,-18.58353 12
-0000ec40: 2e30 3930 3237 2c2d 3235 2e38 3639 3131  .09027,-25.86911
-0000ec50: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
-0000ec60: 6174 6831 3435 3635 2d39 2d35 2d39 2d31  ath14565-9-5-9-1
-0000ec70: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000ec80: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-0000ec90: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
-0000eca0: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-0000ecb0: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
-0000ecc0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-0000ecd0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-0000ece0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000ecf0: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-0000ed00: 3e0a 2020 2020 3c65 6c6c 6970 7365 0a20  >.    <ellipse. 
-0000ed10: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-0000ed20: 6c3a 2330 3730 6532 623b 6669 6c6c 2d6f  l:#070e2b;fill-o
-0000ed30: 7061 6369 7479 3a30 2e39 3930 3434 363b  pacity:0.990446;
-0000ed40: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-0000ed50: 7472 6f6b 652d 7769 6474 683a 302e 3834  troke-width:0.84
-0000ed60: 3530 3235 3b73 7472 6f6b 652d 6d69 7465  5025;stroke-mite
-0000ed70: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-0000ed80: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-0000ed90: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-0000eda0: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
-0000edb0: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
-0000edc0: 7061 7468 3134 3536 372d 362d 312d 392d  path14567-6-1-9-
-0000edd0: 3222 0a20 2020 2020 2020 6378 3d22 3430  2".       cx="40
-0000ede0: 382e 3531 3330 3922 0a20 2020 2020 2020  8.51309".       
-0000edf0: 6379 3d22 3434 312e 3633 3436 3122 0a20  cy="441.63461". 
-0000ee00: 2020 2020 2020 7278 3d22 302e 3834 3232        rx="0.8422
-0000ee10: 3139 3035 220a 2020 2020 2020 2072 793d  1905".       ry=
-0000ee20: 2230 2e38 3432 3231 3931 3122 0a20 2020  "0.84221911".   
-0000ee30: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000ee40: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-0000ee50: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000ee60: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000ee70: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
-0000ee80: 2020 2020 2020 2072 3d22 302e 3834 3232         r="0.8422
-0000ee90: 3139 3131 220a 2020 2020 2020 2073 7479  1911".       sty
-0000eea0: 6c65 3d22 6669 6c6c 3a23 3235 3361 3764  le="fill:#253a7d
-0000eeb0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-0000eec0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-0000eed0: 7472 6f6b 652d 7769 6474 683a 302e 3834  troke-width:0.84
-0000eee0: 3530 3235 3b73 7472 6f6b 652d 6d69 7465  5025;stroke-mite
-0000eef0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-0000ef00: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-0000ef10: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-0000ef20: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
-0000ef30: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
-0000ef40: 7061 7468 3134 3536 372d 332d 3933 2d31  path14567-3-93-1
-0000ef50: 2d36 2d37 220a 2020 2020 2020 2063 783d  -6-7".       cx=
-0000ef60: 2234 3135 2e31 3930 3238 220a 2020 2020  "415.19028".    
-0000ef70: 2020 2063 793d 2234 3538 2e31 3230 3835     cy="458.12085
-0000ef80: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-0000ef90: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-0000efa0: 6572 2d78 3d22 332e 3439 3233 3732 3322  er-x="3.4923723"
-0000efb0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000efc0: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
-0000efd0: 722d 793d 222d 372e 3530 3438 3839 3722  r-y="-7.5048897"
-0000efe0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000eff0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-0000f000: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
-0000f010: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-0000f020: 3330 3022 202f 3e0a 2020 2020 3c63 6972  300" />.    <cir
-0000f030: 636c 650a 2020 2020 2020 2072 3d22 302e  cle.       r="0.
-0000f040: 3834 3232 3139 3131 220a 2020 2020 2020  84221911".      
-0000f050: 2073 7479 6c65 3d22 6669 6c6c 3a23 3235   style="fill:#25
-0000f060: 3361 3764 3b66 696c 6c2d 6f70 6163 6974  3a7d;fill-opacit
-0000f070: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-0000f080: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-0000f090: 302e 3834 3530 3235 3b73 7472 6f6b 652d  0.845025;stroke-
-0000f0a0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000f0b0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000f0c0: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
-0000f0d0: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
-0000f0e0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-0000f0f0: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
-0000f100: 372d 332d 302d 392d 3022 0a20 2020 2020  7-3-0-9-0".     
-0000f110: 2020 6378 3d22 3433 352e 3131 3335 3622    cx="435.11356"
-0000f120: 0a20 2020 2020 2020 6379 3d22 3435 312e  .       cy="451.
-0000f130: 3332 3939 3322 0a20 2020 2020 2020 696e  32993".       in
-0000f140: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
-0000f150: 2d63 656e 7465 722d 783d 2233 2e34 3932  -center-x="3.492
-0000f160: 3337 3136 220a 2020 2020 2020 2069 6e6b  3716".       ink
-0000f170: 7363 6170 653a 7472 616e 7366 6f72 6d2d  scape:transform-
-0000f180: 6365 6e74 6572 2d79 3d22 2d37 2e35 3034  center-y="-7.504
-0000f190: 3839 3131 220a 2020 2020 2020 2069 6e6b  8911".       ink
-0000f1a0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-0000f1b0: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
-0000f1c0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-0000f1d0: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-0000f1e0: 203c 6369 7263 6c65 0a20 2020 2020 2020   <circle.       
-0000f1f0: 723d 2230 2e38 3432 3231 3931 3122 0a20  r="0.84221911". 
-0000f200: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-0000f210: 6c3a 2361 3861 3961 613b 6669 6c6c 2d6f  l:#a8a9aa;fill-o
-0000f220: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-0000f230: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-0000f240: 6964 7468 3a30 2e38 3435 3032 353b 7374  idth:0.845025;st
-0000f250: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-0000f260: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-0000f270: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
-0000f280: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
-0000f290: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-0000f2a0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-0000f2b0: 3637 2d33 2d35 2d38 2d38 2d35 2d39 220a  67-3-5-8-8-5-9".
-0000f2c0: 2020 2020 2020 2063 783d 2234 3335 2e33         cx="435.3
-0000f2d0: 3133 3239 220a 2020 2020 2020 2063 793d  1329".       cy=
-0000f2e0: 2234 3536 2e34 3233 3122 0a20 2020 2020  "456.4231".     
-0000f2f0: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
-0000f300: 666f 726d 2d63 656e 7465 722d 783d 2233  form-center-x="3
-0000f310: 2e34 3932 3337 3036 220a 2020 2020 2020  .4923706".      
-0000f320: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-0000f330: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d37  orm-center-y="-7
-0000f340: 2e35 3034 3839 3538 220a 2020 2020 2020  .5048958".      
-0000f350: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-0000f360: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-0000f370: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-0000f380: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-0000f390: 0a20 2020 203c 6369 7263 6c65 0a20 2020  .    <circle.   
-0000f3a0: 2020 2020 723d 2230 2e38 3432 3231 3931      r="0.8422191
-0000f3b0: 3122 0a20 2020 2020 2020 7374 796c 653d  1".       style=
-0000f3c0: 2266 696c 6c3a 2361 6261 6139 633b 6669  "fill:#abaa9c;fi
-0000f3d0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-0000f3e0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000f3f0: 6b65 2d77 6964 7468 3a30 2e38 3435 3032  ke-width:0.84502
-0000f400: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
-0000f410: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-0000f420: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-0000f430: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-0000f440: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000f450: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-0000f460: 6831 3435 3637 2d33 2d39 2d30 2d39 2d38  h14567-3-9-0-9-8
-0000f470: 2d33 220a 2020 2020 2020 2063 783d 2234  -3".       cx="4
-0000f480: 3330 2e31 3230 3234 220a 2020 2020 2020  30.12024".      
-0000f490: 2063 793d 2234 3630 2e34 3137 3736 220a   cy="460.41776".
-0000f4a0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000f4b0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-0000f4c0: 2d78 3d22 332e 3439 3233 3731 3522 0a20  -x="3.4923715". 
-0000f4d0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
-0000f4e0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
-0000f4f0: 793d 222d 372e 3530 3438 3930 3722 0a20  y="-7.5048907". 
-0000f500: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000f510: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-0000f520: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-0000f530: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-0000f540: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
-0000f550: 650a 2020 2020 2020 2072 3d22 312e 3239  e.       r="1.29
-0000f560: 3938 3437 3122 0a20 2020 2020 2020 7374  98471".       st
-0000f570: 796c 653d 2266 696c 6c3a 2331 3132 3036  yle="fill:#11206
-0000f580: 363b 6669 6c6c 2d6f 7061 6369 7479 3a31  6;fill-opacity:1
-0000f590: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-0000f5a0: 7374 726f 6b65 2d77 6964 7468 3a30 2e38  stroke-width:0.8
-0000f5b0: 3435 3032 353b 7374 726f 6b65 2d6d 6974  45025;stroke-mit
-0000f5c0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-0000f5d0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-0000f5e0: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-0000f5f0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-0000f600: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-0000f610: 2270 6174 6831 3435 3637 2d33 2d32 2d35  "path14567-3-2-5
-0000f620: 2d34 2d33 2d36 220a 2020 2020 2020 2063  -4-3-6".       c
-0000f630: 783d 2234 3234 2e36 3237 3539 220a 2020  x="424.62759".  
-0000f640: 2020 2020 2063 793d 2234 3430 2e36 3934       cy="440.694
-0000f650: 3231 220a 2020 2020 2020 2069 6e6b 7363  21".       inksc
-0000f660: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
-0000f670: 6e74 6572 2d78 3d22 352e 3338 3939 3932  nter-x="5.389992
-0000f680: 3422 0a20 2020 2020 2020 696e 6b73 6361  4".       inksca
-0000f690: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-0000f6a0: 7465 722d 793d 222d 3131 2e35 3832 3735  ter-y="-11.58275
-0000f6b0: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
-0000f6c0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-0000f6d0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
-0000f6e0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-0000f6f0: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
-0000f700: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
-0000f710: 302e 3834 3232 3139 3131 220a 2020 2020  0.84221911".    
-0000f720: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
-0000f730: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
-0000f740: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
-0000f750: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-0000f760: 6b65 2d77 6964 7468 3a30 2e38 3435 3032  ke-width:0.84502
-0000f770: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
-0000f780: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
-0000f790: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
-0000f7a0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
-0000f7b0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-0000f7c0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-0000f7d0: 6831 3435 3637 2d32 2d36 2d30 2d30 2d30  h14567-2-6-0-0-0
-0000f7e0: 220a 2020 2020 2020 2063 783d 2234 3331  ".       cx="431
-0000f7f0: 2e36 3638 3138 220a 2020 2020 2020 2063  .66818".       c
-0000f800: 793d 2234 3432 2e31 3432 3234 220a 2020  y="442.14224".  
-0000f810: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-0000f820: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-0000f830: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000f840: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-0000f850: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
-0000f860: 0a20 2020 2020 2020 723d 2230 2e38 3432  .       r="0.842
-0000f870: 3231 3931 3122 0a20 2020 2020 2020 7374  21911".       st
-0000f880: 796c 653d 2266 696c 6c3a 2365 6466 3066  yle="fill:#edf0f
-0000f890: 633b 6669 6c6c 2d6f 7061 6369 7479 3a30  c;fill-opacity:0
-0000f8a0: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
-0000f8b0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-0000f8c0: 6474 683a 302e 3834 3530 3235 3b73 7472  dth:0.845025;str
-0000f8d0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-0000f8e0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-0000f8f0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-0000f900: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-0000f910: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-0000f920: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-0000f930: 372d 322d 382d 362d 372d 382d 3622 0a20  7-2-8-6-7-8-6". 
-0000f940: 2020 2020 2020 6378 3d22 3431 372e 3038        cx="417.08
-0000f950: 3737 3422 0a20 2020 2020 2020 6379 3d22  774".       cy="
-0000f960: 3434 392e 3133 3238 3722 0a20 2020 2020  449.13287".     
-0000f970: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-0000f980: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-0000f990: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-0000f9a0: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
-0000f9b0: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
-0000f9c0: 2020 2020 2072 3d22 312e 3630 3039 3334       r="1.600934
-0000f9d0: 3722 0a20 2020 2020 2020 7374 796c 653d  7".       style=
-0000f9e0: 2266 696c 6c3a 2365 6466 3066 633b 6669  "fill:#edf0fc;fi
-0000f9f0: 6c6c 2d6f 7061 6369 7479 3a30 2e39 3930  ll-opacity:0.990
-0000fa00: 3434 363b 7374 726f 6b65 3a23 6666 6666  446;stroke:#ffff
-0000fa10: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-0000fa20: 312e 3630 3632 353b 7374 726f 6b65 2d6d  1.60625;stroke-m
-0000fa30: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-0000fa40: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-0000fa50: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
-0000fa60: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
-0000fa70: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
-0000fa80: 643d 2270 6174 6831 3435 3637 2d32 2d37  d="path14567-2-7
-0000fa90: 2d30 2d39 2d30 2d32 220a 2020 2020 2020  -0-9-0-2".      
-0000faa0: 2063 783d 2234 3530 2e32 3933 3138 220a   cx="450.29318".
-0000fab0: 2020 2020 2020 2063 793d 2234 3436 2e30         cy="446.0
-0000fac0: 3836 3938 220a 2020 2020 2020 2069 6e6b  8698".       ink
-0000fad0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-0000fae0: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
-0000faf0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
-0000fb00: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
-0000fb10: 203c 670a 2020 2020 2020 2069 643d 2267   <g.       id="g
-0000fb20: 3133 3831 220a 2020 2020 2020 2074 7261  1381".       tra
-0000fb30: 6e73 666f 726d 3d22 6d61 7472 6978 2837  nsform="matrix(7
-0000fb40: 2e35 3531 3733 3834 2c30 2c30 2c37 2e35  .5517384,0,0,7.5
-0000fb50: 3531 3733 3834 2c2d 3639 332e 3835 3333  517384,-693.8533
-0000fb60: 352c 2d38 3235 2e30 3338 3539 2922 3e0a  5,-825.03859)">.
-0000fb70: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
-0000fb80: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-0000fb90: 3a23 3365 3462 3737 3b66 696c 6c2d 6f70  :#3e4b77;fill-op
-0000fba0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-0000fbb0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-0000fbc0: 6474 683a 303b 7374 726f 6b65 2d6c 696e  dth:0;stroke-lin
-0000fbd0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-0000fbe0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-0000fbf0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-0000fc00: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-0000fc10: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-0000fc20: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-0000fc30: 2020 2020 2064 3d22 6d20 3135 342e 3135       d="m 154.15
-0000fc40: 3236 362c 3134 352e 3235 3030 3820 312e  266,145.25008 1.
-0000fc50: 3433 3734 382c 2d30 2e30 3635 3320 302e  43748,-0.0653 0.
-0000fc60: 3934 3434 372c 2d31 2e30 3531 3338 2063  94447,-1.05138 c
-0000fc70: 202d 312e 3138 3938 332c 302e 3830 3031   -1.18983,0.8001
-0000fc80: 3820 2d31 2e37 3538 3237 2c30 2e39 3238  8 -1.75827,0.928
-0000fc90: 3620 2d32 2e33 3831 3935 2c31 2e31 3136  6 -2.38195,1.116
-0000fca0: 3732 207a 220a 2020 2020 2020 2020 2069  72 z".         i
-0000fcb0: 643d 2270 6174 6831 3435 3437 2d31 2d37  d="path14547-1-7
-0000fcc0: 2d38 2d35 2d30 2d33 2d34 220a 2020 2020  -8-5-0-3-4".    
-0000fcd0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
-0000fce0: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
-0000fcf0: 653d 2230 220a 2020 2020 2020 2020 2073  e="0".         s
-0000fd00: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-0000fd10: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
-0000fd20: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-0000fd30: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
-0000fd40: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-0000fd50: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-0000fd60: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
-0000fd70: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
-0000fd80: 6669 6c6c 3a23 3036 3035 3038 3b66 696c  fill:#060508;fil
-0000fd90: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
-0000fda0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-0000fdb0: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
-0000fdc0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
-0000fdd0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
-0000fde0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
-0000fdf0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
-0000fe00: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
-0000fe10: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-0000fe20: 2020 2020 2020 2020 2064 3d22 6d20 3135           d="m 15
-0000fe30: 352e 3539 3031 342c 3134 352e 3138 3437  5.59014,145.1847
-0000fe40: 3820 322e 3239 3238 352c 302e 3433 3935  8 2.29285,0.4395
-0000fe50: 3220 6320 2d30 2e36 3530 3434 2c2d 302e  2 c -0.65044,-0.
-0000fe60: 3334 3338 3520 2d31 2e30 3237 312c 2d30  34385 -1.0271,-0
-0000fe70: 2e38 3936 3320 2d31 2e33 3438 3338 2c2d  .8963 -1.34838,-
-0000fe80: 312e 3439 3039 3420 7a22 0a20 2020 2020  1.49094 z".     
-0000fe90: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
-0000fea0: 312d 302d 332d 392d 392d 342d 392d 3022  1-0-3-9-9-4-9-0"
-0000feb0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-0000fec0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-0000fed0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-0000fee0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-0000fef0: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
-0000ff00: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-0000ff10: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
-0000ff20: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-0000ff30: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-0000ff40: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
-0000ff50: 7061 7468 0a20 2020 2020 2020 2020 7374  path.         st
-0000ff60: 796c 653d 2266 696c 6c3a 2332 3733 3737  yle="fill:#27377
-0000ff70: 333b 6669 6c6c 2d6f 7061 6369 7479 3a31  3;fill-opacity:1
-0000ff80: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-0000ff90: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-0000ffa0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
-0000ffb0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
-0000ffc0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
-0000ffd0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
-0000ffe0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
-0000fff0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
-00010000: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
-00010010: 226d 2031 3534 2e31 3532 3636 2c31 3435  "m 154.15266,145
-00010020: 2e32 3530 3038 2063 2030 2e33 3136 3332  .25008 c 0.31632
-00010030: 2c30 2e31 3831 3437 2030 2e36 3635 3039  ,0.18147 0.66509
-00010040: 2c30 2e33 3337 3937 2030 2e37 3834 3038  ,0.33797 0.78408
-00010050: 2c30 2e36 3731 3232 206c 2030 2e36 3533  ,0.67122 l 0.653
-00010060: 342c 2d30 2e37 3336 3536 207a 220a 2020  4,-0.73656 z".  
-00010070: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00010080: 3435 3533 2d33 2d32 2d32 2d31 2d33 2d38  4553-3-2-2-1-3-8
-00010090: 2d39 220a 2020 2020 2020 2020 2069 6e6b  -9".         ink
-000100a0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
-000100b0: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
-000100c0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-000100d0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
-000100e0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000100f0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
-00010100: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
-00010110: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
-00010120: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
-00010130: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00010140: 2073 7479 6c65 3d22 6669 6c6c 3a23 3134   style="fill:#14
-00010150: 3236 3732 3b66 696c 6c2d 6f70 6163 6974  2672;fill-opacit
-00010160: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00010170: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00010180: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
-00010190: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-000101a0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-000101b0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-000101c0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-000101d0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-000101e0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
-000101f0: 2064 3d22 6d20 3135 342e 3933 3637 342c   d="m 154.93674,
-00010200: 3134 352e 3932 3133 2032 2e39 3436 3235  145.9213 2.94625
-00010210: 2c2d 302e 3239 3720 2d32 2e32 3932 3835  ,-0.297 -2.29285
-00010220: 2c2d 302e 3433 3935 3620 7a22 0a20 2020  ,-0.43956 z".   
-00010230: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00010240: 3535 352d 342d 312d 362d 372d 322d 322d  555-4-1-6-7-2-2-
-00010250: 3322 0a20 2020 2020 2020 2020 696e 6b73  3".         inks
-00010260: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
-00010270: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
-00010280: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00010290: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-000102a0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000102b0: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
-000102c0: 3330 3022 202f 3e0a 2020 2020 2020 3c70  300" />.      <p
-000102d0: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
-000102e0: 6c65 3d22 6669 6c6c 3a23 3534 3636 3863  le="fill:#54668c
-000102f0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-00010300: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00010310: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
-00010320: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
-00010330: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
-00010340: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
-00010350: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
-00010360: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
-00010370: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
-00010380: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
-00010390: 6d20 3135 342e 3933 3637 342c 3134 352e  m 154.93674,145.
-000103a0: 3932 3133 2063 2030 2e30 3338 322c 302e  9213 c 0.0382,0.
-000103b0: 3332 3933 3820 2d30 2e30 3934 2c30 2e35  32938 -0.094,0.5
-000103c0: 3337 3033 202d 302e 3135 3434 342c 302e  3703 -0.15444,0.
-000103d0: 3739 3539 3720 6c20 332e 3130 3036 392c  79597 l 3.10069,
-000103e0: 2d31 2e30 3932 3937 207a 220a 2020 2020  -1.09297 z".    
-000103f0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00010400: 3539 2d33 2d34 2d32 2d34 2d34 2d33 2d35  59-3-4-2-4-4-3-5
-00010410: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
-00010420: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00010430: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-00010440: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
-00010450: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
-00010460: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00010470: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
-00010480: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
-00010490: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
-000104a0: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
-000104b0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
-000104c0: 7479 6c65 3d22 6669 6c6c 3a23 3038 3130  tyle="fill:#0810
-000104d0: 3639 3b66 696c 6c2d 6f70 6163 6974 793a  69;fill-opacity:
-000104e0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-000104f0: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
-00010500: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-00010510: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-00010520: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00010530: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00010540: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00010550: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-00010560: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
-00010570: 3d22 6d20 3135 342e 3738 3233 2c31 3436  ="m 154.7823,146
-00010580: 2e37 3137 3237 2031 2e32 3833 3035 2c30  .71727 1.28305,0
-00010590: 2e31 3930 3038 2031 2e38 3137 3634 2c2d  .19008 1.81764,-
-000105a0: 312e 3238 3330 3520 7a22 0a20 2020 2020  1.28305 z".     
-000105b0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-000105c0: 312d 392d 322d 322d 382d 302d 312d 3722  1-9-2-2-8-0-1-7"
-000105d0: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-000105e0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
-000105f0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
-00010600: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00010610: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00010620: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00010630: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00010640: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
-00010650: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
-00010660: 3d22 6669 6c6c 3a23 3037 3065 3262 3b66  ="fill:#070e2b;f
-00010670: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
-00010680: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
-00010690: 6f6b 652d 7769 6474 683a 303b 7374 726f  oke-width:0;stro
-000106a0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-000106b0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-000106c0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-000106d0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-000106e0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-000106f0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00010700: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
-00010710: 3135 362e 3036 3533 352c 3134 362e 3930  156.06535,146.90
-00010720: 3733 3520 302e 3735 3433 382c 302e 3939  735 0.75438,0.99
-00010730: 3139 3820 2d30 2e32 3739 3138 2c2d 312e  198 -0.27918,-1.
-00010740: 3333 3635 207a 220a 2020 2020 2020 2020  3365 z".        
-00010750: 2069 643d 2270 6174 6831 3435 3633 2d31   id="path14563-1
-00010760: 2d30 2d36 2d38 2d37 2d32 2d32 220a 2020  -0-6-8-7-2-2".  
-00010770: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00010780: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00010790: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
-000107a0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-000107b0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-000107c0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-000107d0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
-000107e0: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
-000107f0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
-00010800: 696c 6c3a 2330 3730 6532 623b 6669 6c6c  ill:#070e2b;fill
-00010810: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
-00010820: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
-00010830: 2d77 6964 7468 3a30 3b73 7472 6f6b 652d  -width:0;stroke-
-00010840: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
-00010850: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
-00010860: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
-00010870: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
-00010880: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
-00010890: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-000108a0: 2020 2020 2020 2020 643d 226d 2031 3536          d="m 156
-000108b0: 2e30 3635 3335 2c31 3436 2e39 3037 3335  .06535,146.90735
-000108c0: 2030 2e37 3534 3338 2c30 2e39 3931 3938   0.75438,0.99198
-000108d0: 2063 2030 2e31 3434 3532 2c2d 312e 3230   c 0.14452,-1.20
-000108e0: 3134 3620 302e 3635 3331 322c 2d31 2e36  146 0.65312,-1.6
-000108f0: 3334 3320 312e 3036 3332 362c 2d32 2e32  343 1.06326,-2.2
-00010900: 3735 3033 207a 220a 2020 2020 2020 2020  7503 z".        
-00010910: 2069 643d 2270 6174 6831 3435 3635 2d39   id="path14565-9
-00010920: 2d35 2d39 2d37 2d37 2d33 2d34 220a 2020  -5-9-7-7-3-4".  
-00010930: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00010940: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00010950: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
-00010960: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-00010970: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
-00010980: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00010990: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-000109a0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-000109b0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-000109c0: 3022 202f 3e0a 2020 2020 2020 3c63 6972  0" />.      <cir
-000109d0: 636c 650a 2020 2020 2020 2020 2073 7479  cle.         sty
-000109e0: 6c65 3d22 6669 6c6c 3a23 3037 3065 3262  le="fill:#070e2b
-000109f0: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
-00010a00: 3939 3034 3436 3b73 7472 6f6b 653a 2366  990446;stroke:#f
-00010a10: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-00010a20: 7468 3a30 3b73 7472 6f6b 652d 6d69 7465  th:0;stroke-mite
-00010a30: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00010a40: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00010a50: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
-00010a60: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
-00010a70: 793a 3122 0a20 2020 2020 2020 2020 6964  y:1".         id
-00010a80: 3d22 7061 7468 3134 3536 372d 362d 312d  ="path14567-6-1-
-00010a90: 392d 372d 372d 352d 3922 0a20 2020 2020  9-7-7-5-9".     
-00010aa0: 2020 2020 6378 3d22 3135 342e 3138 3331      cx="154.1831
-00010ab0: 3822 0a20 2020 2020 2020 2020 6379 3d22  8".         cy="
-00010ac0: 3134 352e 3235 3136 3222 0a20 2020 2020  145.25162".     
-00010ad0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00010ae0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00010af0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00010b00: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00010b10: 3022 0a20 2020 2020 2020 2020 723d 2230  0".         r="0
-00010b20: 2e30 3734 3036 3737 3739 2220 2f3e 0a20  .074067779" />. 
-00010b30: 2020 2020 203c 6369 7263 6c65 0a20 2020       <circle.   
-00010b40: 2020 2020 2020 723d 2230 2e30 3734 3036        r="0.07406
-00010b50: 3737 3739 220a 2020 2020 2020 2020 2073  7779".         s
-00010b60: 7479 6c65 3d22 6669 6c6c 3a23 3235 3361  tyle="fill:#253a
-00010b70: 3764 3b66 696c 6c2d 6f70 6163 6974 793a  7d;fill-opacity:
-00010b80: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00010b90: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
-00010ba0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00010bb0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00010bc0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00010bd0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-00010be0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00010bf0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00010c00: 6831 3435 3637 2d33 2d39 332d 312d 362d  h14567-3-93-1-6-
-00010c10: 392d 332d 372d 3822 0a20 2020 2020 2020  9-3-7-8".       
-00010c20: 2020 6378 3d22 3135 342e 3737 3034 220a    cx="154.7704".
-00010c30: 2020 2020 2020 2020 2063 793d 2231 3436           cy="146
-00010c40: 2e37 3031 3438 220a 2020 2020 2020 2020  .70148".        
-00010c50: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-00010c60: 6f72 6d2d 6365 6e74 6572 2d78 3d22 342e  orm-center-x="4.
-00010c70: 3634 3332 3536 3622 0a20 2020 2020 2020  6432566".       
-00010c80: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
-00010c90: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
-00010ca0: 392e 3937 3830 3632 3122 0a20 2020 2020  9.9780621".     
-00010cb0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00010cc0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00010cd0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00010ce0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00010cf0: 3022 202f 3e0a 2020 2020 2020 3c63 6972  0" />.      <cir
-00010d00: 636c 650a 2020 2020 2020 2020 2072 3d22  cle.         r="
-00010d10: 302e 3037 3430 3637 3737 3922 0a20 2020  0.074067779".   
-00010d20: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00010d30: 6c3a 2361 6261 6139 633b 6669 6c6c 2d6f  l:#abaa9c;fill-o
-00010d40: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
-00010d50: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
-00010d60: 6964 7468 3a30 3b73 7472 6f6b 652d 6d69  idth:0;stroke-mi
-00010d70: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00010d80: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00010d90: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
-00010da0: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
-00010db0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
-00010dc0: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
-00010dd0: 392d 302d 392d 382d 322d 382d 302d 3522  9-0-9-8-2-8-0-5"
-00010de0: 0a20 2020 2020 2020 2020 6378 3d22 3135  .         cx="15
-00010df0: 362e 3038 3334 220a 2020 2020 2020 2020  6.0834".        
-00010e00: 2063 793d 2231 3436 2e39 3033 3437 220a   cy="146.90347".
-00010e10: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
-00010e20: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
-00010e30: 6572 2d78 3d22 342e 3634 3332 3536 3622  er-x="4.6432566"
-00010e40: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
-00010e50: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
-00010e60: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
-00010e70: 3122 0a20 2020 2020 2020 2020 696e 6b73  1".         inks
-00010e80: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
-00010e90: 3d22 3330 3022 0a20 2020 2020 2020 2020  ="300".         
-00010ea0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00010eb0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-00010ec0: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
-00010ed0: 2020 2020 2072 3d22 302e 3131 3433 3133       r="0.114313
-00010ee0: 3234 220a 2020 2020 2020 2020 2073 7479  24".         sty
-00010ef0: 6c65 3d22 6669 6c6c 3a23 3131 3230 3636  le="fill:#112066
-00010f00: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
-00010f10: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-00010f20: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
-00010f30: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00010f40: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00010f50: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
-00010f60: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
-00010f70: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00010f80: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00010f90: 3435 3637 2d33 2d32 2d35 2d34 2d33 2d38  4567-3-2-5-4-3-8
-00010fa0: 2d30 2d37 2d37 220a 2020 2020 2020 2020  -0-7-7".        
-00010fb0: 2063 783d 2231 3535 2e36 3030 3336 220a   cx="155.60036".
-00010fc0: 2020 2020 2020 2020 2063 793d 2231 3435           cy="145
-00010fd0: 2e31 3638 3931 220a 2020 2020 2020 2020  .16891".        
-00010fe0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
-00010ff0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 372e  orm-center-x="7.
-00011000: 3136 3632 3131 3622 0a20 2020 2020 2020  1662116".       
-00011010: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
-00011020: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
-00011030: 3135 2e33 3939 3735 3122 0a20 2020 2020  15.399751".     
-00011040: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00011050: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00011060: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
-00011070: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-00011080: 3022 202f 3e0a 2020 2020 2020 3c63 6972  0" />.      <cir
-00011090: 636c 650a 2020 2020 2020 2020 2072 3d22  cle.         r="
-000110a0: 302e 3037 3430 3637 3737 3922 0a20 2020  0.074067779".   
-000110b0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-000110c0: 6c3a 2365 6466 3066 633b 6669 6c6c 2d6f  l:#edf0fc;fill-o
-000110d0: 7061 6369 7479 3a30 2e39 3930 3434 363b  pacity:0.990446;
-000110e0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
-000110f0: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
-00011100: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
-00011110: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
-00011120: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
-00011130: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
-00011140: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
-00011150: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00011160: 3435 3637 2d32 2d38 2d36 2d37 2d38 2d32  4567-2-8-6-7-8-2
-00011170: 2d32 2d36 2d39 220a 2020 2020 2020 2020  -2-6-9".        
-00011180: 2063 783d 2231 3534 2e39 3337 3237 220a   cx="154.93727".
-00011190: 2020 2020 2020 2020 2063 793d 2231 3435           cy="145
-000111a0: 2e39 3131 3034 220a 2020 2020 2020 2020  .91104".        
-000111b0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-000111c0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-000111d0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-000111e0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
-000111f0: 2f3e 0a20 2020 2020 203c 6369 7263 6c65  />.      <circle
-00011200: 0a20 2020 2020 2020 2020 723d 2230 2e31  .         r="0.1
-00011210: 3430 3739 3139 3522 0a20 2020 2020 2020  4079195".       
-00011220: 2020 7374 796c 653d 2266 696c 6c3a 2365    style="fill:#e
-00011230: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
-00011240: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
-00011250: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-00011260: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
-00011270: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00011280: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00011290: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
-000112a0: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
-000112b0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-000112c0: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
-000112d0: 2d32 2d37 2d30 2d39 2d30 2d35 2d31 2d31  -2-7-0-9-0-5-1-1
-000112e0: 2d33 220a 2020 2020 2020 2020 2063 783d  -3".         cx=
-000112f0: 2231 3537 2e38 3537 3438 220a 2020 2020  "157.85748".    
-00011300: 2020 2020 2063 793d 2231 3435 2e36 3433       cy="145.643
-00011310: 3137 220a 2020 2020 2020 2020 2069 6e6b  17".         ink
-00011320: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
-00011330: 693d 2233 3030 220a 2020 2020 2020 2020  i="300".        
-00011340: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00011350: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00011360: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
-00011370: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-00011380: 6e6f 6e65 3b66 696c 6c2d 7275 6c65 3a65  none;fill-rule:e
-00011390: 7665 6e6f 6464 3b73 7472 6f6b 653a 2366  venodd;stroke:#f
-000113a0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
-000113b0: 7468 3a30 2e31 3332 3239 323b 7374 726f  th:0.132292;stro
-000113c0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
-000113d0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
-000113e0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
-000113f0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00011400: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00011410: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-00011420: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
-00011430: 3135 342e 3135 3236 362c 3134 352e 3235  154.15266,145.25
-00011440: 3030 3820 6320 302e 3838 3934 382c 2d30  008 c 0.88948,-0
-00011450: 2e31 3831 3233 2031 2e36 3436 3433 2c2d  .18123 1.64643,-
-00011460: 302e 3632 3735 3220 322e 3338 3139 352c  0.62752 2.38195,
-00011470: 2d31 2e31 3136 3638 2030 2e33 3332 3436  -1.11668 0.33246
-00011480: 2c30 2e36 3034 3231 2030 2e36 3532 2c31  ,0.60421 0.652,1
-00011490: 2e32 3230 3237 2031 2e33 3438 3338 2c31  .22027 1.34838,1
-000114a0: 2e34 3930 3920 2d30 2e34 3232 3235 2c30  .4909 -0.42225,0
-000114b0: 2e35 3735 3635 202d 302e 3834 3235 372c  .57565 -0.84257,
-000114c0: 312e 3135 3635 3120 2d31 2e30 3633 3236  1.15651 -1.06326
-000114d0: 2c32 2e32 3735 3033 206c 202d 302e 3735  ,2.27503 l -0.75
-000114e0: 3433 382c 2d30 2e39 3931 3938 202d 312e  438,-0.99198 -1.
-000114f0: 3238 3330 352c 2d30 2e31 3930 3038 2063  28305,-0.19008 c
-00011500: 2030 2e31 3337 3936 2c2d 302e 3330 3835   0.13796,-0.3085
-00011510: 3620 302e 3230 3333 352c 2d30 2e35 3830  6 0.20335,-0.580
-00011520: 3834 2030 2e31 3534 3434 2c2d 302e 3739  84 0.15444,-0.79
-00011530: 3539 3720 2d30 2e32 3031 3734 2c2d 302e  597 -0.20174,-0.
-00011540: 3235 3335 3520 2d30 2e34 3537 3636 2c2d  25355 -0.45766,-
-00011550: 302e 3438 3030 3120 2d30 2e37 3834 3038  0.48001 -0.78408
-00011560: 2c2d 302e 3637 3132 3220 7a22 0a20 2020  ,-0.67122 z".   
-00011570: 2020 2020 2020 6964 3d22 7061 7468 3133        id="path13
-00011580: 3033 2d37 220a 2020 2020 2020 2020 2073  03-7".         s
-00011590: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-000115a0: 733d 2263 6363 6363 6363 6322 202f 3e0a  s="cccccccc" />.
-000115b0: 2020 2020 3c2f 673e 0a20 2020 203c 7061      </g>.    <pa
-000115c0: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-000115d0: 2266 696c 6c3a 2333 6534 6237 373b 6669  "fill:#3e4b77;fi
-000115e0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
-000115f0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-00011600: 6b65 2d77 6964 7468 3a30 3b73 7472 6f6b  ke-width:0;strok
-00011610: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
-00011620: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
-00011630: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
-00011640: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
-00011650: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
-00011660: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
-00011670: 0a20 2020 2020 2020 643d 226d 2034 3731  .       d="m 471
-00011680: 2e35 3934 3531 2c33 3331 2e33 3733 3533  .59451,331.37353
-00011690: 2035 2e34 3332 3939 2c2d 302e 3234 3638   5.43299,-0.2468
-000116a0: 2033 2e35 3639 3635 2c2d 332e 3937 3337   3.56965,-3.9737
-000116b0: 3220 6320 2d34 2e34 3936 3939 2c33 2e30  2 c -4.49699,3.0
-000116c0: 3234 3320 2d36 2e36 3435 3433 2c33 2e35  243 -6.64543,3.5
-000116d0: 3039 3637 202d 392e 3030 3236 342c 342e  0967 -9.00264,4.
-000116e0: 3232 3036 3720 7a22 0a20 2020 2020 2020  22067 z".       
-000116f0: 6964 3d22 7061 7468 3134 3534 372d 312d  id="path14547-1-
-00011700: 372d 382d 352d 302d 3322 0a20 2020 2020  7-8-5-0-3".     
-00011710: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
-00011720: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
-00011730: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
-00011740: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00011750: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
-00011760: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
-00011770: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
-00011780: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
-00011790: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
-000117a0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
-000117b0: 653d 2266 696c 6c3a 2330 3630 3530 383b  e="fill:#060508;
-000117c0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-000117d0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-000117e0: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
-000117f0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
-00011800: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
-00011810: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
-00011820: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
-00011830: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
-00011840: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
-00011850: 3122 0a20 2020 2020 2020 643d 226d 2034  1".       d="m 4
-00011860: 3737 2e30 3237 352c 3333 312e 3132 3637  77.0275,331.1267
-00011870: 3320 382e 3636 3538 392c 312e 3636 3131  3 8.66589,1.6611
-00011880: 3820 6320 2d32 2e34 3538 3335 2c2d 312e  8 c -2.45835,-1.
-00011890: 3239 3935 3920 2d33 2e38 3831 3935 2c2d  29959 -3.88195,-
-000118a0: 332e 3338 3735 3920 2d35 2e30 3936 3234  3.38759 -5.09624
-000118b0: 2c2d 352e 3633 3530 3520 7a22 0a20 2020  ,-5.63505 z".   
-000118c0: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
-000118d0: 312d 302d 332d 392d 392d 342d 3922 0a20  1-0-3-9-9-4-9". 
-000118e0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-000118f0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00011900: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
-00011910: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00011920: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
-00011930: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00011940: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00011950: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00011960: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00011970: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
-00011980: 7374 796c 653d 2266 696c 6c3a 2332 3733  style="fill:#273
-00011990: 3737 333b 6669 6c6c 2d6f 7061 6369 7479  773;fill-opacity
-000119a0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
-000119b0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
-000119c0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
-000119d0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
-000119e0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
-000119f0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
-00011a00: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
-00011a10: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
-00011a20: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
-00011a30: 226d 2034 3731 2e35 3934 3531 2c33 3331  "m 471.59451,331
-00011a40: 2e33 3733 3533 2063 2031 2e31 3935 3534  .37353 c 1.19554
-00011a50: 2c30 2e36 3835 3837 2032 2e35 3133 3732  ,0.68587 2.51372
-00011a60: 2c31 2e32 3737 3337 2032 2e39 3633 3435  ,1.27737 2.96345
-00011a70: 2c32 2e35 3336 3920 6c20 322e 3436 3935  ,2.5369 l 2.4695
-00011a80: 342c 2d32 2e37 3833 3835 207a 220a 2020  4,-2.78385 z".  
-00011a90: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
-00011aa0: 3533 2d33 2d32 2d32 2d31 2d33 2d38 220a  53-3-2-2-1-3-8".
-00011ab0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00011ac0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
-00011ad0: 7572 653d 2230 220a 2020 2020 2020 2073  ure="0".       s
-00011ae0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
-00011af0: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
-00011b00: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00011b10: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-00011b20: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00011b30: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
-00011b40: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00011b50: 2073 7479 6c65 3d22 6669 6c6c 3a23 3134   style="fill:#14
-00011b60: 3236 3732 3b66 696c 6c2d 6f70 6163 6974  2672;fill-opacit
-00011b70: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00011b80: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00011b90: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
-00011ba0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00011bb0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00011bc0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00011bd0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00011be0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-00011bf0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-00011c00: 3d22 6d20 3437 342e 3535 3739 362c 3333  ="m 474.55796,33
-00011c10: 332e 3931 3034 3320 3131 2e31 3335 3433  3.91043 11.13543
-00011c20: 2c2d 312e 3132 3235 3220 2d38 2e36 3635  ,-1.12252 -8.665
-00011c30: 3839 2c2d 312e 3636 3133 3320 7a22 0a20  89,-1.66133 z". 
-00011c40: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00011c50: 3535 352d 342d 312d 362d 372d 322d 3222  555-4-1-6-7-2-2"
-00011c60: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-00011c70: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
-00011c80: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
-00011c90: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-00011ca0: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
-00011cb0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
-00011cc0: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
-00011cd0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
-00011ce0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3534   style="fill:#54
-00011cf0: 3636 3863 3b66 696c 6c2d 6f70 6163 6974  668c;fill-opacit
-00011d00: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
-00011d10: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
-00011d20: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
-00011d30: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00011d40: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00011d50: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00011d60: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00011d70: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-00011d80: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-00011d90: 3d22 6d20 3437 342e 3535 3739 362c 3333  ="m 474.55796,33
-00011da0: 332e 3931 3034 3320 6320 302e 3134 3433  3.91043 c 0.1443
-00011db0: 382c 312e 3234 3439 202d 302e 3335 3532  8,1.2449 -0.3552
-00011dc0: 382c 322e 3032 3937 3220 2d30 2e35 3833  8,2.02972 -0.583
-00011dd0: 3731 2c33 2e30 3038 3339 206c 2031 312e  71,3.00839 l 11.
-00011de0: 3731 3931 342c 2d34 2e31 3330 3931 207a  71914,-4.13091 z
-00011df0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
-00011e00: 6831 3435 3539 2d33 2d34 2d32 2d34 2d34  h14559-3-4-2-4-4
-00011e10: 2d33 220a 2020 2020 2020 2069 6e6b 7363  -3".       inksc
-00011e20: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
-00011e30: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
-00011e40: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
-00011e50: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
-00011e60: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00011e70: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00011e80: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00011e90: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-00011ea0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
-00011eb0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00011ec0: 3a23 3038 3130 3639 3b66 696c 6c2d 6f70  :#081069;fill-op
-00011ed0: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
-00011ee0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-00011ef0: 6474 683a 303b 7374 726f 6b65 2d6c 696e  dth:0;stroke-lin
-00011f00: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
-00011f10: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
-00011f20: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00011f30: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00011f40: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00011f50: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
-00011f60: 2020 2064 3d22 6d20 3437 332e 3937 3432     d="m 473.9742
-00011f70: 352c 3333 362e 3931 3838 3220 342e 3834  5,336.91882 4.84
-00011f80: 3933 322c 302e 3731 3834 3120 362e 3836  932,0.71841 6.86
-00011f90: 3938 322c 2d34 2e38 3439 3332 207a 220a  982,-4.84932 z".
-00011fa0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00011fb0: 3435 3631 2d39 2d32 2d32 2d38 2d30 2d31  4561-9-2-2-8-0-1
-00011fc0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00011fd0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
-00011fe0: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
-00011ff0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00012000: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
-00012010: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
-00012020: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
-00012030: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
-00012040: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-00012050: 3730 6532 623b 6669 6c6c 2d6f 7061 6369  70e2b;fill-opaci
-00012060: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
-00012070: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
-00012080: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
-00012090: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
-000120a0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
-000120b0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-000120c0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000120d0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-000120e0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-000120f0: 643d 226d 2034 3738 2e38 3233 3537 2c33  d="m 478.82357,3
-00012100: 3337 2e36 3337 3233 2032 2e38 3531 322c  37.63723 2.8512,
-00012110: 332e 3734 3932 3220 2d31 2e30 3535 3137  3.74922 -1.05517
-00012120: 2c2d 352e 3035 3133 3420 7a22 0a20 2020  ,-5.05134 z".   
-00012130: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-00012140: 332d 312d 302d 362d 382d 372d 3222 0a20  3-1-0-6-8-7-2". 
-00012150: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00012160: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00012170: 7265 3d22 3022 0a20 2020 2020 2020 696e  re="0".       in
-00012180: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
-00012190: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
-000121a0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
-000121b0: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
-000121c0: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
-000121d0: 7479 6c65 3d22 6669 6c6c 3a23 3037 3065  tyle="fill:#070e
-000121e0: 3262 3b66 696c 6c2d 6f70 6163 6974 793a  2b;fill-opacity:
-000121f0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
-00012200: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
-00012210: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
-00012220: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
-00012230: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
-00012240: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00012250: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00012260: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
-00012270: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
-00012280: 6d20 3437 382e 3832 3335 372c 3333 372e  m 478.82357,337.
-00012290: 3633 3732 3320 322e 3835 3132 2c33 2e37  63723 2.8512,3.7
-000122a0: 3439 3232 2063 2030 2e35 3436 3232 2c2d  4922 c 0.54622,-
-000122b0: 342e 3534 3039 3620 322e 3436 3834 392c  4.54096 2.46849,
-000122c0: 2d36 2e31 3736 3839 2034 2e30 3138 3632  -6.17689 4.01862
-000122d0: 2c2d 382e 3539 3835 3420 7a22 0a20 2020  ,-8.59854 z".   
-000122e0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-000122f0: 352d 392d 352d 392d 372d 372d 3322 0a20  5-9-5-9-7-7-3". 
-00012300: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
-00012310: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
-00012320: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
-00012330: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
-00012340: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
-00012350: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00012360: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00012370: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00012380: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00012390: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-000123a0: 2020 7374 796c 653d 2266 696c 6c3a 2330    style="fill:#0
-000123b0: 3730 6532 623b 6669 6c6c 2d6f 7061 6369  70e2b;fill-opaci
-000123c0: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
-000123d0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
-000123e0: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
-000123f0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
-00012400: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
-00012410: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
-00012420: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
-00012430: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
-00012440: 2069 643d 2270 6174 6831 3435 3637 2d36   id="path14567-6
-00012450: 2d31 2d39 2d37 2d37 2d35 220a 2020 2020  -1-9-7-7-5".    
-00012460: 2020 2063 783d 2234 3731 2e37 3039 3834     cx="471.70984
-00012470: 220a 2020 2020 2020 2063 793d 2233 3331  ".       cy="331
-00012480: 2e33 3739 3333 220a 2020 2020 2020 2069  .37933".       i
-00012490: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-000124a0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-000124b0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-000124c0: 2d79 6470 693d 2233 3030 220a 2020 2020  -ydpi="300".    
-000124d0: 2020 2072 3d22 302e 3237 3939 3431 3222     r="0.2799412"
-000124e0: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
-000124f0: 2020 2020 2020 2072 3d22 302e 3237 3939         r="0.2799
-00012500: 3431 3222 0a20 2020 2020 2020 7374 796c  412".       styl
-00012510: 653d 2266 696c 6c3a 2332 3533 6137 643b  e="fill:#253a7d;
-00012520: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-00012530: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-00012540: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
-00012550: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00012560: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00012570: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-00012580: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-00012590: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000125a0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-000125b0: 372d 332d 3933 2d31 2d36 2d39 2d33 2d37  7-3-93-1-6-9-3-7
-000125c0: 220a 2020 2020 2020 2063 783d 2234 3733  ".       cx="473
-000125d0: 2e39 3239 3236 220a 2020 2020 2020 2063  .92926".       c
-000125e0: 793d 2233 3336 2e38 3539 3133 220a 2020  y="336.85913".  
-000125f0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-00012600: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
-00012610: 3d22 342e 3634 3332 3536 3622 0a20 2020  ="4.6432566".   
-00012620: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
-00012630: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
-00012640: 222d 392e 3937 3830 3632 3122 0a20 2020  "-9.9780621".   
-00012650: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
-00012660: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
-00012670: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-00012680: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
-00012690: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
-000126a0: 2020 2020 2020 2072 3d22 302e 3237 3939         r="0.2799
-000126b0: 3431 3222 0a20 2020 2020 2020 7374 796c  412".       styl
-000126c0: 653d 2266 696c 6c3a 2361 6261 6139 633b  e="fill:#abaa9c;
-000126d0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
-000126e0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
-000126f0: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
-00012700: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
-00012710: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-00012720: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
-00012730: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
-00012740: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-00012750: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
-00012760: 372d 332d 392d 302d 392d 382d 322d 382d  7-3-9-0-9-8-2-8-
-00012770: 3022 0a20 2020 2020 2020 6378 3d22 3437  0".       cx="47
-00012780: 382e 3839 3137 3822 0a20 2020 2020 2020  8.89178".       
-00012790: 6379 3d22 3333 372e 3632 3235 3922 0a20  cy="337.62259". 
-000127a0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
-000127b0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
-000127c0: 783d 2234 2e36 3433 3235 3636 220a 2020  x="4.6432566".  
-000127d0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
-000127e0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
-000127f0: 3d22 2d39 2e39 3738 3036 3231 220a 2020  ="-9.9780621".  
-00012800: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-00012810: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
-00012820: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00012830: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
-00012840: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
-00012850: 0a20 2020 2020 2020 723d 2230 2e34 3332  .       r="0.432
-00012860: 3035 3030 3522 0a20 2020 2020 2020 7374  05005".       st
-00012870: 796c 653d 2266 696c 6c3a 2331 3132 3036  yle="fill:#11206
-00012880: 363b 6669 6c6c 2d6f 7061 6369 7479 3a31  6;fill-opacity:1
-00012890: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
-000128a0: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
-000128b0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-000128c0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
-000128d0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
-000128e0: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
-000128f0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
-00012900: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
-00012910: 3536 372d 332d 322d 352d 342d 332d 382d  567-3-2-5-4-3-8-
-00012920: 302d 3722 0a20 2020 2020 2020 6378 3d22  0-7".       cx="
-00012930: 3437 372e 3036 3631 220a 2020 2020 2020  477.0661".      
-00012940: 2063 793d 2233 3331 2e30 3636 3737 220a   cy="331.06677".
-00012950: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
-00012960: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
-00012970: 2d78 3d22 372e 3136 3632 3131 3622 0a20  -x="7.1662116". 
-00012980: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
-00012990: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
-000129a0: 793d 222d 3135 2e33 3939 3735 3122 0a20  y="-15.399751". 
-000129b0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
-000129c0: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
-000129d0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
-000129e0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
-000129f0: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
-00012a00: 650a 2020 2020 2020 2072 3d22 302e 3237  e.       r="0.27
-00012a10: 3939 3431 3222 0a20 2020 2020 2020 7374  99412".       st
-00012a20: 796c 653d 2266 696c 6c3a 2365 6466 3066  yle="fill:#edf0f
-00012a30: 633b 6669 6c6c 2d6f 7061 6369 7479 3a30  c;fill-opacity:0
-00012a40: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
-00012a50: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
-00012a60: 6474 683a 303b 7374 726f 6b65 2d6d 6974  dth:0;stroke-mit
-00012a70: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
-00012a80: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-00012a90: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
-00012aa0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
-00012ab0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
-00012ac0: 2270 6174 6831 3435 3637 2d32 2d38 2d36  "path14567-2-8-6
-00012ad0: 2d37 2d38 2d32 2d32 2d36 220a 2020 2020  -7-8-2-2-6".    
-00012ae0: 2020 2063 783d 2234 3734 2e35 3539 3937     cx="474.55997
-00012af0: 220a 2020 2020 2020 2063 793d 2233 3333  ".       cy="333
-00012b00: 2e38 3731 3637 220a 2020 2020 2020 2069  .87167".       i
-00012b10: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
-00012b20: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
-00012b30: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00012b40: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
-00012b50: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
-00012b60: 2020 723d 2230 2e35 3332 3132 3730 3822    r="0.53212708"
-00012b70: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
-00012b80: 696c 6c3a 2365 6466 3066 633b 6669 6c6c  ill:#edf0fc;fill
-00012b90: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
-00012ba0: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
-00012bb0: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
-00012bc0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00012bd0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
-00012be0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
-00012bf0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
-00012c00: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
-00012c10: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
-00012c20: 3435 3637 2d32 2d37 2d30 2d39 2d30 2d35  4567-2-7-0-9-0-5
-00012c30: 2d31 2d31 220a 2020 2020 2020 2063 783d  -1-1".       cx=
-00012c40: 2234 3835 2e35 3936 3938 220a 2020 2020  "485.59698".    
-00012c50: 2020 2063 793d 2233 3332 2e38 3539 3235     cy="332.85925
-00012c60: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
-00012c70: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
-00012c80: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
-00012c90: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
-00012ca0: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
-00012cb0: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
-00012cc0: 2266 696c 6c3a 6e6f 6e65 3b66 696c 6c2d  "fill:none;fill-
-00012cd0: 7275 6c65 3a65 7665 6e6f 6464 3b73 7472  rule:evenodd;str
-00012ce0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
-00012cf0: 6b65 2d77 6964 7468 3a30 2e35 3030 3030  ke-width:0.50000
-00012d00: 313b 7374 726f 6b65 2d6c 696e 6563 6170  1;stroke-linecap
-00012d10: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
-00012d20: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
-00012d30: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
-00012d40: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
-00012d50: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
-00012d60: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
-00012d70: 3d22 6d20 3437 312e 3539 3435 312c 3333  ="m 471.59451,33
-00012d80: 312e 3337 3335 3320 6320 332e 3336 3138  1.37353 c 3.3618
-00012d90: 312c 2d30 2e36 3834 3936 2036 2e32 3232  1,-0.68496 6.222
-00012da0: 3732 2c2d 322e 3337 3137 3320 392e 3030  72,-2.37173 9.00
-00012db0: 3236 342c 2d34 2e32 3230 3532 2031 2e32  264,-4.22052 1.2
-00012dc0: 3536 3534 2c32 2e32 3833 3633 2032 2e34  5654,2.28363 2.4
-00012dd0: 3634 3236 2c34 2e36 3132 3034 2035 2e30  6426,4.61204 5.0
-00012de0: 3936 3234 2c35 2e36 3334 3920 2d31 2e35  9624,5.6349 -1.5
-00012df0: 3935 392c 322e 3137 3536 3820 2d33 2e31  959,2.17568 -3.1
-00012e00: 3834 3531 2c34 2e33 3731 3036 202d 342e  8451,4.37106 -4.
-00012e10: 3031 3836 322c 382e 3539 3835 3420 6c20  01862,8.59854 l 
-00012e20: 2d32 2e38 3531 322c 2d33 2e37 3439 3232  -2.8512,-3.74922
-00012e30: 202d 342e 3834 3933 322c 2d30 2e37 3138   -4.84932,-0.718
-00012e40: 3431 2063 2030 2e35 3231 3432 2c2d 312e  41 c 0.52142,-1.
-00012e50: 3136 3632 3120 302e 3736 3835 372c 2d32  16621 0.76857,-2
-00012e60: 2e31 3935 3320 302e 3538 3337 312c 2d33  .1953 0.58371,-3
-00012e70: 2e30 3038 3339 202d 302e 3736 3234 382c  .00839 -0.76248,
-00012e80: 2d30 2e39 3538 3320 2d31 2e37 3239 3734  -0.9583 -1.72974
-00012e90: 2c2d 312e 3831 3432 3120 2d32 2e39 3633  ,-1.81421 -2.963
-00012ea0: 3435 2c2d 322e 3533 3639 207a 220a 2020  45,-2.5369 z".  
-00012eb0: 2020 2020 2069 643d 2270 6174 6831 3330       id="path130
-00012ec0: 3322 0a20 2020 2020 2020 736f 6469 706f  3".       sodipo
-00012ed0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00012ee0: 6363 6363 6363 2220 2f3e 0a20 203c 2f67  cccccc" />.  </g
-00012ef0: 3e0a 3c2f 7376 673e 0a                   >.</svg>.
+00000450: 6f67 6f5f 6e6f 726d 616c 223e 0a20 2020  ogo_normal">.   
+00000460: 203c 696e 6b73 6361 7065 3a70 6167 650a   <inkscape:page.
+00000470: 2020 2020 2020 2078 3d22 3022 0a20 2020         x="0".   
+00000480: 2020 2020 793d 2230 220a 2020 2020 2020      y="0".      
+00000490: 2077 6964 7468 3d22 3430 3022 0a20 2020   width="400".   
+000004a0: 2020 2020 6865 6967 6874 3d22 3230 3022      height="200"
+000004b0: 0a20 2020 2020 2020 6964 3d22 7061 6765  .       id="page
+000004c0: 3332 3622 0a20 2020 2020 2020 696e 6b73  326".       inks
+000004d0: 6361 7065 3a6c 6162 656c 3d22 4c6f 676f  cape:label="Logo
+000004e0: 2220 2f3e 0a20 2020 203c 696e 6b73 6361  " />.    <inksca
+000004f0: 7065 3a70 6167 650a 2020 2020 2020 2078  pe:page.       x
+00000500: 3d22 2d30 2e36 3830 3135 3936 3322 0a20  ="-0.68015963". 
+00000510: 2020 2020 2020 793d 2232 3530 2e36 3238        y="250.628
+00000520: 3534 220a 2020 2020 2020 2077 6964 7468  54".       width
+00000530: 3d22 3235 3622 0a20 2020 2020 2020 6865  ="256".       he
+00000540: 6967 6874 3d22 3235 3622 0a20 2020 2020  ight="256".     
+00000550: 2020 6964 3d22 7061 6765 3332 3822 0a20    id="page328". 
+00000560: 2020 2020 2020 696e 6b73 6361 7065 3a6c        inkscape:l
+00000570: 6162 656c 3d22 4963 6f6e 3235 3622 202f  abel="Icon256" /
+00000580: 3e0a 2020 2020 3c69 6e6b 7363 6170 653a  >.    <inkscape:
+00000590: 7061 6765 0a20 2020 2020 2020 783d 2233  page.       x="3
+000005a0: 3131 2e36 3534 3732 220a 2020 2020 2020  11.65472".      
+000005b0: 2079 3d22 3235 392e 3431 3034 3322 0a20   y="259.41043". 
+000005c0: 2020 2020 2020 7769 6474 683d 2231 3238        width="128
+000005d0: 220a 2020 2020 2020 2068 6569 6768 743d  ".       height=
+000005e0: 2231 3238 220a 2020 2020 2020 2069 643d  "128".       id=
+000005f0: 2270 6167 6533 3831 220a 2020 2020 2020  "page381".      
+00000600: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
+00000610: 2249 636f 6e31 3238 2220 2f3e 0a20 2020  "Icon128" />.   
+00000620: 203c 696e 6b73 6361 7065 3a70 6167 650a   <inkscape:page.
+00000630: 2020 2020 2020 2078 3d22 3331 362e 3237         x="316.27
+00000640: 3236 3422 0a20 2020 2020 2020 793d 2234  264".       y="4
+00000650: 3138 2e39 3738 3736 220a 2020 2020 2020  18.97876".      
+00000660: 2077 6964 7468 3d22 3634 220a 2020 2020   width="64".    
+00000670: 2020 2068 6569 6768 743d 2236 3422 0a20     height="64". 
+00000680: 2020 2020 2020 6964 3d22 7061 6765 3338        id="page38
+00000690: 3322 0a20 2020 2020 2020 696e 6b73 6361  3".       inksca
+000006a0: 7065 3a6c 6162 656c 3d22 4963 6f6e 3634  pe:label="Icon64
+000006b0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+000006c0: 653a 6578 706f 7274 2d66 696c 656e 616d  e:export-filenam
+000006d0: 653d 222e 2f49 636f 6e36 342e 706e 6722  e="./Icon64.png"
+000006e0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+000006f0: 3a65 7870 6f72 742d 7864 7069 3d22 3936  :export-xdpi="96
+00000700: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00000710: 653a 6578 706f 7274 2d79 6470 693d 2239  e:export-ydpi="9
+00000720: 3622 202f 3e0a 2020 2020 3c69 6e6b 7363  6" />.    <inksc
+00000730: 6170 653a 7061 6765 0a20 2020 2020 2020  ape:page.       
+00000740: 783d 2234 3638 2e38 3233 3234 220a 2020  x="468.82324".  
+00000750: 2020 2020 2079 3d22 3236 312e 3331 3234       y="261.3124
+00000760: 3122 0a20 2020 2020 2020 7769 6474 683d  1".       width=
+00000770: 2233 3222 0a20 2020 2020 2020 6865 6967  "32".       heig
+00000780: 6874 3d22 3332 220a 2020 2020 2020 2069  ht="32".       i
+00000790: 643d 2270 6167 6533 3835 220a 2020 2020  d="page385".    
+000007a0: 2020 2069 6e6b 7363 6170 653a 6c61 6265     inkscape:labe
+000007b0: 6c3d 2249 636f 6e33 3222 202f 3e0a 2020  l="Icon32" />.  
+000007c0: 2020 3c69 6e6b 7363 6170 653a 7061 6765    <inkscape:page
+000007d0: 0a20 2020 2020 2020 783d 2234 3730 2e39  .       x="470.9
+000007e0: 3134 3433 220a 2020 2020 2020 2079 3d22  1443".       y="
+000007f0: 3332 362e 3038 3130 3222 0a20 2020 2020  326.08102".     
+00000800: 2020 7769 6474 683d 2231 3622 0a20 2020    width="16".   
+00000810: 2020 2020 6865 6967 6874 3d22 3136 220a      height="16".
+00000820: 2020 2020 2020 2069 643d 2270 6167 6533         id="page3
+00000830: 3837 220a 2020 2020 2020 2069 6e6b 7363  87".       inksc
+00000840: 6170 653a 6c61 6265 6c3d 2249 636f 6e31  ape:label="Icon1
+00000850: 3622 202f 3e0a 2020 2020 3c69 6e6b 7363  6" />.    <inksc
+00000860: 6170 653a 7061 6765 0a20 2020 2020 2020  ape:page.       
+00000870: 783d 2234 3035 2e36 3937 3831 220a 2020  x="405.69781".  
+00000880: 2020 2020 2079 3d22 3432 362e 3133 3332       y="426.1332
+00000890: 3422 0a20 2020 2020 2020 7769 6474 683d  4".       width=
+000008a0: 2234 3822 0a20 2020 2020 2020 6865 6967  "48".       heig
+000008b0: 6874 3d22 3438 220a 2020 2020 2020 2069  ht="48".       i
+000008c0: 643d 2270 6167 6537 3830 3222 0a20 2020  d="page7802".   
+000008d0: 2020 2020 696e 6b73 6361 7065 3a6c 6162      inkscape:lab
+000008e0: 656c 3d22 4963 6f6e 3438 220a 2020 2020  el="Icon48".    
+000008f0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+00000900: 7274 2d66 696c 656e 616d 653d 222e 2f49  rt-filename="./I
+00000910: 636f 6e34 382e 706e 6722 0a20 2020 2020  con48.png".     
+00000920: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00000930: 742d 7864 7069 3d22 3936 220a 2020 2020  t-xdpi="96".    
+00000940: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+00000950: 7274 2d79 6470 693d 2239 3622 202f 3e0a  rt-ydpi="96" />.
+00000960: 2020 2020 3c69 6e6b 7363 6170 653a 7061      <inkscape:pa
+00000970: 6765 0a20 2020 2020 2020 783d 2234 3530  ge.       x="450
+00000980: 220a 2020 2020 2020 2079 3d22 2d31 2e38  ".       y="-1.8
+00000990: 3532 3036 3131 652d 3036 220a 2020 2020  520611e-06".    
+000009a0: 2020 2077 6964 7468 3d22 3430 3022 0a20     width="400". 
+000009b0: 2020 2020 2020 6865 6967 6874 3d22 3230        height="20
+000009c0: 3022 0a20 2020 2020 2020 6964 3d22 7061  0".       id="pa
+000009d0: 6765 3635 3222 0a20 2020 2020 2020 696e  ge652".       in
+000009e0: 6b73 6361 7065 3a6c 6162 656c 3d22 4c6f  kscape:label="Lo
+000009f0: 676f 5f62 6c61 636b 220a 2020 2020 2020  go_black".      
+00000a00: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00000a10: 2d66 696c 656e 616d 653d 222e 2e2f 6262  -filename="../bb
+00000a20: 3766 3538 6635 2f4c 6f67 6f5f 626c 6163  7f58f5/Logo_blac
+00000a30: 6b2e 706e 6722 0a20 2020 2020 2020 696e  k.png".       in
+00000a40: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+00000a50: 7069 3d22 3936 220a 2020 2020 2020 2069  pi="96".       i
+00000a60: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+00000a70: 6470 693d 2239 3622 202f 3e0a 2020 2020  dpi="96" />.    
+00000a80: 3c69 6e6b 7363 6170 653a 7061 6765 0a20  <inkscape:page. 
+00000a90: 2020 2020 2020 783d 2239 3030 220a 2020        x="900".  
+00000aa0: 2020 2020 2079 3d22 2d31 2e38 3532 3036       y="-1.85206
+00000ab0: 3131 652d 3036 220a 2020 2020 2020 2077  11e-06".       w
+00000ac0: 6964 7468 3d22 3430 3022 0a20 2020 2020  idth="400".     
+00000ad0: 2020 6865 6967 6874 3d22 3230 3022 0a20    height="200". 
+00000ae0: 2020 2020 2020 6964 3d22 7061 6765 3230        id="page20
+00000af0: 3134 2220 2f3e 0a20 203c 2f73 6f64 6970  14" />.  </sodip
+00000b00: 6f64 693a 6e61 6d65 6476 6965 773e 0a20  odi:namedview>. 
+00000b10: 203c 6465 6673 0a20 2020 2020 6964 3d22   <defs.     id="
+00000b20: 6465 6673 3222 3e0a 2020 2020 3c66 696c  defs2">.    <fil
+00000b30: 7465 720a 2020 2020 2020 2069 6e6b 7363  ter.       inksc
+00000b40: 6170 653a 636f 6c6c 6563 743d 2261 6c77  ape:collect="alw
+00000b50: 6179 7322 0a20 2020 2020 2020 7374 796c  ays".       styl
+00000b60: 653d 2263 6f6c 6f72 2d69 6e74 6572 706f  e="color-interpo
+00000b70: 6c61 7469 6f6e 2d66 696c 7465 7273 3a73  lation-filters:s
+00000b80: 5247 4222 0a20 2020 2020 2020 6964 3d22  RGB".       id="
+00000b90: 6669 6c74 6572 3135 3035 3122 0a20 2020  filter15051".   
+00000ba0: 2020 2020 783d 222d 302e 3136 3733 3334      x="-0.167334
+00000bb0: 3036 220a 2020 2020 2020 2077 6964 7468  06".       width
+00000bc0: 3d22 312e 3333 3436 3638 3122 0a20 2020  ="1.3346681".   
+00000bd0: 2020 2020 793d 222d 302e 3635 3239 3834      y="-0.652984
+00000be0: 3335 220a 2020 2020 2020 2068 6569 6768  35".       heigh
+00000bf0: 743d 2232 2e33 3035 3936 3837 223e 0a20  t="2.3059687">. 
+00000c00: 2020 2020 203c 6665 4761 7573 7369 616e       <feGaussian
+00000c10: 426c 7572 0a20 2020 2020 2020 2020 696e  Blur.         in
+00000c20: 6b73 6361 7065 3a63 6f6c 6c65 6374 3d22  kscape:collect="
+00000c30: 616c 7761 7973 220a 2020 2020 2020 2020  always".        
+00000c40: 2073 7464 4465 7669 6174 696f 6e3d 2235   stdDeviation="5
+00000c50: 2e32 3236 3032 3039 220a 2020 2020 2020  .2260209".      
+00000c60: 2020 2069 643d 2266 6547 6175 7373 6961     id="feGaussia
+00000c70: 6e42 6c75 7231 3530 3533 2220 2f3e 0a20  nBlur15053" />. 
+00000c80: 2020 203c 2f66 696c 7465 723e 0a20 2020     </filter>.   
+00000c90: 203c 6669 6c74 6572 0a20 2020 2020 2020   <filter.       
+00000ca0: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
+00000cb0: 3d22 616c 7761 7973 220a 2020 2020 2020  ="always".      
+00000cc0: 2073 7479 6c65 3d22 636f 6c6f 722d 696e   style="color-in
+00000cd0: 7465 7270 6f6c 6174 696f 6e2d 6669 6c74  terpolation-filt
+00000ce0: 6572 733a 7352 4742 220a 2020 2020 2020  ers:sRGB".      
+00000cf0: 2069 643d 2266 696c 7465 7231 3530 3531   id="filter15051
+00000d00: 2d33 220a 2020 2020 2020 2078 3d22 2d30  -3".       x="-0
+00000d10: 2e31 3637 3333 3430 3622 0a20 2020 2020  .16733406".     
+00000d20: 2020 7769 6474 683d 2231 2e33 3334 3636    width="1.33466
+00000d30: 3831 220a 2020 2020 2020 2079 3d22 2d30  81".       y="-0
+00000d40: 2e36 3532 3938 3433 3522 0a20 2020 2020  .65298435".     
+00000d50: 2020 6865 6967 6874 3d22 322e 3330 3539    height="2.3059
+00000d60: 3638 3722 3e0a 2020 2020 2020 3c66 6547  687">.      <feG
+00000d70: 6175 7373 6961 6e42 6c75 720a 2020 2020  aussianBlur.    
+00000d80: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+00000d90: 6c6c 6563 743d 2261 6c77 6179 7322 0a20  llect="always". 
+00000da0: 2020 2020 2020 2020 7374 6444 6576 6961          stdDevia
+00000db0: 7469 6f6e 3d22 352e 3232 3630 3230 3922  tion="5.2260209"
+00000dc0: 0a20 2020 2020 2020 2020 6964 3d22 6665  .         id="fe
+00000dd0: 4761 7573 7369 616e 426c 7572 3135 3035  GaussianBlur1505
+00000de0: 332d 3622 202f 3e0a 2020 2020 3c2f 6669  3-6" />.    </fi
+00000df0: 6c74 6572 3e0a 2020 2020 3c66 696c 7465  lter>.    <filte
+00000e00: 720a 2020 2020 2020 2069 6e6b 7363 6170  r.       inkscap
+00000e10: 653a 636f 6c6c 6563 743d 2261 6c77 6179  e:collect="alway
+00000e20: 7322 0a20 2020 2020 2020 7374 796c 653d  s".       style=
+00000e30: 2263 6f6c 6f72 2d69 6e74 6572 706f 6c61  "color-interpola
+00000e40: 7469 6f6e 2d66 696c 7465 7273 3a73 5247  tion-filters:sRG
+00000e50: 4222 0a20 2020 2020 2020 6964 3d22 6669  B".       id="fi
+00000e60: 6c74 6572 3135 3035 312d 332d 3222 0a20  lter15051-3-2". 
+00000e70: 2020 2020 2020 783d 222d 302e 3136 3733        x="-0.1673
+00000e80: 3334 3036 220a 2020 2020 2020 2077 6964  3406".       wid
+00000e90: 7468 3d22 312e 3333 3436 3638 3122 0a20  th="1.3346681". 
+00000ea0: 2020 2020 2020 793d 222d 302e 3635 3239        y="-0.6529
+00000eb0: 3834 3335 220a 2020 2020 2020 2068 6569  8435".       hei
+00000ec0: 6768 743d 2232 2e33 3035 3936 3837 223e  ght="2.3059687">
+00000ed0: 0a20 2020 2020 203c 6665 4761 7573 7369  .      <feGaussi
+00000ee0: 616e 426c 7572 0a20 2020 2020 2020 2020  anBlur.         
+00000ef0: 696e 6b73 6361 7065 3a63 6f6c 6c65 6374  inkscape:collect
+00000f00: 3d22 616c 7761 7973 220a 2020 2020 2020  ="always".      
+00000f10: 2020 2073 7464 4465 7669 6174 696f 6e3d     stdDeviation=
+00000f20: 2235 2e32 3236 3032 3039 220a 2020 2020  "5.2260209".    
+00000f30: 2020 2020 2069 643d 2266 6547 6175 7373       id="feGauss
+00000f40: 6961 6e42 6c75 7231 3530 3533 2d36 2d32  ianBlur15053-6-2
+00000f50: 2220 2f3e 0a20 2020 203c 2f66 696c 7465  " />.    </filte
+00000f60: 723e 0a20 2020 203c 6669 6c74 6572 0a20  r>.    <filter. 
+00000f70: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00000f80: 6f6c 6c65 6374 3d22 616c 7761 7973 220a  ollect="always".
+00000f90: 2020 2020 2020 2073 7479 6c65 3d22 636f         style="co
+00000fa0: 6c6f 722d 696e 7465 7270 6f6c 6174 696f  lor-interpolatio
+00000fb0: 6e2d 6669 6c74 6572 733a 7352 4742 220a  n-filters:sRGB".
+00000fc0: 2020 2020 2020 2069 643d 2266 696c 7465         id="filte
+00000fd0: 7231 3530 3531 2d33 3622 0a20 2020 2020  r15051-36".     
+00000fe0: 2020 783d 222d 302e 3136 3733 3334 3036    x="-0.16733406
+00000ff0: 220a 2020 2020 2020 2077 6964 7468 3d22  ".       width="
+00001000: 312e 3333 3436 3638 3122 0a20 2020 2020  1.3346681".     
+00001010: 2020 793d 222d 302e 3635 3239 3834 3335    y="-0.65298435
+00001020: 220a 2020 2020 2020 2068 6569 6768 743d  ".       height=
+00001030: 2232 2e33 3035 3936 3837 223e 0a20 2020  "2.3059687">.   
+00001040: 2020 203c 6665 4761 7573 7369 616e 426c     <feGaussianBl
+00001050: 7572 0a20 2020 2020 2020 2020 696e 6b73  ur.         inks
+00001060: 6361 7065 3a63 6f6c 6c65 6374 3d22 616c  cape:collect="al
+00001070: 7761 7973 220a 2020 2020 2020 2020 2073  ways".         s
+00001080: 7464 4465 7669 6174 696f 6e3d 2235 2e32  tdDeviation="5.2
+00001090: 3236 3032 3039 220a 2020 2020 2020 2020  260209".        
+000010a0: 2069 643d 2266 6547 6175 7373 6961 6e42   id="feGaussianB
+000010b0: 6c75 7231 3530 3533 2d37 2220 2f3e 0a20  lur15053-7" />. 
+000010c0: 2020 203c 2f66 696c 7465 723e 0a20 203c     </filter>.  <
+000010d0: 2f64 6566 733e 0a20 203c 670a 2020 2020  /defs>.  <g.    
+000010e0: 2069 6e6b 7363 6170 653a 6c61 6265 6c3d   inkscape:label=
+000010f0: 224c 6179 6572 2031 220a 2020 2020 2069  "Layer 1".     i
+00001100: 6e6b 7363 6170 653a 6772 6f75 706d 6f64  nkscape:groupmod
+00001110: 653d 226c 6179 6572 220a 2020 2020 2069  e="layer".     i
+00001120: 643d 226c 6179 6572 3122 3e0a 2020 2020  d="layer1">.    
+00001130: 3c67 0a20 2020 2020 2020 6964 3d22 6c6f  <g.       id="lo
+00001140: 676f 5f6e 6f72 6d61 6c22 3e0a 2020 2020  go_normal">.    
+00001150: 2020 3c72 6563 740a 2020 2020 2020 2020    <rect.        
+00001160: 2073 7479 6c65 3d22 6669 6c6c 3a23 6666   style="fill:#ff
+00001170: 6666 6666 3b73 7472 6f6b 653a 6e6f 6e65  ffff;stroke:none
+00001180: 3b73 7472 6f6b 652d 7769 6474 683a 352e  ;stroke-width:5.
+00001190: 3038 3437 363b 7374 726f 6b65 2d6c 696e  08476;stroke-lin
+000011a0: 6563 6170 3a72 6f75 6e64 3b73 7472 6f6b  ecap:round;strok
+000011b0: 652d 6c69 6e65 6a6f 696e 3a72 6f75 6e64  e-linejoin:round
+000011c0: 3b66 696c 6c2d 6f70 6163 6974 793a 302e  ;fill-opacity:0.
+000011d0: 3032 3030 3937 3036 220a 2020 2020 2020  02009706".      
+000011e0: 2020 2069 643d 2272 6563 7437 3036 220a     id="rect706".
+000011f0: 2020 2020 2020 2020 2077 6964 7468 3d22           width="
+00001200: 3430 3022 0a20 2020 2020 2020 2020 6865  400".         he
+00001210: 6967 6874 3d22 3230 3022 0a20 2020 2020  ight="200".     
+00001220: 2020 2020 783d 222d 362e 3639 3635 3133      x="-6.696513
+00001230: 3165 2d30 3622 0a20 2020 2020 2020 2020  1e-06".         
+00001240: 793d 222d 312e 3835 3230 3631 3165 2d30  y="-1.8520611e-0
+00001250: 3622 0a20 2020 2020 2020 2020 7279 3d22  6".         ry="
+00001260: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
+00001270: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00001280: 3d22 6669 6c6c 3a23 3030 3030 3030 3b66  ="fill:#000000;f
+00001290: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+000012a0: 3834 3038 3b73 7472 6f6b 653a 2330 3030  8408;stroke:#000
+000012b0: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+000012c0: 3a30 2e35 3030 3032 3270 783b 7374 726f  :0.500022px;stro
+000012d0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+000012e0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+000012f0: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
+00001300: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+00001310: 2064 3d22 4d20 3137 332e 3834 3831 312c   d="M 173.84811,
+00001320: 3839 2e30 3639 3531 2033 3337 2e36 3530  89.06951 337.650
+00001330: 3936 2c36 342e 3934 3937 3120 3137 312e  96,64.94971 171.
+00001340: 3837 3434 352c 3830 2e37 3134 3336 205a  87445,80.71436 Z
+00001350: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00001360: 6174 6831 3436 3537 220a 2020 2020 2020  ath14657".      
+00001370: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00001380: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+00001390: 2230 220a 2020 2020 2020 2020 2073 6f64  "0".         sod
+000013a0: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+000013b0: 2263 6363 6322 202f 3e0a 2020 2020 2020  "cccc" />.      
+000013c0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+000013d0: 7479 6c65 3d22 6669 6c6c 3a23 3365 3462  tyle="fill:#3e4b
+000013e0: 3737 3b66 696c 6c2d 6f70 6163 6974 793a  77;fill-opacity:
+000013f0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00001400: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00001410: 3035 3030 353b 7374 726f 6b65 2d6c 696e  05005;stroke-lin
+00001420: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00001430: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00001440: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00001450: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00001460: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00001470: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00001480: 2020 2020 2064 3d22 4d20 3139 2e36 3033       d="M 19.603
+00001490: 3037 2c36 372e 3635 3639 2038 302e 3835  07,67.6569 80.85
+000014a0: 3830 3238 2c36 342e 3838 3531 3220 3132  8028,64.88512 12
+000014b0: 312e 3130 3430 352c 3230 2e32 3834 3534  1.10405,20.28454
+000014c0: 2043 2037 302e 3430 3235 3837 2c35 342e   C 70.402587,54.
+000014d0: 3232 3837 3320 3436 2e31 3739 3630 352c  22873 46.179605,
+000014e0: 3539 2e36 3736 3337 2031 392e 3630 3330  59.67637 19.6030
+000014f0: 372c 3637 2e36 3536 3920 5a22 0a20 2020  7,67.6569 Z".   
+00001500: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00001510: 3534 3722 0a20 2020 2020 2020 2020 696e  547".         in
+00001520: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00001530: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+00001540: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+00001550: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+00001560: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+00001570: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00001580: 2266 696c 6c3a 2331 6332 6336 383b 6669  "fill:#1c2c68;fi
+00001590: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+000015a0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+000015b0: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+000015c0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+000015d0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+000015e0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+000015f0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00001600: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00001610: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00001620: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+00001630: 643d 226d 2038 302e 3835 3830 3238 2c36  d="m 80.858028,6
+00001640: 342e 3838 3531 3220 3236 2e35 3737 3536  4.88512 26.57756
+00001650: 322c 362e 3034 3735 3420 3133 2e36 3638  2,6.04754 13.668
+00001660: 3436 2c2d 3530 2e36 3438 3132 207a 220a  46,-50.64812 z".
+00001670: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00001680: 6831 3435 3439 220a 2020 2020 2020 2020  h14549".        
+00001690: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+000016a0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+000016b0: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+000016c0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000016d0: 2266 696c 6c3a 2330 3630 3530 383b 6669  "fill:#060508;fi
+000016e0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+000016f0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00001700: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+00001710: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00001720: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00001730: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00001740: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00001750: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00001760: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00001770: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+00001780: 643d 224d 2031 3037 2e34 3335 3539 2c37  d="M 107.43559,7
+00001790: 302e 3933 3236 3620 3137 382e 3536 3232  0.93266 178.5622
+000017a0: 332c 3833 2e35 3331 3720 4320 3135 302e  3,83.5317 C 150.
+000017b0: 3834 3534 312c 3638 2e39 3434 3937 2031  84541,68.94497 1
+000017c0: 3334 2e37 3935 3031 2c34 352e 3530 3935  34.79501,45.5095
+000017d0: 3520 3132 312e 3130 3430 352c 3230 2e32  5 121.10405,20.2
+000017e0: 3834 3534 205a 220a 2020 2020 2020 2020  8454 Z".        
+000017f0: 2069 643d 2270 6174 6831 3435 3531 220a   id="path14551".
+00001800: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00001810: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00001820: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+00001830: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+00001840: 7479 7065 733d 2263 6363 6322 202f 3e0a  types="cccc" />.
+00001850: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00001860: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00001870: 3a23 3237 3337 3733 3b66 696c 6c2d 6f70  :#273773;fill-op
+00001880: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+00001890: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+000018a0: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
+000018b0: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+000018c0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+000018d0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+000018e0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+000018f0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00001900: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00001910: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
+00001920: 3139 2e36 3033 3037 2c36 372e 3635 3639  19.60307,67.6569
+00001930: 2063 2031 332e 3437 3933 3132 2c37 2e36   c 13.479312,7.6
+00001940: 3937 3820 3238 2e33 3431 3130 372c 3134  978 28.341107,14
+00001950: 2e33 3336 3935 2033 332e 3431 3137 3936  .33695 33.411796
+00001960: 2c32 382e 3437 3338 3220 6c20 3237 2e38  ,28.47382 l 27.8
+00001970: 3433 3136 322c 2d33 312e 3234 3536 207a  43162,-31.2456 z
+00001980: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00001990: 6174 6831 3435 3533 220a 2020 2020 2020  ath14553".      
+000019a0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+000019b0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+000019c0: 2230 220a 2020 2020 2020 2020 2073 6f64  "0".         sod
+000019d0: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+000019e0: 2263 6363 6322 202f 3e0a 2020 2020 2020  "cccc" />.      
+000019f0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+00001a00: 7479 6c65 3d22 6669 6c6c 3a23 3134 3236  tyle="fill:#1426
+00001a10: 3732 3b66 696c 6c2d 6f70 6163 6974 793a  72;fill-opacity:
+00001a20: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00001a30: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00001a40: 3035 3030 353b 7374 726f 6b65 2d6c 696e  05005;stroke-lin
+00001a50: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00001a60: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00001a70: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00001a80: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00001a90: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00001aa0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00001ab0: 2020 2020 2064 3d22 4d20 3533 2e30 3134       d="M 53.014
+00001ac0: 3836 362c 3936 2e31 3330 3732 2031 3738  866,96.13072 178
+00001ad0: 2e35 3632 3233 2c38 332e 3533 3137 2038  .56223,83.5317 8
+00001ae0: 302e 3835 3830 3238 2c36 342e 3838 3531  0.858028,64.8851
+00001af0: 3220 5a22 0a20 2020 2020 2020 2020 6964  2 Z".         id
+00001b00: 3d22 7061 7468 3134 3535 3522 0a20 2020  ="path14555".   
+00001b10: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00001b20: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00001b30: 7265 3d22 3022 202f 3e0a 2020 2020 2020  re="0" />.      
+00001b40: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+00001b50: 7479 6c65 3d22 6669 6c6c 3a23 3534 3636  tyle="fill:#5466
+00001b60: 3863 3b66 696c 6c2d 6f70 6163 6974 793a  8c;fill-opacity:
+00001b70: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00001b80: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00001b90: 3035 3030 353b 7374 726f 6b65 2d6c 696e  05005;stroke-lin
+00001ba0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00001bb0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00001bc0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00001bd0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00001be0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00001bf0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00001c00: 2020 2020 2064 3d22 6d20 3533 2e30 3134       d="m 53.014
+00001c10: 3836 362c 3936 2e31 3330 3732 2037 322e  866,96.13072 72.
+00001c20: 3339 3232 3234 2c37 2e35 3539 3434 2035  392224,7.55944 5
+00001c30: 332e 3135 3531 342c 2d32 302e 3135 3834  3.15514,-20.1584
+00001c40: 3620 7a22 0a20 2020 2020 2020 2020 6964  6 z".         id
+00001c50: 3d22 7061 7468 3134 3535 3722 0a20 2020  ="path14557".   
+00001c60: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00001c70: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00001c80: 7265 3d22 3022 202f 3e0a 2020 2020 2020  re="0" />.      
+00001c90: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+00001ca0: 7479 6c65 3d22 6669 6c6c 3a23 3232 3334  tyle="fill:#2234
+00001cb0: 3765 3b66 696c 6c2d 6f70 6163 6974 793a  7e;fill-opacity:
+00001cc0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00001cd0: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00001ce0: 3035 3030 353b 7374 726f 6b65 2d6c 696e  05005;stroke-lin
+00001cf0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00001d00: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00001d10: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00001d20: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00001d30: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00001d40: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00001d50: 2020 2020 2064 3d22 6d20 3533 2e30 3134       d="m 53.014
+00001d60: 3836 362c 3936 2e31 3330 3732 2063 2031  866,96.13072 c 1
+00001d70: 2e36 3237 3832 352c 3133 2e39 3732 3532  .627825,13.97252
+00001d80: 202d 342e 3030 3637 3732 2c32 322e 3738   -4.006772,22.78
+00001d90: 3039 3320 2d36 2e35 3831 3130 392c 3333  093 -6.581109,33
+00001da0: 2e37 3635 3431 206c 2037 382e 3937 3333  .76541 l 78.9733
+00001db0: 3333 2c2d 3236 2e32 3035 3937 207a 220a  33,-26.20597 z".
+00001dc0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00001dd0: 6831 3435 3539 220a 2020 2020 2020 2020  h14559".        
+00001de0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+00001df0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+00001e00: 220a 2020 2020 2020 2020 2073 6f64 6970  ".         sodip
+00001e10: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+00001e20: 6363 6322 202f 3e0a 2020 2020 2020 3c70  ccc" />.      <p
+00001e30: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
+00001e40: 6c65 3d22 6669 6c6c 3a23 3038 3130 3639  le="fill:#081069
+00001e50: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00001e60: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00001e70: 7472 6f6b 652d 7769 6474 683a 312e 3035  troke-width:1.05
+00001e80: 3030 353b 7374 726f 6b65 2d6c 696e 6563  005;stroke-linec
+00001e90: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+00001ea0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00001eb0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00001ec0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00001ed0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+00001ee0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00001ef0: 2020 2064 3d22 4d20 3436 2e34 3333 3735     d="M 46.43375
+00001f00: 372c 3132 392e 3839 3631 3320 3130 312e  7,129.89613 101.
+00001f10: 3130 3736 2c31 3337 2e39 3539 3531 2031  1076,137.95951 1
+00001f20: 3738 2e35 3632 3233 2c38 332e 3533 3137  78.56223,83.5317
+00001f30: 205a 220a 2020 2020 2020 2020 2069 643d   Z".         id=
+00001f40: 2270 6174 6831 3435 3631 220a 2020 2020  "path14561".    
+00001f50: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+00001f60: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+00001f70: 653d 2230 2220 2f3e 0a20 2020 2020 203c  e="0" />.      <
+00001f80: 7061 7468 0a20 2020 2020 2020 2020 7374  path.         st
+00001f90: 796c 653d 2266 696c 6c3a 2330 3730 6532  yle="fill:#070e2
+00001fa0: 623b 6669 6c6c 2d6f 7061 6369 7479 3a31  b;fill-opacity:1
+00001fb0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00001fc0: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
+00001fd0: 3530 3035 3b73 7472 6f6b 652d 6c69 6e65  5005;stroke-line
+00001fe0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00001ff0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+00002000: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00002010: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00002020: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00002030: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00002040: 2020 2020 643d 226d 2031 3031 2e31 3037      d="m 101.107
+00002050: 362c 3133 372e 3935 3935 3120 3332 2e31  6,137.95951 32.1
+00002060: 3436 3139 2c34 322e 3038 3037 3920 2d31  4619,42.08079 -1
+00002070: 312e 3839 3636 322c 2d35 362e 3639 3536  1.89662,-56.6956
+00002080: 3620 7a22 0a20 2020 2020 2020 2020 6964  6 z".         id
+00002090: 3d22 7061 7468 3134 3536 3322 0a20 2020  ="path14563".   
+000020a0: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+000020b0: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+000020c0: 7265 3d22 3022 202f 3e0a 2020 2020 2020  re="0" />.      
+000020d0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+000020e0: 7479 6c65 3d22 6669 6c6c 3a23 3238 3364  tyle="fill:#283d
+000020f0: 3837 3b66 696c 6c2d 6f70 6163 6974 793a  87;fill-opacity:
+00002100: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00002110: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00002120: 3035 3030 353b 7374 726f 6b65 2d6c 696e  05005;stroke-lin
+00002130: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00002140: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00002150: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00002160: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00002170: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00002180: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00002190: 2020 2020 2064 3d22 6d20 3132 312e 3335       d="m 121.35
+000021a0: 3731 372c 3132 332e 3334 3436 3420 3131  717,123.34464 11
+000021b0: 2e38 3936 3632 2c35 362e 3639 3536 3620  .89662,56.69566 
+000021c0: 6320 362e 3135 3836 322c 2d35 302e 3936  c 6.15862,-50.96
+000021d0: 3637 3320 3237 2e38 3331 3437 2c2d 3639  673 27.83147,-69
+000021e0: 2e33 3238 3631 2034 352e 3330 3834 342c  .32861 45.30844,
+000021f0: 2d39 362e 3530 3836 207a 220a 2020 2020  -96.5086 z".    
+00002200: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00002210: 3635 220a 2020 2020 2020 2020 2069 6e6b  65".         ink
+00002220: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00002230: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+00002240: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00002250: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+00002260: 202f 3e0a 2020 2020 2020 3c65 6c6c 6970   />.      <ellip
+00002270: 7365 0a20 2020 2020 2020 2020 7374 796c  se.         styl
+00002280: 653d 2266 696c 6c3a 2330 3730 6532 623b  e="fill:#070e2b;
+00002290: 6669 6c6c 2d6f 7061 6369 7479 3a30 2e39  fill-opacity:0.9
+000022a0: 3930 3434 363b 7374 726f 6b65 3a23 6666  90446;stroke:#ff
+000022b0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+000022c0: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
+000022d0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+000022e0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+000022f0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+00002300: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+00002310: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00002320: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
+00002330: 220a 2020 2020 2020 2020 2063 783d 2232  ".         cx="2
+00002340: 302e 3930 3331 3138 220a 2020 2020 2020  0.903118".      
+00002350: 2020 2063 793d 2236 372e 3732 3135 3838     cy="67.721588
+00002360: 220a 2020 2020 2020 2020 2072 783d 2233  ".         rx="3
+00002370: 2e31 3536 3232 3634 220a 2020 2020 2020  .1562264".      
+00002380: 2020 2072 793d 2233 2e31 3432 3032 3422     ry="3.142024"
+00002390: 202f 3e0a 2020 2020 2020 3c65 6c6c 6970   />.      <ellip
+000023a0: 7365 0a20 2020 2020 2020 2020 7374 796c  se.         styl
+000023b0: 653d 2266 696c 6c3a 2332 3533 6137 643b  e="fill:#253a7d;
+000023c0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+000023d0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+000023e0: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+000023f0: 3035 3b73 7472 6f6b 652d 6d69 7465 726c  05;stroke-miterl
+00002400: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00002410: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00002420: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+00002430: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00002440: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
+00002450: 7061 7468 3134 3536 372d 3322 0a20 2020  path14567-3".   
+00002460: 2020 2020 2020 6378 3d22 3435 2e39 3235        cx="45.925
+00002470: 3834 3622 0a20 2020 2020 2020 2020 6379  846".         cy
+00002480: 3d22 3132 392e 3232 3538 3822 0a20 2020  ="129.22588".   
+00002490: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+000024a0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+000024b0: 783d 2232 2e33 3236 3937 3435 220a 2020  x="2.3269745".  
+000024c0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000024d0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+000024e0: 2d79 3d22 2d34 2e39 3738 3031 3633 220a  -y="-4.9780163".
+000024f0: 2020 2020 2020 2020 2072 783d 2233 2e31           rx="3.1
+00002500: 3536 3232 3634 220a 2020 2020 2020 2020  562264".        
+00002510: 2072 793d 2233 2e31 3432 3032 3422 202f   ry="3.142024" /
+00002520: 3e0a 2020 2020 2020 3c65 6c6c 6970 7365  >.      <ellipse
+00002530: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00002540: 2266 696c 6c3a 2332 3533 6137 643b 6669  "fill:#253a7d;fi
+00002550: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00002560: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00002570: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+00002580: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00002590: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+000025a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+000025b0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+000025c0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+000025d0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+000025e0: 7468 3134 3536 372d 332d 3722 0a20 2020  th14567-3-7".   
+000025f0: 2020 2020 2020 6378 3d22 3132 302e 3538        cx="120.58
+00002600: 3836 3222 0a20 2020 2020 2020 2020 6379  862".         cy
+00002610: 3d22 3130 332e 3839 3133 3922 0a20 2020  ="103.89139".   
+00002620: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+00002630: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+00002640: 783d 2232 2e33 3236 3937 3932 220a 2020  x="2.3269792".  
+00002650: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00002660: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+00002670: 2d79 3d22 2d34 2e39 3738 3032 3034 220a  -y="-4.9780204".
+00002680: 2020 2020 2020 2020 2072 783d 2233 2e31           rx="3.1
+00002690: 3536 3232 3634 220a 2020 2020 2020 2020  562264".        
+000026a0: 2072 793d 2233 2e31 3432 3032 3422 202f   ry="3.142024" /
+000026b0: 3e0a 2020 2020 2020 3c65 6c6c 6970 7365  >.      <ellipse
+000026c0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000026d0: 2266 696c 6c3a 2361 3861 3961 613b 6669  "fill:#a8a9aa;fi
+000026e0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+000026f0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00002700: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+00002710: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00002720: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00002730: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00002740: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+00002750: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00002760: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+00002770: 7468 3134 3536 372d 332d 3522 0a20 2020  th14567-3-5".   
+00002780: 2020 2020 2020 6378 3d22 3132 312e 3333        cx="121.33
+00002790: 3731 3422 0a20 2020 2020 2020 2020 6379  714".         cy
+000027a0: 3d22 3132 322e 3839 3232 3422 0a20 2020  ="122.89224".   
+000027b0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+000027c0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+000027d0: 783d 2232 2e33 3236 3936 3722 0a20 2020  x="2.326967".   
+000027e0: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+000027f0: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+00002800: 793d 222d 342e 3937 3830 3035 3922 0a20  y="-4.9780059". 
+00002810: 2020 2020 2020 2020 7278 3d22 332e 3135          rx="3.15
+00002820: 3632 3236 3422 0a20 2020 2020 2020 2020  62264".         
+00002830: 7279 3d22 332e 3134 3230 3234 2220 2f3e  ry="3.142024" />
+00002840: 0a20 2020 2020 203c 656c 6c69 7073 650a  .      <ellipse.
+00002850: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00002860: 6669 6c6c 3a23 6162 6161 3963 3b66 696c  fill:#abaa9c;fil
+00002870: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00002880: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00002890: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
+000028a0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+000028b0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+000028c0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+000028d0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+000028e0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+000028f0: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00002900: 6831 3435 3637 2d33 2d39 220a 2020 2020  h14567-3-9".    
+00002910: 2020 2020 2063 783d 2231 3031 2e38 3736       cx="101.876
+00002920: 3134 220a 2020 2020 2020 2020 2063 793d  14".         cy=
+00002930: 2231 3337 2e37 3934 3835 220a 2020 2020  "137.79485".    
+00002940: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+00002950: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
+00002960: 3d22 322e 3332 3639 3733 220a 2020 2020  ="2.326973".    
+00002970: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+00002980: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
+00002990: 3d22 2d34 2e39 3738 3032 3531 220a 2020  ="-4.9780251".  
+000029a0: 2020 2020 2020 2072 783d 2233 2e31 3536         rx="3.156
+000029b0: 3232 3634 220a 2020 2020 2020 2020 2072  2264".         r
+000029c0: 793d 2233 2e31 3432 3032 3422 202f 3e0a  y="3.142024" />.
+000029d0: 2020 2020 2020 3c65 6c6c 6970 7365 0a20        <ellipse. 
+000029e0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+000029f0: 696c 6c3a 2331 3132 3036 363b 6669 6c6c  ill:#112066;fill
+00002a00: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00002a10: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00002a20: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00002a30: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00002a40: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00002a50: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00002a60: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
+00002a70: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00002a80: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00002a90: 3134 3536 372d 332d 3222 0a20 2020 2020  14567-3-2".     
+00002aa0: 2020 2020 6378 3d22 3831 2e32 3932 3431      cx="81.29241
+00002ab0: 3922 0a20 2020 2020 2020 2020 6379 3d22  9".         cy="
+00002ac0: 3634 2e32 3133 3136 3522 0a20 2020 2020  64.213165".     
+00002ad0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
+00002ae0: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
+00002af0: 2233 2e35 3931 3336 3039 220a 2020 2020  "3.5913609".    
+00002b00: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+00002b10: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
+00002b20: 3d22 2d37 2e36 3832 3839 3536 220a 2020  ="-7.6828956".  
+00002b30: 2020 2020 2020 2072 783d 2234 2e38 3731         rx="4.871
+00002b40: 3139 3239 220a 2020 2020 2020 2020 2072  1929".         r
+00002b50: 793d 2234 2e38 3439 3237 3337 2220 2f3e  y="4.8492737" />
+00002b60: 0a20 2020 2020 203c 656c 6c69 7073 650a  .      <ellipse.
+00002b70: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00002b80: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
+00002b90: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
+00002ba0: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
+00002bb0: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
+00002bc0: 2e30 3530 3035 3b73 7472 6f6b 652d 6d69  .05005;stroke-mi
+00002bd0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00002be0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00002bf0: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
+00002c00: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
+00002c10: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+00002c20: 6964 3d22 7061 7468 3134 3536 372d 3222  id="path14567-2"
+00002c30: 0a20 2020 2020 2020 2020 6378 3d22 3130  .         cx="10
+00002c40: 372e 3637 3730 3222 0a20 2020 2020 2020  7.67702".       
+00002c50: 2020 6379 3d22 3639 2e36 3135 3335 3622    cy="69.615356"
+00002c60: 0a20 2020 2020 2020 2020 7278 3d22 332e  .         rx="3.
+00002c70: 3135 3632 3236 3422 0a20 2020 2020 2020  1562264".       
+00002c80: 2020 7279 3d22 332e 3134 3230 3234 2220    ry="3.142024" 
+00002c90: 2f3e 0a20 2020 2020 203c 656c 6c69 7073  />.      <ellips
+00002ca0: 650a 2020 2020 2020 2020 2073 7479 6c65  e.         style
+00002cb0: 3d22 6669 6c6c 3a23 6564 6630 6663 3b66  ="fill:#edf0fc;f
+00002cc0: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+00002cd0: 3034 3436 3b73 7472 6f6b 653a 2366 6666  0446;stroke:#fff
+00002ce0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00002cf0: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+00002d00: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00002d10: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00002d20: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+00002d30: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+00002d40: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00002d50: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+00002d60: 322d 3822 0a20 2020 2020 2020 2020 6378  2-8".         cx
+00002d70: 3d22 3533 2e30 3336 3537 3522 0a20 2020  ="53.036575".   
+00002d80: 2020 2020 2020 6379 3d22 3935 2e36 3934        cy="95.694
+00002d90: 3937 3722 0a20 2020 2020 2020 2020 7278  977".         rx
+00002da0: 3d22 332e 3135 3632 3236 3422 0a20 2020  ="3.1562264".   
+00002db0: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
+00002dc0: 3234 2220 2f3e 0a20 2020 2020 203c 7061  24" />.      <pa
+00002dd0: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
+00002de0: 653d 2266 696c 6c3a 2330 3030 3030 303b  e="fill:#000000;
+00002df0: 6669 6c6c 2d6f 7061 6369 7479 3a30 2e39  fill-opacity:0.9
+00002e00: 3938 3430 383b 7374 726f 6b65 3a23 3030  98408;stroke:#00
+00002e10: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
+00002e20: 683a 302e 3332 3335 3838 7078 3b73 7472  h:0.323588px;str
+00002e30: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00002e40: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00002e50: 3a6d 6974 6572 3b73 7472 6f6b 652d 6f70  :miter;stroke-op
+00002e60: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00002e70: 2020 643d 226d 2033 3138 2e37 3031 3333    d="m 318.70133
+00002e80: 2c37 322e 3730 3137 3220 3236 2e36 3034  ,72.70172 26.604
+00002e90: 3537 2c2d 382e 3738 3638 3320 2d32 382e  57,-8.78683 -28.
+00002ea0: 3338 3339 352c 2d31 2e34 3735 3836 2063  38395,-1.47586 c
+00002eb0: 2031 312e 3030 3532 362c 332e 3230 3436   11.00526,3.2046
+00002ec0: 3620 3131 2e30 3535 332c 332e 3337 3432  6 11.0553,3.3742
+00002ed0: 3720 312e 3737 3933 382c 3130 2e32 3632  7 1.77938,10.262
+00002ee0: 3639 207a 220a 2020 2020 2020 2020 2069  69 z".         i
+00002ef0: 643d 2270 6174 6831 3436 3537 2d39 220a  d="path14657-9".
+00002f00: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00002f10: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+00002f20: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+00002f30: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+00002f40: 7479 7065 733d 2263 6363 6322 202f 3e0a  types="cccc" />.
+00002f50: 2020 2020 2020 3c65 6c6c 6970 7365 0a20        <ellipse. 
+00002f60: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00002f70: 696c 6c3a 2365 6466 3066 633b 6669 6c6c  ill:#edf0fc;fill
+00002f80: 2d6f 7061 6369 7479 3a30 2e39 3930 3434  -opacity:0.99044
+00002f90: 363b 7374 726f 6b65 3a23 6666 6666 6666  6;stroke:#ffffff
+00002fa0: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00002fb0: 3939 3539 383b 7374 726f 6b65 2d6d 6974  99598;stroke-mit
+00002fc0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00002fd0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00002fe0: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00002ff0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+00003000: 7479 3a31 220a 2020 2020 2020 2020 2069  ty:1".         i
+00003010: 643d 2270 6174 6831 3435 3637 2d32 2d37  d="path14567-2-7
+00003020: 220a 2020 2020 2020 2020 2063 783d 2231  ".         cx="1
+00003030: 3737 2e34 3734 3536 220a 2020 2020 2020  77.47456".      
+00003040: 2020 2063 793d 2238 342e 3333 3137 3236     cy="84.331726
+00003050: 220a 2020 2020 2020 2020 2072 783d 2235  ".         rx="5
+00003060: 2e39 3939 3532 3232 220a 2020 2020 2020  .9995222".      
+00003070: 2020 2072 793d 2235 2e39 3732 3532 3536     ry="5.9725256
+00003080: 2220 2f3e 0a20 2020 2020 203c 7465 7874  " />.      <text
+00003090: 0a20 2020 2020 2020 2020 786d 6c3a 7370  .         xml:sp
+000030a0: 6163 653d 2270 7265 7365 7276 6522 0a20  ace="preserve". 
+000030b0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+000030c0: 6f6e 742d 7374 796c 653a 6e6f 726d 616c  ont-style:normal
+000030d0: 3b66 6f6e 742d 7765 6967 6874 3a6e 6f72  ;font-weight:nor
+000030e0: 6d61 6c3b 666f 6e74 2d73 697a 653a 352e  mal;font-size:5.
+000030f0: 3837 3239 3170 783b 6c69 6e65 2d68 6569  87291px;line-hei
+00003100: 6768 743a 312e 3235 3b66 6f6e 742d 6661  ght:1.25;font-fa
+00003110: 6d69 6c79 3a73 616e 732d 7365 7269 663b  mily:sans-serif;
+00003120: 6c65 7474 6572 2d73 7061 6369 6e67 3a30  letter-spacing:0
+00003130: 7078 3b77 6f72 642d 7370 6163 696e 673a  px;word-spacing:
+00003140: 3070 783b 6669 6c6c 3a23 6666 6666 6666  0px;fill:#ffffff
+00003150: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00003160: 7374 726f 6b65 3a6e 6f6e 653b 7374 726f  stroke:none;stro
+00003170: 6b65 2d77 6964 7468 3a30 2e34 3030 3432  ke-width:0.40042
+00003180: 353b 6669 6c74 6572 3a75 726c 2823 6669  5;filter:url(#fi
+00003190: 6c74 6572 3135 3035 3129 220a 2020 2020  lter15051)".    
+000031a0: 2020 2020 2078 3d22 3737 2e36 3934 3839       x="77.69489
+000031b0: 3322 0a20 2020 2020 2020 2020 793d 2239  3".         y="9
+000031c0: 312e 3938 3834 3439 220a 2020 2020 2020  1.988449".      
+000031d0: 2020 2069 643d 2274 6578 7431 3436 3931     id="text14691
+000031e0: 2d36 220a 2020 2020 2020 2020 2074 7261  -6".         tra
+000031f0: 6e73 666f 726d 3d22 6d61 7472 6978 2832  nsform="matrix(2
+00003200: 2e37 3531 3139 3139 2c30 2c30 2c32 2e37  .7511919,0,0,2.7
+00003210: 3338 3831 322c 2d37 352e 3937 3636 3936  38812,-75.976696
+00003220: 2c2d 3130 382e 3038 3836 3629 223e 3c74  ,-108.08866)"><t
+00003230: 7370 616e 0a20 2020 2020 2020 2020 2020  span.           
+00003240: 736f 6469 706f 6469 3a72 6f6c 653d 226c  sodipodi:role="l
+00003250: 696e 6522 0a20 2020 2020 2020 2020 2020  ine".           
+00003260: 6964 3d22 7473 7061 6e31 3436 3839 2d32  id="tspan14689-2
+00003270: 220a 2020 2020 2020 2020 2020 2078 3d22  ".           x="
+00003280: 3737 2e36 3934 3839 3322 0a20 2020 2020  77.694893".     
+00003290: 2020 2020 2020 793d 2239 312e 3938 3834        y="91.9884
+000032a0: 3439 220a 2020 2020 2020 2020 2020 2073  49".           s
+000032b0: 7479 6c65 3d22 666f 6e74 2d73 7479 6c65  tyle="font-style
+000032c0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d76 6172  :normal;font-var
+000032d0: 6961 6e74 3a6e 6f72 6d61 6c3b 666f 6e74  iant:normal;font
+000032e0: 2d77 6569 6768 743a 6e6f 726d 616c 3b66  -weight:normal;f
+000032f0: 6f6e 742d 7374 7265 7463 683a 6e6f 726d  ont-stretch:norm
+00003300: 616c 3b66 6f6e 742d 7369 7a65 3a32 312e  al;font-size:21.
+00003310: 3335 3670 783b 666f 6e74 2d66 616d 696c  356px;font-famil
+00003320: 793a 496d 7061 6374 3b2d 696e 6b73 6361  y:Impact;-inksca
+00003330: 7065 2d66 6f6e 742d 7370 6563 6966 6963  pe-font-specific
+00003340: 6174 696f 6e3a 496d 7061 6374 3b66 696c  ation:Impact;fil
+00003350: 6c3a 2366 6666 6666 663b 6669 6c6c 2d6f  l:#ffffff;fill-o
+00003360: 7061 6369 7479 3a31 3b73 7472 6f6b 652d  pacity:1;stroke-
+00003370: 7769 6474 683a 302e 3430 3034 3235 223e  width:0.400425">
+00003380: 5361 656e 6f70 793c 2f74 7370 616e 3e3c  Saenopy</tspan><
+00003390: 2f74 6578 743e 0a20 2020 2020 203c 7465  /text>.      <te
+000033a0: 7874 0a20 2020 2020 2020 2020 786d 6c3a  xt.         xml:
+000033b0: 7370 6163 653d 2270 7265 7365 7276 6522  space="preserve"
+000033c0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000033d0: 2266 6f6e 742d 7374 796c 653a 6e6f 726d  "font-style:norm
+000033e0: 616c 3b66 6f6e 742d 7765 6967 6874 3a6e  al;font-weight:n
+000033f0: 6f72 6d61 6c3b 666f 6e74 2d73 697a 653a  ormal;font-size:
+00003400: 3136 2e31 3231 3170 783b 6c69 6e65 2d68  16.1211px;line-h
+00003410: 6569 6768 743a 312e 3235 3b66 6f6e 742d  eight:1.25;font-
+00003420: 6661 6d69 6c79 3a73 616e 732d 7365 7269  family:sans-seri
+00003430: 663b 6c65 7474 6572 2d73 7061 6369 6e67  f;letter-spacing
+00003440: 3a30 7078 3b77 6f72 642d 7370 6163 696e  :0px;word-spacin
+00003450: 673a 3070 783b 6669 6c6c 3a23 3030 3030  g:0px;fill:#0000
+00003460: 3030 3b66 696c 6c2d 6f70 6163 6974 793a  00;fill-opacity:
+00003470: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
+00003480: 726f 6b65 2d77 6964 7468 3a31 2e30 3939  roke-width:1.099
+00003490: 3137 220a 2020 2020 2020 2020 2078 3d22  17".         x="
+000034a0: 3133 352e 3437 3930 3622 0a20 2020 2020  135.47906".     
+000034b0: 2020 2020 793d 2231 3336 2e33 3837 3722      y="136.3877"
+000034c0: 0a20 2020 2020 2020 2020 6964 3d22 7465  .         id="te
+000034d0: 7874 3134 3639 3122 0a20 2020 2020 2020  xt14691".       
+000034e0: 2020 7472 616e 7366 6f72 6d3d 2273 6361    transform="sca
+000034f0: 6c65 2831 2e30 3032 3235 3735 2c30 2e39  le(1.0022575,0.9
+00003500: 3937 3734 3735 3829 223e 3c74 7370 616e  9774758)"><tspan
+00003510: 0a20 2020 2020 2020 2020 2020 736f 6469  .           sodi
+00003520: 706f 6469 3a72 6f6c 653d 226c 696e 6522  podi:role="line"
+00003530: 0a20 2020 2020 2020 2020 2020 6964 3d22  .           id="
+00003540: 7473 7061 6e31 3436 3839 220a 2020 2020  tspan14689".    
+00003550: 2020 2020 2020 2078 3d22 3133 352e 3437         x="135.47
+00003560: 3930 3622 0a20 2020 2020 2020 2020 2020  906".           
+00003570: 793d 2231 3336 2e33 3837 3722 0a20 2020  y="136.3877".   
+00003580: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00003590: 6f6e 742d 7374 796c 653a 6e6f 726d 616c  ont-style:normal
+000035a0: 3b66 6f6e 742d 7661 7269 616e 743a 6e6f  ;font-variant:no
+000035b0: 726d 616c 3b66 6f6e 742d 7765 6967 6874  rmal;font-weight
+000035c0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d73 7472  :normal;font-str
+000035d0: 6574 6368 3a6e 6f72 6d61 6c3b 666f 6e74  etch:normal;font
+000035e0: 2d73 697a 653a 3538 2e36 3232 3170 783b  -size:58.6221px;
+000035f0: 666f 6e74 2d66 616d 696c 793a 2754 6c77  font-family:'Tlw
+00003600: 6720 5479 7069 7374 273b 2d69 6e6b 7363  g Typist';-inksc
+00003610: 6170 652d 666f 6e74 2d73 7065 6369 6669  ape-font-specifi
+00003620: 6361 7469 6f6e 3a27 546c 7767 2054 7970  cation:'Tlwg Typ
+00003630: 6973 7427 3b73 7472 6f6b 652d 7769 6474  ist';stroke-widt
+00003640: 683a 312e 3039 3931 3722 3e53 6165 6e6f  h:1.09917">Saeno
+00003650: 7079 3c2f 7473 7061 6e3e 3c2f 7465 7874  py</tspan></text
+00003660: 3e0a 2020 2020 2020 3c74 6578 740a 2020  >.      <text.  
+00003670: 2020 2020 2020 2078 6d6c 3a73 7061 6365         xml:space
+00003680: 3d22 7072 6573 6572 7665 220a 2020 2020  ="preserve".    
+00003690: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
+000036a0: 2d73 7479 6c65 3a6e 6f72 6d61 6c3b 666f  -style:normal;fo
+000036b0: 6e74 2d77 6569 6768 743a 6e6f 726d 616c  nt-weight:normal
+000036c0: 3b66 6f6e 742d 7369 7a65 3a31 362e 3132  ;font-size:16.12
+000036d0: 3131 7078 3b6c 696e 652d 6865 6967 6874  11px;line-height
+000036e0: 3a31 2e32 353b 666f 6e74 2d66 616d 696c  :1.25;font-famil
+000036f0: 793a 7361 6e73 2d73 6572 6966 3b6c 6574  y:sans-serif;let
+00003700: 7465 722d 7370 6163 696e 673a 3070 783b  ter-spacing:0px;
+00003710: 776f 7264 2d73 7061 6369 6e67 3a30 7078  word-spacing:0px
+00003720: 3b66 696c 6c3a 2330 3030 3030 303b 6669  ;fill:#000000;fi
+00003730: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00003740: 6f6b 653a 6e6f 6e65 3b73 7472 6f6b 652d  oke:none;stroke-
+00003750: 7769 6474 683a 312e 3039 3931 3722 0a20  width:1.09917". 
+00003760: 2020 2020 2020 2020 783d 2231 3335 2e34          x="135.4
+00003770: 3739 3036 220a 2020 2020 2020 2020 2079  7906".         y
+00003780: 3d22 3133 362e 3338 3737 220a 2020 2020  ="136.3877".    
+00003790: 2020 2020 2069 643d 2274 6578 7431 3233       id="text123
+000037a0: 3338 220a 2020 2020 2020 2020 2074 7261  38".         tra
+000037b0: 6e73 666f 726d 3d22 7363 616c 6528 312e  nsform="scale(1.
+000037c0: 3030 3232 3537 352c 302e 3939 3737 3437  0022575,0.997747
+000037d0: 3538 2922 3e3c 7473 7061 6e0a 2020 2020  58)"><tspan.    
+000037e0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000037f0: 726f 6c65 3d22 6c69 6e65 220a 2020 2020  role="line".    
+00003800: 2020 2020 2020 2069 643d 2274 7370 616e         id="tspan
+00003810: 3132 3333 3622 0a20 2020 2020 2020 2020  12336".         
+00003820: 2020 783d 2231 3335 2e34 3739 3036 220a    x="135.47906".
+00003830: 2020 2020 2020 2020 2020 2079 3d22 3133             y="13
+00003840: 362e 3338 3737 220a 2020 2020 2020 2020  6.3877".        
+00003850: 2020 2073 7479 6c65 3d22 666f 6e74 2d73     style="font-s
+00003860: 7479 6c65 3a6e 6f72 6d61 6c3b 666f 6e74  tyle:normal;font
+00003870: 2d76 6172 6961 6e74 3a6e 6f72 6d61 6c3b  -variant:normal;
+00003880: 666f 6e74 2d77 6569 6768 743a 6e6f 726d  font-weight:norm
+00003890: 616c 3b66 6f6e 742d 7374 7265 7463 683a  al;font-stretch:
+000038a0: 6e6f 726d 616c 3b66 6f6e 742d 7369 7a65  normal;font-size
+000038b0: 3a35 382e 3632 3231 7078 3b66 6f6e 742d  :58.6221px;font-
+000038c0: 6661 6d69 6c79 3a27 546c 7767 2054 7970  family:'Tlwg Typ
+000038d0: 6973 7427 3b2d 696e 6b73 6361 7065 2d66  ist';-inkscape-f
+000038e0: 6f6e 742d 7370 6563 6966 6963 6174 696f  ont-specificatio
+000038f0: 6e3a 2754 6c77 6720 5479 7069 7374 273b  n:'Tlwg Typist';
+00003900: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
+00003910: 3939 3137 223e 5361 656e 6f70 793c 2f74  9917">Saenopy</t
+00003920: 7370 616e 3e3c 2f74 6578 743e 0a20 2020  span></text>.   
+00003930: 203c 2f67 3e0a 2020 2020 3c67 0a20 2020   </g>.    <g.   
+00003940: 2020 2020 6964 3d22 6c6f 676f 5f6e 6f72      id="logo_nor
+00003950: 6d61 6c2d 3522 0a20 2020 2020 2020 7472  mal-5".       tr
+00003960: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
+00003970: 7465 2831 2e33 3532 3730 3936 2c2d 3234  te(1.3527096,-24
+00003980: 372e 3731 3439 3429 223e 0a20 2020 2020  7.71494)">.     
+00003990: 203c 7265 6374 0a20 2020 2020 2020 2020   <rect.         
+000039a0: 7374 796c 653d 2266 696c 6c3a 2366 6666  style="fill:#fff
+000039b0: 6666 663b 6669 6c6c 2d6f 7061 6369 7479  fff;fill-opacity
+000039c0: 3a30 2e30 3230 3039 3731 3b73 7472 6f6b  :0.0200971;strok
+000039d0: 653a 6e6f 6e65 3b73 7472 6f6b 652d 7769  e:none;stroke-wi
+000039e0: 6474 683a 352e 3038 3437 363b 7374 726f  dth:5.08476;stro
+000039f0: 6b65 2d6c 696e 6563 6170 3a72 6f75 6e64  ke-linecap:round
+00003a00: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00003a10: 3a72 6f75 6e64 220a 2020 2020 2020 2020  :round".        
+00003a20: 2069 643d 2272 6563 7437 3036 2d33 220a   id="rect706-3".
+00003a30: 2020 2020 2020 2020 2077 6964 7468 3d22           width="
+00003a40: 3430 3022 0a20 2020 2020 2020 2020 6865  400".         he
+00003a50: 6967 6874 3d22 3230 3022 0a20 2020 2020  ight="200".     
+00003a60: 2020 2020 783d 222d 362e 3639 3635 3133      x="-6.696513
+00003a70: 3165 2d30 3622 0a20 2020 2020 2020 2020  1e-06".         
+00003a80: 793d 222d 312e 3835 3230 3631 3165 2d30  y="-1.8520611e-0
+00003a90: 3622 0a20 2020 2020 2020 2020 7279 3d22  6".         ry="
+00003aa0: 3022 202f 3e0a 2020 2020 2020 3c70 6174  0" />.      <pat
+00003ab0: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00003ac0: 3d22 6669 6c6c 3a23 3030 3030 3030 3b66  ="fill:#000000;f
+00003ad0: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+00003ae0: 3834 3038 3b73 7472 6f6b 653a 2330 3030  8408;stroke:#000
+00003af0: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+00003b00: 3a30 2e35 3030 3032 3270 783b 7374 726f  :0.500022px;stro
+00003b10: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00003b20: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00003b30: 6d69 7465 723b 7374 726f 6b65 2d6f 7061  miter;stroke-opa
+00003b40: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+00003b50: 2064 3d22 6d20 3233 382e 3031 3433 2c37   d="m 238.0143,7
+00003b60: 392e 3530 3738 3733 2031 302e 3534 3533  9.507873 10.5453
+00003b70: 332c 2d33 2e38 3833 3335 3920 2d31 312e  3,-3.883359 -11.
+00003b80: 3436 3939 382c 312e 3138 3936 3532 207a  46998,1.189652 z
+00003b90: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00003ba0: 6174 6831 3436 3537 2d35 220a 2020 2020  ath14657-5".    
+00003bb0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+00003bc0: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+00003bd0: 653d 2230 220a 2020 2020 2020 2020 2073  e="0".         s
+00003be0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00003bf0: 733d 2263 6363 6322 202f 3e0a 2020 2020  s="cccc" />.    
+00003c00: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00003c10: 2073 7479 6c65 3d22 6669 6c6c 3a23 3365   style="fill:#3e
+00003c20: 3462 3737 3b66 696c 6c2d 6f70 6163 6974  4b77;fill-opacit
+00003c30: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00003c40: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00003c50: 312e 3035 3030 353b 7374 726f 6b65 2d6c  1.05005;stroke-l
+00003c60: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00003c70: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00003c80: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+00003c90: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00003ca0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00003cb0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00003cc0: 2020 2020 2020 2064 3d22 4d20 3139 2e36         d="M 19.6
+00003cd0: 3033 3037 2c36 372e 3635 3639 2038 362e  0307,67.6569 86.
+00003ce0: 3436 3236 3731 2c36 342e 3431 3035 3333  462671,64.410533
+00003cf0: 2031 3231 2e31 3034 3035 2c32 302e 3238   121.10405,20.28
+00003d00: 3435 3420 4320 3635 2e32 3533 3138 392c  454 C 65.253189,
+00003d10: 3437 2e32 3333 3831 3120 3435 2e32 3435  47.233811 45.245
+00003d20: 3630 392c 3538 2e34 3037 3633 3420 3139  609,58.407634 19
+00003d30: 2e36 3033 3037 2c36 372e 3635 3639 205a  .60307,67.6569 Z
+00003d40: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00003d50: 6174 6831 3435 3437 2d36 220a 2020 2020  ath14547-6".    
+00003d60: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+00003d70: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+00003d80: 653d 2230 220a 2020 2020 2020 2020 2073  e="0".         s
+00003d90: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00003da0: 733d 2263 6363 6322 202f 3e0a 2020 2020  s="cccc" />.    
+00003db0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00003dc0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3163   style="fill:#1c
+00003dd0: 3263 3638 3b66 696c 6c2d 6f70 6163 6974  2c68;fill-opacit
+00003de0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00003df0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00003e00: 312e 3035 3030 353b 7374 726f 6b65 2d6c  1.05005;stroke-l
+00003e10: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00003e20: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00003e30: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+00003e40: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00003e50: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00003e60: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00003e70: 2020 2020 2020 2064 3d22 4d20 3836 2e36         d="M 86.6
+00003e80: 3737 3239 382c 3634 2e35 3035 3435 3620  77298,64.505456 
+00003e90: 3133 322e 3739 3134 342c 3731 2e31 3237  132.79144,71.127
+00003ea0: 3838 3420 3132 312e 3130 3430 352c 3230  884 121.10405,20
+00003eb0: 2e32 3834 3534 205a 220a 2020 2020 2020  .28454 Z".      
+00003ec0: 2020 2069 643d 2270 6174 6831 3435 3439     id="path14549
+00003ed0: 2d32 220a 2020 2020 2020 2020 2069 6e6b  -2".         ink
+00003ee0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00003ef0: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+00003f00: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00003f10: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+00003f20: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00003f30: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00003f40: 6669 6c6c 3a23 3036 3035 3038 3b66 696c  fill:#060508;fil
+00003f50: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00003f60: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00003f70: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
+00003f80: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00003f90: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00003fa0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00003fb0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00003fc0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00003fd0: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00003fe0: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
+00003ff0: 3d22 6d20 3133 322e 3132 3534 372c 3639  ="m 132.12547,69
+00004000: 2e30 3031 3837 3820 3131 312e 3237 372c  .001878 111.277,
+00004010: 382e 3035 3433 3634 2043 2032 3135 2e36  8.054364 C 215.6
+00004020: 3835 3635 2c36 322e 3436 3935 3132 2031  8565,62.469512 1
+00004030: 3631 2e32 3733 3238 2c33 382e 3732 3039  61.27328,38.7209
+00004040: 3438 2031 3231 2e31 3034 3035 2c32 302e  48 121.10405,20.
+00004050: 3238 3435 3420 5a22 0a20 2020 2020 2020  28454 Z".       
+00004060: 2020 6964 3d22 7061 7468 3134 3535 312d    id="path14551-
+00004070: 3922 0a20 2020 2020 2020 2020 696e 6b73  9".         inks
+00004080: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+00004090: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+000040a0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+000040b0: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
+000040c0: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+000040d0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+000040e0: 696c 6c3a 2332 3733 3737 333b 6669 6c6c  ill:#273773;fill
+000040f0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00004100: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00004110: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00004120: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00004130: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00004140: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00004150: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00004160: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00004170: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00004180: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
+00004190: 226d 2031 392e 3630 3330 372c 3637 2e36  "m 19.60307,67.6
+000041a0: 3536 3920 6320 362e 3434 3538 372c 3131  569 c 6.44587,11
+000041b0: 2e34 3536 3733 3320 392e 3839 3434 3632  .456733 9.894462
+000041c0: 2c31 372e 3732 3835 3538 2031 352e 3336  ,17.728558 15.36
+000041d0: 3832 3239 2c33 312e 3336 3437 3337 204c  8229,31.364737 L
+000041e0: 2038 362e 3635 3634 3739 2c36 342e 3439   86.656479,64.49
+000041f0: 3837 3920 5a22 0a20 2020 2020 2020 2020  879 Z".         
+00004200: 6964 3d22 7061 7468 3134 3535 332d 3122  id="path14553-1"
+00004210: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00004220: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+00004230: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+00004240: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00004250: 6574 7970 6573 3d22 6363 6363 2220 2f3e  etypes="cccc" />
+00004260: 0a20 2020 2020 203c 7061 7468 0a20 2020  .      <path.   
+00004270: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00004280: 6c3a 2331 3432 3637 323b 6669 6c6c 2d6f  l:#142672;fill-o
+00004290: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+000042a0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+000042b0: 6964 7468 3a31 2e30 3530 3035 3b73 7472  idth:1.05005;str
+000042c0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+000042d0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+000042e0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+000042f0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00004300: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00004310: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00004320: 3122 0a20 2020 2020 2020 2020 643d 224d  1".         d="M
+00004330: 2033 342e 3936 3336 3239 2c39 382e 3634   34.963629,98.64
+00004340: 3131 3737 2032 3433 2e34 3138 3634 2c37  1177 243.41864,7
+00004350: 372e 3031 3431 3137 2038 362e 3931 3531  7.014117 86.9151
+00004360: 3735 2c36 342e 3336 3837 3236 205a 220a  75,64.368726 Z".
+00004370: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00004380: 6831 3435 3535 2d32 220a 2020 2020 2020  h14555-2".      
+00004390: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+000043a0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+000043b0: 2230 220a 2020 2020 2020 2020 2073 6f64  "0".         sod
+000043c0: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+000043d0: 2263 6363 6322 202f 3e0a 2020 2020 2020  "cccc" />.      
+000043e0: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+000043f0: 7479 6c65 3d22 6669 6c6c 3a23 3534 3636  tyle="fill:#5466
+00004400: 3863 3b66 696c 6c2d 6f70 6163 6974 793a  8c;fill-opacity:
+00004410: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00004420: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00004430: 3035 3030 353b 7374 726f 6b65 2d6c 696e  05005;stroke-lin
+00004440: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+00004450: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+00004460: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00004470: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00004480: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00004490: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+000044a0: 2020 2020 2064 3d22 4d20 3334 2e36 3336       d="M 34.636
+000044b0: 3035 342c 3939 2e30 3035 3536 3820 3133  054,99.005568 13
+000044c0: 332e 3236 3733 372c 3130 352e 3738 3737  3.26737,105.7877
+000044d0: 2032 3433 2e39 3338 3133 2c37 372e 3431   243.93813,77.41
+000044e0: 3430 3234 205a 220a 2020 2020 2020 2020  4024 Z".        
+000044f0: 2069 643d 2270 6174 6831 3435 3537 2d37   id="path14557-7
+00004500: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00004510: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00004520: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00004530: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00004540: 6465 7479 7065 733d 2263 6363 6322 202f  detypes="cccc" /
+00004550: 3e0a 2020 2020 2020 3c70 6174 680a 2020  >.      <path.  
+00004560: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00004570: 6c6c 3a23 3232 3334 3765 3b66 696c 6c2d  ll:#22347e;fill-
+00004580: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00004590: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+000045a0: 7769 6474 683a 312e 3035 3030 353b 7374  width:1.05005;st
+000045b0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+000045c0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+000045d0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+000045e0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+000045f0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+00004600: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+00004610: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
+00004620: 6d20 3335 2e32 3138 3738 322c 3938 2e37  m 35.218782,98.7
+00004630: 3433 3830 3720 6320 352e 3036 3536 3931  43807 c 5.065691
+00004640: 2c31 342e 3438 3336 3533 2035 2e38 3038  ,14.483653 5.808
+00004650: 3237 312c 3138 2e35 3237 3337 3320 3131  271,18.527373 11
+00004660: 2e32 3134 3937 352c 3331 2e31 3532 3332  .214975,31.15232
+00004670: 3320 6c20 3837 2e33 3633 3931 332c 2d32  3 l 87.363913,-2
+00004680: 332e 3438 3630 3720 7a22 0a20 2020 2020  3.48607 z".     
+00004690: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
+000046a0: 392d 3022 0a20 2020 2020 2020 2020 696e  9-0".         in
+000046b0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+000046c0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+000046d0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+000046e0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+000046f0: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+00004700: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00004710: 2266 696c 6c3a 2330 3831 3036 393b 6669  "fill:#081069;fi
+00004720: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00004730: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00004740: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+00004750: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00004760: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00004770: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00004780: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00004790: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+000047a0: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+000047b0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+000047c0: 643d 224d 2034 362e 3433 3337 3537 2c31  d="M 46.433757,1
+000047d0: 3239 2e38 3936 3133 2039 302e 3337 3630  29.89613 90.3760
+000047e0: 3533 2c31 3439 2e38 3732 3939 2032 3433  53,149.87299 243
+000047f0: 2e32 3437 3131 2c37 362e 3833 3839 3237  .24711,76.838927
+00004800: 205a 220a 2020 2020 2020 2020 2069 643d   Z".         id=
+00004810: 2270 6174 6831 3435 3631 2d39 3322 0a20  "path14561-93". 
+00004820: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00004830: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+00004840: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
+00004850: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+00004860: 7970 6573 3d22 6363 6363 2220 2f3e 0a20  ypes="cccc" />. 
+00004870: 2020 2020 203c 7061 7468 0a20 2020 2020       <path.     
+00004880: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00004890: 2330 3730 6532 623b 6669 6c6c 2d6f 7061  #070e2b;fill-opa
+000048a0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+000048b0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+000048c0: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
+000048d0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+000048e0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+000048f0: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00004900: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00004910: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00004920: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00004930: 0a20 2020 2020 2020 2020 643d 226d 2039  .         d="m 9
+00004940: 312e 3934 3137 3339 2c31 3439 2e38 3932  1.941739,149.892
+00004950: 3431 2034 312e 3331 3230 3531 2c33 302e  41 41.312051,30.
+00004960: 3134 3738 3920 342e 3534 3532 382c 2d36  14789 4.54528,-6
+00004970: 312e 3036 3932 3320 7a22 0a20 2020 2020  1.06923 z".     
+00004980: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+00004990: 332d 3622 0a20 2020 2020 2020 2020 696e  3-6".         in
+000049a0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+000049b0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+000049c0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+000049d0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+000049e0: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+000049f0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+00004a00: 2266 696c 6c3a 2332 3833 6438 373b 6669  "fill:#283d87;fi
+00004a10: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00004a20: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00004a30: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+00004a40: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00004a50: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00004a60: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00004a70: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00004a80: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00004a90: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00004aa0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+00004ab0: 643d 226d 2031 3337 2e38 3330 3235 2c31  d="m 137.83025,1
+00004ac0: 3138 2e37 3633 3638 202d 342e 3537 3634  18.76368 -4.5764
+00004ad0: 362c 3631 2e32 3736 3632 2063 2034 382e  6,61.27662 c 48.
+00004ae0: 3531 3332 392c 2d34 382e 3931 3138 3620  51329,-48.91186 
+00004af0: 3830 2e31 3632 2c2d 3739 2e36 3133 3033  80.162,-79.61303
+00004b00: 2031 3039 2e34 3533 3038 2c2d 3130 332e   109.45308,-103.
+00004b10: 3335 3130 3333 207a 220a 2020 2020 2020  351033 z".      
+00004b20: 2020 2069 643d 2270 6174 6831 3435 3635     id="path14565
+00004b30: 2d30 220a 2020 2020 2020 2020 2069 6e6b  -0".         ink
+00004b40: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00004b50: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+00004b60: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00004b70: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+00004b80: 202f 3e0a 2020 2020 2020 3c65 6c6c 6970   />.      <ellip
+00004b90: 7365 0a20 2020 2020 2020 2020 7374 796c  se.         styl
+00004ba0: 653d 2266 696c 6c3a 2330 3730 6532 623b  e="fill:#070e2b;
+00004bb0: 6669 6c6c 2d6f 7061 6369 7479 3a30 2e39  fill-opacity:0.9
+00004bc0: 3930 3434 363b 7374 726f 6b65 3a23 6666  90446;stroke:#ff
+00004bd0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+00004be0: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
+00004bf0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00004c00: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00004c10: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+00004c20: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+00004c30: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00004c40: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
+00004c50: 2d36 3222 0a20 2020 2020 2020 2020 6378  -62".         cx
+00004c60: 3d22 3230 2e39 3033 3131 3822 0a20 2020  ="20.903118".   
+00004c70: 2020 2020 2020 6379 3d22 3637 2e37 3231        cy="67.721
+00004c80: 3538 3822 0a20 2020 2020 2020 2020 7278  588".         rx
+00004c90: 3d22 332e 3135 3632 3236 3422 0a20 2020  ="3.1562264".   
+00004ca0: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
+00004cb0: 3234 2220 2f3e 0a20 2020 2020 203c 656c  24" />.      <el
+00004cc0: 6c69 7073 650a 2020 2020 2020 2020 2073  lipse.         s
+00004cd0: 7479 6c65 3d22 6669 6c6c 3a23 3235 3361  tyle="fill:#253a
+00004ce0: 3764 3b66 696c 6c2d 6f70 6163 6974 793a  7d;fill-opacity:
+00004cf0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00004d00: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00004d10: 3035 3030 353b 7374 726f 6b65 2d6d 6974  05005;stroke-mit
+00004d20: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00004d30: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00004d40: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00004d50: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+00004d60: 7479 3a31 220a 2020 2020 2020 2020 2069  ty:1".         i
+00004d70: 643d 2270 6174 6831 3435 3637 2d33 2d36  d="path14567-3-6
+00004d80: 3122 0a20 2020 2020 2020 2020 6378 3d22  1".         cx="
+00004d90: 3435 2e39 3235 3834 3622 0a20 2020 2020  45.925846".     
+00004da0: 2020 2020 6379 3d22 3132 392e 3232 3538      cy="129.2258
+00004db0: 3822 0a20 2020 2020 2020 2020 696e 6b73  8".         inks
+00004dc0: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
+00004dd0: 656e 7465 722d 783d 2232 2e33 3236 3937  enter-x="2.32697
+00004de0: 3435 220a 2020 2020 2020 2020 2069 6e6b  45".         ink
+00004df0: 7363 6170 653a 7472 616e 7366 6f72 6d2d  scape:transform-
+00004e00: 6365 6e74 6572 2d79 3d22 2d34 2e39 3738  center-y="-4.978
+00004e10: 3031 3633 220a 2020 2020 2020 2020 2072  0163".         r
+00004e20: 783d 2233 2e31 3536 3232 3634 220a 2020  x="3.1562264".  
+00004e30: 2020 2020 2020 2072 793d 2233 2e31 3432         ry="3.142
+00004e40: 3032 3422 202f 3e0a 2020 2020 2020 3c65  024" />.      <e
+00004e50: 6c6c 6970 7365 0a20 2020 2020 2020 2020  llipse.         
+00004e60: 7374 796c 653d 2266 696c 6c3a 2332 3533  style="fill:#253
+00004e70: 6137 643b 6669 6c6c 2d6f 7061 6369 7479  a7d;fill-opacity
+00004e80: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00004e90: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
+00004ea0: 2e30 3530 3035 3b73 7472 6f6b 652d 6d69  .05005;stroke-mi
+00004eb0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00004ec0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00004ed0: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
+00004ee0: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
+00004ef0: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+00004f00: 6964 3d22 7061 7468 3134 3536 372d 332d  id="path14567-3-
+00004f10: 372d 3822 0a20 2020 2020 2020 2020 6378  7-8".         cx
+00004f20: 3d22 3133 322e 3933 3534 3122 0a20 2020  ="132.93541".   
+00004f30: 2020 2020 2020 6379 3d22 3130 352e 3634        cy="105.64
+00004f40: 3130 3522 0a20 2020 2020 2020 2020 696e  105".         in
+00004f50: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
+00004f60: 2d63 656e 7465 722d 783d 2232 2e33 3236  -center-x="2.326
+00004f70: 3937 3932 220a 2020 2020 2020 2020 2069  9792".         i
+00004f80: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00004f90: 6d2d 6365 6e74 6572 2d79 3d22 2d34 2e39  m-center-y="-4.9
+00004fa0: 3738 3032 3034 220a 2020 2020 2020 2020  780204".        
+00004fb0: 2072 783d 2233 2e31 3536 3232 3634 220a   rx="3.1562264".
+00004fc0: 2020 2020 2020 2020 2072 793d 2233 2e31           ry="3.1
+00004fd0: 3432 3032 3422 202f 3e0a 2020 2020 2020  42024" />.      
+00004fe0: 3c65 6c6c 6970 7365 0a20 2020 2020 2020  <ellipse.       
+00004ff0: 2020 7374 796c 653d 2266 696c 6c3a 2361    style="fill:#a
+00005000: 3861 3961 613b 6669 6c6c 2d6f 7061 6369  8a9aa;fill-opaci
+00005010: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+00005020: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00005030: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+00005040: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00005050: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00005060: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+00005070: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+00005080: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00005090: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+000050a0: 332d 352d 3722 0a20 2020 2020 2020 2020  3-5-7".         
+000050b0: 6378 3d22 3133 372e 3735 3832 3922 0a20  cx="137.75829". 
+000050c0: 2020 2020 2020 2020 6379 3d22 3131 382e          cy="118.
+000050d0: 3936 3131 3422 0a20 2020 2020 2020 2020  96114".         
+000050e0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+000050f0: 726d 2d63 656e 7465 722d 783d 2232 2e33  rm-center-x="2.3
+00005100: 3236 3936 3722 0a20 2020 2020 2020 2020  26967".         
+00005110: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+00005120: 726d 2d63 656e 7465 722d 793d 222d 342e  rm-center-y="-4.
+00005130: 3937 3830 3035 3922 0a20 2020 2020 2020  9780059".       
+00005140: 2020 7278 3d22 332e 3135 3632 3236 3422    rx="3.1562264"
+00005150: 0a20 2020 2020 2020 2020 7279 3d22 332e  .         ry="3.
+00005160: 3134 3230 3234 2220 2f3e 0a20 2020 2020  142024" />.     
+00005170: 203c 656c 6c69 7073 650a 2020 2020 2020   <ellipse.      
+00005180: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00005190: 6162 6161 3963 3b66 696c 6c2d 6f70 6163  abaa9c;fill-opac
+000051a0: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+000051b0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+000051c0: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
+000051d0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+000051e0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+000051f0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+00005200: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+00005210: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00005220: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
+00005230: 2d33 2d39 2d39 220a 2020 2020 2020 2020  -3-9-9".        
+00005240: 2063 783d 2239 312e 3031 3934 3738 220a   cx="91.019478".
+00005250: 2020 2020 2020 2020 2063 793d 2231 3439           cy="149
+00005260: 2e35 3730 3832 220a 2020 2020 2020 2020  .57082".        
+00005270: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00005280: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
+00005290: 3332 3639 3733 220a 2020 2020 2020 2020  326973".        
+000052a0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+000052b0: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d34  orm-center-y="-4
+000052c0: 2e39 3738 3032 3531 220a 2020 2020 2020  .9780251".      
+000052d0: 2020 2072 783d 2233 2e31 3536 3232 3634     rx="3.1562264
+000052e0: 220a 2020 2020 2020 2020 2072 793d 2233  ".         ry="3
+000052f0: 2e31 3432 3032 3422 202f 3e0a 2020 2020  .142024" />.    
+00005300: 2020 3c65 6c6c 6970 7365 0a20 2020 2020    <ellipse.     
+00005310: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00005320: 2331 3132 3036 363b 6669 6c6c 2d6f 7061  #112066;fill-opa
+00005330: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+00005340: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+00005350: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
+00005360: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00005370: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00005380: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
+00005390: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
+000053a0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+000053b0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+000053c0: 372d 332d 322d 3222 0a20 2020 2020 2020  7-3-2-2".       
+000053d0: 2020 6378 3d22 3836 2e34 3234 3636 3722    cx="86.424667"
+000053e0: 0a20 2020 2020 2020 2020 6379 3d22 3634  .         cy="64
+000053f0: 2e30 3531 3334 3622 0a20 2020 2020 2020  .051346".       
+00005400: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00005410: 666f 726d 2d63 656e 7465 722d 783d 2233  form-center-x="3
+00005420: 2e35 3931 3336 3039 220a 2020 2020 2020  .5913609".      
+00005430: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
+00005440: 7366 6f72 6d2d 6365 6e74 6572 2d79 3d22  sform-center-y="
+00005450: 2d37 2e36 3832 3839 3536 220a 2020 2020  -7.6828956".    
+00005460: 2020 2020 2072 783d 2234 2e38 3731 3139       rx="4.87119
+00005470: 3239 220a 2020 2020 2020 2020 2072 793d  29".         ry=
+00005480: 2234 2e38 3439 3237 3337 2220 2f3e 0a20  "4.8492737" />. 
+00005490: 2020 2020 203c 656c 6c69 7073 650a 2020       <ellipse.  
+000054a0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+000054b0: 6c6c 3a23 6564 6630 6663 3b66 696c 6c2d  ll:#edf0fc;fill-
+000054c0: 6f70 6163 6974 793a 302e 3939 3034 3436  opacity:0.990446
+000054d0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+000054e0: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
+000054f0: 3530 3035 3b73 7472 6f6b 652d 6d69 7465  5005;stroke-mite
+00005500: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00005510: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00005520: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+00005530: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+00005540: 793a 3122 0a20 2020 2020 2020 2020 6964  y:1".         id
+00005550: 3d22 7061 7468 3134 3536 372d 322d 3022  ="path14567-2-0"
+00005560: 0a20 2020 2020 2020 2020 6378 3d22 3133  .         cx="13
+00005570: 312e 3439 3231 3722 0a20 2020 2020 2020  1.49217".       
+00005580: 2020 6379 3d22 3637 2e32 3730 3339 3322    cy="67.270393"
+00005590: 0a20 2020 2020 2020 2020 7278 3d22 332e  .         rx="3.
+000055a0: 3135 3632 3236 3422 0a20 2020 2020 2020  1562264".       
+000055b0: 2020 7279 3d22 332e 3134 3230 3234 2220    ry="3.142024" 
+000055c0: 2f3e 0a20 2020 2020 203c 656c 6c69 7073  />.      <ellips
+000055d0: 650a 2020 2020 2020 2020 2073 7479 6c65  e.         style
+000055e0: 3d22 6669 6c6c 3a23 6564 6630 6663 3b66  ="fill:#edf0fc;f
+000055f0: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+00005600: 3034 3436 3b73 7472 6f6b 653a 2366 6666  0446;stroke:#fff
+00005610: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00005620: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+00005630: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00005640: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00005650: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+00005660: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+00005670: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00005680: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+00005690: 322d 382d 3233 220a 2020 2020 2020 2020  2-8-23".        
+000056a0: 2063 783d 2233 342e 3338 3339 3635 220a   cx="34.383965".
+000056b0: 2020 2020 2020 2020 2063 793d 2239 382e           cy="98.
+000056c0: 3234 3937 3739 220a 2020 2020 2020 2020  249779".        
+000056d0: 2072 783d 2233 2e31 3536 3232 3634 220a   rx="3.1562264".
+000056e0: 2020 2020 2020 2020 2072 793d 2233 2e31           ry="3.1
+000056f0: 3432 3032 3422 202f 3e0a 2020 2020 2020  42024" />.      
+00005700: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+00005710: 7479 6c65 3d22 6669 6c6c 3a23 3030 3030  tyle="fill:#0000
+00005720: 3030 3b66 696c 6c2d 6f70 6163 6974 793a  00;fill-opacity:
+00005730: 302e 3939 3834 3038 3b73 7472 6f6b 653a  0.998408;stroke:
+00005740: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
+00005750: 6964 7468 3a30 2e33 3233 3538 3870 783b  idth:0.323588px;
+00005760: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00005770: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00005780: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00005790: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+000057a0: 2020 2020 2064 3d22 6d20 3232 322e 3631       d="m 222.61
+000057b0: 3838 372c 3834 2e33 3938 3439 3220 3236  887,84.398492 26
+000057c0: 2e36 3034 3537 2c2d 382e 3738 3638 3320  .60457,-8.78683 
+000057d0: 2d32 382e 3338 3339 352c 2d31 2e34 3735  -28.38395,-1.475
+000057e0: 3836 2063 2031 312e 3030 3532 362c 332e  86 c 11.00526,3.
+000057f0: 3230 3436 3620 3131 2e30 3535 332c 332e  20466 11.0553,3.
+00005800: 3337 3432 3720 312e 3737 3933 382c 3130  37427 1.77938,10
+00005810: 2e32 3632 3639 207a 220a 2020 2020 2020  .26269 z".      
+00005820: 2020 2069 643d 2270 6174 6831 3436 3537     id="path14657
+00005830: 2d39 2d37 220a 2020 2020 2020 2020 2069  -9-7".         i
+00005840: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+00005850: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+00005860: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+00005870: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
+00005880: 6322 202f 3e0a 2020 2020 2020 3c65 6c6c  c" />.      <ell
+00005890: 6970 7365 0a20 2020 2020 2020 2020 7374  ipse.         st
+000058a0: 796c 653d 2266 696c 6c3a 2365 6466 3066  yle="fill:#edf0f
+000058b0: 633b 6669 6c6c 2d6f 7061 6369 7479 3a30  c;fill-opacity:0
+000058c0: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
+000058d0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+000058e0: 6474 683a 312e 3939 3539 383b 7374 726f  dth:1.99598;stro
+000058f0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00005900: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00005910: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
+00005920: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+00005930: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00005940: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00005950: 3637 2d32 2d37 2d35 220a 2020 2020 2020  67-2-7-5".      
+00005960: 2020 2063 783d 2232 3432 2e36 3637 3122     cx="242.6671"
+00005970: 0a20 2020 2020 2020 2020 6379 3d22 3736  .         cy="76
+00005980: 2e37 3737 3432 220a 2020 2020 2020 2020  .77742".        
+00005990: 2072 783d 2235 2e39 3939 3532 3232 220a   rx="5.9995222".
+000059a0: 2020 2020 2020 2020 2072 793d 2235 2e39           ry="5.9
+000059b0: 3732 3532 3536 2220 2f3e 0a20 2020 2020  725256" />.     
+000059c0: 203c 7465 7874 0a20 2020 2020 2020 2020   <text.         
+000059d0: 786d 6c3a 7370 6163 653d 2270 7265 7365  xml:space="prese
+000059e0: 7276 6522 0a20 2020 2020 2020 2020 7374  rve".         st
+000059f0: 796c 653d 2266 6f6e 742d 7374 796c 653a  yle="font-style:
+00005a00: 6e6f 726d 616c 3b66 6f6e 742d 7765 6967  normal;font-weig
+00005a10: 6874 3a6e 6f72 6d61 6c3b 666f 6e74 2d73  ht:normal;font-s
+00005a20: 697a 653a 352e 3837 3239 3170 783b 6c69  ize:5.87291px;li
+00005a30: 6e65 2d68 6569 6768 743a 312e 3235 3b66  ne-height:1.25;f
+00005a40: 6f6e 742d 6661 6d69 6c79 3a73 616e 732d  ont-family:sans-
+00005a50: 7365 7269 663b 6c65 7474 6572 2d73 7061  serif;letter-spa
+00005a60: 6369 6e67 3a30 7078 3b77 6f72 642d 7370  cing:0px;word-sp
+00005a70: 6163 696e 673a 3070 783b 6669 6c6c 3a23  acing:0px;fill:#
+00005a80: 6666 6666 6666 3b66 696c 6c2d 6f70 6163  ffffff;fill-opac
+00005a90: 6974 793a 313b 7374 726f 6b65 3a6e 6f6e  ity:1;stroke:non
+00005aa0: 653b 7374 726f 6b65 2d77 6964 7468 3a30  e;stroke-width:0
+00005ab0: 2e34 3030 3432 353b 6669 6c74 6572 3a75  .400425;filter:u
+00005ac0: 726c 2823 6669 6c74 6572 3135 3035 312d  rl(#filter15051-
+00005ad0: 3336 2922 0a20 2020 2020 2020 2020 783d  36)".         x=
+00005ae0: 2237 372e 3639 3438 3933 220a 2020 2020  "77.694893".    
+00005af0: 2020 2020 2079 3d22 3931 2e39 3838 3434       y="91.98844
+00005b00: 3922 0a20 2020 2020 2020 2020 6964 3d22  9".         id="
+00005b10: 7465 7874 3134 3639 312d 362d 3922 0a20  text14691-6-9". 
+00005b20: 2020 2020 2020 2020 7472 616e 7366 6f72          transfor
+00005b30: 6d3d 226d 6174 7269 7828 322e 3735 3131  m="matrix(2.7511
+00005b40: 3931 392c 302c 302c 322e 3733 3838 3132  919,0,0,2.738812
+00005b50: 2c2d 3735 2e39 3736 3639 362c 2d31 3038  ,-75.976696,-108
+00005b60: 2e30 3838 3636 2922 3e3c 7473 7061 6e0a  .08866)"><tspan.
+00005b70: 2020 2020 2020 2020 2020 2073 6f64 6970             sodip
+00005b80: 6f64 693a 726f 6c65 3d22 6c69 6e65 220a  odi:role="line".
+00005b90: 2020 2020 2020 2020 2020 2069 643d 2274             id="t
+00005ba0: 7370 616e 3134 3638 392d 322d 3222 0a20  span14689-2-2". 
+00005bb0: 2020 2020 2020 2020 2020 783d 2237 372e            x="77.
+00005bc0: 3639 3438 3933 220a 2020 2020 2020 2020  694893".        
+00005bd0: 2020 2079 3d22 3931 2e39 3838 3434 3922     y="91.988449"
+00005be0: 0a20 2020 2020 2020 2020 2020 7374 796c  .           styl
+00005bf0: 653d 2266 6f6e 742d 7374 796c 653a 6e6f  e="font-style:no
+00005c00: 726d 616c 3b66 6f6e 742d 7661 7269 616e  rmal;font-varian
+00005c10: 743a 6e6f 726d 616c 3b66 6f6e 742d 7765  t:normal;font-we
+00005c20: 6967 6874 3a6e 6f72 6d61 6c3b 666f 6e74  ight:normal;font
+00005c30: 2d73 7472 6574 6368 3a6e 6f72 6d61 6c3b  -stretch:normal;
+00005c40: 666f 6e74 2d73 697a 653a 3231 2e33 3536  font-size:21.356
+00005c50: 7078 3b66 6f6e 742d 6661 6d69 6c79 3a49  px;font-family:I
+00005c60: 6d70 6163 743b 2d69 6e6b 7363 6170 652d  mpact;-inkscape-
+00005c70: 666f 6e74 2d73 7065 6369 6669 6361 7469  font-specificati
+00005c80: 6f6e 3a49 6d70 6163 743b 6669 6c6c 3a23  on:Impact;fill:#
+00005c90: 6666 6666 6666 3b66 696c 6c2d 6f70 6163  ffffff;fill-opac
+00005ca0: 6974 793a 313b 7374 726f 6b65 2d77 6964  ity:1;stroke-wid
+00005cb0: 7468 3a30 2e34 3030 3432 3522 3e53 6165  th:0.400425">Sae
+00005cc0: 6e6f 7079 3c2f 7473 7061 6e3e 3c2f 7465  nopy</tspan></te
+00005cd0: 7874 3e0a 2020 2020 2020 3c74 6578 740a  xt>.      <text.
+00005ce0: 2020 2020 2020 2020 2078 6d6c 3a73 7061           xml:spa
+00005cf0: 6365 3d22 7072 6573 6572 7665 220a 2020  ce="preserve".  
+00005d00: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
+00005d10: 6e74 2d73 7479 6c65 3a6e 6f72 6d61 6c3b  nt-style:normal;
+00005d20: 666f 6e74 2d77 6569 6768 743a 6e6f 726d  font-weight:norm
+00005d30: 616c 3b66 6f6e 742d 7369 7a65 3a31 362e  al;font-size:16.
+00005d40: 3132 3131 7078 3b6c 696e 652d 6865 6967  1211px;line-heig
+00005d50: 6874 3a31 2e32 353b 666f 6e74 2d66 616d  ht:1.25;font-fam
+00005d60: 696c 793a 7361 6e73 2d73 6572 6966 3b6c  ily:sans-serif;l
+00005d70: 6574 7465 722d 7370 6163 696e 673a 3070  etter-spacing:0p
+00005d80: 783b 776f 7264 2d73 7061 6369 6e67 3a30  x;word-spacing:0
+00005d90: 7078 3b66 696c 6c3a 2330 3030 3030 303b  px;fill:#000000;
+00005da0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00005db0: 7472 6f6b 653a 6e6f 6e65 3b73 7472 6f6b  troke:none;strok
+00005dc0: 652d 7769 6474 683a 312e 3039 3931 3722  e-width:1.09917"
+00005dd0: 0a20 2020 2020 2020 2020 783d 2231 3335  .         x="135
+00005de0: 2e34 3739 3036 220a 2020 2020 2020 2020  .47906".        
+00005df0: 2079 3d22 3133 362e 3338 3737 220a 2020   y="136.3877".  
+00005e00: 2020 2020 2020 2069 643d 2274 6578 7431         id="text1
+00005e10: 3436 3931 2d32 220a 2020 2020 2020 2020  4691-2".        
+00005e20: 2074 7261 6e73 666f 726d 3d22 7363 616c   transform="scal
+00005e30: 6528 312e 3030 3232 3537 352c 302e 3939  e(1.0022575,0.99
+00005e40: 3737 3437 3538 2922 3e3c 7473 7061 6e0a  774758)"><tspan.
+00005e50: 2020 2020 2020 2020 2020 2073 6f64 6970             sodip
+00005e60: 6f64 693a 726f 6c65 3d22 6c69 6e65 220a  odi:role="line".
+00005e70: 2020 2020 2020 2020 2020 2069 643d 2274             id="t
+00005e80: 7370 616e 3134 3638 392d 3822 0a20 2020  span14689-8".   
+00005e90: 2020 2020 2020 2020 783d 2231 3335 2e34          x="135.4
+00005ea0: 3739 3036 220a 2020 2020 2020 2020 2020  7906".          
+00005eb0: 2079 3d22 3133 362e 3338 3737 220a 2020   y="136.3877".  
+00005ec0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00005ed0: 666f 6e74 2d73 7479 6c65 3a6e 6f72 6d61  font-style:norma
+00005ee0: 6c3b 666f 6e74 2d76 6172 6961 6e74 3a6e  l;font-variant:n
+00005ef0: 6f72 6d61 6c3b 666f 6e74 2d77 6569 6768  ormal;font-weigh
+00005f00: 743a 6e6f 726d 616c 3b66 6f6e 742d 7374  t:normal;font-st
+00005f10: 7265 7463 683a 6e6f 726d 616c 3b66 6f6e  retch:normal;fon
+00005f20: 742d 7369 7a65 3a35 382e 3632 3231 7078  t-size:58.6221px
+00005f30: 3b66 6f6e 742d 6661 6d69 6c79 3a27 546c  ;font-family:'Tl
+00005f40: 7767 2054 7970 6973 7427 3b2d 696e 6b73  wg Typist';-inks
+00005f50: 6361 7065 2d66 6f6e 742d 7370 6563 6966  cape-font-specif
+00005f60: 6963 6174 696f 6e3a 2754 6c77 6720 5479  ication:'Tlwg Ty
+00005f70: 7069 7374 273b 7374 726f 6b65 2d77 6964  pist';stroke-wid
+00005f80: 7468 3a31 2e30 3939 3137 223e 5361 656e  th:1.09917">Saen
+00005f90: 6f70 793c 2f74 7370 616e 3e3c 2f74 6578  opy</tspan></tex
+00005fa0: 743e 0a20 2020 203c 2f67 3e0a 2020 2020  t>.    </g>.    
+00005fb0: 3c72 6563 740a 2020 2020 2020 2073 7479  <rect.       sty
+00005fc0: 6c65 3d22 6669 6c6c 3a23 3030 3030 3030  le="fill:#000000
+00005fd0: 3b73 7472 6f6b 653a 6e6f 6e65 3b73 7472  ;stroke:none;str
+00005fe0: 6f6b 652d 7769 6474 683a 352e 3038 3437  oke-width:5.0847
+00005ff0: 363b 7374 726f 6b65 2d6c 696e 6563 6170  6;stroke-linecap
+00006000: 3a72 6f75 6e64 3b73 7472 6f6b 652d 6c69  :round;stroke-li
+00006010: 6e65 6a6f 696e 3a72 6f75 6e64 3b66 696c  nejoin:round;fil
+00006020: 6c2d 6f70 6163 6974 793a 3022 0a20 2020  l-opacity:0".   
+00006030: 2020 2020 6964 3d22 7265 6374 3730 362d      id="rect706-
+00006040: 3522 0a20 2020 2020 2020 7769 6474 683d  5".       width=
+00006050: 2234 3030 220a 2020 2020 2020 2068 6569  "400".       hei
+00006060: 6768 743d 2232 3030 220a 2020 2020 2020  ght="200".      
+00006070: 2078 3d22 3435 3022 0a20 2020 2020 2020   x="450".       
+00006080: 793d 222d 312e 3835 3230 3631 3165 2d30  y="-1.8520611e-0
+00006090: 3622 0a20 2020 2020 2020 7279 3d22 3022  6".       ry="0"
+000060a0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+000060b0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+000060c0: 3a23 6666 6666 6666 3b66 696c 6c2d 6f70  :#ffffff;fill-op
+000060d0: 6163 6974 793a 302e 3939 3834 3038 3038  acity:0.99840808
+000060e0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+000060f0: 7374 726f 6b65 2d77 6964 7468 3a30 2e35  stroke-width:0.5
+00006100: 3030 3032 3270 783b 7374 726f 6b65 2d6c  00022px;stroke-l
+00006110: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00006120: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00006130: 723b 7374 726f 6b65 2d6f 7061 6369 7479  r;stroke-opacity
+00006140: 3a31 220a 2020 2020 2020 2064 3d22 4d20  :1".       d="M 
+00006150: 3632 332e 3834 3831 322c 3839 2e30 3639  623.84812,89.069
+00006160: 3531 2037 3837 2e36 3530 3937 2c36 342e  51 787.65097,64.
+00006170: 3934 3937 3120 3632 312e 3837 3434 362c  94971 621.87446,
+00006180: 3830 2e37 3134 3336 205a 220a 2020 2020  80.71436 Z".    
+00006190: 2020 2069 643d 2270 6174 6831 3436 3537     id="path14657
+000061a0: 2d33 220a 2020 2020 2020 2069 6e6b 7363  -3".       inksc
+000061b0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+000061c0: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+000061d0: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+000061e0: 7479 7065 733d 2263 6363 6322 202f 3e0a  types="cccc" />.
+000061f0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+00006200: 2073 7479 6c65 3d22 6669 6c6c 3a23 3365   style="fill:#3e
+00006210: 3462 3737 3b66 696c 6c2d 6f70 6163 6974  4b77;fill-opacit
+00006220: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00006230: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00006240: 312e 3035 3030 353b 7374 726f 6b65 2d6c  1.05005;stroke-l
+00006250: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00006260: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00006270: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+00006280: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00006290: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+000062a0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+000062b0: 2020 2020 2064 3d22 6d20 3436 392e 3630       d="m 469.60
+000062c0: 3330 382c 3637 2e36 3536 3920 3631 2e32  308,67.6569 61.2
+000062d0: 3534 3936 2c2d 322e 3737 3137 3820 3430  5496,-2.77178 40
+000062e0: 2e32 3436 3032 2c2d 3434 2e36 3030 3538  .24602,-44.60058
+000062f0: 2043 2035 3230 2e34 3032 362c 3534 2e32   C 520.4026,54.2
+00006300: 3238 3733 2034 3936 2e31 3739 3631 2c35  2873 496.17961,5
+00006310: 392e 3637 3633 3720 3436 392e 3630 3330  9.67637 469.6030
+00006320: 382c 3637 2e36 3536 3920 5a22 0a20 2020  8,67.6569 Z".   
+00006330: 2020 2020 6964 3d22 7061 7468 3134 3534      id="path1454
+00006340: 372d 3522 0a20 2020 2020 2020 696e 6b73  7-5".       inks
+00006350: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+00006360: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+00006370: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00006380: 6574 7970 6573 3d22 6363 6363 2220 2f3e  etypes="cccc" />
+00006390: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+000063a0: 2020 7374 796c 653d 2266 696c 6c3a 2331    style="fill:#1
+000063b0: 6332 6336 383b 6669 6c6c 2d6f 7061 6369  c2c68;fill-opaci
+000063c0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+000063d0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+000063e0: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+000063f0: 6c69 6e65 6361 703a 6275 7474 3b73 7472  linecap:butt;str
+00006400: 6f6b 652d 6c69 6e65 6a6f 696e 3a6d 6974  oke-linejoin:mit
+00006410: 6572 3b73 7472 6f6b 652d 6d69 7465 726c  er;stroke-miterl
+00006420: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00006430: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00006440: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00006450: 2020 2020 2020 643d 226d 2035 3330 2e38        d="m 530.8
+00006460: 3538 3034 2c36 342e 3838 3531 3220 3236  5804,64.88512 26
+00006470: 2e35 3737 3536 2c36 2e30 3437 3534 2031  .57756,6.04754 1
+00006480: 332e 3636 3834 362c 2d35 302e 3634 3831  3.66846,-50.6481
+00006490: 3220 7a22 0a20 2020 2020 2020 6964 3d22  2 z".       id="
+000064a0: 7061 7468 3134 3534 392d 3622 0a20 2020  path14549-6".   
+000064b0: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
+000064c0: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
+000064d0: 3d22 3022 202f 3e0a 2020 2020 3c70 6174  ="0" />.    <pat
+000064e0: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+000064f0: 6669 6c6c 3a23 3036 3035 3038 3b66 696c  fill:#060508;fil
+00006500: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00006510: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00006520: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
+00006530: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00006540: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00006550: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00006560: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00006570: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00006580: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00006590: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+000065a0: 4d20 3535 372e 3433 3536 2c37 302e 3933  M 557.4356,70.93
+000065b0: 3236 3620 3632 382e 3536 3232 342c 3833  266 628.56224,83
+000065c0: 2e35 3331 3720 4320 3630 302e 3834 3534  .5317 C 600.8454
+000065d0: 322c 3638 2e39 3434 3937 2035 3834 2e37  2,68.94497 584.7
+000065e0: 3935 3032 2c34 352e 3530 3935 3520 3537  9502,45.50955 57
+000065f0: 312e 3130 3430 362c 3230 2e32 3834 3534  1.10406,20.28454
+00006600: 205a 220a 2020 2020 2020 2069 643d 2270   Z".       id="p
+00006610: 6174 6831 3435 3531 2d32 220a 2020 2020  ath14551-2".    
+00006620: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00006630: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+00006640: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
+00006650: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+00006660: 6363 6322 202f 3e0a 2020 2020 3c70 6174  ccc" />.    <pat
+00006670: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+00006680: 6669 6c6c 3a23 3237 3337 3733 3b66 696c  fill:#273773;fil
+00006690: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+000066a0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+000066b0: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
+000066c0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+000066d0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+000066e0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+000066f0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00006700: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00006710: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00006720: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+00006730: 6d20 3436 392e 3630 3330 382c 3637 2e36  m 469.60308,67.6
+00006740: 3536 3920 6320 3133 2e34 3739 3331 2c37  569 c 13.47931,7
+00006750: 2e36 3937 3820 3238 2e33 3431 3131 2c31  .6978 28.34111,1
+00006760: 342e 3333 3639 3520 3333 2e34 3131 382c  4.33695 33.4118,
+00006770: 3238 2e34 3733 3832 206c 2032 372e 3834  28.47382 l 27.84
+00006780: 3331 362c 2d33 312e 3234 3536 207a 220a  316,-31.2456 z".
+00006790: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+000067a0: 3435 3533 2d39 220a 2020 2020 2020 2069  4553-9".       i
+000067b0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+000067c0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+000067d0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+000067e0: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+000067f0: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00006800: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00006810: 3a23 3134 3236 3732 3b66 696c 6c2d 6f70  :#142672;fill-op
+00006820: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+00006830: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00006840: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
+00006850: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00006860: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00006870: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+00006880: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00006890: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+000068a0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+000068b0: 220a 2020 2020 2020 2064 3d22 4d20 3530  ".       d="M 50
+000068c0: 332e 3031 3438 382c 3936 2e31 3330 3732  3.01488,96.13072
+000068d0: 2036 3238 2e35 3632 3234 2c38 332e 3533   628.56224,83.53
+000068e0: 3137 2035 3330 2e38 3538 3034 2c36 342e  17 530.85804,64.
+000068f0: 3838 3531 3220 5a22 0a20 2020 2020 2020  88512 Z".       
+00006900: 6964 3d22 7061 7468 3134 3535 352d 3122  id="path14555-1"
+00006910: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00006920: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+00006930: 7475 7265 3d22 3022 202f 3e0a 2020 2020  ture="0" />.    
+00006940: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+00006950: 6c65 3d22 6669 6c6c 3a23 3534 3636 3863  le="fill:#54668c
+00006960: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00006970: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00006980: 7472 6f6b 652d 7769 6474 683a 312e 3035  troke-width:1.05
+00006990: 3030 353b 7374 726f 6b65 2d6c 696e 6563  005;stroke-linec
+000069a0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+000069b0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+000069c0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+000069d0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+000069e0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+000069f0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00006a00: 2064 3d22 6d20 3530 332e 3031 3438 382c   d="m 503.01488,
+00006a10: 3936 2e31 3330 3732 2037 322e 3339 3232  96.13072 72.3922
+00006a20: 322c 372e 3535 3934 3420 3533 2e31 3535  2,7.55944 53.155
+00006a30: 3134 2c2d 3230 2e31 3538 3436 207a 220a  14,-20.15846 z".
+00006a40: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00006a50: 3435 3537 2d32 220a 2020 2020 2020 2069  4557-2".       i
+00006a60: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+00006a70: 722d 6375 7276 6174 7572 653d 2230 2220  r-curvature="0" 
+00006a80: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+00006a90: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00006aa0: 2332 3233 3437 653b 6669 6c6c 2d6f 7061  #22347e;fill-opa
+00006ab0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+00006ac0: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+00006ad0: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
+00006ae0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00006af0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+00006b00: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00006b10: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00006b20: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00006b30: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00006b40: 0a20 2020 2020 2020 643d 226d 2035 3033  .       d="m 503
+00006b50: 2e30 3134 3838 2c39 362e 3133 3037 3220  .01488,96.13072 
+00006b60: 6320 312e 3632 3738 322c 3133 2e39 3732  c 1.62782,13.972
+00006b70: 3532 202d 342e 3030 3637 382c 3232 2e37  52 -4.00678,22.7
+00006b80: 3830 3933 202d 362e 3538 3131 312c 3333  8093 -6.58111,33
+00006b90: 2e37 3635 3431 206c 2037 382e 3937 3333  .76541 l 78.9733
+00006ba0: 332c 2d32 362e 3230 3539 3720 7a22 0a20  3,-26.20597 z". 
+00006bb0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00006bc0: 3535 392d 3722 0a20 2020 2020 2020 696e  559-7".       in
+00006bd0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00006be0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+00006bf0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00006c00: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
+00006c10: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+00006c20: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00006c30: 2330 3831 3036 393b 6669 6c6c 2d6f 7061  #081069;fill-opa
+00006c40: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+00006c50: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+00006c60: 7468 3a31 2e30 3530 3035 3b73 7472 6f6b  th:1.05005;strok
+00006c70: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00006c80: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+00006c90: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00006ca0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00006cb0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00006cc0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00006cd0: 0a20 2020 2020 2020 643d 226d 2034 3936  .       d="m 496
+00006ce0: 2e34 3333 3737 2c31 3239 2e38 3936 3133  .43377,129.89613
+00006cf0: 2035 342e 3637 3338 342c 382e 3036 3333   54.67384,8.0633
+00006d00: 3820 3737 2e34 3534 3633 2c2d 3534 2e34  8 77.45463,-54.4
+00006d10: 3237 3831 207a 220a 2020 2020 2020 2069  2781 z".       i
+00006d20: 643d 2270 6174 6831 3435 3631 2d30 220a  d="path14561-0".
+00006d30: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00006d40: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00006d50: 7572 653d 2230 2220 2f3e 0a20 2020 203c  ure="0" />.    <
+00006d60: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+00006d70: 653d 2266 696c 6c3a 2330 3730 6532 623b  e="fill:#070e2b;
+00006d80: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00006d90: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00006da0: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+00006db0: 3035 3b73 7472 6f6b 652d 6c69 6e65 6361  05;stroke-lineca
+00006dc0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00006dd0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00006de0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00006df0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00006e00: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00006e10: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00006e20: 643d 224d 2035 3531 2e31 3037 3631 2c31  d="M 551.10761,1
+00006e30: 3337 2e39 3539 3531 2035 3833 2e32 3533  37.95951 583.253
+00006e40: 382c 3138 302e 3034 3033 2035 3731 2e33  8,180.0403 571.3
+00006e50: 3537 3138 2c31 3233 2e33 3434 3634 205a  5718,123.34464 Z
+00006e60: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00006e70: 6831 3435 3633 2d39 220a 2020 2020 2020  h14563-9".      
+00006e80: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+00006e90: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+00006ea0: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+00006eb0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00006ec0: 6c3a 2332 3833 6438 373b 6669 6c6c 2d6f  l:#283d87;fill-o
+00006ed0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00006ee0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+00006ef0: 6964 7468 3a31 2e30 3530 3035 3b73 7472  idth:1.05005;str
+00006f00: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00006f10: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00006f20: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+00006f30: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00006f40: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00006f50: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00006f60: 3122 0a20 2020 2020 2020 643d 226d 2035  1".       d="m 5
+00006f70: 3731 2e33 3537 3138 2c31 3233 2e33 3434  71.35718,123.344
+00006f80: 3634 2031 312e 3839 3636 322c 3536 2e36  64 11.89662,56.6
+00006f90: 3935 3636 2063 2036 2e31 3538 3632 2c2d  9566 c 6.15862,-
+00006fa0: 3530 2e39 3636 3733 2032 372e 3833 3134  50.96673 27.8314
+00006fb0: 372c 2d36 392e 3332 3836 3120 3435 2e33  7,-69.32861 45.3
+00006fc0: 3038 3434 2c2d 3936 2e35 3038 3620 7a22  0844,-96.5086 z"
+00006fd0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00006fe0: 3134 3536 352d 3322 0a20 2020 2020 2020  14565-3".       
+00006ff0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+00007000: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+00007010: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00007020: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+00007030: 2220 2f3e 0a20 2020 203c 656c 6c69 7073  " />.    <ellips
+00007040: 650a 2020 2020 2020 2073 7479 6c65 3d22  e.       style="
+00007050: 6669 6c6c 3a23 3037 3065 3262 3b66 696c  fill:#070e2b;fil
+00007060: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
+00007070: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
+00007080: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
+00007090: 2e30 3530 3035 3b73 7472 6f6b 652d 6d69  .05005;stroke-mi
+000070a0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+000070b0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+000070c0: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
+000070d0: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
+000070e0: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
+000070f0: 3d22 7061 7468 3134 3536 372d 3630 220a  ="path14567-60".
+00007100: 2020 2020 2020 2063 783d 2234 3730 2e39         cx="470.9
+00007110: 3033 3134 220a 2020 2020 2020 2063 793d  0314".       cy=
+00007120: 2236 372e 3732 3135 3838 220a 2020 2020  "67.721588".    
+00007130: 2020 2072 783d 2233 2e31 3536 3232 3634     rx="3.1562264
+00007140: 220a 2020 2020 2020 2072 793d 2233 2e31  ".       ry="3.1
+00007150: 3432 3032 3422 202f 3e0a 2020 2020 3c65  42024" />.    <e
+00007160: 6c6c 6970 7365 0a20 2020 2020 2020 7374  llipse.       st
+00007170: 796c 653d 2266 696c 6c3a 2332 3533 6137  yle="fill:#253a7
+00007180: 643b 6669 6c6c 2d6f 7061 6369 7479 3a31  d;fill-opacity:1
+00007190: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+000071a0: 7374 726f 6b65 2d77 6964 7468 3a31 2e30  stroke-width:1.0
+000071b0: 3530 3035 3b73 7472 6f6b 652d 6d69 7465  5005;stroke-mite
+000071c0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+000071d0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+000071e0: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+000071f0: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+00007200: 793a 3122 0a20 2020 2020 2020 6964 3d22  y:1".       id="
+00007210: 7061 7468 3134 3536 372d 332d 3622 0a20  path14567-3-6". 
+00007220: 2020 2020 2020 6378 3d22 3439 352e 3932        cx="495.92
+00007230: 3538 3422 0a20 2020 2020 2020 6379 3d22  584".       cy="
+00007240: 3132 392e 3232 3538 3822 0a20 2020 2020  129.22588".     
+00007250: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00007260: 666f 726d 2d63 656e 7465 722d 783d 2232  form-center-x="2
+00007270: 2e33 3236 3937 3435 220a 2020 2020 2020  .3269745".      
+00007280: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00007290: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d34  orm-center-y="-4
+000072a0: 2e39 3738 3031 3633 220a 2020 2020 2020  .9780163".      
+000072b0: 2072 783d 2233 2e31 3536 3232 3634 220a   rx="3.1562264".
+000072c0: 2020 2020 2020 2072 793d 2233 2e31 3432         ry="3.142
+000072d0: 3032 3422 202f 3e0a 2020 2020 3c65 6c6c  024" />.    <ell
+000072e0: 6970 7365 0a20 2020 2020 2020 7374 796c  ipse.       styl
+000072f0: 653d 2266 696c 6c3a 2332 3533 6137 643b  e="fill:#253a7d;
+00007300: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00007310: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00007320: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+00007330: 3035 3b73 7472 6f6b 652d 6d69 7465 726c  05;stroke-miterl
+00007340: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00007350: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00007360: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+00007370: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00007380: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
+00007390: 7468 3134 3536 372d 332d 372d 3222 0a20  th14567-3-7-2". 
+000073a0: 2020 2020 2020 6378 3d22 3537 302e 3538        cx="570.58
+000073b0: 3836 3222 0a20 2020 2020 2020 6379 3d22  862".       cy="
+000073c0: 3130 332e 3839 3133 3922 0a20 2020 2020  103.89139".     
+000073d0: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+000073e0: 666f 726d 2d63 656e 7465 722d 783d 2232  form-center-x="2
+000073f0: 2e33 3236 3937 3932 220a 2020 2020 2020  .3269792".      
+00007400: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00007410: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d34  orm-center-y="-4
+00007420: 2e39 3738 3032 3034 220a 2020 2020 2020  .9780204".      
+00007430: 2072 783d 2233 2e31 3536 3232 3634 220a   rx="3.1562264".
+00007440: 2020 2020 2020 2072 793d 2233 2e31 3432         ry="3.142
+00007450: 3032 3422 202f 3e0a 2020 2020 3c65 6c6c  024" />.    <ell
+00007460: 6970 7365 0a20 2020 2020 2020 7374 796c  ipse.       styl
+00007470: 653d 2266 696c 6c3a 2361 3861 3961 613b  e="fill:#a8a9aa;
+00007480: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00007490: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+000074a0: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+000074b0: 3035 3b73 7472 6f6b 652d 6d69 7465 726c  05;stroke-miterl
+000074c0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+000074d0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+000074e0: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+000074f0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00007500: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
+00007510: 7468 3134 3536 372d 332d 352d 3622 0a20  th14567-3-5-6". 
+00007520: 2020 2020 2020 6378 3d22 3537 312e 3333        cx="571.33
+00007530: 3731 3622 0a20 2020 2020 2020 6379 3d22  716".       cy="
+00007540: 3132 322e 3839 3232 3422 0a20 2020 2020  122.89224".     
+00007550: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00007560: 666f 726d 2d63 656e 7465 722d 783d 2232  form-center-x="2
+00007570: 2e33 3236 3936 3722 0a20 2020 2020 2020  .326967".       
+00007580: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+00007590: 726d 2d63 656e 7465 722d 793d 222d 342e  rm-center-y="-4.
+000075a0: 3937 3830 3035 3922 0a20 2020 2020 2020  9780059".       
+000075b0: 7278 3d22 332e 3135 3632 3236 3422 0a20  rx="3.1562264". 
+000075c0: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
+000075d0: 3234 2220 2f3e 0a20 2020 203c 656c 6c69  24" />.    <elli
+000075e0: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
+000075f0: 3d22 6669 6c6c 3a23 6162 6161 3963 3b66  ="fill:#abaa9c;f
+00007600: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00007610: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00007620: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00007630: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+00007640: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00007650: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00007660: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+00007670: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00007680: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00007690: 6831 3435 3637 2d33 2d39 2d31 220a 2020  h14567-3-9-1".  
+000076a0: 2020 2020 2063 783d 2235 3531 2e38 3736       cx="551.876
+000076b0: 3136 220a 2020 2020 2020 2063 793d 2231  16".       cy="1
+000076c0: 3337 2e37 3934 3835 220a 2020 2020 2020  37.79485".      
+000076d0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+000076e0: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
+000076f0: 3332 3639 3733 220a 2020 2020 2020 2069  326973".       i
+00007700: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00007710: 6d2d 6365 6e74 6572 2d79 3d22 2d34 2e39  m-center-y="-4.9
+00007720: 3738 3032 3531 220a 2020 2020 2020 2072  780251".       r
+00007730: 783d 2233 2e31 3536 3232 3634 220a 2020  x="3.1562264".  
+00007740: 2020 2020 2072 793d 2233 2e31 3432 3032       ry="3.14202
+00007750: 3422 202f 3e0a 2020 2020 3c65 6c6c 6970  4" />.    <ellip
+00007760: 7365 0a20 2020 2020 2020 7374 796c 653d  se.       style=
+00007770: 2266 696c 6c3a 2331 3132 3036 363b 6669  "fill:#112066;fi
+00007780: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00007790: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+000077a0: 6b65 2d77 6964 7468 3a31 2e30 3530 3035  ke-width:1.05005
+000077b0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+000077c0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+000077d0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+000077e0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+000077f0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00007800: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00007810: 3134 3536 372d 332d 322d 3822 0a20 2020  14567-3-2-8".   
+00007820: 2020 2020 6378 3d22 3533 312e 3239 3234      cx="531.2924
+00007830: 3222 0a20 2020 2020 2020 6379 3d22 3634  2".       cy="64
+00007840: 2e32 3133 3136 3522 0a20 2020 2020 2020  .213165".       
+00007850: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+00007860: 726d 2d63 656e 7465 722d 783d 2233 2e35  rm-center-x="3.5
+00007870: 3931 3336 3039 220a 2020 2020 2020 2069  913609".       i
+00007880: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00007890: 6d2d 6365 6e74 6572 2d79 3d22 2d37 2e36  m-center-y="-7.6
+000078a0: 3832 3839 3536 220a 2020 2020 2020 2072  828956".       r
+000078b0: 783d 2234 2e38 3731 3139 3239 220a 2020  x="4.8711929".  
+000078c0: 2020 2020 2072 793d 2234 2e38 3439 3237       ry="4.84927
+000078d0: 3337 2220 2f3e 0a20 2020 203c 656c 6c69  37" />.    <elli
+000078e0: 7073 650a 2020 2020 2020 2073 7479 6c65  pse.       style
+000078f0: 3d22 6669 6c6c 3a23 6564 6630 6663 3b66  ="fill:#edf0fc;f
+00007900: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+00007910: 3034 3436 3b73 7472 6f6b 653a 2366 6666  0446;stroke:#fff
+00007920: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00007930: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+00007940: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00007950: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00007960: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+00007970: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+00007980: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00007990: 6964 3d22 7061 7468 3134 3536 372d 322d  id="path14567-2-
+000079a0: 3739 220a 2020 2020 2020 2063 783d 2235  79".       cx="5
+000079b0: 3537 2e36 3737 220a 2020 2020 2020 2063  57.677".       c
+000079c0: 793d 2236 392e 3631 3533 3536 220a 2020  y="69.615356".  
+000079d0: 2020 2020 2072 783d 2233 2e31 3536 3232       rx="3.15622
+000079e0: 3634 220a 2020 2020 2020 2072 793d 2233  64".       ry="3
+000079f0: 2e31 3432 3032 3422 202f 3e0a 2020 2020  .142024" />.    
+00007a00: 3c65 6c6c 6970 7365 0a20 2020 2020 2020  <ellipse.       
+00007a10: 7374 796c 653d 2266 696c 6c3a 2365 6466  style="fill:#edf
+00007a20: 3066 633b 6669 6c6c 2d6f 7061 6369 7479  0fc;fill-opacity
+00007a30: 3a30 2e39 3930 3434 363b 7374 726f 6b65  :0.990446;stroke
+00007a40: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+00007a50: 7769 6474 683a 312e 3035 3030 353b 7374  width:1.05005;st
+00007a60: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00007a70: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00007a80: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+00007a90: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+00007aa0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00007ab0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00007ac0: 3637 2d32 2d38 2d32 220a 2020 2020 2020  67-2-8-2".      
+00007ad0: 2063 783d 2235 3033 2e30 3336 3539 220a   cx="503.03659".
+00007ae0: 2020 2020 2020 2063 793d 2239 352e 3639         cy="95.69
+00007af0: 3439 3737 220a 2020 2020 2020 2072 783d  4977".       rx=
+00007b00: 2233 2e31 3536 3232 3634 220a 2020 2020  "3.1562264".    
+00007b10: 2020 2072 793d 2233 2e31 3432 3032 3422     ry="3.142024"
+00007b20: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00007b30: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00007b40: 3a23 6666 6666 6666 3b66 696c 6c2d 6f70  :#ffffff;fill-op
+00007b50: 6163 6974 793a 302e 3939 3834 3038 3038  acity:0.99840808
+00007b60: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00007b70: 7374 726f 6b65 2d77 6964 7468 3a30 2e33  stroke-width:0.3
+00007b80: 3233 3538 3870 783b 7374 726f 6b65 2d6c  23588px;stroke-l
+00007b90: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00007ba0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00007bb0: 723b 7374 726f 6b65 2d6f 7061 6369 7479  r;stroke-opacity
+00007bc0: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
+00007bd0: 3736 382e 3730 3133 342c 3732 2e37 3031  768.70134,72.701
+00007be0: 3732 2032 362e 3630 3435 372c 2d38 2e37  72 26.60457,-8.7
+00007bf0: 3836 3833 202d 3238 2e33 3833 3935 2c2d  8683 -28.38395,-
+00007c00: 312e 3437 3538 3620 6320 3131 2e30 3035  1.47586 c 11.005
+00007c10: 3236 2c33 2e32 3034 3636 2031 312e 3035  26,3.20466 11.05
+00007c20: 3533 2c33 2e33 3734 3237 2031 2e37 3739  53,3.37427 1.779
+00007c30: 3338 2c31 302e 3236 3236 3920 7a22 0a20  38,10.26269 z". 
+00007c40: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00007c50: 3635 372d 392d 3022 0a20 2020 2020 2020  657-9-0".       
+00007c60: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+00007c70: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+00007c80: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00007c90: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+00007ca0: 2220 2f3e 0a20 2020 203c 656c 6c69 7073  " />.    <ellips
+00007cb0: 650a 2020 2020 2020 2073 7479 6c65 3d22  e.       style="
+00007cc0: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
+00007cd0: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
+00007ce0: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
+00007cf0: 663b 7374 726f 6b65 2d77 6964 7468 3a31  f;stroke-width:1
+00007d00: 2e39 3935 3938 3b73 7472 6f6b 652d 6d69  .99598;stroke-mi
+00007d10: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00007d20: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00007d30: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
+00007d40: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
+00007d50: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
+00007d60: 3d22 7061 7468 3134 3536 372d 322d 372d  ="path14567-2-7-
+00007d70: 3222 0a20 2020 2020 2020 6378 3d22 3632  2".       cx="62
+00007d80: 372e 3437 3435 3522 0a20 2020 2020 2020  7.47455".       
+00007d90: 6379 3d22 3834 2e33 3331 3732 3622 0a20  cy="84.331726". 
+00007da0: 2020 2020 2020 7278 3d22 352e 3939 3935        rx="5.9995
+00007db0: 3232 3222 0a20 2020 2020 2020 7279 3d22  222".       ry="
+00007dc0: 352e 3937 3235 3235 3622 202f 3e0a 2020  5.9725256" />.  
+00007dd0: 2020 3c74 6578 740a 2020 2020 2020 2078    <text.       x
+00007de0: 6d6c 3a73 7061 6365 3d22 7072 6573 6572  ml:space="preser
+00007df0: 7665 220a 2020 2020 2020 2073 7479 6c65  ve".       style
+00007e00: 3d22 666f 6e74 2d73 7479 6c65 3a6e 6f72  ="font-style:nor
+00007e10: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
+00007e20: 6e6f 726d 616c 3b66 6f6e 742d 7369 7a65  normal;font-size
+00007e30: 3a35 2e38 3732 3931 7078 3b6c 696e 652d  :5.87291px;line-
+00007e40: 6865 6967 6874 3a31 2e32 353b 666f 6e74  height:1.25;font
+00007e50: 2d66 616d 696c 793a 7361 6e73 2d73 6572  -family:sans-ser
+00007e60: 6966 3b6c 6574 7465 722d 7370 6163 696e  if;letter-spacin
+00007e70: 673a 3070 783b 776f 7264 2d73 7061 6369  g:0px;word-spaci
+00007e80: 6e67 3a30 7078 3b66 696c 6c3a 2335 3435  ng:0px;fill:#545
+00007e90: 3435 343b 6669 6c6c 2d6f 7061 6369 7479  454;fill-opacity
+00007ea0: 3a31 3b73 7472 6f6b 653a 6e6f 6e65 3b73  :1;stroke:none;s
+00007eb0: 7472 6f6b 652d 7769 6474 683a 302e 3430  troke-width:0.40
+00007ec0: 3034 3235 3b66 696c 7465 723a 7572 6c28  0425;filter:url(
+00007ed0: 2366 696c 7465 7231 3530 3531 2d33 2922  #filter15051-3)"
+00007ee0: 0a20 2020 2020 2020 783d 2237 372e 3639  .       x="77.69
+00007ef0: 3438 3933 220a 2020 2020 2020 2079 3d22  4893".       y="
+00007f00: 3931 2e39 3838 3434 3922 0a20 2020 2020  91.988449".     
+00007f10: 2020 6964 3d22 7465 7874 3134 3639 312d    id="text14691-
+00007f20: 362d 3322 0a20 2020 2020 2020 7472 616e  6-3".       tran
+00007f30: 7366 6f72 6d3d 226d 6174 7269 7828 322e  sform="matrix(2.
+00007f40: 3735 3131 3931 392c 302c 302c 322e 3733  7511919,0,0,2.73
+00007f50: 3838 3132 2c33 3734 2e30 3233 3331 2c2d  8812,374.02331,-
+00007f60: 3130 382e 3038 3836 3629 223e 3c74 7370  108.08866)"><tsp
+00007f70: 616e 0a20 2020 2020 2020 2020 736f 6469  an.         sodi
+00007f80: 706f 6469 3a72 6f6c 653d 226c 696e 6522  podi:role="line"
+00007f90: 0a20 2020 2020 2020 2020 6964 3d22 7473  .         id="ts
+00007fa0: 7061 6e31 3436 3839 2d32 2d37 220a 2020  pan14689-2-7".  
+00007fb0: 2020 2020 2020 2078 3d22 3737 2e36 3934         x="77.694
+00007fc0: 3839 3322 0a20 2020 2020 2020 2020 793d  893".         y=
+00007fd0: 2239 312e 3938 3834 3439 220a 2020 2020  "91.988449".    
+00007fe0: 2020 2020 2073 7479 6c65 3d22 666f 6e74       style="font
+00007ff0: 2d73 7479 6c65 3a6e 6f72 6d61 6c3b 666f  -style:normal;fo
+00008000: 6e74 2d76 6172 6961 6e74 3a6e 6f72 6d61  nt-variant:norma
+00008010: 6c3b 666f 6e74 2d77 6569 6768 743a 6e6f  l;font-weight:no
+00008020: 726d 616c 3b66 6f6e 742d 7374 7265 7463  rmal;font-stretc
+00008030: 683a 6e6f 726d 616c 3b66 6f6e 742d 7369  h:normal;font-si
+00008040: 7a65 3a32 312e 3335 3670 783b 666f 6e74  ze:21.356px;font
+00008050: 2d66 616d 696c 793a 496d 7061 6374 3b2d  -family:Impact;-
+00008060: 696e 6b73 6361 7065 2d66 6f6e 742d 7370  inkscape-font-sp
+00008070: 6563 6966 6963 6174 696f 6e3a 496d 7061  ecification:Impa
+00008080: 6374 3b66 696c 6c3a 2335 3435 3435 343b  ct;fill:#545454;
+00008090: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+000080a0: 7472 6f6b 652d 7769 6474 683a 302e 3430  troke-width:0.40
+000080b0: 3034 3235 223e 5361 656e 6f70 793c 2f74  0425">Saenopy</t
+000080c0: 7370 616e 3e3c 2f74 6578 743e 0a20 2020  span></text>.   
+000080d0: 203c 7465 7874 0a20 2020 2020 2020 786d   <text.       xm
+000080e0: 6c3a 7370 6163 653d 2270 7265 7365 7276  l:space="preserv
+000080f0: 6522 0a20 2020 2020 2020 7374 796c 653d  e".       style=
+00008100: 2266 6f6e 742d 7374 796c 653a 6e6f 726d  "font-style:norm
+00008110: 616c 3b66 6f6e 742d 7765 6967 6874 3a6e  al;font-weight:n
+00008120: 6f72 6d61 6c3b 666f 6e74 2d73 697a 653a  ormal;font-size:
+00008130: 3136 2e31 3231 3170 783b 6c69 6e65 2d68  16.1211px;line-h
+00008140: 6569 6768 743a 312e 3235 3b66 6f6e 742d  eight:1.25;font-
+00008150: 6661 6d69 6c79 3a73 616e 732d 7365 7269  family:sans-seri
+00008160: 663b 6c65 7474 6572 2d73 7061 6369 6e67  f;letter-spacing
+00008170: 3a30 7078 3b77 6f72 642d 7370 6163 696e  :0px;word-spacin
+00008180: 673a 3070 783b 6669 6c6c 3a23 6666 6666  g:0px;fill:#ffff
+00008190: 6666 3b66 696c 6c2d 6f70 6163 6974 793a  ff;fill-opacity:
+000081a0: 313b 7374 726f 6b65 3a6e 6f6e 653b 7374  1;stroke:none;st
+000081b0: 726f 6b65 2d77 6964 7468 3a31 2e30 3939  roke-width:1.099
+000081c0: 3137 220a 2020 2020 2020 2078 3d22 3538  17".       x="58
+000081d0: 342e 3436 3535 3222 0a20 2020 2020 2020  4.46552".       
+000081e0: 793d 2231 3336 2e33 3837 3722 0a20 2020  y="136.3877".   
+000081f0: 2020 2020 6964 3d22 7465 7874 3134 3639      id="text1469
+00008200: 312d 3522 0a20 2020 2020 2020 7472 616e  1-5".       tran
+00008210: 7366 6f72 6d3d 2273 6361 6c65 2831 2e30  sform="scale(1.0
+00008220: 3032 3235 3735 2c30 2e39 3937 3734 3735  022575,0.9977475
+00008230: 3829 223e 3c74 7370 616e 0a20 2020 2020  8)"><tspan.     
+00008240: 2020 2020 736f 6469 706f 6469 3a72 6f6c      sodipodi:rol
+00008250: 653d 226c 696e 6522 0a20 2020 2020 2020  e="line".       
+00008260: 2020 6964 3d22 7473 7061 6e31 3436 3839    id="tspan14689
+00008270: 2d39 220a 2020 2020 2020 2020 2078 3d22  -9".         x="
+00008280: 3538 342e 3436 3535 3222 0a20 2020 2020  584.46552".     
+00008290: 2020 2020 793d 2231 3336 2e33 3837 3722      y="136.3877"
+000082a0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000082b0: 2266 6f6e 742d 7374 796c 653a 6e6f 726d  "font-style:norm
+000082c0: 616c 3b66 6f6e 742d 7661 7269 616e 743a  al;font-variant:
+000082d0: 6e6f 726d 616c 3b66 6f6e 742d 7765 6967  normal;font-weig
+000082e0: 6874 3a6e 6f72 6d61 6c3b 666f 6e74 2d73  ht:normal;font-s
+000082f0: 7472 6574 6368 3a6e 6f72 6d61 6c3b 666f  tretch:normal;fo
+00008300: 6e74 2d73 697a 653a 3538 2e36 3232 3170  nt-size:58.6221p
+00008310: 783b 666f 6e74 2d66 616d 696c 793a 2754  x;font-family:'T
+00008320: 6c77 6720 5479 7069 7374 273b 2d69 6e6b  lwg Typist';-ink
+00008330: 7363 6170 652d 666f 6e74 2d73 7065 6369  scape-font-speci
+00008340: 6669 6361 7469 6f6e 3a27 546c 7767 2054  fication:'Tlwg T
+00008350: 7970 6973 7427 3b73 7472 6f6b 652d 7769  ypist';stroke-wi
+00008360: 6474 683a 312e 3039 3931 373b 6669 6c6c  dth:1.09917;fill
+00008370: 3a23 6666 6666 6666 3b66 696c 6c2d 6f70  :#ffffff;fill-op
+00008380: 6163 6974 793a 3122 3e53 6165 6e6f 7079  acity:1">Saenopy
+00008390: 3c2f 7473 7061 6e3e 3c2f 7465 7874 3e0a  </tspan></text>.
+000083a0: 2020 2020 3c67 0a20 2020 2020 2020 6964      <g.       id
+000083b0: 3d22 6731 3432 382d 372d 3822 0a20 2020  ="g1428-7-8".   
+000083c0: 2020 2020 7472 616e 7366 6f72 6d3d 2274      transform="t
+000083d0: 7261 6e73 6c61 7465 2839 3030 2e30 3030  ranslate(900.000
+000083e0: 3031 2922 3e0a 2020 2020 2020 3c72 6563  01)">.      <rec
+000083f0: 740a 2020 2020 2020 2020 2073 7479 6c65  t.         style
+00008400: 3d22 6669 6c6c 3a23 6666 6666 6666 3b73  ="fill:#ffffff;s
+00008410: 7472 6f6b 653a 6e6f 6e65 3b73 7472 6f6b  troke:none;strok
+00008420: 652d 7769 6474 683a 352e 3038 3437 363b  e-width:5.08476;
+00008430: 7374 726f 6b65 2d6c 696e 6563 6170 3a72  stroke-linecap:r
+00008440: 6f75 6e64 3b73 7472 6f6b 652d 6c69 6e65  ound;stroke-line
+00008450: 6a6f 696e 3a72 6f75 6e64 220a 2020 2020  join:round".    
+00008460: 2020 2020 2069 643d 2272 6563 7437 3036       id="rect706
+00008470: 2d35 2d39 220a 2020 2020 2020 2020 2077  -5-9".         w
+00008480: 6964 7468 3d22 3430 3022 0a20 2020 2020  idth="400".     
+00008490: 2020 2020 6865 6967 6874 3d22 3230 3022      height="200"
+000084a0: 0a20 2020 2020 2020 2020 783d 222d 362e  .         x="-6.
+000084b0: 3639 3635 3133 3165 2d30 3622 0a20 2020  6965131e-06".   
+000084c0: 2020 2020 2020 793d 222d 312e 3835 3230        y="-1.8520
+000084d0: 3631 3165 2d30 3622 0a20 2020 2020 2020  611e-06".       
+000084e0: 2020 7279 3d22 3022 202f 3e0a 2020 2020    ry="0" />.    
+000084f0: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00008500: 2073 7479 6c65 3d22 6669 6c6c 3a23 3030   style="fill:#00
+00008510: 3030 3030 3b66 696c 6c2d 6f70 6163 6974  0000;fill-opacit
+00008520: 793a 302e 3939 3834 3038 3b73 7472 6f6b  y:0.998408;strok
+00008530: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
+00008540: 2d77 6964 7468 3a30 2e35 3030 3032 3270  -width:0.500022p
+00008550: 783b 7374 726f 6b65 2d6c 696e 6563 6170  x;stroke-linecap
+00008560: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00008570: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00008580: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00008590: 2020 2020 2020 2064 3d22 4d20 3137 332e         d="M 173.
+000085a0: 3834 3831 312c 3839 2e30 3639 3531 2033  84811,89.06951 3
+000085b0: 3337 2e36 3530 3936 2c36 342e 3934 3937  37.65096,64.9497
+000085c0: 3120 3137 312e 3837 3434 352c 3830 2e37  1 171.87445,80.7
+000085d0: 3134 3336 205a 220a 2020 2020 2020 2020  1436 Z".        
+000085e0: 2069 643d 2270 6174 6831 3436 3537 2d33   id="path14657-3
+000085f0: 2d37 220a 2020 2020 2020 2020 2069 6e6b  -7".         ink
+00008600: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00008610: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+00008620: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00008630: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+00008640: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00008650: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00008660: 6669 6c6c 3a23 3365 3462 3737 3b66 696c  fill:#3e4b77;fil
+00008670: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00008680: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00008690: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
+000086a0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+000086b0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+000086c0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+000086d0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+000086e0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+000086f0: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00008700: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
+00008710: 3d22 4d20 3139 2e36 3033 3037 2c36 372e  ="M 19.60307,67.
+00008720: 3635 3639 2038 302e 3835 3830 3238 2c36  6569 80.858028,6
+00008730: 342e 3838 3531 3220 3132 312e 3130 3430  4.88512 121.1040
+00008740: 352c 3230 2e32 3834 3534 2043 2037 302e  5,20.28454 C 70.
+00008750: 3430 3235 3837 2c35 342e 3232 3837 3320  402587,54.22873 
+00008760: 3436 2e31 3739 3630 352c 3539 2e36 3736  46.179605,59.676
+00008770: 3337 2031 392e 3630 3330 372c 3637 2e36  37 19.60307,67.6
+00008780: 3536 3920 5a22 0a20 2020 2020 2020 2020  569 Z".         
+00008790: 6964 3d22 7061 7468 3134 3534 372d 352d  id="path14547-5-
+000087a0: 3322 0a20 2020 2020 2020 2020 696e 6b73  3".         inks
+000087b0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+000087c0: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+000087d0: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+000087e0: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
+000087f0: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+00008800: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00008810: 696c 6c3a 2331 6332 6336 383b 6669 6c6c  ill:#1c2c68;fill
+00008820: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00008830: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00008840: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00008850: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00008860: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00008870: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00008880: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00008890: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+000088a0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+000088b0: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
+000088c0: 226d 2038 302e 3835 3830 3238 2c36 342e  "m 80.858028,64.
+000088d0: 3838 3531 3220 3236 2e35 3737 3536 322c  88512 26.577562,
+000088e0: 362e 3034 3735 3420 3133 2e36 3638 3436  6.04754 13.66846
+000088f0: 2c2d 3530 2e36 3438 3132 207a 220a 2020  ,-50.64812 z".  
+00008900: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00008910: 3435 3439 2d36 2d36 220a 2020 2020 2020  4549-6-6".      
+00008920: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00008930: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+00008940: 2230 2220 2f3e 0a20 2020 2020 203c 7061  "0" />.      <pa
+00008950: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
+00008960: 653d 2266 696c 6c3a 2330 3630 3530 383b  e="fill:#060508;
+00008970: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00008980: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00008990: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+000089a0: 3035 3b73 7472 6f6b 652d 6c69 6e65 6361  05;stroke-lineca
+000089b0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+000089c0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+000089d0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+000089e0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+000089f0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00008a00: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00008a10: 2020 643d 224d 2031 3037 2e34 3335 3539    d="M 107.43559
+00008a20: 2c37 302e 3933 3236 3620 3137 382e 3536  ,70.93266 178.56
+00008a30: 3232 332c 3833 2e35 3331 3720 4320 3135  223,83.5317 C 15
+00008a40: 302e 3834 3534 312c 3638 2e39 3434 3937  0.84541,68.94497
+00008a50: 2031 3334 2e37 3935 3031 2c34 352e 3530   134.79501,45.50
+00008a60: 3935 3520 3132 312e 3130 3430 352c 3230  955 121.10405,20
+00008a70: 2e32 3834 3534 205a 220a 2020 2020 2020  .28454 Z".      
+00008a80: 2020 2069 643d 2270 6174 6831 3435 3531     id="path14551
+00008a90: 2d32 2d31 220a 2020 2020 2020 2020 2069  -2-1".         i
+00008aa0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+00008ab0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+00008ac0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+00008ad0: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
+00008ae0: 6322 202f 3e0a 2020 2020 2020 3c70 6174  c" />.      <pat
+00008af0: 680a 2020 2020 2020 2020 2073 7479 6c65  h.         style
+00008b00: 3d22 6669 6c6c 3a23 3237 3337 3733 3b66  ="fill:#273773;f
+00008b10: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00008b20: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00008b30: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00008b40: 353b 7374 726f 6b65 2d6c 696e 6563 6170  5;stroke-linecap
+00008b50: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00008b60: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00008b70: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00008b80: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00008b90: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00008ba0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+00008bb0: 2064 3d22 6d20 3139 2e36 3033 3037 2c36   d="m 19.60307,6
+00008bc0: 372e 3635 3639 2063 2031 332e 3437 3933  7.6569 c 13.4793
+00008bd0: 3132 2c37 2e36 3937 3820 3238 2e33 3431  12,7.6978 28.341
+00008be0: 3130 372c 3134 2e33 3336 3935 2033 332e  107,14.33695 33.
+00008bf0: 3431 3137 3936 2c32 382e 3437 3338 3220  411796,28.47382 
+00008c00: 6c20 3237 2e38 3433 3136 322c 2d33 312e  l 27.843162,-31.
+00008c10: 3234 3536 207a 220a 2020 2020 2020 2020  2456 z".        
+00008c20: 2069 643d 2270 6174 6831 3435 3533 2d39   id="path14553-9
+00008c30: 2d32 220a 2020 2020 2020 2020 2069 6e6b  -2".         ink
+00008c40: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00008c50: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+00008c60: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00008c70: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+00008c80: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00008c90: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00008ca0: 6669 6c6c 3a23 3134 3236 3732 3b66 696c  fill:#142672;fil
+00008cb0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00008cc0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00008cd0: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
+00008ce0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00008cf0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00008d00: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00008d10: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00008d20: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00008d30: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00008d40: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
+00008d50: 3d22 4d20 3533 2e30 3134 3836 362c 3936  ="M 53.014866,96
+00008d60: 2e31 3330 3732 2031 3738 2e35 3632 3233  .13072 178.56223
+00008d70: 2c38 332e 3533 3137 2038 302e 3835 3830  ,83.5317 80.8580
+00008d80: 3238 2c36 342e 3838 3531 3220 5a22 0a20  28,64.88512 Z". 
+00008d90: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00008da0: 3134 3535 352d 312d 3922 0a20 2020 2020  14555-1-9".     
+00008db0: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
+00008dc0: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
+00008dd0: 3d22 3022 202f 3e0a 2020 2020 2020 3c70  ="0" />.      <p
+00008de0: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
+00008df0: 6c65 3d22 6669 6c6c 3a23 3534 3636 3863  le="fill:#54668c
+00008e00: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00008e10: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00008e20: 7472 6f6b 652d 7769 6474 683a 312e 3035  troke-width:1.05
+00008e30: 3030 353b 7374 726f 6b65 2d6c 696e 6563  005;stroke-linec
+00008e40: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+00008e50: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00008e60: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00008e70: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00008e80: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+00008e90: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00008ea0: 2020 2064 3d22 6d20 3533 2e30 3134 3836     d="m 53.01486
+00008eb0: 362c 3936 2e31 3330 3732 2037 322e 3339  6,96.13072 72.39
+00008ec0: 3232 3234 2c37 2e35 3539 3434 2035 332e  2224,7.55944 53.
+00008ed0: 3135 3531 342c 2d32 302e 3135 3834 3620  15514,-20.15846 
+00008ee0: 7a22 0a20 2020 2020 2020 2020 6964 3d22  z".         id="
+00008ef0: 7061 7468 3134 3535 372d 322d 3322 0a20  path14557-2-3". 
+00008f00: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00008f10: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+00008f20: 7475 7265 3d22 3022 202f 3e0a 2020 2020  ture="0" />.    
+00008f30: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
+00008f40: 2073 7479 6c65 3d22 6669 6c6c 3a23 3232   style="fill:#22
+00008f50: 3334 3765 3b66 696c 6c2d 6f70 6163 6974  347e;fill-opacit
+00008f60: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+00008f70: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+00008f80: 312e 3035 3030 353b 7374 726f 6b65 2d6c  1.05005;stroke-l
+00008f90: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00008fa0: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00008fb0: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+00008fc0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00008fd0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00008fe0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00008ff0: 2020 2020 2020 2064 3d22 6d20 3533 2e30         d="m 53.0
+00009000: 3134 3836 362c 3936 2e31 3330 3732 2063  14866,96.13072 c
+00009010: 2031 2e36 3237 3832 352c 3133 2e39 3732   1.627825,13.972
+00009020: 3532 202d 342e 3030 3637 3732 2c32 322e  52 -4.006772,22.
+00009030: 3738 3039 3320 2d36 2e35 3831 3130 392c  78093 -6.581109,
+00009040: 3333 2e37 3635 3431 206c 2037 382e 3937  33.76541 l 78.97
+00009050: 3333 3333 2c2d 3236 2e32 3035 3937 207a  3333,-26.20597 z
+00009060: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00009070: 6174 6831 3435 3539 2d37 2d31 220a 2020  ath14559-7-1".  
+00009080: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00009090: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+000090a0: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
+000090b0: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+000090c0: 7065 733d 2263 6363 6322 202f 3e0a 2020  pes="cccc" />.  
+000090d0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+000090e0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+000090f0: 3038 3130 3639 3b66 696c 6c2d 6f70 6163  081069;fill-opac
+00009100: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+00009110: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+00009120: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
+00009130: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00009140: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00009150: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+00009160: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+00009170: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+00009180: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00009190: 2020 2020 2020 2020 2064 3d22 4d20 3436           d="M 46
+000091a0: 2e34 3333 3735 372c 3132 392e 3839 3631  .433757,129.8961
+000091b0: 3320 3130 312e 3130 3736 2c31 3337 2e39  3 101.1076,137.9
+000091c0: 3539 3531 2031 3738 2e35 3632 3233 2c38  5951 178.56223,8
+000091d0: 332e 3533 3137 205a 220a 2020 2020 2020  3.5317 Z".      
+000091e0: 2020 2069 643d 2270 6174 6831 3435 3631     id="path14561
+000091f0: 2d30 2d39 220a 2020 2020 2020 2020 2069  -0-9".         i
+00009200: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+00009210: 722d 6375 7276 6174 7572 653d 2230 2220  r-curvature="0" 
+00009220: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+00009230: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+00009240: 696c 6c3a 2330 3730 6532 623b 6669 6c6c  ill:#070e2b;fill
+00009250: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+00009260: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+00009270: 2d77 6964 7468 3a31 2e30 3530 3035 3b73  -width:1.05005;s
+00009280: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00009290: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+000092a0: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+000092b0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+000092c0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+000092d0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+000092e0: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
+000092f0: 226d 2031 3031 2e31 3037 362c 3133 372e  "m 101.1076,137.
+00009300: 3935 3935 3120 3332 2e31 3436 3139 2c34  95951 32.14619,4
+00009310: 322e 3038 3037 3920 2d31 312e 3839 3636  2.08079 -11.8966
+00009320: 322c 2d35 362e 3639 3536 3620 7a22 0a20  2,-56.69566 z". 
+00009330: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00009340: 3134 3536 332d 392d 3422 0a20 2020 2020  14563-9-4".     
+00009350: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
+00009360: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
+00009370: 3d22 3022 202f 3e0a 2020 2020 2020 3c70  ="0" />.      <p
+00009380: 6174 680a 2020 2020 2020 2020 2073 7479  ath.         sty
+00009390: 6c65 3d22 6669 6c6c 3a23 3238 3364 3837  le="fill:#283d87
+000093a0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+000093b0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+000093c0: 7472 6f6b 652d 7769 6474 683a 312e 3035  troke-width:1.05
+000093d0: 3030 353b 7374 726f 6b65 2d6c 696e 6563  005;stroke-linec
+000093e0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+000093f0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00009400: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00009410: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00009420: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+00009430: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00009440: 2020 2064 3d22 6d20 3132 312e 3335 3731     d="m 121.3571
+00009450: 372c 3132 332e 3334 3436 3420 3131 2e38  7,123.34464 11.8
+00009460: 3936 3632 2c35 362e 3639 3536 3620 6320  9662,56.69566 c 
+00009470: 362e 3135 3836 322c 2d35 302e 3936 3637  6.15862,-50.9667
+00009480: 3320 3237 2e38 3331 3437 2c2d 3639 2e33  3 27.83147,-69.3
+00009490: 3238 3631 2034 352e 3330 3834 342c 2d39  2861 45.30844,-9
+000094a0: 362e 3530 3836 207a 220a 2020 2020 2020  6.5086 z".      
+000094b0: 2020 2069 643d 2270 6174 6831 3435 3635     id="path14565
+000094c0: 2d33 2d37 220a 2020 2020 2020 2020 2069  -3-7".         i
+000094d0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+000094e0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+000094f0: 2020 2020 2020 2020 2073 6f64 6970 6f64           sodipod
+00009500: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
+00009510: 6322 202f 3e0a 2020 2020 2020 3c65 6c6c  c" />.      <ell
+00009520: 6970 7365 0a20 2020 2020 2020 2020 7374  ipse.         st
+00009530: 796c 653d 2266 696c 6c3a 2330 3730 6532  yle="fill:#070e2
+00009540: 623b 6669 6c6c 2d6f 7061 6369 7479 3a30  b;fill-opacity:0
+00009550: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
+00009560: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00009570: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
+00009580: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00009590: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+000095a0: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
+000095b0: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+000095c0: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+000095d0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+000095e0: 3637 2d36 302d 3822 0a20 2020 2020 2020  67-60-8".       
+000095f0: 2020 6378 3d22 3230 2e39 3033 3131 3822    cx="20.903118"
+00009600: 0a20 2020 2020 2020 2020 6379 3d22 3637  .         cy="67
+00009610: 2e37 3231 3538 3822 0a20 2020 2020 2020  .721588".       
+00009620: 2020 7278 3d22 332e 3135 3632 3236 3422    rx="3.1562264"
+00009630: 0a20 2020 2020 2020 2020 7279 3d22 332e  .         ry="3.
+00009640: 3134 3230 3234 2220 2f3e 0a20 2020 2020  142024" />.     
+00009650: 203c 656c 6c69 7073 650a 2020 2020 2020   <ellipse.      
+00009660: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00009670: 3235 3361 3764 3b66 696c 6c2d 6f70 6163  253a7d;fill-opac
+00009680: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+00009690: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+000096a0: 683a 312e 3035 3030 353b 7374 726f 6b65  h:1.05005;stroke
+000096b0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+000096c0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+000096d0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+000096e0: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+000096f0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00009700: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
+00009710: 2d33 2d36 2d34 220a 2020 2020 2020 2020  -3-6-4".        
+00009720: 2063 783d 2234 352e 3932 3538 3436 220a   cx="45.925846".
+00009730: 2020 2020 2020 2020 2063 793d 2231 3239           cy="129
+00009740: 2e32 3235 3838 220a 2020 2020 2020 2020  .22588".        
+00009750: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+00009760: 6f72 6d2d 6365 6e74 6572 2d78 3d22 322e  orm-center-x="2.
+00009770: 3332 3639 3734 3522 0a20 2020 2020 2020  3269745".       
+00009780: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00009790: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
+000097a0: 342e 3937 3830 3136 3322 0a20 2020 2020  4.9780163".     
+000097b0: 2020 2020 7278 3d22 332e 3135 3632 3236      rx="3.156226
+000097c0: 3422 0a20 2020 2020 2020 2020 7279 3d22  4".         ry="
+000097d0: 332e 3134 3230 3234 2220 2f3e 0a20 2020  3.142024" />.   
+000097e0: 2020 203c 656c 6c69 7073 650a 2020 2020     <ellipse.    
+000097f0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00009800: 3a23 3235 3361 3764 3b66 696c 6c2d 6f70  :#253a7d;fill-op
+00009810: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+00009820: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00009830: 6474 683a 312e 3035 3030 353b 7374 726f  dth:1.05005;stro
+00009840: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00009850: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00009860: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
+00009870: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+00009880: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00009890: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+000098a0: 3637 2d33 2d37 2d32 2d35 220a 2020 2020  67-3-7-2-5".    
+000098b0: 2020 2020 2063 783d 2231 3230 2e35 3838       cx="120.588
+000098c0: 3632 220a 2020 2020 2020 2020 2063 793d  62".         cy=
+000098d0: 2231 3033 2e38 3931 3339 220a 2020 2020  "103.89139".    
+000098e0: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+000098f0: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
+00009900: 3d22 322e 3332 3639 3739 3222 0a20 2020  ="2.3269792".   
+00009910: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+00009920: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+00009930: 793d 222d 342e 3937 3830 3230 3422 0a20  y="-4.9780204". 
+00009940: 2020 2020 2020 2020 7278 3d22 332e 3135          rx="3.15
+00009950: 3632 3236 3422 0a20 2020 2020 2020 2020  62264".         
+00009960: 7279 3d22 332e 3134 3230 3234 2220 2f3e  ry="3.142024" />
+00009970: 0a20 2020 2020 203c 656c 6c69 7073 650a  .      <ellipse.
+00009980: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00009990: 6669 6c6c 3a23 6138 6139 6161 3b66 696c  fill:#a8a9aa;fil
+000099a0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+000099b0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+000099c0: 652d 7769 6474 683a 312e 3035 3030 353b  e-width:1.05005;
+000099d0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+000099e0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+000099f0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00009a00: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+00009a10: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00009a20: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
+00009a30: 6831 3435 3637 2d33 2d35 2d36 2d30 220a  h14567-3-5-6-0".
+00009a40: 2020 2020 2020 2020 2063 783d 2231 3231           cx="121
+00009a50: 2e33 3337 3134 220a 2020 2020 2020 2020  .33714".        
+00009a60: 2063 793d 2231 3232 2e38 3932 3234 220a   cy="122.89224".
+00009a70: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00009a80: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+00009a90: 6572 2d78 3d22 322e 3332 3639 3637 220a  er-x="2.326967".
+00009aa0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00009ab0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+00009ac0: 6572 2d79 3d22 2d34 2e39 3738 3030 3539  er-y="-4.9780059
+00009ad0: 220a 2020 2020 2020 2020 2072 783d 2233  ".         rx="3
+00009ae0: 2e31 3536 3232 3634 220a 2020 2020 2020  .1562264".      
+00009af0: 2020 2072 793d 2233 2e31 3432 3032 3422     ry="3.142024"
+00009b00: 202f 3e0a 2020 2020 2020 3c65 6c6c 6970   />.      <ellip
+00009b10: 7365 0a20 2020 2020 2020 2020 7374 796c  se.         styl
+00009b20: 653d 2266 696c 6c3a 2361 6261 6139 633b  e="fill:#abaa9c;
+00009b30: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+00009b40: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+00009b50: 726f 6b65 2d77 6964 7468 3a31 2e30 3530  roke-width:1.050
+00009b60: 3035 3b73 7472 6f6b 652d 6d69 7465 726c  05;stroke-miterl
+00009b70: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00009b80: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00009b90: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+00009ba0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00009bb0: 3122 0a20 2020 2020 2020 2020 6964 3d22  1".         id="
+00009bc0: 7061 7468 3134 3536 372d 332d 392d 312d  path14567-3-9-1-
+00009bd0: 3322 0a20 2020 2020 2020 2020 6378 3d22  3".         cx="
+00009be0: 3130 312e 3837 3631 3422 0a20 2020 2020  101.87614".     
+00009bf0: 2020 2020 6379 3d22 3133 372e 3739 3438      cy="137.7948
+00009c00: 3522 0a20 2020 2020 2020 2020 696e 6b73  5".         inks
+00009c10: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
+00009c20: 656e 7465 722d 783d 2232 2e33 3236 3937  enter-x="2.32697
+00009c30: 3322 0a20 2020 2020 2020 2020 696e 6b73  3".         inks
+00009c40: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
+00009c50: 656e 7465 722d 793d 222d 342e 3937 3830  enter-y="-4.9780
+00009c60: 3235 3122 0a20 2020 2020 2020 2020 7278  251".         rx
+00009c70: 3d22 332e 3135 3632 3236 3422 0a20 2020  ="3.1562264".   
+00009c80: 2020 2020 2020 7279 3d22 332e 3134 3230        ry="3.1420
+00009c90: 3234 2220 2f3e 0a20 2020 2020 203c 656c  24" />.      <el
+00009ca0: 6c69 7073 650a 2020 2020 2020 2020 2073  lipse.         s
+00009cb0: 7479 6c65 3d22 6669 6c6c 3a23 3131 3230  tyle="fill:#1120
+00009cc0: 3636 3b66 696c 6c2d 6f70 6163 6974 793a  66;fill-opacity:
+00009cd0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00009ce0: 3b73 7472 6f6b 652d 7769 6474 683a 312e  ;stroke-width:1.
+00009cf0: 3035 3030 353b 7374 726f 6b65 2d6d 6974  05005;stroke-mit
+00009d00: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00009d10: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00009d20: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00009d30: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+00009d40: 7479 3a31 220a 2020 2020 2020 2020 2069  ty:1".         i
+00009d50: 643d 2270 6174 6831 3435 3637 2d33 2d32  d="path14567-3-2
+00009d60: 2d38 2d36 220a 2020 2020 2020 2020 2063  -8-6".         c
+00009d70: 783d 2238 312e 3239 3234 3139 220a 2020  x="81.292419".  
+00009d80: 2020 2020 2020 2063 793d 2236 342e 3231         cy="64.21
+00009d90: 3331 3635 220a 2020 2020 2020 2020 2069  3165".         i
+00009da0: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00009db0: 6d2d 6365 6e74 6572 2d78 3d22 332e 3539  m-center-x="3.59
+00009dc0: 3133 3630 3922 0a20 2020 2020 2020 2020  13609".         
+00009dd0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+00009de0: 726d 2d63 656e 7465 722d 793d 222d 372e  rm-center-y="-7.
+00009df0: 3638 3238 3935 3622 0a20 2020 2020 2020  6828956".       
+00009e00: 2020 7278 3d22 342e 3837 3131 3932 3922    rx="4.8711929"
+00009e10: 0a20 2020 2020 2020 2020 7279 3d22 342e  .         ry="4.
+00009e20: 3834 3932 3733 3722 202f 3e0a 2020 2020  8492737" />.    
+00009e30: 2020 3c65 6c6c 6970 7365 0a20 2020 2020    <ellipse.     
+00009e40: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00009e50: 2365 6466 3066 633b 6669 6c6c 2d6f 7061  #edf0fc;fill-opa
+00009e60: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
+00009e70: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00009e80: 6f6b 652d 7769 6474 683a 312e 3035 3030  oke-width:1.0500
+00009e90: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+00009ea0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00009eb0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00009ec0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+00009ed0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00009ee0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+00009ef0: 6174 6831 3435 3637 2d32 2d37 392d 3122  ath14567-2-79-1"
+00009f00: 0a20 2020 2020 2020 2020 6378 3d22 3130  .         cx="10
+00009f10: 372e 3637 3730 3222 0a20 2020 2020 2020  7.67702".       
+00009f20: 2020 6379 3d22 3639 2e36 3135 3335 3622    cy="69.615356"
+00009f30: 0a20 2020 2020 2020 2020 7278 3d22 332e  .         rx="3.
+00009f40: 3135 3632 3236 3422 0a20 2020 2020 2020  1562264".       
+00009f50: 2020 7279 3d22 332e 3134 3230 3234 2220    ry="3.142024" 
+00009f60: 2f3e 0a20 2020 2020 203c 656c 6c69 7073  />.      <ellips
+00009f70: 650a 2020 2020 2020 2020 2073 7479 6c65  e.         style
+00009f80: 3d22 6669 6c6c 3a23 6564 6630 6663 3b66  ="fill:#edf0fc;f
+00009f90: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+00009fa0: 3034 3436 3b73 7472 6f6b 653a 2366 6666  0446;stroke:#fff
+00009fb0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00009fc0: 3a31 2e30 3530 3035 3b73 7472 6f6b 652d  :1.05005;stroke-
+00009fd0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00009fe0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00009ff0: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+0000a000: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+0000a010: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000a020: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+0000a030: 322d 382d 322d 3022 0a20 2020 2020 2020  2-8-2-0".       
+0000a040: 2020 6378 3d22 3533 2e30 3336 3537 3522    cx="53.036575"
+0000a050: 0a20 2020 2020 2020 2020 6379 3d22 3935  .         cy="95
+0000a060: 2e36 3934 3937 3722 0a20 2020 2020 2020  .694977".       
+0000a070: 2020 7278 3d22 332e 3135 3632 3236 3422    rx="3.1562264"
+0000a080: 0a20 2020 2020 2020 2020 7279 3d22 332e  .         ry="3.
+0000a090: 3134 3230 3234 2220 2f3e 0a20 2020 2020  142024" />.     
+0000a0a0: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+0000a0b0: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+0000a0c0: 3030 303b 6669 6c6c 2d6f 7061 6369 7479  000;fill-opacity
+0000a0d0: 3a30 2e39 3938 3430 383b 7374 726f 6b65  :0.998408;stroke
+0000a0e0: 3a23 3030 3030 3030 3b73 7472 6f6b 652d  :#000000;stroke-
+0000a0f0: 7769 6474 683a 302e 3332 3335 3838 7078  width:0.323588px
+0000a100: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+0000a110: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+0000a120: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+0000a130: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000a140: 2020 2020 2020 643d 226d 2033 3138 2e37        d="m 318.7
+0000a150: 3031 3333 2c37 322e 3730 3137 3220 3236  0133,72.70172 26
+0000a160: 2e36 3034 3537 2c2d 382e 3738 3638 3320  .60457,-8.78683 
+0000a170: 2d32 382e 3338 3339 352c 2d31 2e34 3735  -28.38395,-1.475
+0000a180: 3836 2063 2031 312e 3030 3532 362c 332e  86 c 11.00526,3.
+0000a190: 3230 3436 3620 3131 2e30 3535 332c 332e  20466 11.0553,3.
+0000a1a0: 3337 3432 3720 312e 3737 3933 382c 3130  37427 1.77938,10
+0000a1b0: 2e32 3632 3639 207a 220a 2020 2020 2020  .26269 z".      
+0000a1c0: 2020 2069 643d 2270 6174 6831 3436 3537     id="path14657
+0000a1d0: 2d39 2d30 2d36 220a 2020 2020 2020 2020  -9-0-6".        
+0000a1e0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+0000a1f0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+0000a200: 220a 2020 2020 2020 2020 2073 6f64 6970  ".         sodip
+0000a210: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+0000a220: 6363 6322 202f 3e0a 2020 2020 2020 3c65  ccc" />.      <e
+0000a230: 6c6c 6970 7365 0a20 2020 2020 2020 2020  llipse.         
+0000a240: 7374 796c 653d 2266 696c 6c3a 2365 6466  style="fill:#edf
+0000a250: 3066 633b 6669 6c6c 2d6f 7061 6369 7479  0fc;fill-opacity
+0000a260: 3a30 2e39 3930 3434 363b 7374 726f 6b65  :0.990446;stroke
+0000a270: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+0000a280: 7769 6474 683a 312e 3939 3539 383b 7374  width:1.99598;st
+0000a290: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000a2a0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000a2b0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+0000a2c0: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+0000a2d0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+0000a2e0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000a2f0: 3435 3637 2d32 2d37 2d32 2d33 220a 2020  4567-2-7-2-3".  
+0000a300: 2020 2020 2020 2063 783d 2231 3737 2e34         cx="177.4
+0000a310: 3734 3536 220a 2020 2020 2020 2020 2063  7456".         c
+0000a320: 793d 2238 342e 3333 3137 3236 220a 2020  y="84.331726".  
+0000a330: 2020 2020 2020 2072 783d 2235 2e39 3939         rx="5.999
+0000a340: 3532 3232 220a 2020 2020 2020 2020 2072  5222".         r
+0000a350: 793d 2235 2e39 3732 3532 3536 2220 2f3e  y="5.9725256" />
+0000a360: 0a20 2020 2020 203c 7465 7874 0a20 2020  .      <text.   
+0000a370: 2020 2020 2020 786d 6c3a 7370 6163 653d        xml:space=
+0000a380: 2270 7265 7365 7276 6522 0a20 2020 2020  "preserve".     
+0000a390: 2020 2020 7374 796c 653d 2266 6f6e 742d      style="font-
+0000a3a0: 7374 796c 653a 6e6f 726d 616c 3b66 6f6e  style:normal;fon
+0000a3b0: 742d 7765 6967 6874 3a6e 6f72 6d61 6c3b  t-weight:normal;
+0000a3c0: 666f 6e74 2d73 697a 653a 352e 3837 3239  font-size:5.8729
+0000a3d0: 3170 783b 6c69 6e65 2d68 6569 6768 743a  1px;line-height:
+0000a3e0: 312e 3235 3b66 6f6e 742d 6661 6d69 6c79  1.25;font-family
+0000a3f0: 3a73 616e 732d 7365 7269 663b 6c65 7474  :sans-serif;lett
+0000a400: 6572 2d73 7061 6369 6e67 3a30 7078 3b77  er-spacing:0px;w
+0000a410: 6f72 642d 7370 6163 696e 673a 3070 783b  ord-spacing:0px;
+0000a420: 6669 6c6c 3a23 6666 6666 6666 3b66 696c  fill:#ffffff;fil
+0000a430: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+0000a440: 6b65 3a6e 6f6e 653b 7374 726f 6b65 2d77  ke:none;stroke-w
+0000a450: 6964 7468 3a30 2e34 3030 3432 353b 6669  idth:0.400425;fi
+0000a460: 6c74 6572 3a75 726c 2823 6669 6c74 6572  lter:url(#filter
+0000a470: 3135 3035 312d 332d 3229 220a 2020 2020  15051-3-2)".    
+0000a480: 2020 2020 2078 3d22 3737 2e36 3934 3839       x="77.69489
+0000a490: 3322 0a20 2020 2020 2020 2020 793d 2239  3".         y="9
+0000a4a0: 312e 3938 3834 3439 220a 2020 2020 2020  1.988449".      
+0000a4b0: 2020 2069 643d 2274 6578 7431 3436 3931     id="text14691
+0000a4c0: 2d36 2d33 2d32 220a 2020 2020 2020 2020  -6-3-2".        
+0000a4d0: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
+0000a4e0: 6978 2832 2e37 3531 3139 3139 2c30 2c30  ix(2.7511919,0,0
+0000a4f0: 2c32 2e37 3338 3831 322c 2d37 352e 3937  ,2.738812,-75.97
+0000a500: 3636 3936 2c2d 3130 382e 3038 3836 3629  6696,-108.08866)
+0000a510: 223e 3c74 7370 616e 0a20 2020 2020 2020  "><tspan.       
+0000a520: 2020 2020 736f 6469 706f 6469 3a72 6f6c      sodipodi:rol
+0000a530: 653d 226c 696e 6522 0a20 2020 2020 2020  e="line".       
+0000a540: 2020 2020 6964 3d22 7473 7061 6e31 3436      id="tspan146
+0000a550: 3839 2d32 2d37 2d30 220a 2020 2020 2020  89-2-7-0".      
+0000a560: 2020 2020 2078 3d22 3737 2e36 3934 3839       x="77.69489
+0000a570: 3322 0a20 2020 2020 2020 2020 2020 793d  3".           y=
+0000a580: 2239 312e 3938 3834 3439 220a 2020 2020  "91.988449".    
+0000a590: 2020 2020 2020 2073 7479 6c65 3d22 666f         style="fo
+0000a5a0: 6e74 2d73 7479 6c65 3a6e 6f72 6d61 6c3b  nt-style:normal;
+0000a5b0: 666f 6e74 2d76 6172 6961 6e74 3a6e 6f72  font-variant:nor
+0000a5c0: 6d61 6c3b 666f 6e74 2d77 6569 6768 743a  mal;font-weight:
+0000a5d0: 6e6f 726d 616c 3b66 6f6e 742d 7374 7265  normal;font-stre
+0000a5e0: 7463 683a 6e6f 726d 616c 3b66 6f6e 742d  tch:normal;font-
+0000a5f0: 7369 7a65 3a32 312e 3335 3670 783b 666f  size:21.356px;fo
+0000a600: 6e74 2d66 616d 696c 793a 496d 7061 6374  nt-family:Impact
+0000a610: 3b2d 696e 6b73 6361 7065 2d66 6f6e 742d  ;-inkscape-font-
+0000a620: 7370 6563 6966 6963 6174 696f 6e3a 496d  specification:Im
+0000a630: 7061 6374 3b66 696c 6c3a 2366 6666 6666  pact;fill:#fffff
+0000a640: 663b 6669 6c6c 2d6f 7061 6369 7479 3a31  f;fill-opacity:1
+0000a650: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+0000a660: 3430 3034 3235 223e 5361 656e 6f70 793c  400425">Saenopy<
+0000a670: 2f74 7370 616e 3e3c 2f74 6578 743e 0a20  /tspan></text>. 
+0000a680: 2020 2020 203c 7465 7874 0a20 2020 2020       <text.     
+0000a690: 2020 2020 786d 6c3a 7370 6163 653d 2270      xml:space="p
+0000a6a0: 7265 7365 7276 6522 0a20 2020 2020 2020  reserve".       
+0000a6b0: 2020 7374 796c 653d 2266 6f6e 742d 7374    style="font-st
+0000a6c0: 796c 653a 6e6f 726d 616c 3b66 6f6e 742d  yle:normal;font-
+0000a6d0: 7765 6967 6874 3a6e 6f72 6d61 6c3b 666f  weight:normal;fo
+0000a6e0: 6e74 2d73 697a 653a 3136 2e31 3231 3170  nt-size:16.1211p
+0000a6f0: 783b 6c69 6e65 2d68 6569 6768 743a 312e  x;line-height:1.
+0000a700: 3235 3b66 6f6e 742d 6661 6d69 6c79 3a73  25;font-family:s
+0000a710: 616e 732d 7365 7269 663b 6c65 7474 6572  ans-serif;letter
+0000a720: 2d73 7061 6369 6e67 3a30 7078 3b77 6f72  -spacing:0px;wor
+0000a730: 642d 7370 6163 696e 673a 3070 783b 6669  d-spacing:0px;fi
+0000a740: 6c6c 3a23 3030 3030 3030 3b66 696c 6c2d  ll:#000000;fill-
+0000a750: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+0000a760: 3a6e 6f6e 653b 7374 726f 6b65 2d77 6964  :none;stroke-wid
+0000a770: 7468 3a31 2e30 3939 3137 220a 2020 2020  th:1.09917".    
+0000a780: 2020 2020 2078 3d22 3133 352e 3437 3930       x="135.4790
+0000a790: 3622 0a20 2020 2020 2020 2020 793d 2231  6".         y="1
+0000a7a0: 3336 2e33 3837 3722 0a20 2020 2020 2020  36.3877".       
+0000a7b0: 2020 6964 3d22 7465 7874 3134 3639 312d    id="text14691-
+0000a7c0: 352d 3622 0a20 2020 2020 2020 2020 7472  5-6".         tr
+0000a7d0: 616e 7366 6f72 6d3d 2273 6361 6c65 2831  ansform="scale(1
+0000a7e0: 2e30 3032 3235 3735 2c30 2e39 3937 3734  .0022575,0.99774
+0000a7f0: 3735 3829 223e 3c74 7370 616e 0a20 2020  758)"><tspan.   
+0000a800: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+0000a810: 3a72 6f6c 653d 226c 696e 6522 0a20 2020  :role="line".   
+0000a820: 2020 2020 2020 2020 6964 3d22 7473 7061          id="tspa
+0000a830: 6e31 3436 3839 2d39 2d31 220a 2020 2020  n14689-9-1".    
+0000a840: 2020 2020 2020 2078 3d22 3133 352e 3437         x="135.47
+0000a850: 3930 3622 0a20 2020 2020 2020 2020 2020  906".           
+0000a860: 793d 2231 3336 2e33 3837 3722 0a20 2020  y="136.3877".   
+0000a870: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+0000a880: 6f6e 742d 7374 796c 653a 6e6f 726d 616c  ont-style:normal
+0000a890: 3b66 6f6e 742d 7661 7269 616e 743a 6e6f  ;font-variant:no
+0000a8a0: 726d 616c 3b66 6f6e 742d 7765 6967 6874  rmal;font-weight
+0000a8b0: 3a6e 6f72 6d61 6c3b 666f 6e74 2d73 7472  :normal;font-str
+0000a8c0: 6574 6368 3a6e 6f72 6d61 6c3b 666f 6e74  etch:normal;font
+0000a8d0: 2d73 697a 653a 3538 2e36 3232 3170 783b  -size:58.6221px;
+0000a8e0: 666f 6e74 2d66 616d 696c 793a 2754 6c77  font-family:'Tlw
+0000a8f0: 6720 5479 7069 7374 273b 2d69 6e6b 7363  g Typist';-inksc
+0000a900: 6170 652d 666f 6e74 2d73 7065 6369 6669  ape-font-specifi
+0000a910: 6361 7469 6f6e 3a27 546c 7767 2054 7970  cation:'Tlwg Typ
+0000a920: 6973 7427 3b73 7472 6f6b 652d 7769 6474  ist';stroke-widt
+0000a930: 683a 312e 3039 3931 3722 3e53 6165 6e6f  h:1.09917">Saeno
+0000a940: 7079 3c2f 7473 7061 6e3e 3c2f 7465 7874  py</tspan></text
+0000a950: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
+0000a960: 670a 2020 2020 2020 2069 643d 2267 3930  g.       id="g90
+0000a970: 3422 0a20 2020 2020 2020 7472 616e 7366  4".       transf
+0000a980: 6f72 6d3d 226d 6174 7269 7828 322e 3638  orm="matrix(2.68
+0000a990: 3739 3734 332c 302c 302c 322e 3638 3739  79743,0,0,2.6879
+0000a9a0: 3734 332c 2d35 2e30 3034 3033 3135 2c2d  743,-5.0040315,-
+0000a9b0: 3939 2e39 3238 3839 3529 223e 0a20 2020  99.928895)">.   
+0000a9c0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+0000a9d0: 2020 7374 796c 653d 2266 696c 6c3a 2333    style="fill:#3
+0000a9e0: 6534 6237 373b 6669 6c6c 2d6f 7061 6369  e4b77;fill-opaci
+0000a9f0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+0000aa00: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+0000aa10: 3a30 2e35 3535 3632 353b 7374 726f 6b65  :0.555625;stroke
+0000aa20: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+0000aa30: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+0000aa40: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+0000aa50: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+0000aa60: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+0000aa70: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+0000aa80: 2020 2020 2020 2020 2064 3d22 6d20 352e           d="m 5.
+0000aa90: 3735 3834 3930 362c 3136 312e 3833 3635  7584906,161.8365
+0000aaa0: 3120 3332 2e33 3339 3632 3034 2c2d 312e  1 32.3396204,-1.
+0000aab0: 3436 3939 3820 3231 2e32 3437 3933 2c2d  46998 21.24793,-
+0000aac0: 3233 2e36 3533 3335 2063 202d 3236 2e37  23.65335 c -26.7
+0000aad0: 3637 3839 2c31 382e 3030 3138 3720 2d33  6789,18.00187 -3
+0000aae0: 392e 3535 3634 342c 3230 2e38 3930 3935  9.55644,20.89095
+0000aaf0: 202d 3533 2e35 3837 3535 3034 2c32 352e   -53.5875504,25.
+0000ab00: 3132 3333 3320 7a22 0a20 2020 2020 2020  12333 z".       
+0000ab10: 2020 6964 3d22 7061 7468 3134 3534 372d    id="path14547-
+0000ab20: 3122 0a20 2020 2020 2020 2020 696e 6b73  1".         inks
+0000ab30: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+0000ab40: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+0000ab50: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+0000ab60: 6f64 6574 7970 6573 3d22 6363 6363 220a  odetypes="cccc".
+0000ab70: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000ab80: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000ab90: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
+0000aba0: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000abb0: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
+0000abc0: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+0000abd0: 7374 796c 653d 2266 696c 6c3a 2331 6332  style="fill:#1c2
+0000abe0: 6336 383b 6669 6c6c 2d6f 7061 6369 7479  c68;fill-opacity
+0000abf0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+0000ac00: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+0000ac10: 2e35 3535 3632 353b 7374 726f 6b65 2d6c  .555625;stroke-l
+0000ac20: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+0000ac30: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+0000ac40: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+0000ac50: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000ac60: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000ac70: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+0000ac80: 2020 2020 2020 2064 3d22 6d20 3338 2e30         d="m 38.0
+0000ac90: 3938 3131 312c 3136 302e 3336 3635 3320  98111,160.36653 
+0000aca0: 3134 2e30 3331 3635 2c33 2e32 3037 3234  14.03165,3.20724
+0000acb0: 2037 2e32 3136 3238 2c2d 3236 2e38 3630   7.21628,-26.860
+0000acc0: 3539 207a 220a 2020 2020 2020 2020 2069  59 z".         i
+0000acd0: 643d 2270 6174 6831 3435 3439 2d31 220a  d="path14549-1".
+0000ace0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000acf0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+0000ad00: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+0000ad10: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000ad20: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+0000ad30: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000ad40: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+0000ad50: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+0000ad60: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+0000ad70: 2266 696c 6c3a 2330 3630 3530 383b 6669  "fill:#060508;fi
+0000ad80: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+0000ad90: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000ada0: 6b65 2d77 6964 7468 3a30 2e35 3535 3632  ke-width:0.55562
+0000adb0: 353b 7374 726f 6b65 2d6c 696e 6563 6170  5;stroke-linecap
+0000adc0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+0000add0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+0000ade0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+0000adf0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+0000ae00: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+0000ae10: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+0000ae20: 2064 3d22 6d20 3532 2e31 3239 3736 312c   d="m 52.129761,
+0000ae30: 3136 332e 3537 3337 3720 3337 2e35 3531  163.57377 37.551
+0000ae40: 3337 2c36 2e36 3831 3734 2063 202d 3134  37,6.68174 c -14
+0000ae50: 2e36 3333 3132 2c2d 372e 3733 3538 3920  .63312,-7.73589 
+0000ae60: 2d32 332e 3130 3639 342c 2d32 302e 3136  -23.10694,-20.16
+0000ae70: 3435 3620 2d33 302e 3333 3530 392c 2d33  456 -30.33509,-3
+0000ae80: 332e 3534 3233 3320 7a22 0a20 2020 2020  3.54233 z".     
+0000ae90: 2020 2020 6964 3d22 7061 7468 3134 3535      id="path1455
+0000aea0: 312d 3022 0a20 2020 2020 2020 2020 696e  1-0".         in
+0000aeb0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+0000aec0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+0000aed0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+0000aee0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+0000aef0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+0000af00: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000af10: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
+0000af20: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+0000af30: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+0000af40: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+0000af50: 2020 7374 796c 653d 2266 696c 6c3a 2332    style="fill:#2
+0000af60: 3733 3737 333b 6669 6c6c 2d6f 7061 6369  73773;fill-opaci
+0000af70: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+0000af80: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+0000af90: 3a30 2e35 3535 3632 353b 7374 726f 6b65  :0.555625;stroke
+0000afa0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+0000afb0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+0000afc0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+0000afd0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+0000afe0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+0000aff0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+0000b000: 2020 2020 2020 2020 2064 3d22 6d20 352e           d="m 5.
+0000b010: 3735 3834 3930 362c 3136 312e 3833 3635  7584906,161.8365
+0000b020: 3120 6320 372e 3131 3634 3230 342c 342e  1 c 7.1164204,4.
+0000b030: 3038 3234 3420 3134 2e39 3632 3732 3034  08244 14.9627204
+0000b040: 2c37 2e36 3033 3433 2031 372e 3633 3937  ,7.60343 17.6397
+0000b050: 3930 342c 3135 2e31 3030 3734 206c 2031  904,15.10074 l 1
+0000b060: 342e 3639 3938 332c 2d31 362e 3537 3037  4.69983,-16.5707
+0000b070: 3220 7a22 0a20 2020 2020 2020 2020 6964  2 z".         id
+0000b080: 3d22 7061 7468 3134 3535 332d 3322 0a20  ="path14553-3". 
+0000b090: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+0000b0a0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+0000b0b0: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
+0000b0c0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+0000b0d0: 7970 6573 3d22 6363 6363 220a 2020 2020  ypes="cccc".    
+0000b0e0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000b0f0: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+0000b100: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000b110: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+0000b120: 3030 2220 2f3e 0a20 2020 2020 203c 7061  00" />.      <pa
+0000b130: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
+0000b140: 653d 2266 696c 6c3a 2331 3432 3637 323b  e="fill:#142672;
+0000b150: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000b160: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000b170: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
+0000b180: 3632 353b 7374 726f 6b65 2d6c 696e 6563  625;stroke-linec
+0000b190: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000b1a0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000b1b0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000b1c0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000b1d0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000b1e0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000b1f0: 2020 2064 3d22 6d20 3233 2e33 3938 3238     d="m 23.39828
+0000b200: 312c 3137 362e 3933 3732 3520 3636 2e32  1,176.93725 66.2
+0000b210: 3832 3835 2c2d 362e 3638 3137 3420 2d35  8285,-6.68174 -5
+0000b220: 312e 3538 3330 322c 2d39 2e38 3838 3938  1.58302,-9.88898
+0000b230: 207a 220a 2020 2020 2020 2020 2069 643d   z".         id=
+0000b240: 2270 6174 6831 3435 3535 2d34 220a 2020  "path14555-4".  
+0000b250: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000b260: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+0000b270: 7572 653d 2230 220a 2020 2020 2020 2020  ure="0".        
+0000b280: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+0000b290: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+0000b2a0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000b2b0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+0000b2c0: 2f3e 0a20 2020 2020 203c 7061 7468 0a20  />.      <path. 
+0000b2d0: 2020 2020 2020 2020 7374 796c 653d 2266          style="f
+0000b2e0: 696c 6c3a 2335 3436 3638 633b 6669 6c6c  ill:#54668c;fill
+0000b2f0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+0000b300: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+0000b310: 2d77 6964 7468 3a30 2e35 3535 3632 353b  -width:0.555625;
+0000b320: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+0000b330: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+0000b340: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+0000b350: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000b360: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000b370: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+0000b380: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
+0000b390: 3d22 6d20 3233 2e33 3938 3238 312c 3137  ="m 23.398281,17
+0000b3a0: 362e 3933 3732 3520 3338 2e32 3139 3535  6.93725 38.21955
+0000b3b0: 2c34 2e30 3039 3034 2032 382e 3036 3333  ,4.00904 28.0633
+0000b3c0: 2c2d 3130 2e36 3930 3738 207a 220a 2020  ,-10.69078 z".  
+0000b3d0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000b3e0: 3435 3537 2d30 220a 2020 2020 2020 2020  4557-0".        
+0000b3f0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+0000b400: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+0000b410: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+0000b420: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000b430: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
+0000b440: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+0000b450: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+0000b460: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+0000b470: 2020 7374 796c 653d 2266 696c 6c3a 2332    style="fill:#2
+0000b480: 3233 3437 653b 6669 6c6c 2d6f 7061 6369  2347e;fill-opaci
+0000b490: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+0000b4a0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+0000b4b0: 3a30 2e35 3535 3632 353b 7374 726f 6b65  :0.555625;stroke
+0000b4c0: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+0000b4d0: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+0000b4e0: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+0000b4f0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+0000b500: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+0000b510: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+0000b520: 2020 2020 2020 2020 2064 3d22 6d20 3233           d="m 23
+0000b530: 2e33 3938 3238 312c 3137 362e 3933 3732  .398281,176.9372
+0000b540: 3520 6320 302e 3835 3934 322c 372e 3431  5 c 0.85942,7.41
+0000b550: 3031 3420 2d32 2e31 3135 3337 2c31 322e  014 -2.11537,12.
+0000b560: 3038 3135 3720 2d33 2e34 3734 352c 3137  08157 -3.4745,17
+0000b570: 2e39 3037 3035 206c 2034 312e 3639 3430  .90705 l 41.6940
+0000b580: 352c 2d31 332e 3839 3830 3120 7a22 0a20  5,-13.89801 z". 
+0000b590: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+0000b5a0: 3134 3535 392d 3322 0a20 2020 2020 2020  14559-3".       
+0000b5b0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000b5c0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000b5d0: 3022 0a20 2020 2020 2020 2020 736f 6469  0".         sodi
+0000b5e0: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
+0000b5f0: 6363 6363 220a 2020 2020 2020 2020 2069  cccc".         i
+0000b600: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+0000b610: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+0000b620: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000b630: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+0000b640: 0a20 2020 2020 203c 7061 7468 0a20 2020  .      <path.   
+0000b650: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+0000b660: 6c3a 2330 3831 3036 393b 6669 6c6c 2d6f  l:#081069;fill-o
+0000b670: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+0000b680: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+0000b690: 6964 7468 3a30 2e35 3535 3632 353b 7374  idth:0.555625;st
+0000b6a0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+0000b6b0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+0000b6c0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+0000b6d0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+0000b6e0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+0000b6f0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+0000b700: 3a31 220a 2020 2020 2020 2020 2064 3d22  :1".         d="
+0000b710: 6d20 3139 2e39 3233 3738 312c 3139 342e  m 19.923781,194.
+0000b720: 3834 3433 2032 382e 3836 3531 312c 342e  8443 28.86511,4.
+0000b730: 3237 3633 3220 3430 2e38 3932 3234 2c2d  27632 40.89224,-
+0000b740: 3238 2e38 3635 3131 207a 220a 2020 2020  28.86511 z".    
+0000b750: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+0000b760: 3631 2d39 220a 2020 2020 2020 2020 2069  61-9".         i
+0000b770: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+0000b780: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+0000b790: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000b7a0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000b7b0: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
+0000b7c0: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000b7d0: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
+0000b7e0: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+0000b7f0: 7374 796c 653d 2266 696c 6c3a 2330 3730  style="fill:#070
+0000b800: 6532 623b 6669 6c6c 2d6f 7061 6369 7479  e2b;fill-opacity
+0000b810: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+0000b820: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+0000b830: 2e35 3535 3632 353b 7374 726f 6b65 2d6c  .555625;stroke-l
+0000b840: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+0000b850: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+0000b860: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+0000b870: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000b880: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000b890: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+0000b8a0: 2020 2020 2020 2064 3d22 6d20 3438 2e37         d="m 48.7
+0000b8b0: 3838 3839 312c 3139 392e 3132 3036 3220  88891,199.12062 
+0000b8c0: 3136 2e39 3731 3631 2c32 322e 3331 3730  16.97161,22.3170
+0000b8d0: 3120 2d36 2e32 3830 3833 2c2d 3330 2e30  1 -6.28083,-30.0
+0000b8e0: 3637 3832 207a 220a 2020 2020 2020 2020  6782 z".        
+0000b8f0: 2069 643d 2270 6174 6831 3435 3633 2d31   id="path14563-1
+0000b900: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+0000b910: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+0000b920: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+0000b930: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000b940: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+0000b950: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000b960: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+0000b970: 3030 2220 2f3e 0a20 2020 2020 203c 7061  00" />.      <pa
+0000b980: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
+0000b990: 653d 2266 696c 6c3a 2332 3833 6438 373b  e="fill:#283d87;
+0000b9a0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000b9b0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000b9c0: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
+0000b9d0: 3632 353b 7374 726f 6b65 2d6c 696e 6563  625;stroke-linec
+0000b9e0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000b9f0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000ba00: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000ba10: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000ba20: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000ba30: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000ba40: 2020 2064 3d22 6d20 3539 2e34 3739 3637     d="m 59.47967
+0000ba50: 312c 3139 312e 3336 3938 3120 362e 3238  1,191.36981 6.28
+0000ba60: 3038 332c 3330 2e30 3637 3832 2063 2033  083,30.06782 c 3
+0000ba70: 2e32 3531 3435 2c2d 3237 2e30 3239 3537  .25145,-27.02957
+0000ba80: 2031 342e 3639 3336 352c 2d33 362e 3736   14.69365,-36.76
+0000ba90: 3735 3620 3233 2e39 3230 3633 2c2d 3531  756 23.92063,-51
+0000baa0: 2e31 3832 3132 207a 220a 2020 2020 2020  .18212 z".      
+0000bab0: 2020 2069 643d 2270 6174 6831 3435 3635     id="path14565
+0000bac0: 2d39 220a 2020 2020 2020 2020 2069 6e6b  -9".         ink
+0000bad0: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+0000bae0: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+0000baf0: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+0000bb00: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+0000bb10: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+0000bb20: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000bb30: 3330 3022 0a20 2020 2020 2020 2020 696e  300".         in
+0000bb40: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+0000bb50: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+0000bb60: 2020 3c65 6c6c 6970 7365 0a20 2020 2020    <ellipse.     
+0000bb70: 2020 2020 7374 796c 653d 226f 7061 6369      style="opaci
+0000bb80: 7479 3a31 3b66 696c 6c3a 2330 3730 6532  ty:1;fill:#070e2
+0000bb90: 623b 6669 6c6c 2d6f 7061 6369 7479 3a30  b;fill-opacity:0
+0000bba0: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
+0000bbb0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000bbc0: 6474 683a 302e 3535 3536 3235 3b73 7472  dth:0.555625;str
+0000bbd0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000bbe0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000bbf0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+0000bc00: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+0000bc10: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000bc20: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000bc30: 3536 372d 3622 0a20 2020 2020 2020 2020  567-6".         
+0000bc40: 6378 3d22 362e 3434 3438 3632 3822 0a20  cx="6.4448628". 
+0000bc50: 2020 2020 2020 2020 6379 3d22 3136 312e          cy="161.
+0000bc60: 3837 3038 3222 0a20 2020 2020 2020 2020  87082".         
+0000bc70: 7278 3d22 312e 3636 3633 3332 3722 0a20  rx="1.6663327". 
+0000bc80: 2020 2020 2020 2020 7279 3d22 312e 3636          ry="1.66
+0000bc90: 3633 3332 3822 0a20 2020 2020 2020 2020  63328".         
+0000bca0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+0000bcb0: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+0000bcc0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000bcd0: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+0000bce0: 3e0a 2020 2020 2020 3c63 6972 636c 650a  >.      <circle.
+0000bcf0: 2020 2020 2020 2020 2072 3d22 312e 3636           r="1.66
+0000bd00: 3633 3332 3822 0a20 2020 2020 2020 2020  63328".         
+0000bd10: 7374 796c 653d 226f 7061 6369 7479 3a31  style="opacity:1
+0000bd20: 3b66 696c 6c3a 2332 3533 6137 643b 6669  ;fill:#253a7d;fi
+0000bd30: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+0000bd40: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000bd50: 6b65 2d77 6964 7468 3a30 2e35 3535 3632  ke-width:0.55562
+0000bd60: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+0000bd70: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000bd80: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000bd90: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+0000bda0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000bdb0: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+0000bdc0: 6174 6831 3435 3637 2d33 2d39 3322 0a20  ath14567-3-93". 
+0000bdd0: 2020 2020 2020 2020 6378 3d22 3139 2e36          cx="19.6
+0000bde0: 3535 3633 3222 0a20 2020 2020 2020 2020  55632".         
+0000bdf0: 6379 3d22 3139 342e 3438 3838 3522 0a20  cy="194.48885". 
+0000be00: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+0000be10: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+0000be20: 722d 783d 2234 2e36 3433 3235 3636 220a  r-x="4.6432566".
+0000be30: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000be40: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000be50: 6572 2d79 3d22 2d39 2e39 3738 3036 3231  er-y="-9.9780621
+0000be60: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+0000be70: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000be80: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
+0000be90: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+0000bea0: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+0000beb0: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
+0000bec0: 2020 2020 723d 2231 2e36 3636 3333 3238      r="1.6663328
+0000bed0: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
+0000bee0: 3d22 6f70 6163 6974 793a 313b 6669 6c6c  ="opacity:1;fill
+0000bef0: 3a23 3235 3361 3764 3b66 696c 6c2d 6f70  :#253a7d;fill-op
+0000bf00: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+0000bf10: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000bf20: 6474 683a 302e 3535 3536 3235 3b73 7472  dth:0.555625;str
+0000bf30: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000bf40: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000bf50: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+0000bf60: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+0000bf70: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000bf80: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000bf90: 3536 372d 332d 372d 3322 0a20 2020 2020  567-3-7-3".     
+0000bfa0: 2020 2020 6378 3d22 3539 2e30 3733 3932      cx="59.07392
+0000bfb0: 3122 0a20 2020 2020 2020 2020 6379 3d22  1".         cy="
+0000bfc0: 3138 312e 3035 3330 3122 0a20 2020 2020  181.05301".     
+0000bfd0: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
+0000bfe0: 6e73 666f 726d 2d63 656e 7465 722d 783d  nsform-center-x=
+0000bff0: 2234 2e36 3433 3235 3636 220a 2020 2020  "4.6432566".    
+0000c000: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+0000c010: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
+0000c020: 3d22 2d39 2e39 3738 3036 3231 220a 2020  ="-9.9780621".  
+0000c030: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000c040: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+0000c050: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+0000c060: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000c070: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
+0000c080: 6369 7263 6c65 0a20 2020 2020 2020 2020  circle.         
+0000c090: 723d 2231 2e36 3636 3333 3238 220a 2020  r="1.6663328".  
+0000c0a0: 2020 2020 2020 2073 7479 6c65 3d22 6f70         style="op
+0000c0b0: 6163 6974 793a 313b 6669 6c6c 3a23 6138  acity:1;fill:#a8
+0000c0c0: 6139 6161 3b66 696c 6c2d 6f70 6163 6974  a9aa;fill-opacit
+0000c0d0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+0000c0e0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+0000c0f0: 302e 3535 3536 3235 3b73 7472 6f6b 652d  0.555625;stroke-
+0000c100: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000c110: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000c120: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+0000c130: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+0000c140: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000c150: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+0000c160: 332d 352d 3822 0a20 2020 2020 2020 2020  3-5-8".         
+0000c170: 6378 3d22 3539 2e34 3639 3039 3322 0a20  cx="59.469093". 
+0000c180: 2020 2020 2020 2020 6379 3d22 3139 312e          cy="191.
+0000c190: 3132 3938 3722 0a20 2020 2020 2020 2020  12987".         
+0000c1a0: 696e 6b73 6361 7065 3a74 7261 6e73 666f  inkscape:transfo
+0000c1b0: 726d 2d63 656e 7465 722d 783d 2234 2e36  rm-center-x="4.6
+0000c1c0: 3433 3235 3636 220a 2020 2020 2020 2020  432566".        
+0000c1d0: 2069 6e6b 7363 6170 653a 7472 616e 7366   inkscape:transf
+0000c1e0: 6f72 6d2d 6365 6e74 6572 2d79 3d22 2d39  orm-center-y="-9
+0000c1f0: 2e39 3738 3036 3231 220a 2020 2020 2020  .9780621".      
+0000c200: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000c210: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+0000c220: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000c230: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+0000c240: 2220 2f3e 0a20 2020 2020 203c 6369 7263  " />.      <circ
+0000c250: 6c65 0a20 2020 2020 2020 2020 723d 2231  le.         r="1
+0000c260: 2e36 3636 3333 3238 220a 2020 2020 2020  .6663328".      
+0000c270: 2020 2073 7479 6c65 3d22 6f70 6163 6974     style="opacit
+0000c280: 793a 313b 6669 6c6c 3a23 6162 6161 3963  y:1;fill:#abaa9c
+0000c290: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000c2a0: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000c2b0: 7472 6f6b 652d 7769 6474 683a 302e 3535  troke-width:0.55
+0000c2c0: 3536 3235 3b73 7472 6f6b 652d 6d69 7465  5625;stroke-mite
+0000c2d0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+0000c2e0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+0000c2f0: 7472 6f6b 652d 6461 7368 6f66 6673 6574  troke-dashoffset
+0000c300: 3a30 3b73 7472 6f6b 652d 6f70 6163 6974  :0;stroke-opacit
+0000c310: 793a 3122 0a20 2020 2020 2020 2020 6964  y:1".         id
+0000c320: 3d22 7061 7468 3134 3536 372d 332d 392d  ="path14567-3-9-
+0000c330: 3022 0a20 2020 2020 2020 2020 6378 3d22  0".         cx="
+0000c340: 3439 2e31 3934 3634 3922 0a20 2020 2020  49.194649".     
+0000c350: 2020 2020 6379 3d22 3139 392e 3033 3332      cy="199.0332
+0000c360: 3822 0a20 2020 2020 2020 2020 696e 6b73  8".         inks
+0000c370: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
+0000c380: 656e 7465 722d 783d 2234 2e36 3433 3235  enter-x="4.64325
+0000c390: 3636 220a 2020 2020 2020 2020 2069 6e6b  66".         ink
+0000c3a0: 7363 6170 653a 7472 616e 7366 6f72 6d2d  scape:transform-
+0000c3b0: 6365 6e74 6572 2d79 3d22 2d39 2e39 3738  center-y="-9.978
+0000c3c0: 3036 3231 220a 2020 2020 2020 2020 2069  0621".         i
+0000c3d0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+0000c3e0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+0000c3f0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000c400: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+0000c410: 0a20 2020 2020 203c 6369 7263 6c65 0a20  .      <circle. 
+0000c420: 2020 2020 2020 2020 723d 2232 2e35 3731          r="2.571
+0000c430: 3735 3131 220a 2020 2020 2020 2020 2073  7511".         s
+0000c440: 7479 6c65 3d22 6f70 6163 6974 793a 313b  tyle="opacity:1;
+0000c450: 6669 6c6c 3a23 3131 3230 3636 3b66 696c  fill:#112066;fil
+0000c460: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+0000c470: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+0000c480: 652d 7769 6474 683a 302e 3535 3536 3235  e-width:0.555625
+0000c490: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+0000c4a0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+0000c4b0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+0000c4c0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+0000c4d0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+0000c4e0: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+0000c4f0: 7468 3134 3536 372d 332d 322d 3522 0a20  th14567-3-2-5". 
+0000c500: 2020 2020 2020 2020 6378 3d22 3338 2e33          cx="38.3
+0000c510: 3237 3434 3622 0a20 2020 2020 2020 2020  27446".         
+0000c520: 6379 3d22 3136 302e 3031 3031 3822 0a20  cy="160.01018". 
+0000c530: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+0000c540: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+0000c550: 722d 783d 2237 2e31 3636 3231 3136 220a  r-x="7.1662116".
+0000c560: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000c570: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000c580: 6572 2d79 3d22 2d31 352e 3339 3937 3531  er-y="-15.399751
+0000c590: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+0000c5a0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000c5b0: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
+0000c5c0: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+0000c5d0: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+0000c5e0: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
+0000c5f0: 2020 2020 723d 2231 2e36 3636 3333 3238      r="1.6663328
+0000c600: 220a 2020 2020 2020 2020 2073 7479 6c65  ".         style
+0000c610: 3d22 6f70 6163 6974 793a 313b 6669 6c6c  ="opacity:1;fill
+0000c620: 3a23 6564 6630 6663 3b66 696c 6c2d 6f70  :#edf0fc;fill-op
+0000c630: 6163 6974 793a 302e 3939 3034 3436 3b73  acity:0.990446;s
+0000c640: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000c650: 726f 6b65 2d77 6964 7468 3a30 2e35 3535  roke-width:0.555
+0000c660: 3632 353b 7374 726f 6b65 2d6d 6974 6572  625;stroke-miter
+0000c670: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+0000c680: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+0000c690: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
+0000c6a0: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
+0000c6b0: 3a31 220a 2020 2020 2020 2020 2069 643d  :1".         id=
+0000c6c0: 2270 6174 6831 3435 3637 2d32 2d36 220a  "path14567-2-6".
+0000c6d0: 2020 2020 2020 2020 2063 783d 2235 322e           cx="52.
+0000c6e0: 3235 3732 3235 220a 2020 2020 2020 2020  257225".        
+0000c6f0: 2063 793d 2231 3632 2e38 3735 3137 220a   cy="162.87517".
+0000c700: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000c710: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000c720: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
+0000c730: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000c740: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
+0000c750: 203c 6369 7263 6c65 0a20 2020 2020 2020   <circle.       
+0000c760: 2020 723d 2231 2e36 3636 3333 3238 220a    r="1.6663328".
+0000c770: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+0000c780: 6f70 6163 6974 793a 313b 6669 6c6c 3a23  opacity:1;fill:#
+0000c790: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
+0000c7a0: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
+0000c7b0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000c7c0: 6b65 2d77 6964 7468 3a30 2e35 3535 3632  ke-width:0.55562
+0000c7d0: 353b 7374 726f 6b65 2d6d 6974 6572 6c69  5;stroke-miterli
+0000c7e0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000c7f0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000c800: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+0000c810: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000c820: 220a 2020 2020 2020 2020 2069 643d 2270  ".         id="p
+0000c830: 6174 6831 3435 3637 2d32 2d38 2d36 220a  ath14567-2-8-6".
+0000c840: 2020 2020 2020 2020 2063 783d 2232 332e           cx="23.
+0000c850: 3430 3937 3532 220a 2020 2020 2020 2020  409752".        
+0000c860: 2063 793d 2231 3736 2e37 3036 3135 220a   cy="176.70615".
+0000c870: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+0000c880: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000c890: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
+0000c8a0: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000c8b0: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
+0000c8c0: 203c 6369 7263 6c65 0a20 2020 2020 2020   <circle.       
+0000c8d0: 2020 723d 2233 2e31 3637 3435 3338 220a    r="3.1674538".
+0000c8e0: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+0000c8f0: 6f70 6163 6974 793a 313b 6669 6c6c 3a23  opacity:1;fill:#
+0000c900: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
+0000c910: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
+0000c920: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000c930: 6b65 2d77 6964 7468 3a31 2e30 3536 3136  ke-width:1.05616
+0000c940: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+0000c950: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+0000c960: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+0000c970: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+0000c980: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+0000c990: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+0000c9a0: 7468 3134 3536 372d 322d 372d 3022 0a20  th14567-2-7-0". 
+0000c9b0: 2020 2020 2020 2020 6378 3d22 3839 2e31          cx="89.1
+0000c9c0: 3036 3839 3522 0a20 2020 2020 2020 2020  06895".         
+0000c9d0: 6379 3d22 3137 302e 3637 3937 3922 0a20  cy="170.67979". 
+0000c9e0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+0000c9f0: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+0000ca00: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
+0000ca10: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000ca20: 3d22 3330 3022 202f 3e0a 2020 2020 3c2f  ="300" />.    </
+0000ca30: 673e 0a20 2020 203c 7061 7468 0a20 2020  g>.    <path.   
+0000ca40: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+0000ca50: 2333 6534 6237 373b 6669 6c6c 2d6f 7061  #3e4b77;fill-opa
+0000ca60: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+0000ca70: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+0000ca80: 7468 3a30 2e39 3939 3939 393b 7374 726f  th:0.999999;stro
+0000ca90: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+0000caa0: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+0000cab0: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+0000cac0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+0000cad0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+0000cae0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000caf0: 220a 2020 2020 2020 2064 3d22 6d20 3331  ".       d="m 31
+0000cb00: 372e 3032 3933 352c 3330 312e 3533 3934  7.02935,301.5394
+0000cb10: 3420 3433 2e34 3634 3033 2c2d 312e 3937  4 43.46403,-1.97
+0000cb20: 3536 3420 3238 2e35 3536 3935 2c2d 3331  564 28.55695,-31
+0000cb30: 2e37 3839 3739 2063 202d 3335 2e39 3735  .78979 c -35.975
+0000cb40: 372c 3234 2e31 3934 3237 202d 3533 2e31  7,24.19427 -53.1
+0000cb50: 3633 3335 2c32 382e 3037 3731 3620 2d37  6335,28.07716 -7
+0000cb60: 322e 3032 3039 382c 3333 2e37 3635 3433  2.02098,33.76543
+0000cb70: 207a 220a 2020 2020 2020 2069 643d 2270   z".       id="p
+0000cb80: 6174 6831 3435 3437 2d31 2d37 220a 2020  ath14547-1-7".  
+0000cb90: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+0000cba0: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+0000cbb0: 653d 2230 220a 2020 2020 2020 2073 6f64  e="0".       sod
+0000cbc0: 6970 6f64 693a 6e6f 6465 7479 7065 733d  ipodi:nodetypes=
+0000cbd0: 2263 6363 6322 0a20 2020 2020 2020 696e  "cccc".       in
+0000cbe0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+0000cbf0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+0000cc00: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+0000cc10: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
+0000cc20: 2020 3c70 6174 680a 2020 2020 2020 2073    <path.       s
+0000cc30: 7479 6c65 3d22 6669 6c6c 3a23 3163 3263  tyle="fill:#1c2c
+0000cc40: 3638 3b66 696c 6c2d 6f70 6163 6974 793a  68;fill-opacity:
+0000cc50: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+0000cc60: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+0000cc70: 3939 3939 3939 3b73 7472 6f6b 652d 6c69  999999;stroke-li
+0000cc80: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+0000cc90: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+0000cca0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+0000ccb0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+0000ccc0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+0000ccd0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000cce0: 2020 2020 643d 226d 2033 3630 2e34 3933      d="m 360.493
+0000ccf0: 3338 2c32 3939 2e35 3633 3820 3138 2e38  38,299.5638 18.8
+0000cd00: 3538 3336 2c34 2e33 3130 3532 2039 2e36  5836,4.31052 9.6
+0000cd10: 3938 3539 2c2d 3336 2e31 3030 3331 207a  9859,-36.10031 z
+0000cd20: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+0000cd30: 6831 3435 3439 2d31 2d30 220a 2020 2020  h14549-1-0".    
+0000cd40: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+0000cd50: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+0000cd60: 2230 220a 2020 2020 2020 2069 6e6b 7363  "0".       inksc
+0000cd70: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000cd80: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000cd90: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000cda0: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000cdb0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+0000cdc0: 653d 2266 696c 6c3a 2330 3630 3530 383b  e="fill:#060508;
+0000cdd0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000cde0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000cdf0: 726f 6b65 2d77 6964 7468 3a30 2e39 3939  roke-width:0.999
+0000ce00: 3939 393b 7374 726f 6b65 2d6c 696e 6563  999;stroke-linec
+0000ce10: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000ce20: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000ce30: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000ce40: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000ce50: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000ce60: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000ce70: 2064 3d22 6d20 3337 392e 3335 3137 342c   d="m 379.35174,
+0000ce80: 3330 332e 3837 3433 3220 3530 2e34 3638  303.87432 50.468
+0000ce90: 3538 2c38 2e39 3830 3135 2063 202d 3139  58,8.98015 c -19
+0000cea0: 2e36 3636 3734 2c2d 3130 2e33 3936 3935  .66674,-10.39695
+0000ceb0: 202d 3331 2e30 3535 3434 2c2d 3237 2e31   -31.05544,-27.1
+0000cec0: 3030 3931 202d 3430 2e37 3639 3939 2c2d  0091 -40.76999,-
+0000ced0: 3435 2e30 3830 3436 207a 220a 2020 2020  45.08046 z".    
+0000cee0: 2020 2069 643d 2270 6174 6831 3435 3531     id="path14551
+0000cef0: 2d30 2d33 220a 2020 2020 2020 2069 6e6b  -0-3".       ink
+0000cf00: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+0000cf10: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+0000cf20: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+0000cf30: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
+0000cf40: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000cf50: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+0000cf60: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+0000cf70: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+0000cf80: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
+0000cf90: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+0000cfa0: 6c6c 3a23 3237 3337 3733 3b66 696c 6c2d  ll:#273773;fill-
+0000cfb0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+0000cfc0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+0000cfd0: 7769 6474 683a 302e 3939 3939 3939 3b73  width:0.999999;s
+0000cfe0: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+0000cff0: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+0000d000: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+0000d010: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+0000d020: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+0000d030: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+0000d040: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+0000d050: 2033 3137 2e30 3239 3335 2c33 3031 2e35   317.02935,301.5
+0000d060: 3339 3434 2063 2039 2e35 3634 3338 2c35  3944 c 9.56438,5
+0000d070: 2e34 3836 3734 2032 302e 3130 3937 2c31  .48674 20.1097,1
+0000d080: 302e 3231 3839 3320 3233 2e37 3037 3635  0.21893 23.70765
+0000d090: 2c32 302e 3239 3531 3920 6c20 3139 2e37  ,20.29519 l 19.7
+0000d0a0: 3536 3338 2c2d 3232 2e32 3730 3833 207a  5638,-22.27083 z
+0000d0b0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+0000d0c0: 6831 3435 3533 2d33 2d32 220a 2020 2020  h14553-3-2".    
+0000d0d0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+0000d0e0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+0000d0f0: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
+0000d100: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+0000d110: 6363 6322 0a20 2020 2020 2020 696e 6b73  ccc".       inks
+0000d120: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+0000d130: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+0000d140: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+0000d150: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+0000d160: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+0000d170: 6c65 3d22 6669 6c6c 3a23 3134 3236 3732  le="fill:#142672
+0000d180: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000d190: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000d1a0: 7472 6f6b 652d 7769 6474 683a 302e 3939  troke-width:0.99
+0000d1b0: 3939 3939 3b73 7472 6f6b 652d 6c69 6e65  9999;stroke-line
+0000d1c0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+0000d1d0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+0000d1e0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+0000d1f0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+0000d200: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+0000d210: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+0000d220: 2020 643d 226d 2033 3430 2e37 3337 2c33    d="m 340.737,3
+0000d230: 3231 2e38 3334 3633 2038 392e 3038 3333  21.83463 89.0833
+0000d240: 322c 2d38 2e39 3830 3136 202d 3639 2e33  2,-8.98016 -69.3
+0000d250: 3236 3934 2c2d 3133 2e32 3930 3637 207a  2694,-13.29067 z
+0000d260: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+0000d270: 6831 3435 3535 2d34 2d31 220a 2020 2020  h14555-4-1".    
+0000d280: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+0000d290: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+0000d2a0: 2230 220a 2020 2020 2020 2069 6e6b 7363  "0".       inksc
+0000d2b0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000d2c0: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000d2d0: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000d2e0: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000d2f0: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+0000d300: 653d 2266 696c 6c3a 2335 3436 3638 633b  e="fill:#54668c;
+0000d310: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000d320: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000d330: 726f 6b65 2d77 6964 7468 3a30 2e39 3939  roke-width:0.999
+0000d340: 3939 393b 7374 726f 6b65 2d6c 696e 6563  999;stroke-linec
+0000d350: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000d360: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000d370: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000d380: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000d390: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000d3a0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000d3b0: 2064 3d22 6d20 3334 302e 3733 372c 3332   d="m 340.737,32
+0000d3c0: 312e 3833 3436 3320 3531 2e33 3636 3538  1.83463 51.36658
+0000d3d0: 2c35 2e33 3838 3120 3337 2e37 3136 3734  ,5.3881 37.71674
+0000d3e0: 2c2d 3134 2e33 3638 3236 207a 220a 2020  ,-14.36826 z".  
+0000d3f0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+0000d400: 3537 2d30 2d37 220a 2020 2020 2020 2069  57-0-7".       i
+0000d410: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+0000d420: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+0000d430: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000d440: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+0000d450: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000d460: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+0000d470: 3030 2220 2f3e 0a20 2020 203c 7061 7468  00" />.    <path
+0000d480: 0a20 2020 2020 2020 7374 796c 653d 2266  .       style="f
+0000d490: 696c 6c3a 2332 3233 3437 653b 6669 6c6c  ill:#22347e;fill
+0000d4a0: 2d6f 7061 6369 7479 3a31 3b73 7472 6f6b  -opacity:1;strok
+0000d4b0: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+0000d4c0: 2d77 6964 7468 3a30 2e39 3939 3939 393b  -width:0.999999;
+0000d4d0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+0000d4e0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+0000d4f0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+0000d500: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000d510: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000d520: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+0000d530: 7479 3a31 220a 2020 2020 2020 2064 3d22  ty:1".       d="
+0000d540: 6d20 3334 302e 3733 372c 3332 312e 3833  m 340.737,321.83
+0000d550: 3436 3320 6320 312e 3135 3530 352c 392e  463 c 1.15505,9.
+0000d560: 3935 3931 3320 2d32 2e38 3433 3033 2c31  95913 -2.84303,1
+0000d570: 362e 3233 3734 3920 2d34 2e36 3639 3638  6.23749 -4.66968
+0000d580: 2c32 342e 3036 3638 3620 6c20 3536 2e30  ,24.06686 l 56.0
+0000d590: 3336 3236 2c2d 3138 2e36 3738 3736 207a  3626,-18.67876 z
+0000d5a0: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+0000d5b0: 6831 3435 3539 2d33 2d34 220a 2020 2020  h14559-3-4".    
+0000d5c0: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+0000d5d0: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+0000d5e0: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
+0000d5f0: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+0000d600: 6363 6322 0a20 2020 2020 2020 696e 6b73  ccc".       inks
+0000d610: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+0000d620: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+0000d630: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+0000d640: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+0000d650: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+0000d660: 6c65 3d22 6669 6c6c 3a23 3038 3130 3639  le="fill:#081069
+0000d670: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000d680: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000d690: 7472 6f6b 652d 7769 6474 683a 302e 3939  troke-width:0.99
+0000d6a0: 3939 3939 3b73 7472 6f6b 652d 6c69 6e65  9999;stroke-line
+0000d6b0: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+0000d6c0: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+0000d6d0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+0000d6e0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+0000d6f0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+0000d700: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+0000d710: 2020 643d 226d 2033 3336 2e30 3637 3332    d="m 336.06732
+0000d720: 2c33 3435 2e39 3031 3439 2033 382e 3739  ,345.90149 38.79
+0000d730: 3433 332c 352e 3734 3733 2035 342e 3935  433,5.7473 54.95
+0000d740: 3836 372c 2d33 382e 3739 3433 3220 7a22  867,-38.79432 z"
+0000d750: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000d760: 3134 3536 312d 392d 3222 0a20 2020 2020  14561-9-2".     
+0000d770: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000d780: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000d790: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000d7a0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000d7b0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000d7c0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000d7d0: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
+0000d7e0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+0000d7f0: 3d22 6669 6c6c 3a23 3037 3065 3262 3b66  ="fill:#070e2b;f
+0000d800: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+0000d810: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+0000d820: 6f6b 652d 7769 6474 683a 302e 3939 3939  oke-width:0.9999
+0000d830: 3939 3b73 7472 6f6b 652d 6c69 6e65 6361  99;stroke-lineca
+0000d840: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+0000d850: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+0000d860: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000d870: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000d880: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+0000d890: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000d8a0: 643d 226d 2033 3734 2e38 3631 3635 2c33  d="m 374.86165,3
+0000d8b0: 3531 2e36 3438 3739 2032 322e 3830 3936  51.64879 22.8096
+0000d8c0: 332c 3239 2e39 3933 3820 2d38 2e34 3431  3,29.9938 -8.441
+0000d8d0: 3335 2c2d 3430 2e34 3130 3738 207a 220a  35,-40.41078 z".
+0000d8e0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000d8f0: 3435 3633 2d31 2d30 220a 2020 2020 2020  4563-1-0".      
+0000d900: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+0000d910: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+0000d920: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000d930: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000d940: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000d950: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000d960: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
+0000d970: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+0000d980: 2266 696c 6c3a 2332 3833 6438 373b 6669  "fill:#283d87;fi
+0000d990: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+0000d9a0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000d9b0: 6b65 2d77 6964 7468 3a30 2e39 3939 3939  ke-width:0.99999
+0000d9c0: 393b 7374 726f 6b65 2d6c 696e 6563 6170  9;stroke-linecap
+0000d9d0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+0000d9e0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+0000d9f0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+0000da00: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+0000da10: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+0000da20: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+0000da30: 3d22 6d20 3338 392e 3232 3939 332c 3334  ="m 389.22993,34
+0000da40: 312e 3233 3138 3120 382e 3434 3133 352c  1.23181 8.44135,
+0000da50: 3430 2e34 3130 3738 2063 2034 2e33 3639  40.41078 c 4.369
+0000da60: 3933 2c2d 3336 2e33 3237 3432 2031 392e  93,-36.32742 19.
+0000da70: 3734 3830 372c 2d34 392e 3431 3531 3320  74807,-49.41513 
+0000da80: 3332 2e31 3439 3034 2c2d 3638 2e37 3838  32.14904,-68.788
+0000da90: 3132 207a 220a 2020 2020 2020 2069 643d  12 z".       id=
+0000daa0: 2270 6174 6831 3435 3635 2d39 2d35 220a  "path14565-9-5".
+0000dab0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000dac0: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+0000dad0: 7572 653d 2230 220a 2020 2020 2020 2073  ure="0".       s
+0000dae0: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+0000daf0: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
+0000db00: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+0000db10: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+0000db20: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+0000db30: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+0000db40: 2020 2020 3c65 6c6c 6970 7365 0a20 2020      <ellipse.   
+0000db50: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+0000db60: 2330 3730 6532 623b 6669 6c6c 2d6f 7061  #070e2b;fill-opa
+0000db70: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
+0000db80: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+0000db90: 6f6b 652d 7769 6474 683a 302e 3939 3939  oke-width:0.9999
+0000dba0: 3939 3b73 7472 6f6b 652d 6d69 7465 726c  99;stroke-miterl
+0000dbb0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+0000dbc0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+0000dbd0: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+0000dbe0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+0000dbf0: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
+0000dc00: 7468 3134 3536 372d 362d 3122 0a20 2020  th14567-6-1".   
+0000dc10: 2020 2020 6378 3d22 3331 372e 3935 3138      cx="317.9518
+0000dc20: 3422 0a20 2020 2020 2020 6379 3d22 3330  4".       cy="30
+0000dc30: 312e 3538 3535 3722 0a20 2020 2020 2020  1.58557".       
+0000dc40: 7278 3d22 322e 3233 3935 3239 3622 0a20  rx="2.2395296". 
+0000dc50: 2020 2020 2020 7279 3d22 322e 3233 3935        ry="2.2395
+0000dc60: 3239 3822 0a20 2020 2020 2020 696e 6b73  298".       inks
+0000dc70: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+0000dc80: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+0000dc90: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+0000dca0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+0000dcb0: 3c63 6972 636c 650a 2020 2020 2020 2072  <circle.       r
+0000dcc0: 3d22 322e 3233 3935 3239 3822 0a20 2020  ="2.2395298".   
+0000dcd0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+0000dce0: 2332 3533 6137 643b 6669 6c6c 2d6f 7061  #253a7d;fill-opa
+0000dcf0: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+0000dd00: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+0000dd10: 7468 3a30 2e39 3939 3939 393b 7374 726f  th:0.999999;stro
+0000dd20: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+0000dd30: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+0000dd40: 3a6e 6f6e 653b 7374 726f 6b65 2d64 6173  :none;stroke-das
+0000dd50: 686f 6666 7365 743a 303b 7374 726f 6b65  hoffset:0;stroke
+0000dd60: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+0000dd70: 2020 2069 643d 2270 6174 6831 3435 3637     id="path14567
+0000dd80: 2d33 2d39 332d 3122 0a20 2020 2020 2020  -3-93-1".       
+0000dd90: 6378 3d22 3333 352e 3730 3639 3122 0a20  cx="335.70691". 
+0000dda0: 2020 2020 2020 6379 3d22 3334 352e 3432        cy="345.42
+0000ddb0: 3337 3722 0a20 2020 2020 2020 696e 6b73  377".       inks
+0000ddc0: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
+0000ddd0: 656e 7465 722d 783d 2234 2e36 3433 3235  enter-x="4.64325
+0000dde0: 3636 220a 2020 2020 2020 2069 6e6b 7363  66".       inksc
+0000ddf0: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+0000de00: 6e74 6572 2d79 3d22 2d39 2e39 3738 3036  nter-y="-9.97806
+0000de10: 3231 220a 2020 2020 2020 2069 6e6b 7363  21".       inksc
+0000de20: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000de30: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000de40: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000de50: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000de60: 6369 7263 6c65 0a20 2020 2020 2020 723d  circle.       r=
+0000de70: 2232 2e32 3339 3532 3938 220a 2020 2020  "2.2395298".    
+0000de80: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+0000de90: 3235 3361 3764 3b66 696c 6c2d 6f70 6163  253a7d;fill-opac
+0000dea0: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+0000deb0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+0000dec0: 683a 302e 3939 3939 3939 3b73 7472 6f6b  h:0.999999;strok
+0000ded0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+0000dee0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+0000def0: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
+0000df00: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
+0000df10: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+0000df20: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+0000df30: 332d 372d 332d 3022 0a20 2020 2020 2020  3-7-3-0".       
+0000df40: 6378 3d22 3338 382e 3638 3436 220a 2020  cx="388.6846".  
+0000df50: 2020 2020 2063 793d 2233 3237 2e33 3636       cy="327.366
+0000df60: 3231 220a 2020 2020 2020 2069 6e6b 7363  21".       inksc
+0000df70: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+0000df80: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
+0000df90: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+0000dfa0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000dfb0: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
+0000dfc0: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
+0000dfd0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000dfe0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000dff0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000e000: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
+0000e010: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
+0000e020: 322e 3233 3935 3239 3822 0a20 2020 2020  2.2395298".     
+0000e030: 2020 7374 796c 653d 2266 696c 6c3a 2361    style="fill:#a
+0000e040: 3861 3961 613b 6669 6c6c 2d6f 7061 6369  8a9aa;fill-opaci
+0000e050: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+0000e060: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+0000e070: 3a30 2e39 3939 3939 393b 7374 726f 6b65  :0.999999;stroke
+0000e080: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000e090: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000e0a0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+0000e0b0: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+0000e0c0: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000e0d0: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
+0000e0e0: 2d35 2d38 2d38 220a 2020 2020 2020 2063  -5-8-8".       c
+0000e0f0: 783d 2233 3839 2e32 3135 3733 220a 2020  x="389.21573".  
+0000e100: 2020 2020 2063 793d 2233 3430 2e39 3039       cy="340.909
+0000e110: 3336 220a 2020 2020 2020 2069 6e6b 7363  36".       inksc
+0000e120: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+0000e130: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
+0000e140: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+0000e150: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000e160: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
+0000e170: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
+0000e180: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000e190: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000e1a0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000e1b0: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
+0000e1c0: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
+0000e1d0: 322e 3233 3935 3239 3822 0a20 2020 2020  2.2395298".     
+0000e1e0: 2020 7374 796c 653d 2266 696c 6c3a 2361    style="fill:#a
+0000e1f0: 6261 6139 633b 6669 6c6c 2d6f 7061 6369  baa9c;fill-opaci
+0000e200: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+0000e210: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+0000e220: 3a30 2e39 3939 3939 393b 7374 726f 6b65  :0.999999;stroke
+0000e230: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000e240: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000e250: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+0000e260: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+0000e270: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000e280: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
+0000e290: 2d39 2d30 2d39 220a 2020 2020 2020 2063  -9-0-9".       c
+0000e2a0: 783d 2233 3735 2e34 3036 3938 220a 2020  x="375.40698".  
+0000e2b0: 2020 2020 2063 793d 2233 3531 2e35 3331       cy="351.531
+0000e2c0: 3433 220a 2020 2020 2020 2069 6e6b 7363  43".       inksc
+0000e2d0: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+0000e2e0: 6e74 6572 2d78 3d22 342e 3634 3332 3536  nter-x="4.643256
+0000e2f0: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+0000e300: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000e310: 7465 722d 793d 222d 392e 3937 3830 3632  ter-y="-9.978062
+0000e320: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
+0000e330: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000e340: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000e350: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000e360: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
+0000e370: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
+0000e380: 332e 3435 3634 3030 3422 0a20 2020 2020  3.4564004".     
+0000e390: 2020 7374 796c 653d 2266 696c 6c3a 2331    style="fill:#1
+0000e3a0: 3132 3036 363b 6669 6c6c 2d6f 7061 6369  12066;fill-opaci
+0000e3b0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+0000e3c0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+0000e3d0: 3a30 2e39 3939 3939 393b 7374 726f 6b65  :0.999999;stroke
+0000e3e0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+0000e3f0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+0000e400: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+0000e410: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+0000e420: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000e430: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
+0000e440: 2d32 2d35 2d34 220a 2020 2020 2020 2063  -2-5-4".       c
+0000e450: 783d 2233 3630 2e38 3031 3631 220a 2020  x="360.80161".  
+0000e460: 2020 2020 2063 793d 2232 3939 2e30 3834       cy="299.084
+0000e470: 3922 0a20 2020 2020 2020 696e 6b73 6361  9".       inksca
+0000e480: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+0000e490: 7465 722d 783d 2237 2e31 3636 3231 3136  ter-x="7.1662116
+0000e4a0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000e4b0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+0000e4c0: 6572 2d79 3d22 2d31 352e 3339 3937 3531  er-y="-15.399751
+0000e4d0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000e4e0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+0000e4f0: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+0000e500: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+0000e510: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
+0000e520: 7263 6c65 0a20 2020 2020 2020 723d 2232  rcle.       r="2
+0000e530: 2e32 3339 3532 3938 220a 2020 2020 2020  .2395298".      
+0000e540: 2073 7479 6c65 3d22 6669 6c6c 3a23 6564   style="fill:#ed
+0000e550: 6630 6663 3b66 696c 6c2d 6f70 6163 6974  f0fc;fill-opacit
+0000e560: 793a 302e 3939 3034 3436 3b73 7472 6f6b  y:0.990446;strok
+0000e570: 653a 2366 6666 6666 663b 7374 726f 6b65  e:#ffffff;stroke
+0000e580: 2d77 6964 7468 3a30 2e39 3939 3939 393b  -width:0.999999;
+0000e590: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+0000e5a0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+0000e5b0: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+0000e5c0: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+0000e5d0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+0000e5e0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000e5f0: 3435 3637 2d32 2d36 2d30 220a 2020 2020  4567-2-6-0".    
+0000e600: 2020 2063 783d 2233 3739 2e35 3233 3034     cx="379.52304
+0000e610: 220a 2020 2020 2020 2063 793d 2233 3032  ".       cy="302
+0000e620: 2e39 3335 3336 220a 2020 2020 2020 2069  .93536".       i
+0000e630: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+0000e640: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+0000e650: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+0000e660: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+0000e670: 2020 203c 6369 7263 6c65 0a20 2020 2020     <circle.     
+0000e680: 2020 723d 2232 2e32 3339 3532 3938 220a    r="2.2395298".
+0000e690: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+0000e6a0: 6c6c 3a23 6564 6630 6663 3b66 696c 6c2d  ll:#edf0fc;fill-
+0000e6b0: 6f70 6163 6974 793a 302e 3939 3034 3436  opacity:0.990446
+0000e6c0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+0000e6d0: 7374 726f 6b65 2d77 6964 7468 3a30 2e39  stroke-width:0.9
+0000e6e0: 3939 3939 393b 7374 726f 6b65 2d6d 6974  99999;stroke-mit
+0000e6f0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+0000e700: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+0000e710: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+0000e720: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+0000e730: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+0000e740: 2270 6174 6831 3435 3637 2d32 2d38 2d36  "path14567-2-8-6
+0000e750: 2d37 220a 2020 2020 2020 2063 783d 2233  -7".       cx="3
+0000e760: 3430 2e37 3532 3431 220a 2020 2020 2020  40.75241".      
+0000e770: 2063 793d 2233 3231 2e35 3234 3035 220a   cy="321.52405".
+0000e780: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000e790: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+0000e7a0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000e7b0: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+0000e7c0: 3030 2220 2f3e 0a20 2020 203c 6369 7263  00" />.    <circ
+0000e7d0: 6c65 0a20 2020 2020 2020 723d 2234 2e32  le.       r="4.2
+0000e7e0: 3537 3031 3731 220a 2020 2020 2020 2073  570171".       s
+0000e7f0: 7479 6c65 3d22 6669 6c6c 3a23 6564 6630  tyle="fill:#edf0
+0000e800: 6663 3b66 696c 6c2d 6f70 6163 6974 793a  fc;fill-opacity:
+0000e810: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
+0000e820: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+0000e830: 6964 7468 3a30 2e39 3939 3939 393b 7374  idth:0.999999;st
+0000e840: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000e850: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000e860: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+0000e870: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+0000e880: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+0000e890: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+0000e8a0: 3637 2d32 2d37 2d30 2d39 220a 2020 2020  67-2-7-0-9".    
+0000e8b0: 2020 2063 783d 2234 3239 2e30 3438 3535     cx="429.04855
+0000e8c0: 220a 2020 2020 2020 2063 793d 2233 3133  ".       cy="313
+0000e8d0: 2e34 3234 3638 220a 2020 2020 2020 2069  .42468".       i
+0000e8e0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+0000e8f0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+0000e900: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+0000e910: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+0000e920: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+0000e930: 7374 796c 653d 2266 696c 6c3a 2333 6534  style="fill:#3e4
+0000e940: 6237 373b 6669 6c6c 2d6f 7061 6369 7479  b77;fill-opacity
+0000e950: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+0000e960: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+0000e970: 2e37 3438 3939 373b 7374 726f 6b65 2d6c  .748997;stroke-l
+0000e980: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+0000e990: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+0000e9a0: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+0000e9b0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000e9c0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000e9d0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+0000e9e0: 2020 2020 2064 3d22 6d20 3331 392e 3133       d="m 319.13
+0000e9f0: 3437 352c 3434 302e 3131 3937 3420 3231  475,440.11974 21
+0000ea00: 2e37 3332 3032 2c2d 302e 3938 3738 3220  .73202,-0.98782 
+0000ea10: 3134 2e32 3738 3437 2c2d 3135 2e38 3934  14.27847,-15.894
+0000ea20: 3920 6320 2d31 372e 3938 3738 352c 3132  9 c -17.98785,12
+0000ea30: 2e30 3937 3134 202d 3236 2e35 3831 3638  .09714 -26.58168
+0000ea40: 2c31 342e 3033 3835 3820 2d33 362e 3031  ,14.03858 -36.01
+0000ea50: 3034 392c 3136 2e38 3832 3732 207a 220a  049,16.88272 z".
+0000ea60: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000ea70: 3435 3437 2d31 2d37 2d38 220a 2020 2020  4547-1-7-8".    
+0000ea80: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+0000ea90: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+0000eaa0: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
+0000eab0: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+0000eac0: 6363 6322 0a20 2020 2020 2020 696e 6b73  ccc".       inks
+0000ead0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+0000eae0: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+0000eaf0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+0000eb00: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+0000eb10: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+0000eb20: 6c65 3d22 6669 6c6c 3a23 3163 3263 3638  le="fill:#1c2c68
+0000eb30: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000eb40: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000eb50: 7472 6f6b 652d 7769 6474 683a 302e 3734  troke-width:0.74
+0000eb60: 3839 3937 3b73 7472 6f6b 652d 6c69 6e65  8997;stroke-line
+0000eb70: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+0000eb80: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+0000eb90: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+0000eba0: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+0000ebb0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+0000ebc0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+0000ebd0: 2020 643d 226d 2033 3430 2e38 3636 3737    d="m 340.86677
+0000ebe0: 2c34 3339 2e31 3331 3932 2039 2e34 3239  ,439.13192 9.429
+0000ebf0: 3137 2c32 2e31 3535 3234 2034 2e38 3439  17,2.15524 4.849
+0000ec00: 332c 2d31 382e 3035 3031 3420 7a22 0a20  3,-18.05014 z". 
+0000ec10: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000ec20: 3534 392d 312d 302d 3122 0a20 2020 2020  549-1-0-1".     
+0000ec30: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000ec40: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000ec50: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+0000ec60: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000ec70: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000ec80: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000ec90: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
+0000eca0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+0000ecb0: 3d22 6669 6c6c 3a23 3036 3035 3038 3b66  ="fill:#060508;f
+0000ecc0: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+0000ecd0: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+0000ece0: 6f6b 652d 7769 6474 683a 302e 3734 3839  oke-width:0.7489
+0000ecf0: 3937 3b73 7472 6f6b 652d 6c69 6e65 6361  97;stroke-lineca
+0000ed00: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+0000ed10: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+0000ed20: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000ed30: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000ed40: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+0000ed50: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000ed60: 643d 226d 2033 3530 2e32 3935 3934 2c34  d="m 350.29594,4
+0000ed70: 3431 2e32 3837 3136 2032 352e 3233 3432  41.28716 25.2342
+0000ed80: 382c 342e 3439 3030 3920 6320 2d39 2e38  8,4.49009 c -9.8
+0000ed90: 3333 3336 2c2d 352e 3139 3834 3720 2d31  3336,-5.19847 -1
+0000eda0: 352e 3532 3737 312c 2d31 332e 3535 3034  5.52771,-13.5504
+0000edb0: 3620 2d32 302e 3338 3439 382c 2d32 322e  6 -20.38498,-22.
+0000edc0: 3534 3032 3320 7a22 0a20 2020 2020 2020  54023 z".       
+0000edd0: 6964 3d22 7061 7468 3134 3535 312d 302d  id="path14551-0-
+0000ede0: 332d 3922 0a20 2020 2020 2020 696e 6b73  3-9".       inks
+0000edf0: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+0000ee00: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+0000ee10: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+0000ee20: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
+0000ee30: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000ee40: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+0000ee50: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+0000ee60: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+0000ee70: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+0000ee80: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+0000ee90: 6c3a 2332 3733 3737 333b 6669 6c6c 2d6f  l:#273773;fill-o
+0000eea0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+0000eeb0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+0000eec0: 6964 7468 3a30 2e37 3438 3939 373b 7374  idth:0.748997;st
+0000eed0: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+0000eee0: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+0000eef0: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+0000ef00: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+0000ef10: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+0000ef20: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+0000ef30: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
+0000ef40: 3331 392e 3133 3437 352c 3434 302e 3131  319.13475,440.11
+0000ef50: 3937 3420 6320 342e 3738 3231 392c 322e  974 c 4.78219,2.
+0000ef60: 3734 3333 3720 3130 2e30 3534 3835 2c35  74337 10.05485,5
+0000ef70: 2e31 3039 3435 2031 312e 3835 3338 322c  .10945 11.85382,
+0000ef80: 3130 2e31 3437 3620 6c20 392e 3837 3832  10.1476 l 9.8782
+0000ef90: 2c2d 3131 2e31 3335 3432 207a 220a 2020  ,-11.13542 z".  
+0000efa0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+0000efb0: 3533 2d33 2d32 2d32 220a 2020 2020 2020  53-3-2-2".      
+0000efc0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+0000efd0: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+0000efe0: 220a 2020 2020 2020 2073 6f64 6970 6f64  ".       sodipod
+0000eff0: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
+0000f000: 6322 0a20 2020 2020 2020 696e 6b73 6361  c".       inksca
+0000f010: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+0000f020: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+0000f030: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+0000f040: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
+0000f050: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+0000f060: 3d22 6669 6c6c 3a23 3134 3236 3732 3b66  ="fill:#142672;f
+0000f070: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+0000f080: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+0000f090: 6f6b 652d 7769 6474 683a 302e 3734 3839  oke-width:0.7489
+0000f0a0: 3937 3b73 7472 6f6b 652d 6c69 6e65 6361  97;stroke-lineca
+0000f0b0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+0000f0c0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+0000f0d0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000f0e0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000f0f0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+0000f100: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+0000f110: 643d 226d 2033 3330 2e39 3838 3537 2c34  d="m 330.98857,4
+0000f120: 3530 2e32 3637 3334 2034 342e 3534 3136  50.26734 44.5416
+0000f130: 352c 2d34 2e34 3930 3039 202d 3334 2e36  5,-4.49009 -34.6
+0000f140: 3633 3435 2c2d 362e 3634 3533 3320 7a22  6345,-6.64533 z"
+0000f150: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000f160: 3134 3535 352d 342d 312d 3622 0a20 2020  14555-4-1-6".   
+0000f170: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
+0000f180: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
+0000f190: 3d22 3022 0a20 2020 2020 2020 696e 6b73  ="0".       inks
+0000f1a0: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+0000f1b0: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+0000f1c0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+0000f1d0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+0000f1e0: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+0000f1f0: 6c65 3d22 6669 6c6c 3a23 3534 3636 3863  le="fill:#54668c
+0000f200: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+0000f210: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+0000f220: 7472 6f6b 652d 7769 6474 683a 302e 3734  troke-width:0.74
+0000f230: 3839 3937 3b73 7472 6f6b 652d 6c69 6e65  8997;stroke-line
+0000f240: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+0000f250: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+0000f260: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+0000f270: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+0000f280: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+0000f290: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+0000f2a0: 2020 643d 226d 2033 3330 2e39 3838 3537    d="m 330.98857
+0000f2b0: 2c34 3530 2e32 3637 3334 2032 352e 3638  ,450.26734 25.68
+0000f2c0: 3333 2c32 2e36 3934 3035 2031 382e 3835  33,2.69405 18.85
+0000f2d0: 3833 352c 2d37 2e31 3834 3134 207a 220a  835,-7.18414 z".
+0000f2e0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+0000f2f0: 3435 3537 2d30 2d37 2d33 220a 2020 2020  4557-0-7-3".    
+0000f300: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+0000f310: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+0000f320: 2230 220a 2020 2020 2020 2069 6e6b 7363  "0".       inksc
+0000f330: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000f340: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000f350: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000f360: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000f370: 7061 7468 0a20 2020 2020 2020 7374 796c  path.       styl
+0000f380: 653d 2266 696c 6c3a 2332 3233 3437 653b  e="fill:#22347e;
+0000f390: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000f3a0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000f3b0: 726f 6b65 2d77 6964 7468 3a30 2e37 3438  roke-width:0.748
+0000f3c0: 3939 373b 7374 726f 6b65 2d6c 696e 6563  997;stroke-linec
+0000f3d0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+0000f3e0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+0000f3f0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+0000f400: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+0000f410: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+0000f420: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+0000f430: 2064 3d22 6d20 3333 302e 3938 3835 372c   d="m 330.98857,
+0000f440: 3435 302e 3236 3733 3420 6320 302e 3537  450.26734 c 0.57
+0000f450: 3735 332c 342e 3937 3935 3620 2d31 2e34  753,4.97956 -1.4
+0000f460: 3231 3531 2c38 2e31 3138 3733 202d 322e  2151,8.11873 -2.
+0000f470: 3333 3438 342c 3132 2e30 3333 3432 206c  33484,12.03342 l
+0000f480: 2032 382e 3031 3831 342c 2d39 2e33 3339   28.01814,-9.339
+0000f490: 3337 207a 220a 2020 2020 2020 2069 643d  37 z".       id=
+0000f4a0: 2270 6174 6831 3435 3539 2d33 2d34 2d32  "path14559-3-4-2
+0000f4b0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+0000f4c0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+0000f4d0: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+0000f4e0: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
+0000f4f0: 7065 733d 2263 6363 6322 0a20 2020 2020  pes="cccc".     
+0000f500: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+0000f510: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+0000f520: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000f530: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+0000f540: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
+0000f550: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+0000f560: 3038 3130 3639 3b66 696c 6c2d 6f70 6163  081069;fill-opac
+0000f570: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+0000f580: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+0000f590: 683a 302e 3734 3839 3937 3b73 7472 6f6b  h:0.748997;strok
+0000f5a0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+0000f5b0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+0000f5c0: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+0000f5d0: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+0000f5e0: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+0000f5f0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+0000f600: 0a20 2020 2020 2020 643d 226d 2033 3238  .       d="m 328
+0000f610: 2e36 3533 3733 2c34 3632 2e33 3030 3736  .65373,462.30076
+0000f620: 2031 392e 3339 3731 372c 322e 3837 3336   19.39717,2.8736
+0000f630: 3620 3237 2e34 3739 3332 2c2d 3139 2e33  6 27.47932,-19.3
+0000f640: 3937 3137 207a 220a 2020 2020 2020 2069  9717 z".       i
+0000f650: 643d 2270 6174 6831 3435 3631 2d39 2d32  d="path14561-9-2
+0000f660: 2d32 220a 2020 2020 2020 2069 6e6b 7363  -2".       inksc
+0000f670: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+0000f680: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+0000f690: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+0000f6a0: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+0000f6b0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+0000f6c0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+0000f6d0: 2f3e 0a20 2020 203c 7061 7468 0a20 2020  />.    <path.   
+0000f6e0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+0000f6f0: 2330 3730 6532 623b 6669 6c6c 2d6f 7061  #070e2b;fill-opa
+0000f700: 6369 7479 3a31 3b73 7472 6f6b 653a 2366  city:1;stroke:#f
+0000f710: 6666 6666 663b 7374 726f 6b65 2d77 6964  fffff;stroke-wid
+0000f720: 7468 3a30 2e37 3438 3939 373b 7374 726f  th:0.748997;stro
+0000f730: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+0000f740: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+0000f750: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+0000f760: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+0000f770: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+0000f780: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000f790: 220a 2020 2020 2020 2064 3d22 6d20 3334  ".       d="m 34
+0000f7a0: 382e 3035 3039 2c34 3635 2e31 3734 3432  8.0509,465.17442
+0000f7b0: 2031 312e 3430 3438 312c 3134 2e39 3936   11.40481,14.996
+0000f7c0: 3839 202d 342e 3232 3036 372c 2d32 302e  89 -4.22067,-20.
+0000f7d0: 3230 3533 3920 7a22 0a20 2020 2020 2020  20539 z".       
+0000f7e0: 6964 3d22 7061 7468 3134 3536 332d 312d  id="path14563-1-
+0000f7f0: 302d 3622 0a20 2020 2020 2020 696e 6b73  0-6".       inks
+0000f800: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+0000f810: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+0000f820: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000f830: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+0000f840: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000f850: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+0000f860: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+0000f870: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+0000f880: 3a23 3238 3364 3837 3b66 696c 6c2d 6f70  :#283d87;fill-op
+0000f890: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+0000f8a0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000f8b0: 6474 683a 302e 3734 3839 3937 3b73 7472  dth:0.748997;str
+0000f8c0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+0000f8d0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+0000f8e0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+0000f8f0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+0000f900: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+0000f910: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+0000f920: 3122 0a20 2020 2020 2020 643d 226d 2033  1".       d="m 3
+0000f930: 3535 2e32 3335 3034 2c34 3539 2e39 3635  55.23504,459.965
+0000f940: 3932 2034 2e32 3230 3637 2c32 302e 3230  92 4.22067,20.20
+0000f950: 3533 3920 6320 322e 3138 3439 362c 2d31  539 c 2.18496,-1
+0000f960: 382e 3136 3337 2039 2e38 3734 3034 2c2d  8.1637 9.87404,-
+0000f970: 3234 2e37 3037 3537 2031 362e 3037 3435  24.70757 16.0745
+0000f980: 312c 2d33 342e 3339 3430 3620 7a22 0a20  1,-34.39406 z". 
+0000f990: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+0000f9a0: 3536 352d 392d 352d 3922 0a20 2020 2020  565-9-5-9".     
+0000f9b0: 2020 696e 6b73 6361 7065 3a63 6f6e 6e65    inkscape:conne
+0000f9c0: 6374 6f72 2d63 7572 7661 7475 7265 3d22  ctor-curvature="
+0000f9d0: 3022 0a20 2020 2020 2020 736f 6469 706f  0".       sodipo
+0000f9e0: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+0000f9f0: 6363 220a 2020 2020 2020 2069 6e6b 7363  cc".       inksc
+0000fa00: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+0000fa10: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+0000fa20: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+0000fa30: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+0000fa40: 6369 7263 6c65 0a20 2020 2020 2020 7374  circle.       st
+0000fa50: 796c 653d 2266 696c 6c3a 2330 3730 6532  yle="fill:#070e2
+0000fa60: 623b 6669 6c6c 2d6f 7061 6369 7479 3a30  b;fill-opacity:0
+0000fa70: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
+0000fa80: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+0000fa90: 6474 683a 302e 3734 3839 3937 3b73 7472  dth:0.748997;str
+0000faa0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+0000fab0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+0000fac0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6461  y:none;stroke-da
+0000fad0: 7368 6f66 6673 6574 3a30 3b73 7472 6f6b  shoffset:0;strok
+0000fae0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+0000faf0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+0000fb00: 372d 362d 312d 3922 0a20 2020 2020 2020  7-6-1-9".       
+0000fb10: 6378 3d22 3331 392e 3539 3539 3822 0a20  cx="319.59598". 
+0000fb20: 2020 2020 2020 6379 3d22 3434 302e 3134        cy="440.14
+0000fb30: 3237 3922 0a20 2020 2020 2020 696e 6b73  279".       inks
+0000fb40: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+0000fb50: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+0000fb60: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+0000fb70: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+0000fb80: 723d 2231 2e31 3139 3736 3439 2220 2f3e  r="1.1197649" />
+0000fb90: 0a20 2020 203c 6369 7263 6c65 0a20 2020  .    <circle.   
+0000fba0: 2020 2020 723d 2231 2e31 3139 3736 3439      r="1.1197649
+0000fbb0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+0000fbc0: 6669 6c6c 3a23 3235 3361 3764 3b66 696c  fill:#253a7d;fil
+0000fbd0: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+0000fbe0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+0000fbf0: 652d 7769 6474 683a 302e 3734 3839 3937  e-width:0.748997
+0000fc00: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+0000fc10: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+0000fc20: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+0000fc30: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+0000fc40: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+0000fc50: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+0000fc60: 3134 3536 372d 332d 3933 2d31 2d36 220a  14567-3-93-1-6".
+0000fc70: 2020 2020 2020 2063 783d 2233 3238 2e34         cx="328.4
+0000fc80: 3733 3534 220a 2020 2020 2020 2063 793d  7354".       cy=
+0000fc90: 2234 3632 2e30 3631 3839 220a 2020 2020  "462.06189".    
+0000fca0: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
+0000fcb0: 7366 6f72 6d2d 6365 6e74 6572 2d78 3d22  sform-center-x="
+0000fcc0: 342e 3634 3332 3536 3622 0a20 2020 2020  4.6432566".     
+0000fcd0: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+0000fce0: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
+0000fcf0: 392e 3937 3830 3632 3122 0a20 2020 2020  9.9780621".     
+0000fd00: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+0000fd10: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+0000fd20: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000fd30: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+0000fd40: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
+0000fd50: 2020 2020 2072 3d22 312e 3131 3937 3634       r="1.119764
+0000fd60: 3922 0a20 2020 2020 2020 7374 796c 653d  9".       style=
+0000fd70: 2266 696c 6c3a 2332 3533 6137 643b 6669  "fill:#253a7d;fi
+0000fd80: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+0000fd90: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+0000fda0: 6b65 2d77 6964 7468 3a30 2e37 3438 3939  ke-width:0.74899
+0000fdb0: 373b 7374 726f 6b65 2d6d 6974 6572 6c69  7;stroke-miterli
+0000fdc0: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+0000fdd0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+0000fde0: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+0000fdf0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+0000fe00: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+0000fe10: 6831 3435 3637 2d33 2d37 2d33 2d30 2d39  h14567-3-7-3-0-9
+0000fe20: 220a 2020 2020 2020 2063 783d 2233 3534  ".       cx="354
+0000fe30: 2e39 3632 3337 220a 2020 2020 2020 2063  .96237".       c
+0000fe40: 793d 2234 3533 2e30 3333 3131 220a 2020  y="453.03311".  
+0000fe50: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+0000fe60: 616e 7366 6f72 6d2d 6365 6e74 6572 2d78  ansform-center-x
+0000fe70: 3d22 342e 3634 3332 3536 3622 0a20 2020  ="4.6432566".   
+0000fe80: 2020 2020 696e 6b73 6361 7065 3a74 7261      inkscape:tra
+0000fe90: 6e73 666f 726d 2d63 656e 7465 722d 793d  nsform-center-y=
+0000fea0: 222d 392e 3937 3830 3632 3122 0a20 2020  "-9.9780621".   
+0000feb0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+0000fec0: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+0000fed0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+0000fee0: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+0000fef0: 202f 3e0a 2020 2020 3c63 6972 636c 650a   />.    <circle.
+0000ff00: 2020 2020 2020 2072 3d22 312e 3131 3937         r="1.1197
+0000ff10: 3634 3922 0a20 2020 2020 2020 7374 796c  649".       styl
+0000ff20: 653d 2266 696c 6c3a 2361 3861 3961 613b  e="fill:#a8a9aa;
+0000ff30: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+0000ff40: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+0000ff50: 726f 6b65 2d77 6964 7468 3a30 2e37 3438  roke-width:0.748
+0000ff60: 3939 373b 7374 726f 6b65 2d6d 6974 6572  997;stroke-miter
+0000ff70: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+0000ff80: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+0000ff90: 726f 6b65 2d64 6173 686f 6666 7365 743a  roke-dashoffset:
+0000ffa0: 303b 7374 726f 6b65 2d6f 7061 6369 7479  0;stroke-opacity
+0000ffb0: 3a31 220a 2020 2020 2020 2069 643d 2270  :1".       id="p
+0000ffc0: 6174 6831 3435 3637 2d33 2d35 2d38 2d38  ath14567-3-5-8-8
+0000ffd0: 2d35 220a 2020 2020 2020 2063 783d 2233  -5".       cx="3
+0000ffe0: 3535 2e32 3237 3934 220a 2020 2020 2020  55.22794".      
+0000fff0: 2063 793d 2234 3539 2e38 3034 3639 220a   cy="459.80469".
+00010000: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00010010: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+00010020: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
+00010030: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+00010040: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+00010050: 793d 222d 392e 3937 3830 3632 3122 0a20  y="-9.9780621". 
+00010060: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00010070: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+00010080: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00010090: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+000100a0: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
+000100b0: 650a 2020 2020 2020 2072 3d22 312e 3131  e.       r="1.11
+000100c0: 3937 3634 3922 0a20 2020 2020 2020 7374  97649".       st
+000100d0: 796c 653d 2266 696c 6c3a 2361 6261 6139  yle="fill:#abaa9
+000100e0: 633b 6669 6c6c 2d6f 7061 6369 7479 3a31  c;fill-opacity:1
+000100f0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00010100: 7374 726f 6b65 2d77 6964 7468 3a30 2e37  stroke-width:0.7
+00010110: 3438 3939 373b 7374 726f 6b65 2d6d 6974  48997;stroke-mit
+00010120: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00010130: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00010140: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00010150: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+00010160: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+00010170: 2270 6174 6831 3435 3637 2d33 2d39 2d30  "path14567-3-9-0
+00010180: 2d39 2d38 220a 2020 2020 2020 2063 783d  -9-8".       cx=
+00010190: 2233 3438 2e33 3233 3538 220a 2020 2020  "348.32358".    
+000101a0: 2020 2063 793d 2234 3635 2e31 3135 3732     cy="465.11572
+000101b0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+000101c0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+000101d0: 6572 2d78 3d22 342e 3634 3332 3536 3622  er-x="4.6432566"
+000101e0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+000101f0: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+00010200: 722d 793d 222d 392e 3937 3830 3632 3122  r-y="-9.9780621"
+00010210: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00010220: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+00010230: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+00010240: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+00010250: 3330 3022 202f 3e0a 2020 2020 3c63 6972  300" />.    <cir
+00010260: 636c 650a 2020 2020 2020 2072 3d22 312e  cle.       r="1.
+00010270: 3732 3832 3030 3222 0a20 2020 2020 2020  7282002".       
+00010280: 7374 796c 653d 2266 696c 6c3a 2331 3132  style="fill:#112
+00010290: 3036 363b 6669 6c6c 2d6f 7061 6369 7479  066;fill-opacity
+000102a0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+000102b0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+000102c0: 2e37 3438 3939 373b 7374 726f 6b65 2d6d  .748997;stroke-m
+000102d0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+000102e0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+000102f0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
+00010300: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
+00010310: 6369 7479 3a31 220a 2020 2020 2020 2069  city:1".       i
+00010320: 643d 2270 6174 6831 3435 3637 2d33 2d32  d="path14567-3-2
+00010330: 2d35 2d34 2d33 220a 2020 2020 2020 2063  -5-4-3".       c
+00010340: 783d 2233 3431 2e30 3230 3837 220a 2020  x="341.02087".  
+00010350: 2020 2020 2063 793d 2234 3338 2e38 3932       cy="438.892
+00010360: 3436 220a 2020 2020 2020 2069 6e6b 7363  46".       inksc
+00010370: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+00010380: 6e74 6572 2d78 3d22 372e 3136 3632 3131  nter-x="7.166211
+00010390: 3622 0a20 2020 2020 2020 696e 6b73 6361  6".       inksca
+000103a0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+000103b0: 7465 722d 793d 222d 3135 2e33 3939 3735  ter-y="-15.39975
+000103c0: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
+000103d0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+000103e0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+000103f0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+00010400: 3d22 3330 3022 202f 3e0a 2020 2020 3c63  ="300" />.    <c
+00010410: 6972 636c 650a 2020 2020 2020 2072 3d22  ircle.       r="
+00010420: 312e 3131 3937 3634 3922 0a20 2020 2020  1.1197649".     
+00010430: 2020 7374 796c 653d 2266 696c 6c3a 2365    style="fill:#e
+00010440: 6466 3066 633b 6669 6c6c 2d6f 7061 6369  df0fc;fill-opaci
+00010450: 7479 3a30 2e39 3930 3434 363b 7374 726f  ty:0.990446;stro
+00010460: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00010470: 652d 7769 6474 683a 302e 3734 3839 3937  e-width:0.748997
+00010480: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00010490: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+000104a0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+000104b0: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+000104c0: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+000104d0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+000104e0: 3134 3536 372d 322d 362d 302d 3022 0a20  14567-2-6-0-0". 
+000104f0: 2020 2020 2020 6378 3d22 3335 302e 3338        cx="350.38
+00010500: 3135 3922 0a20 2020 2020 2020 6379 3d22  159".       cy="
+00010510: 3434 302e 3831 3737 3222 0a20 2020 2020  440.81772".     
+00010520: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00010530: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+00010540: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00010550: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+00010560: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
+00010570: 2020 2020 2072 3d22 312e 3131 3937 3634       r="1.119764
+00010580: 3922 0a20 2020 2020 2020 7374 796c 653d  9".       style=
+00010590: 2266 696c 6c3a 2365 6466 3066 633b 6669  "fill:#edf0fc;fi
+000105a0: 6c6c 2d6f 7061 6369 7479 3a30 2e39 3930  ll-opacity:0.990
+000105b0: 3434 363b 7374 726f 6b65 3a23 6666 6666  446;stroke:#ffff
+000105c0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+000105d0: 302e 3734 3839 3937 3b73 7472 6f6b 652d  0.748997;stroke-
+000105e0: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+000105f0: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00010600: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+00010610: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+00010620: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00010630: 6964 3d22 7061 7468 3134 3536 372d 322d  id="path14567-2-
+00010640: 382d 362d 372d 3822 0a20 2020 2020 2020  8-6-7-8".       
+00010650: 6378 3d22 3333 302e 3939 3632 3822 0a20  cx="330.99628". 
+00010660: 2020 2020 2020 6379 3d22 3435 302e 3131        cy="450.11
+00010670: 3230 3322 0a20 2020 2020 2020 696e 6b73  203".       inks
+00010680: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+00010690: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+000106a0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+000106b0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+000106c0: 3c63 6972 636c 650a 2020 2020 2020 2072  <circle.       r
+000106d0: 3d22 322e 3132 3835 3038 3622 0a20 2020  ="2.1285086".   
+000106e0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+000106f0: 2365 6466 3066 633b 6669 6c6c 2d6f 7061  #edf0fc;fill-opa
+00010700: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
+00010710: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00010720: 6f6b 652d 7769 6474 683a 312e 3432 3337  oke-width:1.4237
+00010730: 333b 7374 726f 6b65 2d6d 6974 6572 6c69  3;stroke-miterli
+00010740: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00010750: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00010760: 6b65 2d64 6173 686f 6666 7365 743a 303b  ke-dashoffset:0;
+00010770: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+00010780: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00010790: 6831 3435 3637 2d32 2d37 2d30 2d39 2d30  h14567-2-7-0-9-0
+000107a0: 220a 2020 2020 2020 2063 783d 2233 3735  ".       cx="375
+000107b0: 2e31 3434 3335 220a 2020 2020 2020 2063  .14435".       c
+000107c0: 793d 2234 3436 2e30 3632 3338 220a 2020  y="446.06238".  
+000107d0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+000107e0: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+000107f0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00010800: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+00010810: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+00010820: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00010830: 6c3a 2333 6534 6237 373b 6669 6c6c 2d6f  l:#3e4b77;fill-o
+00010840: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00010850: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+00010860: 6964 7468 3a30 2e38 3435 3032 353b 7374  idth:0.845025;st
+00010870: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00010880: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00010890: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+000108a0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+000108b0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+000108c0: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+000108d0: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
+000108e0: 3430 382e 3136 3632 2c34 3431 2e36 3137  408.1662,441.617
+000108f0: 3320 3136 2e33 3435 352c 2d30 2e37 3432  3 16.3455,-0.742
+00010900: 3938 2031 302e 3733 3934 2c2d 3131 2e39  98 10.7394,-11.9
+00010910: 3535 3138 2063 202d 3133 2e35 3239 3337  5518 c -13.52937
+00010920: 2c39 2e30 3938 3733 202d 3139 2e39 3933  ,9.09873 -19.993
+00010930: 3132 2c31 302e 3535 3839 3820 2d32 372e  12,10.55898 -27.
+00010940: 3038 3439 2c31 322e 3639 3831 3620 7a22  0849,12.69816 z"
+00010950: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00010960: 3134 3534 372d 312d 372d 382d 3322 0a20  14547-1-7-8-3". 
+00010970: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00010980: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00010990: 7265 3d22 3022 0a20 2020 2020 2020 736f  re="0".       so
+000109a0: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+000109b0: 3d22 6363 6363 220a 2020 2020 2020 2069  ="cccc".       i
+000109c0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+000109d0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+000109e0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+000109f0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+00010a00: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00010a10: 7374 796c 653d 2266 696c 6c3a 2331 6332  style="fill:#1c2
+00010a20: 6336 383b 6669 6c6c 2d6f 7061 6369 7479  c68;fill-opacity
+00010a30: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00010a40: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+00010a50: 2e38 3435 3032 353b 7374 726f 6b65 2d6c  .845025;stroke-l
+00010a60: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00010a70: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00010a80: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+00010a90: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00010aa0: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00010ab0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00010ac0: 2020 2020 2064 3d22 6d20 3432 342e 3531       d="m 424.51
+00010ad0: 3137 2c34 3430 2e38 3734 3332 2037 2e30  17,440.87432 7.0
+00010ae0: 3932 3035 2c31 2e36 3231 3034 2033 2e36  9205,1.62104 3.6
+00010af0: 3437 3335 2c2d 3133 2e35 3736 3232 207a  4735,-13.57622 z
+00010b00: 220a 2020 2020 2020 2069 643d 2270 6174  ".       id="pat
+00010b10: 6831 3435 3439 2d31 2d30 2d31 2d36 220a  h14549-1-0-1-6".
+00010b20: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00010b30: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00010b40: 7572 653d 2230 220a 2020 2020 2020 2069  ure="0".       i
+00010b50: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+00010b60: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+00010b70: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00010b80: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+00010b90: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00010ba0: 7374 796c 653d 2266 696c 6c3a 2330 3630  style="fill:#060
+00010bb0: 3530 383b 6669 6c6c 2d6f 7061 6369 7479  508;fill-opacity
+00010bc0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00010bd0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+00010be0: 2e38 3435 3032 353b 7374 726f 6b65 2d6c  .845025;stroke-l
+00010bf0: 696e 6563 6170 3a62 7574 743b 7374 726f  inecap:butt;stro
+00010c00: 6b65 2d6c 696e 656a 6f69 6e3a 6d69 7465  ke-linejoin:mite
+00010c10: 723b 7374 726f 6b65 2d6d 6974 6572 6c69  r;stroke-miterli
+00010c20: 6d69 743a 343b 7374 726f 6b65 2d64 6173  mit:4;stroke-das
+00010c30: 6861 7272 6179 3a6e 6f6e 653b 7374 726f  harray:none;stro
+00010c40: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00010c50: 2020 2020 2064 3d22 6d20 3433 312e 3630       d="m 431.60
+00010c60: 3337 352c 3434 322e 3439 3533 3620 3138  375,442.49536 18
+00010c70: 2e39 3739 372c 332e 3337 3731 3820 6320  .9797,3.37718 c 
+00010c80: 2d37 2e33 3936 3037 2c2d 332e 3930 3939  -7.39607,-3.9099
+00010c90: 3820 2d31 312e 3637 392c 2d31 302e 3139  8 -11.679,-10.19
+00010ca0: 3138 3320 2d31 352e 3333 3233 352c 2d31  183 -15.33235,-1
+00010cb0: 362e 3935 3334 207a 220a 2020 2020 2020  6.9534 z".      
+00010cc0: 2069 643d 2270 6174 6831 3435 3531 2d30   id="path14551-0
+00010cd0: 2d33 2d39 2d37 220a 2020 2020 2020 2069  -3-9-7".       i
+00010ce0: 6e6b 7363 6170 653a 636f 6e6e 6563 746f  nkscape:connecto
+00010cf0: 722d 6375 7276 6174 7572 653d 2230 220a  r-curvature="0".
+00010d00: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
+00010d10: 6e6f 6465 7479 7065 733d 2263 6363 6322  nodetypes="cccc"
+00010d20: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00010d30: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+00010d40: 3022 0a20 2020 2020 2020 696e 6b73 6361  0".       inksca
+00010d50: 7065 3a65 7870 6f72 742d 7964 7069 3d22  pe:export-ydpi="
+00010d60: 3330 3022 202f 3e0a 2020 2020 3c70 6174  300" />.    <pat
+00010d70: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
+00010d80: 6669 6c6c 3a23 3237 3337 3733 3b66 696c  fill:#273773;fil
+00010d90: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00010da0: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00010db0: 652d 7769 6474 683a 302e 3834 3530 3235  e-width:0.845025
+00010dc0: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00010dd0: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00010de0: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00010df0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00010e00: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00010e10: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00010e20: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
+00010e30: 226d 2034 3038 2e31 3636 322c 3434 312e  "m 408.1662,441.
+00010e40: 3631 3733 2063 2033 2e35 3936 3837 2c32  6173 c 3.59687,2
+00010e50: 2e30 3633 3420 372e 3536 3236 352c 332e  .0634 7.56265,3.
+00010e60: 3834 3330 3220 382e 3931 3537 332c 372e  84302 8.91573,7.
+00010e70: 3633 3234 206c 2037 2e34 3239 3737 2c2d  6324 l 7.42977,-
+00010e80: 382e 3337 3533 3820 7a22 0a20 2020 2020  8.37538 z".     
+00010e90: 2020 6964 3d22 7061 7468 3134 3535 332d    id="path14553-
+00010ea0: 332d 322d 322d 3522 0a20 2020 2020 2020  3-2-2-5".       
+00010eb0: 696e 6b73 6361 7065 3a63 6f6e 6e65 6374  inkscape:connect
+00010ec0: 6f72 2d63 7572 7661 7475 7265 3d22 3022  or-curvature="0"
+00010ed0: 0a20 2020 2020 2020 736f 6469 706f 6469  .       sodipodi
+00010ee0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+00010ef0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00010f00: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+00010f10: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+00010f20: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+00010f30: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
+00010f40: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+00010f50: 2266 696c 6c3a 2331 3432 3637 323b 6669  "fill:#142672;fi
+00010f60: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00010f70: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00010f80: 6b65 2d77 6964 7468 3a30 2e38 3435 3032  ke-width:0.84502
+00010f90: 353b 7374 726f 6b65 2d6c 696e 6563 6170  5;stroke-linecap
+00010fa0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00010fb0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00010fc0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00010fd0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00010fe0: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00010ff0: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00011000: 3d22 6d20 3431 372e 3038 3139 332c 3434  ="m 417.08193,44
+00011010: 392e 3234 3937 2033 332e 3530 3135 322c  9.2497 33.50152,
+00011020: 2d33 2e33 3737 3136 202d 3236 2e30 3731  -3.37716 -26.071
+00011030: 3735 2c2d 342e 3939 3832 3220 7a22 0a20  75,-4.99822 z". 
+00011040: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00011050: 3535 352d 342d 312d 362d 3322 0a20 2020  555-4-1-6-3".   
+00011060: 2020 2020 696e 6b73 6361 7065 3a63 6f6e      inkscape:con
+00011070: 6e65 6374 6f72 2d63 7572 7661 7475 7265  nector-curvature
+00011080: 3d22 3022 0a20 2020 2020 2020 696e 6b73  ="0".       inks
+00011090: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+000110a0: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+000110b0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+000110c0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+000110d0: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+000110e0: 6c65 3d22 6669 6c6c 3a23 3534 3636 3863  le="fill:#54668c
+000110f0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00011100: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00011110: 7472 6f6b 652d 7769 6474 683a 302e 3834  troke-width:0.84
+00011120: 3530 3235 3b73 7472 6f6b 652d 6c69 6e65  5025;stroke-line
+00011130: 6361 703a 6275 7474 3b73 7472 6f6b 652d  cap:butt;stroke-
+00011140: 6c69 6e65 6a6f 696e 3a6d 6974 6572 3b73  linejoin:miter;s
+00011150: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00011160: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00011170: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00011180: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00011190: 2020 643d 226d 2034 3137 2e30 3831 3933    d="m 417.08193
+000111a0: 2c34 3439 2e32 3439 3720 3139 2e33 3137  ,449.2497 19.317
+000111b0: 3431 2c32 2e30 3236 3331 2031 342e 3138  41,2.02631 14.18
+000111c0: 3431 312c 2d35 2e34 3033 3437 207a 220a  411,-5.40347 z".
+000111d0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+000111e0: 3435 3537 2d30 2d37 2d33 2d35 220a 2020  4557-0-7-3-5".  
+000111f0: 2020 2020 2069 6e6b 7363 6170 653a 636f       inkscape:co
+00011200: 6e6e 6563 746f 722d 6375 7276 6174 7572  nnector-curvatur
+00011210: 653d 2230 220a 2020 2020 2020 2069 6e6b  e="0".       ink
+00011220: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
+00011230: 693d 2233 3030 220a 2020 2020 2020 2069  i="300".       i
+00011240: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+00011250: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+00011260: 203c 7061 7468 0a20 2020 2020 2020 7374   <path.       st
+00011270: 796c 653d 2266 696c 6c3a 2332 3233 3437  yle="fill:#22347
+00011280: 653b 6669 6c6c 2d6f 7061 6369 7479 3a31  e;fill-opacity:1
+00011290: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+000112a0: 7374 726f 6b65 2d77 6964 7468 3a30 2e38  stroke-width:0.8
+000112b0: 3435 3032 353b 7374 726f 6b65 2d6c 696e  45025;stroke-lin
+000112c0: 6563 6170 3a62 7574 743b 7374 726f 6b65  ecap:butt;stroke
+000112d0: 2d6c 696e 656a 6f69 6e3a 6d69 7465 723b  -linejoin:miter;
+000112e0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+000112f0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00011300: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00011310: 2d6f 7061 6369 7479 3a31 220a 2020 2020  -opacity:1".    
+00011320: 2020 2064 3d22 6d20 3431 372e 3038 3139     d="m 417.0819
+00011330: 332c 3434 392e 3234 3937 2063 2030 2e34  3,449.2497 c 0.4
+00011340: 3334 3338 2c33 2e37 3435 3333 202d 312e  3438,3.74533 -1.
+00011350: 3036 3931 382c 362e 3130 3634 3320 2d31  06918,6.10643 -1
+00011360: 2e37 3536 3133 2c39 2e30 3530 3832 206c  .75613,9.05082 l
+00011370: 2032 312e 3037 3335 342c 2d37 2e30 3234   21.07354,-7.024
+00011380: 3531 207a 220a 2020 2020 2020 2069 643d  51 z".       id=
+00011390: 2270 6174 6831 3435 3539 2d33 2d34 2d32  "path14559-3-4-2
+000113a0: 2d36 220a 2020 2020 2020 2069 6e6b 7363  -6".       inksc
+000113b0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+000113c0: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+000113d0: 2020 2073 6f64 6970 6f64 693a 6e6f 6465     sodipodi:node
+000113e0: 7479 7065 733d 2263 6363 6322 0a20 2020  types="cccc".   
+000113f0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00011400: 6f72 742d 7864 7069 3d22 3330 3022 0a20  ort-xdpi="300". 
+00011410: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00011420: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+00011430: 202f 3e0a 2020 2020 3c70 6174 680a 2020   />.    <path.  
+00011440: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00011450: 3a23 3038 3130 3639 3b66 696c 6c2d 6f70  :#081069;fill-op
+00011460: 6163 6974 793a 313b 7374 726f 6b65 3a23  acity:1;stroke:#
+00011470: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00011480: 6474 683a 302e 3834 3530 3235 3b73 7472  dth:0.845025;str
+00011490: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+000114a0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+000114b0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+000114c0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+000114d0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+000114e0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+000114f0: 3122 0a20 2020 2020 2020 643d 226d 2034  1".       d="m 4
+00011500: 3135 2e33 3235 382c 3435 382e 3330 3035  15.3258,458.3005
+00011510: 3220 3134 2e35 3839 3337 2c32 2e31 3631  2 14.58937,2.161
+00011520: 3339 2032 302e 3636 3832 382c 2d31 342e  39 20.66828,-14.
+00011530: 3538 3933 3720 7a22 0a20 2020 2020 2020  58937 z".       
+00011540: 6964 3d22 7061 7468 3134 3536 312d 392d  id="path14561-9-
+00011550: 322d 322d 3222 0a20 2020 2020 2020 696e  2-2-2".       in
+00011560: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00011570: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+00011580: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00011590: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+000115a0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+000115b0: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+000115c0: 3022 202f 3e0a 2020 2020 3c70 6174 680a  0" />.    <path.
+000115d0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+000115e0: 6c6c 3a23 3037 3065 3262 3b66 696c 6c2d  ll:#070e2b;fill-
+000115f0: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00011600: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+00011610: 7769 6474 683a 302e 3834 3530 3235 3b73  width:0.845025;s
+00011620: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00011630: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00011640: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00011650: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00011660: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00011670: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00011680: 793a 3122 0a20 2020 2020 2020 643d 226d  y:1".       d="m
+00011690: 2034 3239 2e39 3135 3137 2c34 3630 2e34   429.91517,460.4
+000116a0: 3631 3931 2038 2e35 3738 3031 2c31 312e  6191 8.57801,11.
+000116b0: 3237 3937 3420 2d33 2e31 3734 3534 2c2d  27974 -3.17454,-
+000116c0: 3135 2e31 3937 3236 207a 220a 2020 2020  15.19726 z".    
+000116d0: 2020 2069 643d 2270 6174 6831 3435 3633     id="path14563
+000116e0: 2d31 2d30 2d36 2d39 220a 2020 2020 2020  -1-0-6-9".      
+000116f0: 2069 6e6b 7363 6170 653a 636f 6e6e 6563   inkscape:connec
+00011700: 746f 722d 6375 7276 6174 7572 653d 2230  tor-curvature="0
+00011710: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00011720: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+00011730: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+00011740: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+00011750: 2233 3030 2220 2f3e 0a20 2020 203c 7061  "300" />.    <pa
+00011760: 7468 0a20 2020 2020 2020 7374 796c 653d  th.       style=
+00011770: 2266 696c 6c3a 2332 3833 6438 373b 6669  "fill:#283d87;fi
+00011780: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+00011790: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+000117a0: 6b65 2d77 6964 7468 3a30 2e38 3435 3032  ke-width:0.84502
+000117b0: 353b 7374 726f 6b65 2d6c 696e 6563 6170  5;stroke-linecap
+000117c0: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+000117d0: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+000117e0: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+000117f0: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00011800: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00011810: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00011820: 3d22 6d20 3433 352e 3331 3836 342c 3435  ="m 435.31864,45
+00011830: 362e 3534 3433 3920 332e 3137 3435 342c  6.54439 3.17454,
+00011840: 3135 2e31 3937 3236 2063 2031 2e36 3433  15.19726 c 1.643
+00011850: 3339 2c2d 3133 2e36 3631 3632 2037 2e34  39,-13.66162 7.4
+00011860: 3236 3635 2c2d 3138 2e35 3833 3533 2031  2665,-18.58353 1
+00011870: 322e 3039 3032 372c 2d32 352e 3836 3931  2.09027,-25.8691
+00011880: 3120 7a22 0a20 2020 2020 2020 6964 3d22  1 z".       id="
+00011890: 7061 7468 3134 3536 352d 392d 352d 392d  path14565-9-5-9-
+000118a0: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
+000118b0: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+000118c0: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+000118d0: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+000118e0: 7970 6573 3d22 6363 6363 220a 2020 2020  ypes="cccc".    
+000118f0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+00011900: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+00011910: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+00011920: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+00011930: 2f3e 0a20 2020 203c 656c 6c69 7073 650a  />.    <ellipse.
+00011940: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00011950: 6c6c 3a23 3037 3065 3262 3b66 696c 6c2d  ll:#070e2b;fill-
+00011960: 6f70 6163 6974 793a 302e 3939 3034 3436  opacity:0.990446
+00011970: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00011980: 7374 726f 6b65 2d77 6964 7468 3a30 2e38  stroke-width:0.8
+00011990: 3435 3032 353b 7374 726f 6b65 2d6d 6974  45025;stroke-mit
+000119a0: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+000119b0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+000119c0: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+000119d0: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+000119e0: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+000119f0: 2270 6174 6831 3435 3637 2d36 2d31 2d39  "path14567-6-1-9
+00011a00: 2d32 220a 2020 2020 2020 2063 783d 2234  -2".       cx="4
+00011a10: 3038 2e35 3133 3039 220a 2020 2020 2020  08.51309".      
+00011a20: 2063 793d 2234 3431 2e36 3334 3631 220a   cy="441.63461".
+00011a30: 2020 2020 2020 2072 783d 2230 2e38 3432         rx="0.842
+00011a40: 3231 3930 3522 0a20 2020 2020 2020 7279  21905".       ry
+00011a50: 3d22 302e 3834 3232 3139 3131 220a 2020  ="0.84221911".  
+00011a60: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+00011a70: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+00011a80: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00011a90: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+00011aa0: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
+00011ab0: 0a20 2020 2020 2020 723d 2230 2e38 3432  .       r="0.842
+00011ac0: 3231 3931 3122 0a20 2020 2020 2020 7374  21911".       st
+00011ad0: 796c 653d 2266 696c 6c3a 2332 3533 6137  yle="fill:#253a7
+00011ae0: 643b 6669 6c6c 2d6f 7061 6369 7479 3a31  d;fill-opacity:1
+00011af0: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00011b00: 7374 726f 6b65 2d77 6964 7468 3a30 2e38  stroke-width:0.8
+00011b10: 3435 3032 353b 7374 726f 6b65 2d6d 6974  45025;stroke-mit
+00011b20: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00011b30: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00011b40: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00011b50: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+00011b60: 7479 3a31 220a 2020 2020 2020 2069 643d  ty:1".       id=
+00011b70: 2270 6174 6831 3435 3637 2d33 2d39 332d  "path14567-3-93-
+00011b80: 312d 362d 3722 0a20 2020 2020 2020 6378  1-6-7".       cx
+00011b90: 3d22 3431 352e 3139 3032 3822 0a20 2020  ="415.19028".   
+00011ba0: 2020 2020 6379 3d22 3435 382e 3132 3038      cy="458.1208
+00011bb0: 3522 0a20 2020 2020 2020 696e 6b73 6361  5".       inksca
+00011bc0: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+00011bd0: 7465 722d 783d 2233 2e34 3932 3337 3233  ter-x="3.4923723
+00011be0: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00011bf0: 653a 7472 616e 7366 6f72 6d2d 6365 6e74  e:transform-cent
+00011c00: 6572 2d79 3d22 2d37 2e35 3034 3838 3937  er-y="-7.5048897
+00011c10: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00011c20: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+00011c30: 3030 220a 2020 2020 2020 2069 6e6b 7363  00".       inksc
+00011c40: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+00011c50: 2233 3030 2220 2f3e 0a20 2020 203c 6369  "300" />.    <ci
+00011c60: 7263 6c65 0a20 2020 2020 2020 723d 2230  rcle.       r="0
+00011c70: 2e38 3432 3231 3931 3122 0a20 2020 2020  .84221911".     
+00011c80: 2020 7374 796c 653d 2266 696c 6c3a 2332    style="fill:#2
+00011c90: 3533 6137 643b 6669 6c6c 2d6f 7061 6369  53a7d;fill-opaci
+00011ca0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+00011cb0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00011cc0: 3a30 2e38 3435 3032 353b 7374 726f 6b65  :0.845025;stroke
+00011cd0: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00011ce0: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00011cf0: 6f6e 653b 7374 726f 6b65 2d64 6173 686f  one;stroke-dasho
+00011d00: 6666 7365 743a 303b 7374 726f 6b65 2d6f  ffset:0;stroke-o
+00011d10: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00011d20: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
+00011d30: 2d37 2d33 2d30 2d39 2d30 220a 2020 2020  -7-3-0-9-0".    
+00011d40: 2020 2063 783d 2234 3335 2e31 3133 3536     cx="435.11356
+00011d50: 220a 2020 2020 2020 2063 793d 2234 3531  ".       cy="451
+00011d60: 2e33 3239 3933 220a 2020 2020 2020 2069  .32993".       i
+00011d70: 6e6b 7363 6170 653a 7472 616e 7366 6f72  nkscape:transfor
+00011d80: 6d2d 6365 6e74 6572 2d78 3d22 332e 3439  m-center-x="3.49
+00011d90: 3233 3731 3622 0a20 2020 2020 2020 696e  23716".       in
+00011da0: 6b73 6361 7065 3a74 7261 6e73 666f 726d  kscape:transform
+00011db0: 2d63 656e 7465 722d 793d 222d 372e 3530  -center-y="-7.50
+00011dc0: 3438 3931 3122 0a20 2020 2020 2020 696e  48911".       in
+00011dd0: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+00011de0: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+00011df0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00011e00: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
+00011e10: 2020 3c63 6972 636c 650a 2020 2020 2020    <circle.      
+00011e20: 2072 3d22 302e 3834 3232 3139 3131 220a   r="0.84221911".
+00011e30: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00011e40: 6c6c 3a23 6138 6139 6161 3b66 696c 6c2d  ll:#a8a9aa;fill-
+00011e50: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00011e60: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+00011e70: 7769 6474 683a 302e 3834 3530 3235 3b73  width:0.845025;s
+00011e80: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00011e90: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00011ea0: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00011eb0: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
+00011ec0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00011ed0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00011ee0: 3536 372d 332d 352d 382d 382d 352d 3922  567-3-5-8-8-5-9"
+00011ef0: 0a20 2020 2020 2020 6378 3d22 3433 352e  .       cx="435.
+00011f00: 3331 3332 3922 0a20 2020 2020 2020 6379  31329".       cy
+00011f10: 3d22 3435 362e 3432 3331 220a 2020 2020  ="456.4231".    
+00011f20: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
+00011f30: 7366 6f72 6d2d 6365 6e74 6572 2d78 3d22  sform-center-x="
+00011f40: 332e 3439 3233 3730 3622 0a20 2020 2020  3.4923706".     
+00011f50: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00011f60: 666f 726d 2d63 656e 7465 722d 793d 222d  form-center-y="-
+00011f70: 372e 3530 3438 3935 3822 0a20 2020 2020  7.5048958".     
+00011f80: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00011f90: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+00011fa0: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00011fb0: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+00011fc0: 3e0a 2020 2020 3c63 6972 636c 650a 2020  >.    <circle.  
+00011fd0: 2020 2020 2072 3d22 302e 3834 3232 3139       r="0.842219
+00011fe0: 3131 220a 2020 2020 2020 2073 7479 6c65  11".       style
+00011ff0: 3d22 6669 6c6c 3a23 6162 6161 3963 3b66  ="fill:#abaa9c;f
+00012000: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00012010: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00012020: 6f6b 652d 7769 6474 683a 302e 3834 3530  oke-width:0.8450
+00012030: 3235 3b73 7472 6f6b 652d 6d69 7465 726c  25;stroke-miterl
+00012040: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+00012050: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+00012060: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+00012070: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00012080: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
+00012090: 7468 3134 3536 372d 332d 392d 302d 392d  th14567-3-9-0-9-
+000120a0: 382d 3322 0a20 2020 2020 2020 6378 3d22  8-3".       cx="
+000120b0: 3433 302e 3132 3032 3422 0a20 2020 2020  430.12024".     
+000120c0: 2020 6379 3d22 3436 302e 3431 3737 3622    cy="460.41776"
+000120d0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+000120e0: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+000120f0: 722d 783d 2233 2e34 3932 3337 3135 220a  r-x="3.4923715".
+00012100: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00012110: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+00012120: 2d79 3d22 2d37 2e35 3034 3839 3037 220a  -y="-7.5048907".
+00012130: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00012140: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+00012150: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00012160: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+00012170: 3030 2220 2f3e 0a20 2020 203c 6369 7263  00" />.    <circ
+00012180: 6c65 0a20 2020 2020 2020 723d 2231 2e32  le.       r="1.2
+00012190: 3939 3834 3731 220a 2020 2020 2020 2073  998471".       s
+000121a0: 7479 6c65 3d22 6669 6c6c 3a23 3131 3230  tyle="fill:#1120
+000121b0: 3636 3b66 696c 6c2d 6f70 6163 6974 793a  66;fill-opacity:
+000121c0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+000121d0: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
+000121e0: 3834 3530 3235 3b73 7472 6f6b 652d 6d69  845025;stroke-mi
+000121f0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00012200: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00012210: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
+00012220: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
+00012230: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
+00012240: 3d22 7061 7468 3134 3536 372d 332d 322d  ="path14567-3-2-
+00012250: 352d 342d 332d 3622 0a20 2020 2020 2020  5-4-3-6".       
+00012260: 6378 3d22 3432 342e 3632 3735 3922 0a20  cx="424.62759". 
+00012270: 2020 2020 2020 6379 3d22 3434 302e 3639        cy="440.69
+00012280: 3432 3122 0a20 2020 2020 2020 696e 6b73  421".       inks
+00012290: 6361 7065 3a74 7261 6e73 666f 726d 2d63  cape:transform-c
+000122a0: 656e 7465 722d 783d 2235 2e33 3839 3939  enter-x="5.38999
+000122b0: 3234 220a 2020 2020 2020 2069 6e6b 7363  24".       inksc
+000122c0: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+000122d0: 6e74 6572 2d79 3d22 2d31 312e 3538 3237  nter-y="-11.5827
+000122e0: 3533 220a 2020 2020 2020 2069 6e6b 7363  53".       inksc
+000122f0: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+00012300: 2233 3030 220a 2020 2020 2020 2069 6e6b  "300".       ink
+00012310: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+00012320: 693d 2233 3030 2220 2f3e 0a20 2020 203c  i="300" />.    <
+00012330: 6369 7263 6c65 0a20 2020 2020 2020 723d  circle.       r=
+00012340: 2230 2e38 3432 3231 3931 3122 0a20 2020  "0.84221911".   
+00012350: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00012360: 2365 6466 3066 633b 6669 6c6c 2d6f 7061  #edf0fc;fill-opa
+00012370: 6369 7479 3a30 2e39 3930 3434 363b 7374  city:0.990446;st
+00012380: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00012390: 6f6b 652d 7769 6474 683a 302e 3834 3530  oke-width:0.8450
+000123a0: 3235 3b73 7472 6f6b 652d 6d69 7465 726c  25;stroke-miterl
+000123b0: 696d 6974 3a34 3b73 7472 6f6b 652d 6461  imit:4;stroke-da
+000123c0: 7368 6172 7261 793a 6e6f 6e65 3b73 7472  sharray:none;str
+000123d0: 6f6b 652d 6461 7368 6f66 6673 6574 3a30  oke-dashoffset:0
+000123e0: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+000123f0: 3122 0a20 2020 2020 2020 6964 3d22 7061  1".       id="pa
+00012400: 7468 3134 3536 372d 322d 362d 302d 302d  th14567-2-6-0-0-
+00012410: 3022 0a20 2020 2020 2020 6378 3d22 3433  0".       cx="43
+00012420: 312e 3636 3831 3822 0a20 2020 2020 2020  1.66818".       
+00012430: 6379 3d22 3434 322e 3134 3232 3422 0a20  cy="442.14224". 
+00012440: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00012450: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+00012460: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00012470: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+00012480: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
+00012490: 650a 2020 2020 2020 2072 3d22 302e 3834  e.       r="0.84
+000124a0: 3232 3139 3131 220a 2020 2020 2020 2073  221911".       s
+000124b0: 7479 6c65 3d22 6669 6c6c 3a23 6564 6630  tyle="fill:#edf0
+000124c0: 6663 3b66 696c 6c2d 6f70 6163 6974 793a  fc;fill-opacity:
+000124d0: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
+000124e0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+000124f0: 6964 7468 3a30 2e38 3435 3032 353b 7374  idth:0.845025;st
+00012500: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00012510: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00012520: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+00012530: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+00012540: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00012550: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00012560: 3637 2d32 2d38 2d36 2d37 2d38 2d36 220a  67-2-8-6-7-8-6".
+00012570: 2020 2020 2020 2063 783d 2234 3137 2e30         cx="417.0
+00012580: 3837 3734 220a 2020 2020 2020 2063 793d  8774".       cy=
+00012590: 2234 3439 2e31 3332 3837 220a 2020 2020  "449.13287".    
+000125a0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+000125b0: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+000125c0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+000125d0: 706f 7274 2d79 6470 693d 2233 3030 2220  port-ydpi="300" 
+000125e0: 2f3e 0a20 2020 203c 6369 7263 6c65 0a20  />.    <circle. 
+000125f0: 2020 2020 2020 723d 2231 2e36 3030 3933        r="1.60093
+00012600: 3437 220a 2020 2020 2020 2073 7479 6c65  47".       style
+00012610: 3d22 6669 6c6c 3a23 6564 6630 6663 3b66  ="fill:#edf0fc;f
+00012620: 696c 6c2d 6f70 6163 6974 793a 302e 3939  ill-opacity:0.99
+00012630: 3034 3436 3b73 7472 6f6b 653a 2366 6666  0446;stroke:#fff
+00012640: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00012650: 3a31 2e36 3036 3235 3b73 7472 6f6b 652d  :1.60625;stroke-
+00012660: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00012670: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00012680: 6e65 3b73 7472 6f6b 652d 6461 7368 6f66  ne;stroke-dashof
+00012690: 6673 6574 3a30 3b73 7472 6f6b 652d 6f70  fset:0;stroke-op
+000126a0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+000126b0: 6964 3d22 7061 7468 3134 3536 372d 322d  id="path14567-2-
+000126c0: 372d 302d 392d 302d 3222 0a20 2020 2020  7-0-9-0-2".     
+000126d0: 2020 6378 3d22 3435 302e 3239 3331 3822    cx="450.29318"
+000126e0: 0a20 2020 2020 2020 6379 3d22 3434 362e  .       cy="446.
+000126f0: 3038 3639 3822 0a20 2020 2020 2020 696e  08698".       in
+00012700: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+00012710: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+00012720: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00012730: 7964 7069 3d22 3330 3022 202f 3e0a 2020  ydpi="300" />.  
+00012740: 2020 3c67 0a20 2020 2020 2020 6964 3d22    <g.       id="
+00012750: 6731 3338 3122 0a20 2020 2020 2020 7472  g1381".       tr
+00012760: 616e 7366 6f72 6d3d 226d 6174 7269 7828  ansform="matrix(
+00012770: 372e 3535 3137 3338 342c 302c 302c 372e  7.5517384,0,0,7.
+00012780: 3535 3137 3338 342c 2d36 3933 2e38 3533  5517384,-693.853
+00012790: 3335 2c2d 3832 352e 3033 3835 3929 223e  35,-825.03859)">
+000127a0: 0a20 2020 2020 203c 7061 7468 0a20 2020  .      <path.   
+000127b0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+000127c0: 6c3a 2333 6534 6237 373b 6669 6c6c 2d6f  l:#3e4b77;fill-o
+000127d0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+000127e0: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+000127f0: 6964 7468 3a30 3b73 7472 6f6b 652d 6c69  idth:0;stroke-li
+00012800: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00012810: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00012820: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00012830: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00012840: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00012850: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00012860: 2020 2020 2020 643d 226d 2031 3534 2e31        d="m 154.1
+00012870: 3532 3636 2c31 3435 2e32 3530 3038 2031  5266,145.25008 1
+00012880: 2e34 3337 3438 2c2d 302e 3036 3533 2030  .43748,-0.0653 0
+00012890: 2e39 3434 3437 2c2d 312e 3035 3133 3820  .94447,-1.05138 
+000128a0: 6320 2d31 2e31 3839 3833 2c30 2e38 3030  c -1.18983,0.800
+000128b0: 3138 202d 312e 3735 3832 372c 302e 3932  18 -1.75827,0.92
+000128c0: 3836 202d 322e 3338 3139 352c 312e 3131  86 -2.38195,1.11
+000128d0: 3637 3220 7a22 0a20 2020 2020 2020 2020  672 z".         
+000128e0: 6964 3d22 7061 7468 3134 3534 372d 312d  id="path14547-1-
+000128f0: 372d 382d 352d 302d 332d 3422 0a20 2020  7-8-5-0-3-4".   
+00012900: 2020 2020 2020 696e 6b73 6361 7065 3a63        inkscape:c
+00012910: 6f6e 6e65 6374 6f72 2d63 7572 7661 7475  onnector-curvatu
+00012920: 7265 3d22 3022 0a20 2020 2020 2020 2020  re="0".         
+00012930: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
+00012940: 6573 3d22 6363 6363 220a 2020 2020 2020  es="cccc".      
+00012950: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+00012960: 7274 2d78 6470 693d 2233 3030 220a 2020  rt-xdpi="300".  
+00012970: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00012980: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+00012990: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
+000129a0: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
+000129b0: 2266 696c 6c3a 2330 3630 3530 383b 6669  "fill:#060508;fi
+000129c0: 6c6c 2d6f 7061 6369 7479 3a31 3b73 7472  ll-opacity:1;str
+000129d0: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+000129e0: 6b65 2d77 6964 7468 3a30 3b73 7472 6f6b  ke-width:0;strok
+000129f0: 652d 6c69 6e65 6361 703a 6275 7474 3b73  e-linecap:butt;s
+00012a00: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a6d  troke-linejoin:m
+00012a10: 6974 6572 3b73 7472 6f6b 652d 6d69 7465  iter;stroke-mite
+00012a20: 726c 696d 6974 3a34 3b73 7472 6f6b 652d  rlimit:4;stroke-
+00012a30: 6461 7368 6172 7261 793a 6e6f 6e65 3b73  dasharray:none;s
+00012a40: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00012a50: 0a20 2020 2020 2020 2020 643d 226d 2031  .         d="m 1
+00012a60: 3535 2e35 3930 3134 2c31 3435 2e31 3834  55.59014,145.184
+00012a70: 3738 2032 2e32 3932 3835 2c30 2e34 3339  78 2.29285,0.439
+00012a80: 3532 2063 202d 302e 3635 3034 342c 2d30  52 c -0.65044,-0
+00012a90: 2e33 3433 3835 202d 312e 3032 3731 2c2d  .34385 -1.0271,-
+00012aa0: 302e 3839 3633 202d 312e 3334 3833 382c  0.8963 -1.34838,
+00012ab0: 2d31 2e34 3930 3934 207a 220a 2020 2020  -1.49094 z".    
+00012ac0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00012ad0: 3531 2d30 2d33 2d39 2d39 2d34 2d39 2d30  51-0-3-9-9-4-9-0
+00012ae0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00012af0: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00012b00: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00012b10: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+00012b20: 6465 7479 7065 733d 2263 6363 6322 0a20  detypes="cccc". 
+00012b30: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00012b40: 3a65 7870 6f72 742d 7864 7069 3d22 3330  :export-xdpi="30
+00012b50: 3022 0a20 2020 2020 2020 2020 696e 6b73  0".         inks
+00012b60: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+00012b70: 3d22 3330 3022 202f 3e0a 2020 2020 2020  ="300" />.      
+00012b80: 3c70 6174 680a 2020 2020 2020 2020 2073  <path.         s
+00012b90: 7479 6c65 3d22 6669 6c6c 3a23 3237 3337  tyle="fill:#2737
+00012ba0: 3733 3b66 696c 6c2d 6f70 6163 6974 793a  73;fill-opacity:
+00012bb0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+00012bc0: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
+00012bd0: 7374 726f 6b65 2d6c 696e 6563 6170 3a62  stroke-linecap:b
+00012be0: 7574 743b 7374 726f 6b65 2d6c 696e 656a  utt;stroke-linej
+00012bf0: 6f69 6e3a 6d69 7465 723b 7374 726f 6b65  oin:miter;stroke
+00012c00: 2d6d 6974 6572 6c69 6d69 743a 343b 7374  -miterlimit:4;st
+00012c10: 726f 6b65 2d64 6173 6861 7272 6179 3a6e  roke-dasharray:n
+00012c20: 6f6e 653b 7374 726f 6b65 2d6f 7061 6369  one;stroke-opaci
+00012c30: 7479 3a31 220a 2020 2020 2020 2020 2064  ty:1".         d
+00012c40: 3d22 6d20 3135 342e 3135 3236 362c 3134  ="m 154.15266,14
+00012c50: 352e 3235 3030 3820 6320 302e 3331 3633  5.25008 c 0.3163
+00012c60: 322c 302e 3138 3134 3720 302e 3636 3530  2,0.18147 0.6650
+00012c70: 392c 302e 3333 3739 3720 302e 3738 3430  9,0.33797 0.7840
+00012c80: 382c 302e 3637 3132 3220 6c20 302e 3635  8,0.67122 l 0.65
+00012c90: 3334 2c2d 302e 3733 3635 3620 7a22 0a20  34,-0.73656 z". 
+00012ca0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00012cb0: 3134 3535 332d 332d 322d 322d 312d 332d  14553-3-2-2-1-3-
+00012cc0: 382d 3922 0a20 2020 2020 2020 2020 696e  8-9".         in
+00012cd0: 6b73 6361 7065 3a63 6f6e 6e65 6374 6f72  kscape:connector
+00012ce0: 2d63 7572 7661 7475 7265 3d22 3022 0a20  -curvature="0". 
+00012cf0: 2020 2020 2020 2020 736f 6469 706f 6469          sodipodi
+00012d00: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
+00012d10: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00012d20: 6170 653a 6578 706f 7274 2d78 6470 693d  ape:export-xdpi=
+00012d30: 2233 3030 220a 2020 2020 2020 2020 2069  "300".         i
+00012d40: 6e6b 7363 6170 653a 6578 706f 7274 2d79  nkscape:export-y
+00012d50: 6470 693d 2233 3030 2220 2f3e 0a20 2020  dpi="300" />.   
+00012d60: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00012d70: 2020 7374 796c 653d 2266 696c 6c3a 2331    style="fill:#1
+00012d80: 3432 3637 323b 6669 6c6c 2d6f 7061 6369  42672;fill-opaci
+00012d90: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+00012da0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00012db0: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
+00012dc0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00012dd0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00012de0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00012df0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00012e00: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00012e10: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00012e20: 2020 643d 226d 2031 3534 2e39 3336 3734    d="m 154.93674
+00012e30: 2c31 3435 2e39 3231 3320 322e 3934 3632  ,145.9213 2.9462
+00012e40: 352c 2d30 2e32 3937 202d 322e 3239 3238  5,-0.297 -2.2928
+00012e50: 352c 2d30 2e34 3339 3536 207a 220a 2020  5,-0.43956 z".  
+00012e60: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00012e70: 3435 3535 2d34 2d31 2d36 2d37 2d32 2d32  4555-4-1-6-7-2-2
+00012e80: 2d33 220a 2020 2020 2020 2020 2069 6e6b  -3".         ink
+00012e90: 7363 6170 653a 636f 6e6e 6563 746f 722d  scape:connector-
+00012ea0: 6375 7276 6174 7572 653d 2230 220a 2020  curvature="0".  
+00012eb0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00012ec0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+00012ed0: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00012ee0: 6170 653a 6578 706f 7274 2d79 6470 693d  ape:export-ydpi=
+00012ef0: 2233 3030 2220 2f3e 0a20 2020 2020 203c  "300" />.      <
+00012f00: 7061 7468 0a20 2020 2020 2020 2020 7374  path.         st
+00012f10: 796c 653d 2266 696c 6c3a 2335 3436 3638  yle="fill:#54668
+00012f20: 633b 6669 6c6c 2d6f 7061 6369 7479 3a31  c;fill-opacity:1
+00012f30: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00012f40: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
+00012f50: 7472 6f6b 652d 6c69 6e65 6361 703a 6275  troke-linecap:bu
+00012f60: 7474 3b73 7472 6f6b 652d 6c69 6e65 6a6f  tt;stroke-linejo
+00012f70: 696e 3a6d 6974 6572 3b73 7472 6f6b 652d  in:miter;stroke-
+00012f80: 6d69 7465 726c 696d 6974 3a34 3b73 7472  miterlimit:4;str
+00012f90: 6f6b 652d 6461 7368 6172 7261 793a 6e6f  oke-dasharray:no
+00012fa0: 6e65 3b73 7472 6f6b 652d 6f70 6163 6974  ne;stroke-opacit
+00012fb0: 793a 3122 0a20 2020 2020 2020 2020 643d  y:1".         d=
+00012fc0: 226d 2031 3534 2e39 3336 3734 2c31 3435  "m 154.93674,145
+00012fd0: 2e39 3231 3320 6320 302e 3033 3832 2c30  .9213 c 0.0382,0
+00012fe0: 2e33 3239 3338 202d 302e 3039 342c 302e  .32938 -0.094,0.
+00012ff0: 3533 3730 3320 2d30 2e31 3534 3434 2c30  53703 -0.15444,0
+00013000: 2e37 3935 3937 206c 2033 2e31 3030 3639  .79597 l 3.10069
+00013010: 2c2d 312e 3039 3239 3720 7a22 0a20 2020  ,-1.09297 z".   
+00013020: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+00013030: 3535 392d 332d 342d 322d 342d 342d 332d  559-3-4-2-4-4-3-
+00013040: 3522 0a20 2020 2020 2020 2020 696e 6b73  5".         inks
+00013050: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+00013060: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+00013070: 2020 2020 2020 736f 6469 706f 6469 3a6e        sodipodi:n
+00013080: 6f64 6574 7970 6573 3d22 6363 6363 220a  odetypes="cccc".
+00013090: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+000130a0: 653a 6578 706f 7274 2d78 6470 693d 2233  e:export-xdpi="3
+000130b0: 3030 220a 2020 2020 2020 2020 2069 6e6b  00".         ink
+000130c0: 7363 6170 653a 6578 706f 7274 2d79 6470  scape:export-ydp
+000130d0: 693d 2233 3030 2220 2f3e 0a20 2020 2020  i="300" />.     
+000130e0: 203c 7061 7468 0a20 2020 2020 2020 2020   <path.         
+000130f0: 7374 796c 653d 2266 696c 6c3a 2330 3831  style="fill:#081
+00013100: 3036 393b 6669 6c6c 2d6f 7061 6369 7479  069;fill-opacity
+00013110: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00013120: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+00013130: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00013140: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00013150: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00013160: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00013170: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00013180: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00013190: 6974 793a 3122 0a20 2020 2020 2020 2020  ity:1".         
+000131a0: 643d 226d 2031 3534 2e37 3832 332c 3134  d="m 154.7823,14
+000131b0: 362e 3731 3732 3720 312e 3238 3330 352c  6.71727 1.28305,
+000131c0: 302e 3139 3030 3820 312e 3831 3736 342c  0.19008 1.81764,
+000131d0: 2d31 2e32 3833 3035 207a 220a 2020 2020  -1.28305 z".    
+000131e0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+000131f0: 3631 2d39 2d32 2d32 2d38 2d30 2d31 2d37  61-9-2-2-8-0-1-7
+00013200: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00013210: 6170 653a 636f 6e6e 6563 746f 722d 6375  ape:connector-cu
+00013220: 7276 6174 7572 653d 2230 220a 2020 2020  rvature="0".    
+00013230: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+00013240: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+00013250: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00013260: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+00013270: 3030 2220 2f3e 0a20 2020 2020 203c 7061  00" />.      <pa
+00013280: 7468 0a20 2020 2020 2020 2020 7374 796c  th.         styl
+00013290: 653d 2266 696c 6c3a 2330 3730 6532 623b  e="fill:#070e2b;
+000132a0: 6669 6c6c 2d6f 7061 6369 7479 3a31 3b73  fill-opacity:1;s
+000132b0: 7472 6f6b 653a 2366 6666 6666 663b 7374  troke:#ffffff;st
+000132c0: 726f 6b65 2d77 6964 7468 3a30 3b73 7472  roke-width:0;str
+000132d0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+000132e0: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+000132f0: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+00013300: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00013310: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00013320: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00013330: 3122 0a20 2020 2020 2020 2020 643d 226d  1".         d="m
+00013340: 2031 3536 2e30 3635 3335 2c31 3436 2e39   156.06535,146.9
+00013350: 3037 3335 2030 2e37 3534 3338 2c30 2e39  0735 0.75438,0.9
+00013360: 3931 3938 202d 302e 3237 3931 382c 2d31  9198 -0.27918,-1
+00013370: 2e33 3336 3520 7a22 0a20 2020 2020 2020  .3365 z".       
+00013380: 2020 6964 3d22 7061 7468 3134 3536 332d    id="path14563-
+00013390: 312d 302d 362d 382d 372d 322d 3222 0a20  1-0-6-8-7-2-2". 
+000133a0: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+000133b0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+000133c0: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
+000133d0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+000133e0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+000133f0: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00013400: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+00013410: 202f 3e0a 2020 2020 2020 3c70 6174 680a   />.      <path.
+00013420: 2020 2020 2020 2020 2073 7479 6c65 3d22           style="
+00013430: 6669 6c6c 3a23 3037 3065 3262 3b66 696c  fill:#070e2b;fil
+00013440: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
+00013450: 6b65 3a23 6666 6666 6666 3b73 7472 6f6b  ke:#ffffff;strok
+00013460: 652d 7769 6474 683a 303b 7374 726f 6b65  e-width:0;stroke
+00013470: 2d6c 696e 6563 6170 3a62 7574 743b 7374  -linecap:butt;st
+00013480: 726f 6b65 2d6c 696e 656a 6f69 6e3a 6d69  roke-linejoin:mi
+00013490: 7465 723b 7374 726f 6b65 2d6d 6974 6572  ter;stroke-miter
+000134a0: 6c69 6d69 743a 343b 7374 726f 6b65 2d64  limit:4;stroke-d
+000134b0: 6173 6861 7272 6179 3a6e 6f6e 653b 7374  asharray:none;st
+000134c0: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+000134d0: 2020 2020 2020 2020 2064 3d22 6d20 3135           d="m 15
+000134e0: 362e 3036 3533 352c 3134 362e 3930 3733  6.06535,146.9073
+000134f0: 3520 302e 3735 3433 382c 302e 3939 3139  5 0.75438,0.9919
+00013500: 3820 6320 302e 3134 3435 322c 2d31 2e32  8 c 0.14452,-1.2
+00013510: 3031 3436 2030 2e36 3533 3132 2c2d 312e  0146 0.65312,-1.
+00013520: 3633 3433 2031 2e30 3633 3236 2c2d 322e  6343 1.06326,-2.
+00013530: 3237 3530 3320 7a22 0a20 2020 2020 2020  27503 z".       
+00013540: 2020 6964 3d22 7061 7468 3134 3536 352d    id="path14565-
+00013550: 392d 352d 392d 372d 372d 332d 3422 0a20  9-5-9-7-7-3-4". 
+00013560: 2020 2020 2020 2020 696e 6b73 6361 7065          inkscape
+00013570: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+00013580: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
+00013590: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
+000135a0: 7970 6573 3d22 6363 6363 220a 2020 2020  ypes="cccc".    
+000135b0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+000135c0: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+000135d0: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+000135e0: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+000135f0: 3030 2220 2f3e 0a20 2020 2020 203c 6369  00" />.      <ci
+00013600: 7263 6c65 0a20 2020 2020 2020 2020 7374  rcle.         st
+00013610: 796c 653d 2266 696c 6c3a 2330 3730 6532  yle="fill:#070e2
+00013620: 623b 6669 6c6c 2d6f 7061 6369 7479 3a30  b;fill-opacity:0
+00013630: 2e39 3930 3434 363b 7374 726f 6b65 3a23  .990446;stroke:#
+00013640: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00013650: 6474 683a 303b 7374 726f 6b65 2d6d 6974  dth:0;stroke-mit
+00013660: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00013670: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00013680: 7374 726f 6b65 2d64 6173 686f 6666 7365  stroke-dashoffse
+00013690: 743a 303b 7374 726f 6b65 2d6f 7061 6369  t:0;stroke-opaci
+000136a0: 7479 3a31 220a 2020 2020 2020 2020 2069  ty:1".         i
+000136b0: 643d 2270 6174 6831 3435 3637 2d36 2d31  d="path14567-6-1
+000136c0: 2d39 2d37 2d37 2d35 2d39 220a 2020 2020  -9-7-7-5-9".    
+000136d0: 2020 2020 2063 783d 2231 3534 2e31 3833       cx="154.183
+000136e0: 3138 220a 2020 2020 2020 2020 2063 793d  18".         cy=
+000136f0: 2231 3435 2e32 3531 3632 220a 2020 2020  "145.25162".    
+00013700: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+00013710: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+00013720: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00013730: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+00013740: 3030 220a 2020 2020 2020 2020 2072 3d22  00".         r="
+00013750: 302e 3037 3430 3637 3737 3922 202f 3e0a  0.074067779" />.
+00013760: 2020 2020 2020 3c63 6972 636c 650a 2020        <circle.  
+00013770: 2020 2020 2020 2072 3d22 302e 3037 3430         r="0.0740
+00013780: 3637 3737 3922 0a20 2020 2020 2020 2020  67779".         
+00013790: 7374 796c 653d 2266 696c 6c3a 2332 3533  style="fill:#253
+000137a0: 6137 643b 6669 6c6c 2d6f 7061 6369 7479  a7d;fill-opacity
+000137b0: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+000137c0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+000137d0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+000137e0: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+000137f0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00013800: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+00013810: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00013820: 0a20 2020 2020 2020 2020 6964 3d22 7061  .         id="pa
+00013830: 7468 3134 3536 372d 332d 3933 2d31 2d36  th14567-3-93-1-6
+00013840: 2d39 2d33 2d37 2d38 220a 2020 2020 2020  -9-3-7-8".      
+00013850: 2020 2063 783d 2231 3534 2e37 3730 3422     cx="154.7704"
+00013860: 0a20 2020 2020 2020 2020 6379 3d22 3134  .         cy="14
+00013870: 362e 3730 3134 3822 0a20 2020 2020 2020  6.70148".       
+00013880: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00013890: 666f 726d 2d63 656e 7465 722d 783d 2234  form-center-x="4
+000138a0: 2e36 3433 3235 3636 220a 2020 2020 2020  .6432566".      
+000138b0: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
+000138c0: 7366 6f72 6d2d 6365 6e74 6572 2d79 3d22  sform-center-y="
+000138d0: 2d39 2e39 3738 3036 3231 220a 2020 2020  -9.9780621".    
+000138e0: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+000138f0: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+00013900: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00013910: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+00013920: 3030 2220 2f3e 0a20 2020 2020 203c 6369  00" />.      <ci
+00013930: 7263 6c65 0a20 2020 2020 2020 2020 723d  rcle.         r=
+00013940: 2230 2e30 3734 3036 3737 3739 220a 2020  "0.074067779".  
+00013950: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00013960: 6c6c 3a23 6162 6161 3963 3b66 696c 6c2d  ll:#abaa9c;fill-
+00013970: 6f70 6163 6974 793a 313b 7374 726f 6b65  opacity:1;stroke
+00013980: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+00013990: 7769 6474 683a 303b 7374 726f 6b65 2d6d  width:0;stroke-m
+000139a0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+000139b0: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+000139c0: 653b 7374 726f 6b65 2d64 6173 686f 6666  e;stroke-dashoff
+000139d0: 7365 743a 303b 7374 726f 6b65 2d6f 7061  set:0;stroke-opa
+000139e0: 6369 7479 3a31 220a 2020 2020 2020 2020  city:1".        
+000139f0: 2069 643d 2270 6174 6831 3435 3637 2d33   id="path14567-3
+00013a00: 2d39 2d30 2d39 2d38 2d32 2d38 2d30 2d35  -9-0-9-8-2-8-0-5
+00013a10: 220a 2020 2020 2020 2020 2063 783d 2231  ".         cx="1
+00013a20: 3536 2e30 3833 3422 0a20 2020 2020 2020  56.0834".       
+00013a30: 2020 6379 3d22 3134 362e 3930 3334 3722    cy="146.90347"
+00013a40: 0a20 2020 2020 2020 2020 696e 6b73 6361  .         inksca
+00013a50: 7065 3a74 7261 6e73 666f 726d 2d63 656e  pe:transform-cen
+00013a60: 7465 722d 783d 2234 2e36 3433 3235 3636  ter-x="4.6432566
+00013a70: 220a 2020 2020 2020 2020 2069 6e6b 7363  ".         inksc
+00013a80: 6170 653a 7472 616e 7366 6f72 6d2d 6365  ape:transform-ce
+00013a90: 6e74 6572 2d79 3d22 2d39 2e39 3738 3036  nter-y="-9.97806
+00013aa0: 3231 220a 2020 2020 2020 2020 2069 6e6b  21".         ink
+00013ab0: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
+00013ac0: 693d 2233 3030 220a 2020 2020 2020 2020  i="300".        
+00013ad0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00013ae0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+00013af0: 2020 2020 203c 6369 7263 6c65 0a20 2020       <circle.   
+00013b00: 2020 2020 2020 723d 2230 2e31 3134 3331        r="0.11431
+00013b10: 3332 3422 0a20 2020 2020 2020 2020 7374  324".         st
+00013b20: 796c 653d 2266 696c 6c3a 2331 3132 3036  yle="fill:#11206
+00013b30: 363b 6669 6c6c 2d6f 7061 6369 7479 3a31  6;fill-opacity:1
+00013b40: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00013b50: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
+00013b60: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00013b70: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00013b80: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00013b90: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
+00013ba0: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00013bb0: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00013bc0: 3134 3536 372d 332d 322d 352d 342d 332d  14567-3-2-5-4-3-
+00013bd0: 382d 302d 372d 3722 0a20 2020 2020 2020  8-0-7-7".       
+00013be0: 2020 6378 3d22 3135 352e 3630 3033 3622    cx="155.60036"
+00013bf0: 0a20 2020 2020 2020 2020 6379 3d22 3134  .         cy="14
+00013c00: 352e 3136 3839 3122 0a20 2020 2020 2020  5.16891".       
+00013c10: 2020 696e 6b73 6361 7065 3a74 7261 6e73    inkscape:trans
+00013c20: 666f 726d 2d63 656e 7465 722d 783d 2237  form-center-x="7
+00013c30: 2e31 3636 3231 3136 220a 2020 2020 2020  .1662116".      
+00013c40: 2020 2069 6e6b 7363 6170 653a 7472 616e     inkscape:tran
+00013c50: 7366 6f72 6d2d 6365 6e74 6572 2d79 3d22  sform-center-y="
+00013c60: 2d31 352e 3339 3937 3531 220a 2020 2020  -15.399751".    
+00013c70: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+00013c80: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+00013c90: 2020 2020 2020 2020 2069 6e6b 7363 6170           inkscap
+00013ca0: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+00013cb0: 3030 2220 2f3e 0a20 2020 2020 203c 6369  00" />.      <ci
+00013cc0: 7263 6c65 0a20 2020 2020 2020 2020 723d  rcle.         r=
+00013cd0: 2230 2e30 3734 3036 3737 3739 220a 2020  "0.074067779".  
+00013ce0: 2020 2020 2020 2073 7479 6c65 3d22 6669         style="fi
+00013cf0: 6c6c 3a23 6564 6630 6663 3b66 696c 6c2d  ll:#edf0fc;fill-
+00013d00: 6f70 6163 6974 793a 302e 3939 3034 3436  opacity:0.990446
+00013d10: 3b73 7472 6f6b 653a 2366 6666 6666 663b  ;stroke:#ffffff;
+00013d20: 7374 726f 6b65 2d77 6964 7468 3a30 3b73  stroke-width:0;s
+00013d30: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+00013d40: 3a34 3b73 7472 6f6b 652d 6461 7368 6172  :4;stroke-dashar
+00013d50: 7261 793a 6e6f 6e65 3b73 7472 6f6b 652d  ray:none;stroke-
+00013d60: 6461 7368 6f66 6673 6574 3a30 3b73 7472  dashoffset:0;str
+00013d70: 6f6b 652d 6f70 6163 6974 793a 3122 0a20  oke-opacity:1". 
+00013d80: 2020 2020 2020 2020 6964 3d22 7061 7468          id="path
+00013d90: 3134 3536 372d 322d 382d 362d 372d 382d  14567-2-8-6-7-8-
+00013da0: 322d 322d 362d 3922 0a20 2020 2020 2020  2-2-6-9".       
+00013db0: 2020 6378 3d22 3135 342e 3933 3732 3722    cx="154.93727"
+00013dc0: 0a20 2020 2020 2020 2020 6379 3d22 3134  .         cy="14
+00013dd0: 352e 3931 3130 3422 0a20 2020 2020 2020  5.91104".       
+00013de0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00013df0: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+00013e00: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00013e10: 7870 6f72 742d 7964 7069 3d22 3330 3022  xport-ydpi="300"
+00013e20: 202f 3e0a 2020 2020 2020 3c63 6972 636c   />.      <circl
+00013e30: 650a 2020 2020 2020 2020 2072 3d22 302e  e.         r="0.
+00013e40: 3134 3037 3931 3935 220a 2020 2020 2020  14079195".      
+00013e50: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00013e60: 6564 6630 6663 3b66 696c 6c2d 6f70 6163  edf0fc;fill-opac
+00013e70: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
+00013e80: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00013e90: 6b65 2d77 6964 7468 3a30 3b73 7472 6f6b  ke-width:0;strok
+00013ea0: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00013eb0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00013ec0: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
+00013ed0: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
+00013ee0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00013ef0: 2020 2020 6964 3d22 7061 7468 3134 3536      id="path1456
+00013f00: 372d 322d 372d 302d 392d 302d 352d 312d  7-2-7-0-9-0-5-1-
+00013f10: 312d 3322 0a20 2020 2020 2020 2020 6378  1-3".         cx
+00013f20: 3d22 3135 372e 3835 3734 3822 0a20 2020  ="157.85748".   
+00013f30: 2020 2020 2020 6379 3d22 3134 352e 3634        cy="145.64
+00013f40: 3331 3722 0a20 2020 2020 2020 2020 696e  317".         in
+00013f50: 6b73 6361 7065 3a65 7870 6f72 742d 7864  kscape:export-xd
+00013f60: 7069 3d22 3330 3022 0a20 2020 2020 2020  pi="300".       
+00013f70: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00013f80: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+00013f90: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
+00013fa0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00013fb0: 3a6e 6f6e 653b 6669 6c6c 2d72 756c 653a  :none;fill-rule:
+00013fc0: 6576 656e 6f64 643b 7374 726f 6b65 3a23  evenodd;stroke:#
+00013fd0: 6666 6666 6666 3b73 7472 6f6b 652d 7769  ffffff;stroke-wi
+00013fe0: 6474 683a 302e 3133 3232 3932 3b73 7472  dth:0.132292;str
+00013ff0: 6f6b 652d 6c69 6e65 6361 703a 6275 7474  oke-linecap:butt
+00014000: 3b73 7472 6f6b 652d 6c69 6e65 6a6f 696e  ;stroke-linejoin
+00014010: 3a6d 6974 6572 3b73 7472 6f6b 652d 6d69  :miter;stroke-mi
+00014020: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+00014030: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+00014040: 3b73 7472 6f6b 652d 6f70 6163 6974 793a  ;stroke-opacity:
+00014050: 3122 0a20 2020 2020 2020 2020 643d 226d  1".         d="m
+00014060: 2031 3534 2e31 3532 3636 2c31 3435 2e32   154.15266,145.2
+00014070: 3530 3038 2063 2030 2e38 3839 3438 2c2d  5008 c 0.88948,-
+00014080: 302e 3138 3132 3320 312e 3634 3634 332c  0.18123 1.64643,
+00014090: 2d30 2e36 3237 3532 2032 2e33 3831 3935  -0.62752 2.38195
+000140a0: 2c2d 312e 3131 3636 3820 302e 3333 3234  ,-1.11668 0.3324
+000140b0: 362c 302e 3630 3432 3120 302e 3635 322c  6,0.60421 0.652,
+000140c0: 312e 3232 3032 3720 312e 3334 3833 382c  1.22027 1.34838,
+000140d0: 312e 3439 3039 202d 302e 3432 3232 352c  1.4909 -0.42225,
+000140e0: 302e 3537 3536 3520 2d30 2e38 3432 3537  0.57565 -0.84257
+000140f0: 2c31 2e31 3536 3531 202d 312e 3036 3332  ,1.15651 -1.0632
+00014100: 362c 322e 3237 3530 3320 6c20 2d30 2e37  6,2.27503 l -0.7
+00014110: 3534 3338 2c2d 302e 3939 3139 3820 2d31  5438,-0.99198 -1
+00014120: 2e32 3833 3035 2c2d 302e 3139 3030 3820  .28305,-0.19008 
+00014130: 6320 302e 3133 3739 362c 2d30 2e33 3038  c 0.13796,-0.308
+00014140: 3536 2030 2e32 3033 3335 2c2d 302e 3538  56 0.20335,-0.58
+00014150: 3038 3420 302e 3135 3434 342c 2d30 2e37  084 0.15444,-0.7
+00014160: 3935 3937 202d 302e 3230 3137 342c 2d30  9597 -0.20174,-0
+00014170: 2e32 3533 3535 202d 302e 3435 3736 362c  .25355 -0.45766,
+00014180: 2d30 2e34 3830 3031 202d 302e 3738 3430  -0.48001 -0.7840
+00014190: 382c 2d30 2e36 3731 3232 207a 220a 2020  8,-0.67122 z".  
+000141a0: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+000141b0: 3330 332d 3722 0a20 2020 2020 2020 2020  303-7".         
+000141c0: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
+000141d0: 6573 3d22 6363 6363 6363 6363 2220 2f3e  es="cccccccc" />
+000141e0: 0a20 2020 203c 2f67 3e0a 2020 2020 3c70  .    </g>.    <p
+000141f0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+00014200: 3d22 6669 6c6c 3a23 3365 3462 3737 3b66  ="fill:#3e4b77;f
+00014210: 696c 6c2d 6f70 6163 6974 793a 313b 7374  ill-opacity:1;st
+00014220: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00014230: 6f6b 652d 7769 6474 683a 303b 7374 726f  oke-width:0;stro
+00014240: 6b65 2d6c 696e 6563 6170 3a62 7574 743b  ke-linecap:butt;
+00014250: 7374 726f 6b65 2d6c 696e 656a 6f69 6e3a  stroke-linejoin:
+00014260: 6d69 7465 723b 7374 726f 6b65 2d6d 6974  miter;stroke-mit
+00014270: 6572 6c69 6d69 743a 343b 7374 726f 6b65  erlimit:4;stroke
+00014280: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
+00014290: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
+000142a0: 220a 2020 2020 2020 2064 3d22 6d20 3437  ".       d="m 47
+000142b0: 312e 3539 3435 312c 3333 312e 3337 3335  1.59451,331.3735
+000142c0: 3320 352e 3433 3239 392c 2d30 2e32 3436  3 5.43299,-0.246
+000142d0: 3820 332e 3536 3936 352c 2d33 2e39 3733  8 3.56965,-3.973
+000142e0: 3732 2063 202d 342e 3439 3639 392c 332e  72 c -4.49699,3.
+000142f0: 3032 3433 202d 362e 3634 3534 332c 332e  0243 -6.64543,3.
+00014300: 3530 3936 3720 2d39 2e30 3032 3634 2c34  50967 -9.00264,4
+00014310: 2e32 3230 3637 207a 220a 2020 2020 2020  .22067 z".      
+00014320: 2069 643d 2270 6174 6831 3435 3437 2d31   id="path14547-1
+00014330: 2d37 2d38 2d35 2d30 2d33 220a 2020 2020  -7-8-5-0-3".    
+00014340: 2020 2069 6e6b 7363 6170 653a 636f 6e6e     inkscape:conn
+00014350: 6563 746f 722d 6375 7276 6174 7572 653d  ector-curvature=
+00014360: 2230 220a 2020 2020 2020 2073 6f64 6970  "0".       sodip
+00014370: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+00014380: 6363 6322 0a20 2020 2020 2020 696e 6b73  ccc".       inks
+00014390: 6361 7065 3a65 7870 6f72 742d 7864 7069  cape:export-xdpi
+000143a0: 3d22 3330 3022 0a20 2020 2020 2020 696e  ="300".       in
+000143b0: 6b73 6361 7065 3a65 7870 6f72 742d 7964  kscape:export-yd
+000143c0: 7069 3d22 3330 3022 202f 3e0a 2020 2020  pi="300" />.    
+000143d0: 3c70 6174 680a 2020 2020 2020 2073 7479  <path.       sty
+000143e0: 6c65 3d22 6669 6c6c 3a23 3036 3035 3038  le="fill:#060508
+000143f0: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00014400: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00014410: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
+00014420: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
+00014430: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
+00014440: 6e3a 6d69 7465 723b 7374 726f 6b65 2d6d  n:miter;stroke-m
+00014450: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
+00014460: 6b65 2d64 6173 6861 7272 6179 3a6e 6f6e  ke-dasharray:non
+00014470: 653b 7374 726f 6b65 2d6f 7061 6369 7479  e;stroke-opacity
+00014480: 3a31 220a 2020 2020 2020 2064 3d22 6d20  :1".       d="m 
+00014490: 3437 372e 3032 3735 2c33 3331 2e31 3236  477.0275,331.126
+000144a0: 3733 2038 2e36 3635 3839 2c31 2e36 3631  73 8.66589,1.661
+000144b0: 3138 2063 202d 322e 3435 3833 352c 2d31  18 c -2.45835,-1
+000144c0: 2e32 3939 3539 202d 332e 3838 3139 352c  .29959 -3.88195,
+000144d0: 2d33 2e33 3837 3539 202d 352e 3039 3632  -3.38759 -5.0962
+000144e0: 342c 2d35 2e36 3335 3035 207a 220a 2020  4,-5.63505 z".  
+000144f0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00014500: 3531 2d30 2d33 2d39 2d39 2d34 2d39 220a  51-0-3-9-9-4-9".
+00014510: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00014520: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00014530: 7572 653d 2230 220a 2020 2020 2020 2073  ure="0".       s
+00014540: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00014550: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
+00014560: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00014570: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+00014580: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00014590: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+000145a0: 2020 2020 3c70 6174 680a 2020 2020 2020      <path.      
+000145b0: 2073 7479 6c65 3d22 6669 6c6c 3a23 3237   style="fill:#27
+000145c0: 3337 3733 3b66 696c 6c2d 6f70 6163 6974  3773;fill-opacit
+000145d0: 793a 313b 7374 726f 6b65 3a23 6666 6666  y:1;stroke:#ffff
+000145e0: 6666 3b73 7472 6f6b 652d 7769 6474 683a  ff;stroke-width:
+000145f0: 303b 7374 726f 6b65 2d6c 696e 6563 6170  0;stroke-linecap
+00014600: 3a62 7574 743b 7374 726f 6b65 2d6c 696e  :butt;stroke-lin
+00014610: 656a 6f69 6e3a 6d69 7465 723b 7374 726f  ejoin:miter;stro
+00014620: 6b65 2d6d 6974 6572 6c69 6d69 743a 343b  ke-miterlimit:4;
+00014630: 7374 726f 6b65 2d64 6173 6861 7272 6179  stroke-dasharray
+00014640: 3a6e 6f6e 653b 7374 726f 6b65 2d6f 7061  :none;stroke-opa
+00014650: 6369 7479 3a31 220a 2020 2020 2020 2064  city:1".       d
+00014660: 3d22 6d20 3437 312e 3539 3435 312c 3333  ="m 471.59451,33
+00014670: 312e 3337 3335 3320 6320 312e 3139 3535  1.37353 c 1.1955
+00014680: 342c 302e 3638 3538 3720 322e 3531 3337  4,0.68587 2.5137
+00014690: 322c 312e 3237 3733 3720 322e 3936 3334  2,1.27737 2.9634
+000146a0: 352c 322e 3533 3639 206c 2032 2e34 3639  5,2.5369 l 2.469
+000146b0: 3534 2c2d 322e 3738 3338 3520 7a22 0a20  54,-2.78385 z". 
+000146c0: 2020 2020 2020 6964 3d22 7061 7468 3134        id="path14
+000146d0: 3535 332d 332d 322d 322d 312d 332d 3822  553-3-2-2-1-3-8"
+000146e0: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+000146f0: 3a63 6f6e 6e65 6374 6f72 2d63 7572 7661  :connector-curva
+00014700: 7475 7265 3d22 3022 0a20 2020 2020 2020  ture="0".       
+00014710: 736f 6469 706f 6469 3a6e 6f64 6574 7970  sodipodi:nodetyp
+00014720: 6573 3d22 6363 6363 220a 2020 2020 2020  es="cccc".      
+00014730: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00014740: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+00014750: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+00014760: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+00014770: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00014780: 2020 7374 796c 653d 2266 696c 6c3a 2331    style="fill:#1
+00014790: 3432 3637 323b 6669 6c6c 2d6f 7061 6369  42672;fill-opaci
+000147a0: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+000147b0: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+000147c0: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
+000147d0: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+000147e0: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+000147f0: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00014800: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00014810: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00014820: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+00014830: 643d 226d 2034 3734 2e35 3537 3936 2c33  d="m 474.55796,3
+00014840: 3333 2e39 3130 3433 2031 312e 3133 3534  33.91043 11.1354
+00014850: 332c 2d31 2e31 3232 3532 202d 382e 3636  3,-1.12252 -8.66
+00014860: 3538 392c 2d31 2e36 3631 3333 207a 220a  589,-1.66133 z".
+00014870: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00014880: 3435 3535 2d34 2d31 2d36 2d37 2d32 2d32  4555-4-1-6-7-2-2
+00014890: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+000148a0: 653a 636f 6e6e 6563 746f 722d 6375 7276  e:connector-curv
+000148b0: 6174 7572 653d 2230 220a 2020 2020 2020  ature="0".      
+000148c0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+000148d0: 2d78 6470 693d 2233 3030 220a 2020 2020  -xdpi="300".    
+000148e0: 2020 2069 6e6b 7363 6170 653a 6578 706f     inkscape:expo
+000148f0: 7274 2d79 6470 693d 2233 3030 2220 2f3e  rt-ydpi="300" />
+00014900: 0a20 2020 203c 7061 7468 0a20 2020 2020  .    <path.     
+00014910: 2020 7374 796c 653d 2266 696c 6c3a 2335    style="fill:#5
+00014920: 3436 3638 633b 6669 6c6c 2d6f 7061 6369  4668c;fill-opaci
+00014930: 7479 3a31 3b73 7472 6f6b 653a 2366 6666  ty:1;stroke:#fff
+00014940: 6666 663b 7374 726f 6b65 2d77 6964 7468  fff;stroke-width
+00014950: 3a30 3b73 7472 6f6b 652d 6c69 6e65 6361  :0;stroke-lineca
+00014960: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00014970: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00014980: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00014990: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+000149a0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+000149b0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+000149c0: 643d 226d 2034 3734 2e35 3537 3936 2c33  d="m 474.55796,3
+000149d0: 3333 2e39 3130 3433 2063 2030 2e31 3434  33.91043 c 0.144
+000149e0: 3338 2c31 2e32 3434 3920 2d30 2e33 3535  38,1.2449 -0.355
+000149f0: 3238 2c32 2e30 3239 3732 202d 302e 3538  28,2.02972 -0.58
+00014a00: 3337 312c 332e 3030 3833 3920 6c20 3131  371,3.00839 l 11
+00014a10: 2e37 3139 3134 2c2d 342e 3133 3039 3120  .71914,-4.13091 
+00014a20: 7a22 0a20 2020 2020 2020 6964 3d22 7061  z".       id="pa
+00014a30: 7468 3134 3535 392d 332d 342d 322d 342d  th14559-3-4-2-4-
+00014a40: 342d 3322 0a20 2020 2020 2020 696e 6b73  4-3".       inks
+00014a50: 6361 7065 3a63 6f6e 6e65 6374 6f72 2d63  cape:connector-c
+00014a60: 7572 7661 7475 7265 3d22 3022 0a20 2020  urvature="0".   
+00014a70: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
+00014a80: 6574 7970 6573 3d22 6363 6363 220a 2020  etypes="cccc".  
+00014a90: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+00014aa0: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+00014ab0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00014ac0: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+00014ad0: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
+00014ae0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+00014af0: 6c3a 2330 3831 3036 393b 6669 6c6c 2d6f  l:#081069;fill-o
+00014b00: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
+00014b10: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+00014b20: 6964 7468 3a30 3b73 7472 6f6b 652d 6c69  idth:0;stroke-li
+00014b30: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
+00014b40: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
+00014b50: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00014b60: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00014b70: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00014b80: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
+00014b90: 2020 2020 643d 226d 2034 3733 2e39 3734      d="m 473.974
+00014ba0: 3235 2c33 3336 2e39 3138 3832 2034 2e38  25,336.91882 4.8
+00014bb0: 3439 3332 2c30 2e37 3138 3431 2036 2e38  4932,0.71841 6.8
+00014bc0: 3639 3832 2c2d 342e 3834 3933 3220 7a22  6982,-4.84932 z"
+00014bd0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00014be0: 3134 3536 312d 392d 322d 322d 382d 302d  14561-9-2-2-8-0-
+00014bf0: 3122 0a20 2020 2020 2020 696e 6b73 6361  1".       inksca
+00014c00: 7065 3a63 6f6e 6e65 6374 6f72 2d63 7572  pe:connector-cur
+00014c10: 7661 7475 7265 3d22 3022 0a20 2020 2020  vature="0".     
+00014c20: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00014c30: 742d 7864 7069 3d22 3330 3022 0a20 2020  t-xdpi="300".   
+00014c40: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00014c50: 6f72 742d 7964 7069 3d22 3330 3022 202f  ort-ydpi="300" /
+00014c60: 3e0a 2020 2020 3c70 6174 680a 2020 2020  >.    <path.    
+00014c70: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00014c80: 3037 3065 3262 3b66 696c 6c2d 6f70 6163  070e2b;fill-opac
+00014c90: 6974 793a 313b 7374 726f 6b65 3a23 6666  ity:1;stroke:#ff
+00014ca0: 6666 6666 3b73 7472 6f6b 652d 7769 6474  ffff;stroke-widt
+00014cb0: 683a 303b 7374 726f 6b65 2d6c 696e 6563  h:0;stroke-linec
+00014cc0: 6170 3a62 7574 743b 7374 726f 6b65 2d6c  ap:butt;stroke-l
+00014cd0: 696e 656a 6f69 6e3a 6d69 7465 723b 7374  inejoin:miter;st
+00014ce0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00014cf0: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00014d00: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d6f  ay:none;stroke-o
+00014d10: 7061 6369 7479 3a31 220a 2020 2020 2020  pacity:1".      
+00014d20: 2064 3d22 6d20 3437 382e 3832 3335 372c   d="m 478.82357,
+00014d30: 3333 372e 3633 3732 3320 322e 3835 3132  337.63723 2.8512
+00014d40: 2c33 2e37 3439 3232 202d 312e 3035 3531  ,3.74922 -1.0551
+00014d50: 372c 2d35 2e30 3531 3334 207a 220a 2020  7,-5.05134 z".  
+00014d60: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00014d70: 3633 2d31 2d30 2d36 2d38 2d37 2d32 220a  63-1-0-6-8-7-2".
+00014d80: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00014d90: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00014da0: 7572 653d 2230 220a 2020 2020 2020 2069  ure="0".       i
+00014db0: 6e6b 7363 6170 653a 6578 706f 7274 2d78  nkscape:export-x
+00014dc0: 6470 693d 2233 3030 220a 2020 2020 2020  dpi="300".      
+00014dd0: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
+00014de0: 2d79 6470 693d 2233 3030 2220 2f3e 0a20  -ydpi="300" />. 
+00014df0: 2020 203c 7061 7468 0a20 2020 2020 2020     <path.       
+00014e00: 7374 796c 653d 2266 696c 6c3a 2330 3730  style="fill:#070
+00014e10: 6532 623b 6669 6c6c 2d6f 7061 6369 7479  e2b;fill-opacity
+00014e20: 3a31 3b73 7472 6f6b 653a 2366 6666 6666  :1;stroke:#fffff
+00014e30: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+00014e40: 3b73 7472 6f6b 652d 6c69 6e65 6361 703a  ;stroke-linecap:
+00014e50: 6275 7474 3b73 7472 6f6b 652d 6c69 6e65  butt;stroke-line
+00014e60: 6a6f 696e 3a6d 6974 6572 3b73 7472 6f6b  join:miter;strok
+00014e70: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00014e80: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00014e90: 6e6f 6e65 3b73 7472 6f6b 652d 6f70 6163  none;stroke-opac
+00014ea0: 6974 793a 3122 0a20 2020 2020 2020 643d  ity:1".       d=
+00014eb0: 226d 2034 3738 2e38 3233 3537 2c33 3337  "m 478.82357,337
+00014ec0: 2e36 3337 3233 2032 2e38 3531 322c 332e  .63723 2.8512,3.
+00014ed0: 3734 3932 3220 6320 302e 3534 3632 322c  74922 c 0.54622,
+00014ee0: 2d34 2e35 3430 3936 2032 2e34 3638 3439  -4.54096 2.46849
+00014ef0: 2c2d 362e 3137 3638 3920 342e 3031 3836  ,-6.17689 4.0186
+00014f00: 322c 2d38 2e35 3938 3534 207a 220a 2020  2,-8.59854 z".  
+00014f10: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00014f20: 3635 2d39 2d35 2d39 2d37 2d37 2d33 220a  65-9-5-9-7-7-3".
+00014f30: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+00014f40: 636f 6e6e 6563 746f 722d 6375 7276 6174  connector-curvat
+00014f50: 7572 653d 2230 220a 2020 2020 2020 2073  ure="0".       s
+00014f60: 6f64 6970 6f64 693a 6e6f 6465 7479 7065  odipodi:nodetype
+00014f70: 733d 2263 6363 6322 0a20 2020 2020 2020  s="cccc".       
+00014f80: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00014f90: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+00014fa0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00014fb0: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+00014fc0: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
+00014fd0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+00014fe0: 3037 3065 3262 3b66 696c 6c2d 6f70 6163  070e2b;fill-opac
+00014ff0: 6974 793a 302e 3939 3034 3436 3b73 7472  ity:0.990446;str
+00015000: 6f6b 653a 2366 6666 6666 663b 7374 726f  oke:#ffffff;stro
+00015010: 6b65 2d77 6964 7468 3a30 3b73 7472 6f6b  ke-width:0;strok
+00015020: 652d 6d69 7465 726c 696d 6974 3a34 3b73  e-miterlimit:4;s
+00015030: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+00015040: 6e6f 6e65 3b73 7472 6f6b 652d 6461 7368  none;stroke-dash
+00015050: 6f66 6673 6574 3a30 3b73 7472 6f6b 652d  offset:0;stroke-
+00015060: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00015070: 2020 6964 3d22 7061 7468 3134 3536 372d    id="path14567-
+00015080: 362d 312d 392d 372d 372d 3522 0a20 2020  6-1-9-7-7-5".   
+00015090: 2020 2020 6378 3d22 3437 312e 3730 3938      cx="471.7098
+000150a0: 3422 0a20 2020 2020 2020 6379 3d22 3333  4".       cy="33
+000150b0: 312e 3337 3933 3322 0a20 2020 2020 2020  1.37933".       
+000150c0: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+000150d0: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+000150e0: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+000150f0: 742d 7964 7069 3d22 3330 3022 0a20 2020  t-ydpi="300".   
+00015100: 2020 2020 723d 2230 2e32 3739 3934 3132      r="0.2799412
+00015110: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
+00015120: 0a20 2020 2020 2020 723d 2230 2e32 3739  .       r="0.279
+00015130: 3934 3132 220a 2020 2020 2020 2073 7479  9412".       sty
+00015140: 6c65 3d22 6669 6c6c 3a23 3235 3361 3764  le="fill:#253a7d
+00015150: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00015160: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00015170: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
+00015180: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00015190: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+000151a0: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+000151b0: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+000151c0: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+000151d0: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+000151e0: 3637 2d33 2d39 332d 312d 362d 392d 332d  67-3-93-1-6-9-3-
+000151f0: 3722 0a20 2020 2020 2020 6378 3d22 3437  7".       cx="47
+00015200: 332e 3932 3932 3622 0a20 2020 2020 2020  3.92926".       
+00015210: 6379 3d22 3333 362e 3835 3931 3322 0a20  cy="336.85913". 
+00015220: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+00015230: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+00015240: 783d 2234 2e36 3433 3235 3636 220a 2020  x="4.6432566".  
+00015250: 2020 2020 2069 6e6b 7363 6170 653a 7472       inkscape:tr
+00015260: 616e 7366 6f72 6d2d 6365 6e74 6572 2d79  ansform-center-y
+00015270: 3d22 2d39 2e39 3738 3036 3231 220a 2020  ="-9.9780621".  
+00015280: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
+00015290: 706f 7274 2d78 6470 693d 2233 3030 220a  port-xdpi="300".
+000152a0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000152b0: 6578 706f 7274 2d79 6470 693d 2233 3030  export-ydpi="300
+000152c0: 2220 2f3e 0a20 2020 203c 6369 7263 6c65  " />.    <circle
+000152d0: 0a20 2020 2020 2020 723d 2230 2e32 3739  .       r="0.279
+000152e0: 3934 3132 220a 2020 2020 2020 2073 7479  9412".       sty
+000152f0: 6c65 3d22 6669 6c6c 3a23 6162 6161 3963  le="fill:#abaa9c
+00015300: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00015310: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+00015320: 7472 6f6b 652d 7769 6474 683a 303b 7374  troke-width:0;st
+00015330: 726f 6b65 2d6d 6974 6572 6c69 6d69 743a  roke-miterlimit:
+00015340: 343b 7374 726f 6b65 2d64 6173 6861 7272  4;stroke-dasharr
+00015350: 6179 3a6e 6f6e 653b 7374 726f 6b65 2d64  ay:none;stroke-d
+00015360: 6173 686f 6666 7365 743a 303b 7374 726f  ashoffset:0;stro
+00015370: 6b65 2d6f 7061 6369 7479 3a31 220a 2020  ke-opacity:1".  
+00015380: 2020 2020 2069 643d 2270 6174 6831 3435       id="path145
+00015390: 3637 2d33 2d39 2d30 2d39 2d38 2d32 2d38  67-3-9-0-9-8-2-8
+000153a0: 2d30 220a 2020 2020 2020 2063 783d 2234  -0".       cx="4
+000153b0: 3738 2e38 3931 3738 220a 2020 2020 2020  78.89178".      
+000153c0: 2063 793d 2233 3337 2e36 3232 3539 220a   cy="337.62259".
+000153d0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000153e0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+000153f0: 2d78 3d22 342e 3634 3332 3536 3622 0a20  -x="4.6432566". 
+00015400: 2020 2020 2020 696e 6b73 6361 7065 3a74        inkscape:t
+00015410: 7261 6e73 666f 726d 2d63 656e 7465 722d  ransform-center-
+00015420: 793d 222d 392e 3937 3830 3632 3122 0a20  y="-9.9780621". 
+00015430: 2020 2020 2020 696e 6b73 6361 7065 3a65        inkscape:e
+00015440: 7870 6f72 742d 7864 7069 3d22 3330 3022  xport-xdpi="300"
+00015450: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00015460: 3a65 7870 6f72 742d 7964 7069 3d22 3330  :export-ydpi="30
+00015470: 3022 202f 3e0a 2020 2020 3c63 6972 636c  0" />.    <circl
+00015480: 650a 2020 2020 2020 2072 3d22 302e 3433  e.       r="0.43
+00015490: 3230 3530 3035 220a 2020 2020 2020 2073  205005".       s
+000154a0: 7479 6c65 3d22 6669 6c6c 3a23 3131 3230  tyle="fill:#1120
+000154b0: 3636 3b66 696c 6c2d 6f70 6163 6974 793a  66;fill-opacity:
+000154c0: 313b 7374 726f 6b65 3a23 6666 6666 6666  1;stroke:#ffffff
+000154d0: 3b73 7472 6f6b 652d 7769 6474 683a 303b  ;stroke-width:0;
+000154e0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+000154f0: 743a 343b 7374 726f 6b65 2d64 6173 6861  t:4;stroke-dasha
+00015500: 7272 6179 3a6e 6f6e 653b 7374 726f 6b65  rray:none;stroke
+00015510: 2d64 6173 686f 6666 7365 743a 303b 7374  -dashoffset:0;st
+00015520: 726f 6b65 2d6f 7061 6369 7479 3a31 220a  roke-opacity:1".
+00015530: 2020 2020 2020 2069 643d 2270 6174 6831         id="path1
+00015540: 3435 3637 2d33 2d32 2d35 2d34 2d33 2d38  4567-3-2-5-4-3-8
+00015550: 2d30 2d37 220a 2020 2020 2020 2063 783d  -0-7".       cx=
+00015560: 2234 3737 2e30 3636 3122 0a20 2020 2020  "477.0661".     
+00015570: 2020 6379 3d22 3333 312e 3036 3637 3722    cy="331.06677"
+00015580: 0a20 2020 2020 2020 696e 6b73 6361 7065  .       inkscape
+00015590: 3a74 7261 6e73 666f 726d 2d63 656e 7465  :transform-cente
+000155a0: 722d 783d 2237 2e31 3636 3231 3136 220a  r-x="7.1662116".
+000155b0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000155c0: 7472 616e 7366 6f72 6d2d 6365 6e74 6572  transform-center
+000155d0: 2d79 3d22 2d31 352e 3339 3937 3531 220a  -y="-15.399751".
+000155e0: 2020 2020 2020 2069 6e6b 7363 6170 653a         inkscape:
+000155f0: 6578 706f 7274 2d78 6470 693d 2233 3030  export-xdpi="300
+00015600: 220a 2020 2020 2020 2069 6e6b 7363 6170  ".       inkscap
+00015610: 653a 6578 706f 7274 2d79 6470 693d 2233  e:export-ydpi="3
+00015620: 3030 2220 2f3e 0a20 2020 203c 6369 7263  00" />.    <circ
+00015630: 6c65 0a20 2020 2020 2020 723d 2230 2e32  le.       r="0.2
+00015640: 3739 3934 3132 220a 2020 2020 2020 2073  799412".       s
+00015650: 7479 6c65 3d22 6669 6c6c 3a23 6564 6630  tyle="fill:#edf0
+00015660: 6663 3b66 696c 6c2d 6f70 6163 6974 793a  fc;fill-opacity:
+00015670: 302e 3939 3034 3436 3b73 7472 6f6b 653a  0.990446;stroke:
+00015680: 2366 6666 6666 663b 7374 726f 6b65 2d77  #ffffff;stroke-w
+00015690: 6964 7468 3a30 3b73 7472 6f6b 652d 6d69  idth:0;stroke-mi
+000156a0: 7465 726c 696d 6974 3a34 3b73 7472 6f6b  terlimit:4;strok
+000156b0: 652d 6461 7368 6172 7261 793a 6e6f 6e65  e-dasharray:none
+000156c0: 3b73 7472 6f6b 652d 6461 7368 6f66 6673  ;stroke-dashoffs
+000156d0: 6574 3a30 3b73 7472 6f6b 652d 6f70 6163  et:0;stroke-opac
+000156e0: 6974 793a 3122 0a20 2020 2020 2020 6964  ity:1".       id
+000156f0: 3d22 7061 7468 3134 3536 372d 322d 382d  ="path14567-2-8-
+00015700: 362d 372d 382d 322d 322d 3622 0a20 2020  6-7-8-2-2-6".   
+00015710: 2020 2020 6378 3d22 3437 342e 3535 3939      cx="474.5599
+00015720: 3722 0a20 2020 2020 2020 6379 3d22 3333  7".       cy="33
+00015730: 332e 3837 3136 3722 0a20 2020 2020 2020  3.87167".       
+00015740: 696e 6b73 6361 7065 3a65 7870 6f72 742d  inkscape:export-
+00015750: 7864 7069 3d22 3330 3022 0a20 2020 2020  xdpi="300".     
+00015760: 2020 696e 6b73 6361 7065 3a65 7870 6f72    inkscape:expor
+00015770: 742d 7964 7069 3d22 3330 3022 202f 3e0a  t-ydpi="300" />.
+00015780: 2020 2020 3c63 6972 636c 650a 2020 2020      <circle.    
+00015790: 2020 2072 3d22 302e 3533 3231 3237 3038     r="0.53212708
+000157a0: 220a 2020 2020 2020 2073 7479 6c65 3d22  ".       style="
+000157b0: 6669 6c6c 3a23 6564 6630 6663 3b66 696c  fill:#edf0fc;fil
+000157c0: 6c2d 6f70 6163 6974 793a 302e 3939 3034  l-opacity:0.9904
+000157d0: 3436 3b73 7472 6f6b 653a 2366 6666 6666  46;stroke:#fffff
+000157e0: 663b 7374 726f 6b65 2d77 6964 7468 3a30  f;stroke-width:0
+000157f0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
+00015800: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
+00015810: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
+00015820: 652d 6461 7368 6f66 6673 6574 3a30 3b73  e-dashoffset:0;s
+00015830: 7472 6f6b 652d 6f70 6163 6974 793a 3122  troke-opacity:1"
+00015840: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
+00015850: 3134 3536 372d 322d 372d 302d 392d 302d  14567-2-7-0-9-0-
+00015860: 352d 312d 3122 0a20 2020 2020 2020 6378  5-1-1".       cx
+00015870: 3d22 3438 352e 3539 3639 3822 0a20 2020  ="485.59698".   
+00015880: 2020 2020 6379 3d22 3333 322e 3835 3932      cy="332.8592
+00015890: 3522 0a20 2020 2020 2020 696e 6b73 6361  5".       inksca
+000158a0: 7065 3a65 7870 6f72 742d 7864 7069 3d22  pe:export-xdpi="
+000158b0: 3330 3022 0a20 2020 2020 2020 696e 6b73  300".       inks
+000158c0: 6361 7065 3a65 7870 6f72 742d 7964 7069  cape:export-ydpi
+000158d0: 3d22 3330 3022 202f 3e0a 2020 2020 3c70  ="300" />.    <p
+000158e0: 6174 680a 2020 2020 2020 2073 7479 6c65  ath.       style
+000158f0: 3d22 6669 6c6c 3a6e 6f6e 653b 6669 6c6c  ="fill:none;fill
+00015900: 2d72 756c 653a 6576 656e 6f64 643b 7374  -rule:evenodd;st
+00015910: 726f 6b65 3a23 6666 6666 6666 3b73 7472  roke:#ffffff;str
+00015920: 6f6b 652d 7769 6474 683a 302e 3530 3030  oke-width:0.5000
+00015930: 3031 3b73 7472 6f6b 652d 6c69 6e65 6361  01;stroke-lineca
+00015940: 703a 6275 7474 3b73 7472 6f6b 652d 6c69  p:butt;stroke-li
+00015950: 6e65 6a6f 696e 3a6d 6974 6572 3b73 7472  nejoin:miter;str
+00015960: 6f6b 652d 6d69 7465 726c 696d 6974 3a34  oke-miterlimit:4
+00015970: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
+00015980: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
+00015990: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
+000159a0: 643d 226d 2034 3731 2e35 3934 3531 2c33  d="m 471.59451,3
+000159b0: 3331 2e33 3733 3533 2063 2033 2e33 3631  31.37353 c 3.361
+000159c0: 3831 2c2d 302e 3638 3439 3620 362e 3232  81,-0.68496 6.22
+000159d0: 3237 322c 2d32 2e33 3731 3733 2039 2e30  272,-2.37173 9.0
+000159e0: 3032 3634 2c2d 342e 3232 3035 3220 312e  0264,-4.22052 1.
+000159f0: 3235 3635 342c 322e 3238 3336 3320 322e  25654,2.28363 2.
+00015a00: 3436 3432 362c 342e 3631 3230 3420 352e  46426,4.61204 5.
+00015a10: 3039 3632 342c 352e 3633 3439 202d 312e  09624,5.6349 -1.
+00015a20: 3539 3539 2c32 2e31 3735 3638 202d 332e  5959,2.17568 -3.
+00015a30: 3138 3435 312c 342e 3337 3130 3620 2d34  18451,4.37106 -4
+00015a40: 2e30 3138 3632 2c38 2e35 3938 3534 206c  .01862,8.59854 l
+00015a50: 202d 322e 3835 3132 2c2d 332e 3734 3932   -2.8512,-3.7492
+00015a60: 3220 2d34 2e38 3439 3332 2c2d 302e 3731  2 -4.84932,-0.71
+00015a70: 3834 3120 6320 302e 3532 3134 322c 2d31  841 c 0.52142,-1
+00015a80: 2e31 3636 3231 2030 2e37 3638 3537 2c2d  .16621 0.76857,-
+00015a90: 322e 3139 3533 2030 2e35 3833 3731 2c2d  2.1953 0.58371,-
+00015aa0: 332e 3030 3833 3920 2d30 2e37 3632 3438  3.00839 -0.76248
+00015ab0: 2c2d 302e 3935 3833 202d 312e 3732 3937  ,-0.9583 -1.7297
+00015ac0: 342c 2d31 2e38 3134 3231 202d 322e 3936  4,-1.81421 -2.96
+00015ad0: 3334 352c 2d32 2e35 3336 3920 7a22 0a20  345,-2.5369 z". 
+00015ae0: 2020 2020 2020 6964 3d22 7061 7468 3133        id="path13
+00015af0: 3033 220a 2020 2020 2020 2073 6f64 6970  03".       sodip
+00015b00: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+00015b10: 6363 6363 6363 6322 202f 3e0a 2020 3c2f  ccccccc" />.  </
+00015b20: 673e 0a3c 2f73 7667 3e0a                 g>.</svg>.
```

### Comparing `saenopy-1.0.1/saenopy/img/Logo_black.png` & `saenopy-1.0.2/saenopy/img/Logo_black.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/arrowscale.ico` & `saenopy-1.0.2/saenopy/img/arrowscale.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/autoscale0.ico` & `saenopy-1.0.2/saenopy/img/autoscale0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/autoscale1.ico` & `saenopy-1.0.2/saenopy/img/autoscale1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/buttons.svg` & `saenopy-1.0.2/saenopy/img/buttons.svg`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/center0.ico` & `saenopy-1.0.2/saenopy/img/center0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/center1.ico` & `saenopy-1.0.2/saenopy/img/center1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/contrast0.ico` & `saenopy-1.0.2/saenopy/img/contrast0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/contrast1.ico` & `saenopy-1.0.2/saenopy/img/contrast1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/grid.ico` & `saenopy-1.0.2/saenopy/img/grid.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/grid2.ico` & `saenopy-1.0.2/saenopy/img/grid2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/grid3.ico` & `saenopy-1.0.2/saenopy/img/grid3.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/logo_splash.png` & `saenopy-1.0.2/saenopy/img/logo_splash.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/nan0.ico` & `saenopy-1.0.2/saenopy/img/nan0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/nan1.ico` & `saenopy-1.0.2/saenopy/img/nan1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/show_image.ico` & `saenopy-1.0.2/saenopy/img/show_image.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/show_image2.ico` & `saenopy-1.0.2/saenopy/img/show_image2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/show_image3.ico` & `saenopy-1.0.2/saenopy/img/show_image3.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/slice0.ico` & `saenopy-1.0.2/saenopy/img/slice0.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/slice1.ico` & `saenopy-1.0.2/saenopy/img/slice1.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/slice2.ico` & `saenopy-1.0.2/saenopy/img/slice2.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/slice_all.ico` & `saenopy-1.0.2/saenopy/img/slice_all.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/thumbnails/BFTFM.png` & `saenopy-1.0.2/saenopy/img/thumbnails/BFTFM.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/thumbnails/BFTFM_2.png` & `saenopy-1.0.2/saenopy/img/thumbnails/BFTFM_2.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/thumbnails/Bead_example_icon.png` & `saenopy-1.0.2/saenopy/img/thumbnails/Bead_example_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/thumbnails/Dynamic_icon.png` & `saenopy-1.0.2/saenopy/img/thumbnails/Dynamic_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/thumbnails/StainedOrganoid_icon.png` & `saenopy-1.0.2/saenopy/img/thumbnails/StainedOrganoid_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/thumbnails/liver_fibroblast_icon.png` & `saenopy-1.0.2/saenopy/img/thumbnails/liver_fibroblast_icon.png`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/view_single.ico` & `saenopy-1.0.2/saenopy/img/view_single.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/img/view_two.ico` & `saenopy-1.0.2/saenopy/img/view_two.ico`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/macro.py` & `saenopy-1.0.2/saenopy/macro.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/materials.py` & `saenopy-1.0.2/saenopy/materials.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/mesh.py` & `saenopy-1.0.2/saenopy/mesh.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/multigrid_helper.py` & `saenopy-1.0.2/saenopy/multigrid_helper.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/result_file.py` & `saenopy-1.0.2/saenopy/result_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -245,22 +245,23 @@
 
 
 def make_path_absolute(template, output):
     if not Path(template).is_absolute():
         return str(Path(output).absolute() / template)
     return str(Path(template).absolute())
 
+
 class Result(Saveable):
     __save_parameters__ = ['stacks', 'stack_reference', 'template',
                            'time_delta', 'piv_parameters', 'mesh_piv',
                            'mesh_parameters', 'material_parameters',
                            'solve_parameters', 'solvers',
                            '___save_name__', '___save_version__']
     ___save_name__ = "Result"
-    ___save_version__ = "1.3"
+    ___save_version__ = "1.4"
     output: str = None
     state: False
 
     stack_parameters: dict = None
     stacks: List[Stack] = None
     stack_reference: Stack = None
     template: str = None
@@ -285,14 +286,17 @@
                 if r["new"] is not None:
                     if isinstance(r["old"], Callable):
                         obj_data[r["new"]] = r["old"](obj_data)
                     elif r["old"] in obj_data:
                         obj_data[r["new"]] = obj_data[r["old"]]
                     elif "default" in r:
                         obj_data[r["new"]] = r["default"]
+                    else:
+                        raise ValueError(f"File does not contain parameter {r['old']} and {r['new']} does not have a "
+                                         f"default value.")
                 if r.get("renames_child", None) is not None:
                     apply_rename(obj_data[r["new"]], r.get("renames_child", None))
 
         def apply_delete(obj_data, rename):
             if isinstance(obj_data, list):
                 return [apply_delete(o, rename) for o in obj_data]
 
@@ -308,21 +312,21 @@
                 data_dict["stack"] = [data_dict["stack"][1]]
 
         if data_dict["___save_version__"] < "1.2":  # pragma: no cover
             print(f"convert old version {data_dict['___save_version__']} to 1.2")
             renames = [
                 dict(old="stack", new="stack", renames_child=[
                     dict(old="shape", new="_shape"),
-                    dict(old="leica_file", new="leica_file", default=None),
+                    dict(old="leica_file", new=None),
                     dict(old="crop", new="crop", default=None),
                     dict(old="packed_files", new="packed_files", default=None),
                 ]),
                 dict(old="stack_reference", new="stack_reference", renames_child=[
                     dict(old="shape", new="_shape"),
-                    dict(old="leica_file", new="leica_file", default=None),
+                    dict(old="leica_file", new=None),
                     dict(old="crop", new="crop", default=None),
                     dict(old="packed_files", new="packed_files", default=None),
                 ]),
                 dict(old="piv_parameter", new="piv_parameters", renames_child=[
                     dict(old="win_um", new="window_size"),
                     dict(old="elementsize", new="element_size"),
                     dict(old="signoise_filter", new="signal_to_noise"),
@@ -339,23 +343,23 @@
                 dict(old="solve_parameter", new="material_parameters", renames_child=[
                     dict(old="d0", new="d_0"),
                     dict(old="ds", new="d_s"),
                     dict(old="alpha", new=None),
                     dict(old="stepper", new=None),
                     dict(old="i_max", new=None),
                     dict(old="rel_conv_crit", new=None),
-                ]),
+                ], default=dict(k=1645, d0=0.0008, lambda_s=0.0075, ds=0.033)),
                 dict(old="solve_parameter", new="solve_parameters", renames_child=[
                     dict(old="k", new=None),
                     dict(old="d0", new=None),
                     dict(old="lambda_s", new=None),
                     dict(old="ds", new=None),
                     dict(old="stepper", new="step_size"),
                     dict(old="i_max", new="max_iterations"),
-                ]),
+                ], default=dict(alpha=1e10, stepper=0.33, i_max=100, rel_conv_crit=0.01)),
 
                 dict(old="mesh_piv", new="mesh_piv", renames_child=[
                     dict(old="R", new="nodes"),
                     dict(old="T", new="tetrahedra"),
                     dict(old="node_vars", new=None),
                     dict(old=lambda d: d["node_vars"]["U_measured"], new="displacements_measured"),
                 ]),
@@ -382,19 +386,20 @@
                     dict(old="U_target", new=None),
                     dict(old="U_target_mask", new=None),
                     dict(old="reg_mask", new=None),
                     dict(old="f", new=None),
                     dict(old="f_target", new=None),
                     dict(old="E_glo", new=None),
                     dict(old="var", new=None),
-                    dict(old="relrec", new="regularisation_results"),
+                    dict(old="regularisation_parameters", new="regularisation_parameters", default=None),
+                    dict(old="relrec", new="regularisation_results", default=[]),
                     dict(old="material_model", new="material_model", renames_child=[
                         dict(old="d0", new="d_0"),
                         dict(old="ds", new="d_s"),
-                    ]),
+                    ], default=dict(k=1645, d0=0.0008, lambda_s=0.0075, ds=0.033)),
                 ]),
                 dict(old="time_delta", new="time_delta", default=None),
                 dict(old="stack_parameters", new=None),
             ]
             apply_rename(data_dict, renames)
             apply_delete(data_dict, renames)
 
@@ -405,14 +410,27 @@
                 dict(old="stack", new="stacks"),
                 dict(old="solver", new="solvers"),
             ]
             apply_rename(data_dict, renames)
             apply_delete(data_dict, renames)
 
             data_dict["___save_version__"] = "1.3"
+        if data_dict["___save_version__"] < "1.4":  # pragma: no cover
+            print(f"convert old version {data_dict['___save_version__']} to 1.4")
+            renames = [
+                dict(old="solvers", new="solvers", renames_child=[
+                    dict(old="mesh", new="mesh", renames_child=[
+                        dict(old="cell_boundary_mask", new="cell_boundary_mask", default=None)
+                    ]),
+                ]),
+            ]
+            apply_rename(data_dict, renames)
+            apply_delete(data_dict, renames)
+
+            data_dict["___save_version__"] = "1.4"
         return super().from_dict(data_dict)
 
     def __init__(self, output=None, template=None, stack=None, time_delta=None, **kwargs):
         if output is not None:
             self.output = str(Path(output).absolute())
 
         self.stacks = stack
@@ -450,14 +468,20 @@
                 self.solvers[0].regularisation_results = None
             if "stack_reference" in kwargs:
                 self.mesh_piv = [None] * (len(self.stacks))
             else:
                 self.mesh_piv = [None] * (len(self.stacks) - 1)
             self.solvers = [None] * (len(self.mesh_piv))
 
+    def get_absolute_path(self):
+        return make_path_absolute(self.template, Path(self.output).parent)
+
+    def get_absolute_path_reference(self):
+        return make_path_absolute(self.stack_reference.template, Path(self.output).parent)
+
     def save(self, filename: str = None, file_format=".saenopy"):
         if filename is not None:
             for stack in self.stacks:
                 stack.paths_absolute()
             if self.stack_reference is not None:
                 self.stack_reference.paths_absolute()
             self.template = make_path_absolute(self.template, Path(self.output).parent)
```

### Comparing `saenopy-1.0.1/saenopy/saveable.py` & `saenopy-1.0.2/saenopy/saveable.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/solver.py` & `saenopy-1.0.2/saenopy/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from saenopy.saveable import Saveable
 from typing import List
 
 
 class SolverMesh(Mesh):
     __save_parameters__ = ["nodes", "tetrahedra", "displacements", "forces",
                            "displacements_fixed", "displacements_target", "displacements_target_mask",
-                           "forces_target", "strain_energy", "movable",
+                           "forces_target", "strain_energy", "movable", "cell_boundary_mask",
                            "regularisation_mask"]
     number_tetrahedra = 0  # the number of tetrahedra
     number_nodes = 0  # the number of vertices
 
     energy: NDArray[Shape["N_t"], Float] = field(doc="the energy stored in each tetrahedron, dimensions: N_T",
                                                  validators=check_tetrahedra_scalar_field, default=None)
     volume: NDArray[Shape["N_t"], Float] = field(doc="the volume of each tetrahedron, dimensions: N_T",
@@ -36,14 +36,15 @@
     Phi_valid = False
     displacements: NDArray[Shape["N_c, 3"], Float] = field(doc="the displacements of each node, dimensions: N_c x 3",
                                                            validators=check_node_vector_field, default=None)
     displacements_fixed: NDArray[Shape["N_c, 3"], Float] = field(validators=check_node_vector_field, default=None)
     displacements_target: NDArray[Shape["N_c, 3"], Float] = field(validators=check_node_vector_field, default=None)
     displacements_target_mask: NDArray[Shape["N_c"], Bool] = field(validators=check_node_scalar_field, default=None)
     regularisation_mask: NDArray[Shape["N_c"], Bool] = field(validators=check_node_scalar_field, default=None)
+    cell_boundary_mask: NDArray[Shape["N_c"], Bool] = field(validators=check_node_scalar_field, default=None)
 
     forces: NDArray[Shape["N_c, 3"], Float] = field(doc="the global forces on each node, dimensions: N_c x 3",
                                                     validators=check_node_vector_field, default=None)
     forces_target: NDArray[Shape["N_c, 3"], Float] = field(doc="the external forces on each node, dimensions: N_c x 3",
                                                            validators=check_node_vector_field, default=None)
     stiffness_tensor: NDArray[Shape["N_c, N_c, 3, 3"], Float] = None  # the global stiffness tensor, dimensions: N_c x N_c x 3 x 3
 
@@ -634,14 +635,18 @@
                 self.localweight[:] = 1 / Fvalues[:]
             else:
                 self.localweight *= 1.0
 
         index = self.localweight < 1e-10
         self.localweight[index & self.mesh.movable] = 1e-10
 
+        if self.mesh.cell_boundary_mask is not None:
+            self.localweight[:] = 0.03
+            self.localweight[self.mesh.cell_boundary_mask] = 0.003*0.001
+
         self.localweight[~self.mesh.regularisation_mask] = 0
 
         counter = np.sum(1.0 - self.localweight[self.mesh.movable])
         counterall = np.sum(self.mesh.movable)
 
         if self.verbose:
             print("total weight: ", counter, "/", counterall)
@@ -1017,14 +1022,55 @@
         elif mode == "next":
             xpos2 = U
     else:
         xpos2 = U
     return xpos2
 
 
+def get_cell_boundary(result, channel=1, thershold=20, smooth=2, element_size=14.00e-6, boundary=True, pos=None):
+    from scipy.ndimage import gaussian_filter
+    import matplotlib.pyplot as plt
+    import numpy as np
+
+    for i in range(len(result.stacks)):
+        stack_deformed = result.stacks[i]
+        voxel_size1 = stack_deformed.voxel_size
+
+        im = stack_deformed[:, :, 0, :, channel]
+        im = gaussian_filter(im, sigma=smooth, truncate=2.0)
+
+        im_thresh = (im[:, :, :] > thershold).astype(np.uint8)
+        from skimage.morphology import erosion
+        if boundary:
+            im_thresh = (im_thresh - erosion(im_thresh)).astype(bool)
+        else:
+            im_thresh = im_thresh.astype(bool)
+        du, dv, dw = voxel_size1
+
+        u = im_thresh
+        y, x, z = np.indices(u.shape)
+        y, x, z = (y * stack_deformed.shape[0] * dv / u.shape[0] * 1e-6,
+                   x * stack_deformed.shape[1] * du / u.shape[1] * 1e-6,
+                   z * stack_deformed.shape[2] * dw / u.shape[2] * 1e-6)
+        z -= np.max(z)/2
+        x -= np.max(x)/2
+        y -= np.max(y)/2
+
+        x = x[im_thresh]
+        y = y[im_thresh]
+        z = z[im_thresh]
+
+        yxz = np.vstack([y, x, z])
+
+        dist_to_cell = np.min(np.linalg.norm(result.solvers[0].mesh.nodes[:, :, None] - yxz[None, :, :], axis=1), axis=1)
+        included = dist_to_cell < element_size/2
+
+        result.solvers[i].mesh.cell_boundary_mask = included
+
+
 from saenopy.get_deformations import PivMesh
 def interpolate_mesh(mesh: PivMesh, xpos2: np.ndarray, params: dict) -> Solver:
     import saenopy
     from saenopy.multigrid_helper import get_scaled_mesh, get_nodes_with_one_face
 
     x, y, z = (mesh.nodes.max(axis=0) - mesh.nodes.min(axis=0)) * 1e6
     if params["mesh_size"] == "piv":
```

### Comparing `saenopy-1.0.1/saenopy/stack.py` & `saenopy-1.0.2/saenopy/stack.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/saenopy/unused/macro.py` & `saenopy-1.0.2/saenopy/unused/macro.py`

 * *Files identical despite different names*

### Comparing `saenopy-1.0.1/PKG-INFO` & `saenopy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saenopy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Semi-elastic fiber optimisation in python.
 License: MIT
 Author: rgerum
 Author-email: 14153051+rgerum@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -59,18 +59,18 @@
 
 ## Installation
 
 ### Standalone
 To use saenopy without a complicated installation you can use our standalone binaries to get started right away on Windows or Linux.
 
 Windows
-https://github.com/rgerum/saenopy/releases/download/v1.0.1/saenopy.exe
+https://github.com/rgerum/saenopy/releases/download/v1.0.2/saenopy.exe
 
 Linux
-https://github.com/rgerum/saenopy/releases/download/v1.0.1/saenopy
+https://github.com/rgerum/saenopy/releases/download/v1.0.2/saenopy
 
 ### Using Python
 
 If you are experienced with python or even want to use our Python API, you need to install saenopy as a python package.
 Saenopy can be installed directly using pip:
 
     ``pip install saenopy``
```

