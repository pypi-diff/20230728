# Comparing `tmp/Xplique-1.0.2.tar.gz` & `tmp/Xplique-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xplique-1.0.2.tar", last modified: Thu Jul 20 20:43:57 2023, max compression
+gzip compressed data, was "Xplique-1.0.3.tar", last modified: Fri Jul 28 18:48:19 2023, max compression
```

## Comparing `Xplique-1.0.2.tar` & `Xplique-1.0.3.tar`

### file list

```diff
@@ -1,132 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-20 20:43:46.000000 Xplique-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    22482 2023-07-20 20:43:57.904782 Xplique-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21956 2023-07-20 20:43:46.000000 Xplique-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.892782 Xplique-1.0.2/Xplique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    22482 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4085 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-20 20:43:57.000000 Xplique-1.0.2/Xplique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 20:43:57.904782 Xplique-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-07-20 20:43:46.000000 Xplique-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.892782 Xplique-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.892782 Xplique-1.0.2/tests/attributions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_callable.py
--rw-r--r--   0 runner    (1001) docker     (122)     4955 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_deconvnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3019 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_grad_cam.py
--rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_grad_cam_pp.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_gradient_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_guided_backprop.py
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_hsic.py
--rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_kernel_shap.py
--rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_lime.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_object_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_occlusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_rise.py
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_saliency.py
--rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_smoothgrad.py
--rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_sobol.py
--rw-r--r--   0 runner    (1001) docker     (122)     5240 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/attributions/test_tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/commons/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/commons/test_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/commons/test_model_override.py
--rw-r--r--   0 runner    (1001) docker     (122)     4547 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/commons/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/concepts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/concepts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/concepts/test_cav.py
--rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/concepts/test_tcav.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/features_visualizations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_maco.py
--rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_objectives.py
--rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_preconditionning.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/features_visualizations/test_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/generic/test_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/test_common.py
--rw-r--r--   0 runner    (1001) docker     (122)     5983 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/test_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/test_mege.py
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/metrics/test_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/tests/plots/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/plots/test_metric_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/plots/test_timeseries_plots.py
--rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-07-20 20:43:46.000000 Xplique-1.0.2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.896782 Xplique-1.0.2/xplique/
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.900782 Xplique-1.0.2/xplique/attributions/
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5716 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/deconvnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.900782 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/kernels.py
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/replicated_designs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/samplers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py
--rw-r--r--   0 runner    (1001) docker     (122)     9897 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py
--rw-r--r--   0 runner    (1001) docker     (122)     7543 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/grad_cam.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/grad_cam_pp.py
--rw-r--r--   0 runner    (1001) docker     (122)     2317 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/gradient_input.py
--rw-r--r--   0 runner    (1001) docker     (122)     2936 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/guided_backpropagation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/integrated_gradients.py
--rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/kernel_shap.py
--rw-r--r--   0 runner    (1001) docker     (122)    26149 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/lime.py
--rw-r--r--   0 runner    (1001) docker     (122)     9954 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/object_detector.py
--rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/occlusion.py
--rw-r--r--   0 runner    (1001) docker     (122)     7484 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/rise.py
--rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/saliency.py
--rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/smoothgrad.py
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/square_grad.py
--rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/attributions/vargrad.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.900782 Xplique-1.0.2/xplique/commons/
--rw-r--r--   0 runner    (1001) docker     (122)      568 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/callable_operations.py
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)      882 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/model_override.py
--rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/operators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/commons/tf_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/concepts/
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/concepts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/concepts/cav.py
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/concepts/tcav.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/features_visualizations/
--rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     7083 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/maco.py
--rw-r--r--   0 runner    (1001) docker     (122)    11045 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/objectives.py
--rw-r--r--   0 runner    (1001) docker     (122)     6520 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/optim.py
--rw-r--r--   0 runner    (1001) docker     (122)     7627 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/preconditioning.py
--rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5581 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/features_visualizations/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16580 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/fidelity.py
--rw-r--r--   0 runner    (1001) docker     (122)     8702 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/representativity.py
--rw-r--r--   0 runner    (1001) docker     (122)     3797 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/metrics/stability.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/plots/
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6566 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     5389 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    12877 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)     5166 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/plots/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 20:43:57.904782 Xplique-1.0.2/xplique/types/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-20 20:43:46.000000 Xplique-1.0.2/xplique/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.433872 Xplique-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-28 18:48:08.000000 Xplique-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    23081 2023-07-28 18:48:19.433872 Xplique-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    22555 2023-07-28 18:48:08.000000 Xplique-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.413872 Xplique-1.0.3/Xplique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    23081 2023-07-28 18:48:19.000000 Xplique-1.0.3/Xplique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-28 18:48:19.000000 Xplique-1.0.3/Xplique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-28 18:48:19.000000 Xplique-1.0.3/Xplique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-07-28 18:48:19.000000 Xplique-1.0.3/Xplique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-28 18:48:19.000000 Xplique-1.0.3/Xplique.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-28 18:48:19.433872 Xplique-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-07-28 18:48:08.000000 Xplique-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.413872 Xplique-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.417872 Xplique-1.0.3/tests/attributions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8120 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_callable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4955 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_deconvnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_forgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3019 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_grad_cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_grad_cam_pp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_gradient_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_guided_backprop.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_kernel_shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6117 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_occlusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_rise.py
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_saliency.py
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_smoothgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4954 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_sobol.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5240 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/attributions/test_tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.417872 Xplique-1.0.3/tests/commons/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/commons/test_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5704 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/commons/test_model_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4547 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/commons/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.421872 Xplique-1.0.3/tests/concepts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/concepts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/concepts/test_cav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1361 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/concepts/test_tcav.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.421872 Xplique-1.0.3/tests/features_visualizations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/features_visualizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/features_visualizations/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/features_visualizations/test_maco.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5314 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/features_visualizations/test_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3780 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/features_visualizations/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/features_visualizations/test_preconditionning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/features_visualizations/test_regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/features_visualizations/test_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.421872 Xplique-1.0.3/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2513 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/generic/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.421872 Xplique-1.0.3/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/metrics/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5983 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/metrics/test_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (122)      720 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/metrics/test_mege.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/metrics/test_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.421872 Xplique-1.0.3/tests/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1438 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/plots/test_metric_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/plots/test_timeseries_plots.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3763 2023-07-28 18:48:08.000000 Xplique-1.0.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.421872 Xplique-1.0.3/xplique/
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.425872 Xplique-1.0.3/xplique/attributions/
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5716 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2971 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/deconvnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.429872 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3029 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4274 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/replicated_designs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9897 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7543 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/grad_cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/grad_cam_pp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2317 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/gradient_input.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2936 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/guided_backpropagation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/integrated_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6873 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/kernel_shap.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26149 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9954 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/object_detector.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/occlusion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7484 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/rise.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/saliency.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5991 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/smoothgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/square_grad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1746 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/attributions/vargrad.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.429872 Xplique-1.0.3/xplique/commons/
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/commons/callable_operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2052 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/commons/data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      882 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/commons/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/commons/forgrad.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6439 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/commons/model_override.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/commons/operators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1433 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/commons/tf_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.429872 Xplique-1.0.3/xplique/concepts/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/concepts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4603 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/concepts/cav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/concepts/tcav.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.429872 Xplique-1.0.3/xplique/features_visualizations/
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/features_visualizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/features_visualizations/losses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7083 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/features_visualizations/maco.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11045 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/features_visualizations/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6520 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/features_visualizations/optim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7627 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/features_visualizations/preconditioning.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/features_visualizations/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5581 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/features_visualizations/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.429872 Xplique-1.0.3/xplique/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16580 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/metrics/fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8702 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/metrics/representativity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3797 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/metrics/stability.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.433872 Xplique-1.0.3/xplique/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6566 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/plots/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5389 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/plots/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12877 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/plots/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5166 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/plots/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-28 18:48:19.433872 Xplique-1.0.3/xplique/types/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-28 18:48:08.000000 Xplique-1.0.3/xplique/types/__init__.py
```

### Comparing `Xplique-1.0.2/LICENSE` & `Xplique-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/PKG-INFO` & `Xplique-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xplique
-Version: 1.0.2
+Version: 1.0.3
 Summary: Explanations toolbox for Tensorflow 2
 Author: Thomas FEL
 Author-email: thomas_fel@brown.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -95,14 +95,15 @@
     <a href="https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2">
         <img width="95%" src="./docs/assets/attributions.jpeg">
     </a>
 </p>
 
 - [**Attribution Methods**: Sanity checks paper](https://colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) </sub>
 - [**Attribution Methods**: Tabular data and Regression](https://colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) </sub>
+- [**FORGRad**: Gradient strikes back with FORGrad](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) </sub>
 - [**Attribution Methods**: Metrics](https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) </sub>
 
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg"> 
         <img width="95%" src="./docs/assets/metrics.jpeg">
     </a>
 </p>
@@ -229,14 +230,15 @@
 | Rise                   | Callable*     | [Paper](https://arxiv.org/abs/1806.07421) | WIP                | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1icu2b1JGfpTRa-ic8tBSXnqqfuCGW2mO) |
 | Saliency               | TF            | [Paper](https://arxiv.org/abs/1312.6034)  | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19eB3uwAtCKZgkoWtMzrF0LTJ-htF_KE7) |
 | SmoothGrad             | TF            | [Paper](https://arxiv.org/abs/1706.03825) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | SquareGrad             | TF            | [Paper](https://arxiv.org/abs/1806.10758) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | VarGrad                | TF            | [Paper](https://arxiv.org/abs/1810.03292) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | Sobol Attribution      | TF            | [Paper](https://arxiv.org/abs/2111.04138) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) |
 | Hsic Attribution      | TF            | [Paper](https://arxiv.org/abs/2206.06219) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) |
+| FORGrad enhancement      | TF            | [Paper](https://arxiv.org/abs/2307.09591) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) |
 
 
 * : See the [Callable documentation](https://deel-ai.github.io/xplique/callable/)
 
 | **Attribution Metrics** | Type of Model | Property         | Source                                    |
 | :---------------------- | :------------ | :--------------- | :---------------------------------------- |
 | MuFidelity              | TF            | Fidelity         | [Paper](https://arxiv.org/abs/2005.00631) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Xplique Version: 1.0.2 Summary: Explanations
+Metadata-Version: 2.1 Name: Xplique Version: 1.0.3 Summary: Explanations
 toolbox for Tensorflow 2 Author: Thomas FEL Author-email: thomas_fel@brown.edu
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: tests Provides-Extra: docs License-File: LICENSE
                                    [Xplique]
@@ -46,14 +46,18 @@
 colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) -
 [**Attribution Methods**: Tabular data and Regression](https://
 colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) -
+[**FORGRad**: Gradient strikes back with FORGrad](https://
+colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) -
 [**Attribution Methods**: Metrics](https://colab.research.google.com/drive/
 1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg)
                          [./docs/assets/metrics.jpeg]
 - [**Concepts Methods**: Testing with Concept Activation Vectors](https://
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE) [![Open In
@@ -162,15 +166,18 @@
 [Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) | |
 Sobol Attribution | TF | [Paper](https://arxiv.org/abs/2111.04138) | | â | |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | |
 Hsic Attribution | TF | [Paper](https://arxiv.org/abs/2206.06219) | | â | |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | *
+(https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | |
+FORGrad enhancement | TF | [Paper](https://arxiv.org/abs/2307.09591) | | â |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) | *
 : See the [Callable documentation](https://deel-ai.github.io/xplique/callable/
 ) | **Attribution Metrics** | Type of Model | Property | Source | | :----------
 ------------ | :------------ | :--------------- | :----------------------------
 ------------ | | MuFidelity | TF | Fidelity | [Paper](https://arxiv.org/abs/
 2005.00631) | | Deletion | TF | Fidelity | [Paper](https://arxiv.org/abs/
 1806.07421) | | Insertion | TF | Fidelity | [Paper](https://arxiv.org/abs/
 1806.07421) | | Average Stability | TF | Stability | [Paper](https://arxiv.org/
```

### Comparing `Xplique-1.0.2/README.md` & `Xplique-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     <a href="https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2">
         <img width="95%" src="./docs/assets/attributions.jpeg">
     </a>
 </p>
 
 - [**Attribution Methods**: Sanity checks paper](https://colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) </sub>
 - [**Attribution Methods**: Tabular data and Regression](https://colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) </sub>
+- [**FORGRad**: Gradient strikes back with FORGrad](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) </sub>
 - [**Attribution Methods**: Metrics](https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) </sub>
 
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg"> 
         <img width="95%" src="./docs/assets/metrics.jpeg">
     </a>
 </p>
@@ -211,14 +212,15 @@
 | Rise                   | Callable*     | [Paper](https://arxiv.org/abs/1806.07421) | WIP                | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1icu2b1JGfpTRa-ic8tBSXnqqfuCGW2mO) |
 | Saliency               | TF            | [Paper](https://arxiv.org/abs/1312.6034)  | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19eB3uwAtCKZgkoWtMzrF0LTJ-htF_KE7) |
 | SmoothGrad             | TF            | [Paper](https://arxiv.org/abs/1706.03825) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | SquareGrad             | TF            | [Paper](https://arxiv.org/abs/1806.10758) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | VarGrad                | TF            | [Paper](https://arxiv.org/abs/1810.03292) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | Sobol Attribution      | TF            | [Paper](https://arxiv.org/abs/2111.04138) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) |
 | Hsic Attribution      | TF            | [Paper](https://arxiv.org/abs/2206.06219) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) |
+| FORGrad enhancement      | TF            | [Paper](https://arxiv.org/abs/2307.09591) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) |
 
 
 * : See the [Callable documentation](https://deel-ai.github.io/xplique/callable/)
 
 | **Attribution Metrics** | Type of Model | Property         | Source                                    |
 | :---------------------- | :------------ | :--------------- | :---------------------------------------- |
 | MuFidelity              | TF            | Fidelity         | [Paper](https://arxiv.org/abs/2005.00631) |
```

#### html2text {}

```diff
@@ -39,14 +39,18 @@
 colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) -
 [**Attribution Methods**: Tabular data and Regression](https://
 colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) -
+[**FORGRad**: Gradient strikes back with FORGrad](https://
+colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) -
 [**Attribution Methods**: Metrics](https://colab.research.google.com/drive/
 1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg)
                          [./docs/assets/metrics.jpeg]
 - [**Concepts Methods**: Testing with Concept Activation Vectors](https://
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE) [![Open In
@@ -155,15 +159,18 @@
 [Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) | |
 Sobol Attribution | TF | [Paper](https://arxiv.org/abs/2111.04138) | | â | |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | |
 Hsic Attribution | TF | [Paper](https://arxiv.org/abs/2206.06219) | | â | |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | *
+(https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | |
+FORGrad enhancement | TF | [Paper](https://arxiv.org/abs/2307.09591) | | â |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) | *
 : See the [Callable documentation](https://deel-ai.github.io/xplique/callable/
 ) | **Attribution Metrics** | Type of Model | Property | Source | | :----------
 ------------ | :------------ | :--------------- | :----------------------------
 ------------ | | MuFidelity | TF | Fidelity | [Paper](https://arxiv.org/abs/
 2005.00631) | | Deletion | TF | Fidelity | [Paper](https://arxiv.org/abs/
 1806.07421) | | Insertion | TF | Fidelity | [Paper](https://arxiv.org/abs/
 1806.07421) | | Average Stability | TF | Stability | [Paper](https://arxiv.org/
```

### Comparing `Xplique-1.0.2/Xplique.egg-info/PKG-INFO` & `Xplique-1.0.3/Xplique.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xplique
-Version: 1.0.2
+Version: 1.0.3
 Summary: Explanations toolbox for Tensorflow 2
 Author: Thomas FEL
 Author-email: thomas_fel@brown.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -95,14 +95,15 @@
     <a href="https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2">
         <img width="95%" src="./docs/assets/attributions.jpeg">
     </a>
 </p>
 
 - [**Attribution Methods**: Sanity checks paper](https://colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) </sub>
 - [**Attribution Methods**: Tabular data and Regression](https://colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) </sub>
+- [**FORGRad**: Gradient strikes back with FORGrad](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) </sub>
 - [**Attribution Methods**: Metrics](https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) <sub> [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) </sub>
 
 <p align="center" width="100%">
     <a href="https://colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg"> 
         <img width="95%" src="./docs/assets/metrics.jpeg">
     </a>
 </p>
@@ -229,14 +230,15 @@
 | Rise                   | Callable*     | [Paper](https://arxiv.org/abs/1806.07421) | WIP                | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1icu2b1JGfpTRa-ic8tBSXnqqfuCGW2mO) |
 | Saliency               | TF            | [Paper](https://arxiv.org/abs/1312.6034)  | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19eB3uwAtCKZgkoWtMzrF0LTJ-htF_KE7) |
 | SmoothGrad             | TF            | [Paper](https://arxiv.org/abs/1706.03825) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | SquareGrad             | TF            | [Paper](https://arxiv.org/abs/1806.10758) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | VarGrad                | TF            | [Paper](https://arxiv.org/abs/1810.03292) | ✔                  | ✔                 | WIP                | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) |
 | Sobol Attribution      | TF            | [Paper](https://arxiv.org/abs/2111.04138) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) |
 | Hsic Attribution      | TF            | [Paper](https://arxiv.org/abs/2206.06219) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) |
+| FORGrad enhancement      | TF            | [Paper](https://arxiv.org/abs/2307.09591) |                    | ✔                 |                    | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) |
 
 
 * : See the [Callable documentation](https://deel-ai.github.io/xplique/callable/)
 
 | **Attribution Metrics** | Type of Model | Property         | Source                                    |
 | :---------------------- | :------------ | :--------------- | :---------------------------------------- |
 | MuFidelity              | TF            | Fidelity         | [Paper](https://arxiv.org/abs/2005.00631) |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Xplique Version: 1.0.2 Summary: Explanations
+Metadata-Version: 2.1 Name: Xplique Version: 1.0.3 Summary: Explanations
 toolbox for Tensorflow 2 Author: Thomas FEL Author-email: thomas_fel@brown.edu
 License: MIT Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
 Provides-Extra: tests Provides-Extra: docs License-File: LICENSE
                                    [Xplique]
@@ -46,14 +46,18 @@
 colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1uJOmAg6RjlOIJj6SWN9sYRamBdHAuyaS) -
 [**Attribution Methods**: Tabular data and Regression](https://
 colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) [![Open In
 Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1pjDJmAa9oeSquYtbYh6tksU6eTmObIcq) -
+[**FORGRad**: Gradient strikes back with FORGrad](https://
+colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) -
 [**Attribution Methods**: Metrics](https://colab.research.google.com/drive/
 1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg) [![Open In Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1WEpVpFSq-oL1Ejugr8Ojb3tcbqXIOPBg)
                          [./docs/assets/metrics.jpeg]
 - [**Concepts Methods**: Testing with Concept Activation Vectors](https://
 colab.research.google.com/drive/1iuEz46ZjgG97vTBH8p-vod3y14UETvVE) [![Open In
@@ -162,15 +166,18 @@
 [Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/12-tlM_TdZ12oc5lNL2S2g-hcMJV8tZUD) | |
 Sobol Attribution | TF | [Paper](https://arxiv.org/abs/2111.04138) | | â | |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | |
 Hsic Attribution | TF | [Paper](https://arxiv.org/abs/2206.06219) | | â | |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | *
+(https://colab.research.google.com/drive/1XproaVxXjO9nrBSyyy7BuKJ1vy21iHs2) | |
+FORGrad enhancement | TF | [Paper](https://arxiv.org/abs/2307.09591) | | â |
+| [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/1ibLzn7r9QQIEmZxApObowzx8n9ukinYB) | *
 : See the [Callable documentation](https://deel-ai.github.io/xplique/callable/
 ) | **Attribution Metrics** | Type of Model | Property | Source | | :----------
 ------------ | :------------ | :--------------- | :----------------------------
 ------------ | | MuFidelity | TF | Fidelity | [Paper](https://arxiv.org/abs/
 2005.00631) | | Deletion | TF | Fidelity | [Paper](https://arxiv.org/abs/
 1806.07421) | | Insertion | TF | Fidelity | [Paper](https://arxiv.org/abs/
 1806.07421) | | Average Stability | TF | Stability | [Paper](https://arxiv.org/
```

### Comparing `Xplique-1.0.2/Xplique.egg-info/SOURCES.txt` & `Xplique-1.0.3/Xplique.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Xplique.egg-info/top_level.txt
 tests/__init__.py
 tests/utils.py
 tests/attributions/__init__.py
 tests/attributions/test_callable.py
 tests/attributions/test_common.py
 tests/attributions/test_deconvnet.py
+tests/attributions/test_forgrad.py
 tests/attributions/test_grad_cam.py
 tests/attributions/test_grad_cam_pp.py
 tests/attributions/test_gradient_input.py
 tests/attributions/test_guided_backprop.py
 tests/attributions/test_hsic.py
 tests/attributions/test_integrated_gradients.py
 tests/attributions/test_kernel_shap.py
@@ -80,14 +81,15 @@
 xplique/attributions/global_sensitivity_analysis/samplers.py
 xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py
 xplique/attributions/global_sensitivity_analysis/sobol_estimators.py
 xplique/commons/__init__.py
 xplique/commons/callable_operations.py
 xplique/commons/data_conversion.py
 xplique/commons/exceptions.py
+xplique/commons/forgrad.py
 xplique/commons/model_override.py
 xplique/commons/operators.py
 xplique/commons/tf_operations.py
 xplique/concepts/__init__.py
 xplique/concepts/cav.py
 xplique/concepts/tcav.py
 xplique/features_visualizations/__init__.py
```

### Comparing `Xplique-1.0.2/setup.py` & `Xplique-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as fh:
     README = fh.read()
 
 setup(
     name="Xplique",
-    version="1.0.2",
+    version="1.0.3",
     description="Explanations toolbox for Tensorflow 2",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Thomas FEL",
     author_email="thomas_fel@brown.edu",
     license="MIT",
     install_requires=['tensorflow>=2.1.0', 'numpy', 'scikit-learn', 'scikit-image',
```

### Comparing `Xplique-1.0.2/tests/attributions/test_callable.py` & `Xplique-1.0.3/tests/attributions/test_callable.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_common.py` & `Xplique-1.0.3/tests/attributions/test_common.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_deconvnet.py` & `Xplique-1.0.3/tests/attributions/test_deconvnet.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_grad_cam.py` & `Xplique-1.0.3/tests/attributions/test_grad_cam.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_grad_cam_pp.py` & `Xplique-1.0.3/tests/attributions/test_grad_cam_pp.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_gradient_input.py` & `Xplique-1.0.3/tests/attributions/test_gradient_input.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_guided_backprop.py` & `Xplique-1.0.3/tests/attributions/test_guided_backprop.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_hsic.py` & `Xplique-1.0.3/tests/attributions/test_hsic.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_integrated_gradients.py` & `Xplique-1.0.3/tests/attributions/test_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_kernel_shap.py` & `Xplique-1.0.3/tests/attributions/test_kernel_shap.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_lime.py` & `Xplique-1.0.3/tests/attributions/test_lime.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_object_detector.py` & `Xplique-1.0.3/tests/attributions/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_occlusion.py` & `Xplique-1.0.3/tests/attributions/test_occlusion.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_rise.py` & `Xplique-1.0.3/tests/attributions/test_rise.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_saliency.py` & `Xplique-1.0.3/tests/attributions/test_saliency.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_smoothgrad.py` & `Xplique-1.0.3/tests/attributions/test_smoothgrad.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_sobol.py` & `Xplique-1.0.3/tests/attributions/test_sobol.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/attributions/test_tabular_data.py` & `Xplique-1.0.3/tests/attributions/test_tabular_data.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/commons/test_data_conversion.py` & `Xplique-1.0.3/tests/commons/test_data_conversion.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/commons/test_model_override.py` & `Xplique-1.0.3/tests/commons/test_model_override.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/commons/test_operators.py` & `Xplique-1.0.3/tests/commons/test_operators.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/concepts/test_cav.py` & `Xplique-1.0.3/tests/concepts/test_cav.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/concepts/test_tcav.py` & `Xplique-1.0.3/tests/concepts/test_tcav.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/features_visualizations/test_losses.py` & `Xplique-1.0.3/tests/features_visualizations/test_losses.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/features_visualizations/test_maco.py` & `Xplique-1.0.3/tests/features_visualizations/test_maco.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/features_visualizations/test_objectives.py` & `Xplique-1.0.3/tests/features_visualizations/test_objectives.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/features_visualizations/test_optim.py` & `Xplique-1.0.3/tests/features_visualizations/test_optim.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/features_visualizations/test_preconditionning.py` & `Xplique-1.0.3/tests/features_visualizations/test_preconditionning.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/features_visualizations/test_regularizers.py` & `Xplique-1.0.3/tests/features_visualizations/test_regularizers.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/features_visualizations/test_transformations.py` & `Xplique-1.0.3/tests/features_visualizations/test_transformations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/generic/test_wrapper.py` & `Xplique-1.0.3/tests/generic/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/metrics/test_common.py` & `Xplique-1.0.3/tests/metrics/test_common.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/metrics/test_fidelity.py` & `Xplique-1.0.3/tests/metrics/test_fidelity.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/metrics/test_mege.py` & `Xplique-1.0.3/tests/metrics/test_mege.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/metrics/test_stability.py` & `Xplique-1.0.3/tests/metrics/test_stability.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/plots/test_metric_plots.py` & `Xplique-1.0.3/tests/plots/test_metric_plots.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/plots/test_timeseries_plots.py` & `Xplique-1.0.3/tests/plots/test_timeseries_plots.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/tests/utils.py` & `Xplique-1.0.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/__init__.py` & `Xplique-1.0.3/xplique/attributions/__init__.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/base.py` & `Xplique-1.0.3/xplique/attributions/base.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/deconvnet.py` & `Xplique-1.0.3/xplique/attributions/deconvnet.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/__init__.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/gsa_attribution_method.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/hsic_attribution_method.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/hsic_estimators.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/kernels.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/kernels.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/perturbations.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/perturbations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/replicated_designs.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/replicated_designs.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/samplers.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/samplers.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/sobol_attribution_method.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py` & `Xplique-1.0.3/xplique/attributions/global_sensitivity_analysis/sobol_estimators.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/grad_cam.py` & `Xplique-1.0.3/xplique/attributions/grad_cam.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/grad_cam_pp.py` & `Xplique-1.0.3/xplique/attributions/grad_cam_pp.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/gradient_input.py` & `Xplique-1.0.3/xplique/attributions/gradient_input.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/guided_backpropagation.py` & `Xplique-1.0.3/xplique/attributions/guided_backpropagation.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/integrated_gradients.py` & `Xplique-1.0.3/xplique/attributions/integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/kernel_shap.py` & `Xplique-1.0.3/xplique/attributions/kernel_shap.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/lime.py` & `Xplique-1.0.3/xplique/attributions/lime.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/object_detector.py` & `Xplique-1.0.3/xplique/attributions/object_detector.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/occlusion.py` & `Xplique-1.0.3/xplique/attributions/occlusion.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/rise.py` & `Xplique-1.0.3/xplique/attributions/rise.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/saliency.py` & `Xplique-1.0.3/xplique/attributions/saliency.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/smoothgrad.py` & `Xplique-1.0.3/xplique/attributions/smoothgrad.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/square_grad.py` & `Xplique-1.0.3/xplique/attributions/square_grad.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/attributions/vargrad.py` & `Xplique-1.0.3/xplique/attributions/vargrad.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/commons/__init__.py` & `Xplique-1.0.3/xplique/commons/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,7 +6,8 @@
 from .model_override import guided_relu_policy, deconv_relu_policy, override_relu_gradient, \
                             find_layer, open_relu_policy
 from .tf_operations import repeat_labels, batch_tensor
 from .callable_operations import predictions_one_hot_callable
 from .operators import check_operator, operator_batching,\
                        get_inference_function, get_gradient_functions
 from .exceptions import no_gradients_available, raise_invalid_operator
+from .forgrad import forgrad
```

### Comparing `Xplique-1.0.2/xplique/commons/callable_operations.py` & `Xplique-1.0.3/xplique/commons/callable_operations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/commons/data_conversion.py` & `Xplique-1.0.3/xplique/commons/data_conversion.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/commons/exceptions.py` & `Xplique-1.0.3/xplique/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/commons/model_override.py` & `Xplique-1.0.3/xplique/commons/model_override.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/commons/operators.py` & `Xplique-1.0.3/xplique/commons/operators.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/commons/tf_operations.py` & `Xplique-1.0.3/xplique/commons/tf_operations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/concepts/cav.py` & `Xplique-1.0.3/xplique/concepts/cav.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/concepts/tcav.py` & `Xplique-1.0.3/xplique/concepts/tcav.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/features_visualizations/losses.py` & `Xplique-1.0.3/xplique/features_visualizations/losses.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/features_visualizations/maco.py` & `Xplique-1.0.3/xplique/features_visualizations/maco.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/features_visualizations/objectives.py` & `Xplique-1.0.3/xplique/features_visualizations/objectives.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/features_visualizations/optim.py` & `Xplique-1.0.3/xplique/features_visualizations/optim.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/features_visualizations/preconditioning.py` & `Xplique-1.0.3/xplique/features_visualizations/preconditioning.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/features_visualizations/regularizers.py` & `Xplique-1.0.3/xplique/features_visualizations/regularizers.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/features_visualizations/transformations.py` & `Xplique-1.0.3/xplique/features_visualizations/transformations.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/metrics/base.py` & `Xplique-1.0.3/xplique/metrics/base.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/metrics/fidelity.py` & `Xplique-1.0.3/xplique/metrics/fidelity.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/metrics/representativity.py` & `Xplique-1.0.3/xplique/metrics/representativity.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/metrics/stability.py` & `Xplique-1.0.3/xplique/metrics/stability.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/plots/image.py` & `Xplique-1.0.3/xplique/plots/image.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/plots/metrics.py` & `Xplique-1.0.3/xplique/plots/metrics.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/plots/tabular.py` & `Xplique-1.0.3/xplique/plots/tabular.py`

 * *Files identical despite different names*

### Comparing `Xplique-1.0.2/xplique/plots/timeseries.py` & `Xplique-1.0.3/xplique/plots/timeseries.py`

 * *Files identical despite different names*

