# Comparing `tmp/edsteva-0.2.3.tar.gz` & `tmp/edsteva-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edsteva-0.2.3.tar", max compression
+gzip compressed data, was "edsteva-0.2.4.tar", max compression
```

## Comparing `edsteva-0.2.3.tar` & `edsteva-0.2.4.tar`

### file list

```diff
@@ -1,176 +1,176 @@
--rw-r--r--   0        0        0     1485 2023-07-05 07:04:21.350945 edsteva-0.2.3/LICENSE
--rw-r--r--   0        0        0     3030 2023-07-05 07:04:21.350945 edsteva-0.2.3/README.md
--rw-r--r--   0        0        0     3083 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/__init__.py
--rw-r--r--   0        0        0      138 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/__init__.py
--rw-r--r--   0        0        0     2345 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/files.py
--rw-r--r--   0        0        0    11701 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/hive.py
--rw-r--r--   0        0        0     6221 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/i2b2_mapping.py
--rw-r--r--   0        0        0     2957 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/postgres.py
--rw-r--r--   0        0        0     9050 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/settings.py
--rw-r--r--   0        0        0       37 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/__init__.py
--rw-r--r--   0        0        0     4044 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/biology.py
--rw-r--r--   0        0        0     1053 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/care_site.py
--rw-r--r--   0        0        0     4169 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/note.py
--rw-r--r--   0        0        0    27017 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/synthetic.py
--rw-r--r--   0        0        0     2997 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/utils.py
--rw-r--r--   0        0        0     3835 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/io/synthetic/visit.py
--rw-r--r--   0        0        0      395 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/metrics/__init__.py
--rw-r--r--   0        0        0     2169 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/metrics/error.py
--rw-r--r--   0        0        0     2558 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/metrics/error_after_t0.py
--rw-r--r--   0        0        0     2718 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/metrics/error_between_t0_t1.py
--rw-r--r--   0        0        0       42 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/__init__.py
--rw-r--r--   0        0        0    10800 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/base.py
--rw-r--r--   0        0        0       83 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/__init__.py
--rw-r--r--   0        0        0      239 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/algos/__init__.py
--rw-r--r--   0        0        0     3329 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/algos/loss_minimization.py
--rw-r--r--   0        0        0     5590 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/rectangle_function.py
--rw-r--r--   0        0        0     1450 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/__init__.py
--rw-r--r--   0        0        0     5197 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/defaults.py
--rw-r--r--   0        0        0     1207 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py
--rw-r--r--   0        0        0     1036 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py
--rw-r--r--   0        0        0      284 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/probe_dashboard.py
--rw-r--r--   0        0        0      165 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/probe_plot.py
--rw-r--r--   0        0        0       68 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/__init__.py
--rw-r--r--   0        0        0      336 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/algos/__init__.py
--rw-r--r--   0        0        0     2670 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/algos/loss_minimization.py
--rw-r--r--   0        0        0     2488 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/algos/quantile.py
--rw-r--r--   0        0        0     5292 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/step_function.py
--rw-r--r--   0        0        0     1395 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/__init__.py
--rw-r--r--   0        0        0     4315 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/defaults.py
--rw-r--r--   0        0        0      960 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      789 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/normalized_probe_plot.py
--rw-r--r--   0        0        0      284 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/probe_dashboard.py
--rw-r--r--   0        0        0      165 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/models/step_function/viz_configs/probe_plot.py
--rw-r--r--   0        0        0      257 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/__init__.py
--rw-r--r--   0        0        0    14067 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/base.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/__init__.py
--rw-r--r--   0        0        0     9091 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/biology.py
--rw-r--r--   0        0        0      488 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     5645 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/per_measurement.py
--rw-r--r--   0        0        0     6468 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     2595 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/__init__.py
--rw-r--r--   0        0        0     5239 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/defaults.py
--rw-r--r--   0        0        0      417 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/estimates_densities_plot.py
--rw-r--r--   0        0        0      618 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_plot.py
--rw-r--r--   0        0        0      516 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/__init__.py
--rw-r--r--   0        0        0     5538 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/defaults.py
--rw-r--r--   0        0        0      417 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/estimates_densities_plot.py
--rw-r--r--   0        0        0      618 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_plot.py
--rw-r--r--   0        0        0      516 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     5539 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      417 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      618 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      516 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/condition/__init__.py
--rw-r--r--   0        0        0      483 2023-07-05 07:04:21.366945 edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     7900 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/per_condition.py
--rw-r--r--   0        0        0     8932 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     6392 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/condition.py
--rw-r--r--   0        0        0     2437 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/__init__.py
--rw-r--r--   0        0        0     5310 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/defaults.py
--rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/__init__.py
--rw-r--r--   0        0        0     5542 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/defaults.py
--rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     6131 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/__init__.py
--rw-r--r--   0        0        0      457 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     7222 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/completeness_predictors/per_note.py
--rw-r--r--   0        0        0     8556 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     6418 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/note.py
--rw-r--r--   0        0        0     2278 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/__init__.py
--rw-r--r--   0        0        0     4891 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/defaults.py
--rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/__init__.py
--rw-r--r--   0        0        0     5148 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/defaults.py
--rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     5782 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/utils/__init__.py
--rw-r--r--   0        0        0    10772 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/utils/filter_df.py
--rw-r--r--   0        0        0    22314 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/utils/prepare_df.py
--rw-r--r--   0        0        0     6672 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/utils/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/__init__.py
--rw-r--r--   0        0        0      291 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/completeness_predictors/__init__.py
--rw-r--r--   0        0        0     8230 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/completeness_predictors/per_visit.py
--rw-r--r--   0        0        0     5326 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/visit.py
--rw-r--r--   0        0        0     1795 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/__init__.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/__init__.py
--rw-r--r--   0        0        0     4649 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/defaults.py
--rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/probe_plot.py
--rw-r--r--   0        0        0      322 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/__init__.py
--rw-r--r--   0        0        0     4904 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/defaults.py
--rw-r--r--   0        0        0      285 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/estimates_densities_plot.py
--rw-r--r--   0        0        0      486 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_dashboard.py
--rw-r--r--   0        0        0      244 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_plot.py
--rw-r--r--   0        0        0      384 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/probe_dashboard.py
--rw-r--r--   0        0        0      168 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/probe_plot.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/utils/__init__.py
--rw-r--r--   0        0        0     2498 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/utils/checks.py
--rw-r--r--   0        0        0     1155 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/utils/file_management.py
--rw-r--r--   0        0        0     1970 2023-07-05 07:04:21.370945 edsteva-0.2.3/edsteva/utils/framework.py
--rw-r--r--   0        0        0      176 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/utils/loss_functions.py
--rw-r--r--   0        0        0      344 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/utils/typing.py
--rw-r--r--   0        0        0       52 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/__init__.py
--rw-r--r--   0        0        0      242 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/normalized_probe/__init__.py
--rw-r--r--   0        0        0    11909 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/normalized_probe/normalized_probe.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/probe/__init__.py
--rw-r--r--   0        0        0     4232 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/probe/fitted_probe.py
--rw-r--r--   0        0        0     3477 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/probe/probe.py
--rw-r--r--   0        0        0     7686 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/dashboards/probe/wrapper.py
--rw-r--r--   0        0        0      339 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/estimates_densities/__init__.py
--rw-r--r--   0        0        0     8510 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/estimates_densities/estimates_densities.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/normalized_probe/__init__.py
--rw-r--r--   0        0        0     7621 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/normalized_probe/normalized_probe.py
--rw-r--r--   0        0        0        0 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/probe/__init__.py
--rw-r--r--   0        0        0     2334 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/probe/fitted_probe.py
--rw-r--r--   0        0        0     1483 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/probe/probe.py
--rw-r--r--   0        0        0     5453 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/plots/probe/wrapper.py
--rw-r--r--   0        0        0    16408 2023-07-05 07:04:21.374945 edsteva-0.2.3/edsteva/viz/utils.py
--rw-r--r--   0        0        0     3492 2023-07-05 07:04:21.374945 edsteva-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5759 1970-01-01 00:00:00.000000 edsteva-0.2.3/setup.py
--rw-r--r--   0        0        0     4570 1970-01-01 00:00:00.000000 edsteva-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-07-28 18:13:08.176347 edsteva-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3030 2023-07-28 18:13:08.176347 edsteva-0.2.4/README.md
+-rw-r--r--   0        0        0     3083 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/__init__.py
+-rw-r--r--   0        0        0     2345 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/files.py
+-rw-r--r--   0        0        0    11701 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/hive.py
+-rw-r--r--   0        0        0     6221 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/i2b2_mapping.py
+-rw-r--r--   0        0        0     2957 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/postgres.py
+-rw-r--r--   0        0        0     9050 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/settings.py
+-rw-r--r--   0        0        0       37 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/synthetic/__init__.py
+-rw-r--r--   0        0        0     4044 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/synthetic/biology.py
+-rw-r--r--   0        0        0     1053 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/synthetic/care_site.py
+-rw-r--r--   0        0        0     4170 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/synthetic/note.py
+-rw-r--r--   0        0        0    27126 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/synthetic/synthetic.py
+-rw-r--r--   0        0        0     2997 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/synthetic/utils.py
+-rw-r--r--   0        0        0     3835 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/io/synthetic/visit.py
+-rw-r--r--   0        0        0      395 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/metrics/__init__.py
+-rw-r--r--   0        0        0     2169 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/metrics/error.py
+-rw-r--r--   0        0        0     2558 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/metrics/error_after_t0.py
+-rw-r--r--   0        0        0     2718 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/metrics/error_between_t0_t1.py
+-rw-r--r--   0        0        0       42 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/__init__.py
+-rw-r--r--   0        0        0    10800 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/base.py
+-rw-r--r--   0        0        0       83 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/__init__.py
+-rw-r--r--   0        0        0      239 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/algos/__init__.py
+-rw-r--r--   0        0        0     3329 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/algos/loss_minimization.py
+-rw-r--r--   0        0        0     5590 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/rectangle_function.py
+-rw-r--r--   0        0        0     1450 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/__init__.py
+-rw-r--r--   0        0        0     5653 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/defaults.py
+-rw-r--r--   0        0        0     1254 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0     1083 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py
+-rw-r--r--   0        0        0      284 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/probe_dashboard.py
+-rw-r--r--   0        0        0      165 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/probe_plot.py
+-rw-r--r--   0        0        0       68 2023-07-28 18:13:08.188347 edsteva-0.2.4/edsteva/models/step_function/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/algos/__init__.py
+-rw-r--r--   0        0        0     2670 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/algos/loss_minimization.py
+-rw-r--r--   0        0        0     2488 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/algos/quantile.py
+-rw-r--r--   0        0        0     5292 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/step_function.py
+-rw-r--r--   0        0        0     1395 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/viz_configs/__init__.py
+-rw-r--r--   0        0        0     4773 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/viz_configs/defaults.py
+-rw-r--r--   0        0        0     1007 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      836 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/viz_configs/normalized_probe_plot.py
+-rw-r--r--   0        0        0      284 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/viz_configs/probe_dashboard.py
+-rw-r--r--   0        0        0      165 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/models/step_function/viz_configs/probe_plot.py
+-rw-r--r--   0        0        0      257 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/__init__.py
+-rw-r--r--   0        0        0    14067 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/base.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/__init__.py
+-rw-r--r--   0        0        0     9091 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/biology.py
+-rw-r--r--   0        0        0      488 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     5645 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/completeness_predictors/per_measurement.py
+-rw-r--r--   0        0        0     6468 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     2595 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/__init__.py
+-rw-r--r--   0        0        0     5214 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/estimates_densities_plot.py
+-rw-r--r--   0        0        0      571 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/__init__.py
+-rw-r--r--   0        0        0     5480 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/estimates_densities_plot.py
+-rw-r--r--   0        0        0      571 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     5481 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      417 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      571 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      516 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/__init__.py
+-rw-r--r--   0        0        0      483 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     7900 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/completeness_predictors/per_condition.py
+-rw-r--r--   0        0        0     8932 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     6392 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/condition.py
+-rw-r--r--   0        0        0     2437 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/n_condition/__init__.py
+-rw-r--r--   0        0        0     5285 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/n_condition/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/n_condition/estimates_densities_plot.py
+-rw-r--r--   0        0        0      439 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/n_condition/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/n_condition/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_condition/__init__.py
+-rw-r--r--   0        0        0     5484 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_condition/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_condition/estimates_densities_plot.py
+-rw-r--r--   0        0        0      439 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_condition/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_condition/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     6073 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      439 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     7222 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/completeness_predictors/per_note.py
+-rw-r--r--   0        0        0     8556 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     6418 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/note.py
+-rw-r--r--   0        0        0     2278 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/n_note/__init__.py
+-rw-r--r--   0        0        0     4866 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/n_note/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/n_note/estimates_densities_plot.py
+-rw-r--r--   0        0        0      439 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/n_note/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/n_note/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/n_note/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/n_note/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_note/__init__.py
+-rw-r--r--   0        0        0     5090 2023-07-28 18:13:08.192347 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_note/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_note/estimates_densities_plot.py
+-rw-r--r--   0        0        0      439 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_note/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_note/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_note/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_note/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     5724 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      439 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/note/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/utils/__init__.py
+-rw-r--r--   0        0        0    10772 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/utils/filter_df.py
+-rw-r--r--   0        0        0    22314 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/utils/prepare_df.py
+-rw-r--r--   0        0        0     6714 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/__init__.py
+-rw-r--r--   0        0        0      291 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     8230 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     5326 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/visit.py
+-rw-r--r--   0        0        0     1795 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/n_visit/__init__.py
+-rw-r--r--   0        0        0     4624 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/n_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/n_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      439 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/n_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/n_visit/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     4846 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      285 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      439 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      201 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      384 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      168 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/probes/visit/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/utils/__init__.py
+-rw-r--r--   0        0        0     2498 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/utils/checks.py
+-rw-r--r--   0        0        0     1155 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/utils/file_management.py
+-rw-r--r--   0        0        0     1970 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/utils/framework.py
+-rw-r--r--   0        0        0      176 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/utils/loss_functions.py
+-rw-r--r--   0        0        0      344 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/utils/typing.py
+-rw-r--r--   0        0        0       52 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/dashboards/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/dashboards/normalized_probe/__init__.py
+-rw-r--r--   0        0        0    12036 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/dashboards/normalized_probe/normalized_probe.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/dashboards/probe/__init__.py
+-rw-r--r--   0        0        0     4232 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/dashboards/probe/fitted_probe.py
+-rw-r--r--   0        0        0     3477 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/dashboards/probe/probe.py
+-rw-r--r--   0        0        0     7699 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/dashboards/probe/wrapper.py
+-rw-r--r--   0        0        0      339 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/estimates_densities/__init__.py
+-rw-r--r--   0        0        0     8901 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/estimates_densities/estimates_densities.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/normalized_probe/__init__.py
+-rw-r--r--   0        0        0     7750 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/normalized_probe/normalized_probe.py
+-rw-r--r--   0        0        0        0 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/probe/__init__.py
+-rw-r--r--   0        0        0     2334 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/probe/fitted_probe.py
+-rw-r--r--   0        0        0     1483 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/probe/probe.py
+-rw-r--r--   0        0        0     5454 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/plots/probe/wrapper.py
+-rw-r--r--   0        0        0    16579 2023-07-28 18:13:08.196348 edsteva-0.2.4/edsteva/viz/utils.py
+-rw-r--r--   0        0        0     3520 2023-07-28 18:13:08.196348 edsteva-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5759 1970-01-01 00:00:00.000000 edsteva-0.2.4/setup.py
+-rw-r--r--   0        0        0     4570 1970-01-01 00:00:00.000000 edsteva-0.2.4/PKG-INFO
```

### Comparing `edsteva-0.2.3/LICENSE` & `edsteva-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/README.md` & `edsteva-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 ```shell
 pip install edsteva
 ```
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```
-pip install edsteva==0.2.3
+pip install edsteva==0.2.4
 ```
 ## Example
 
 A scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -8,14 +8,14 @@
 https://github.com/aphp/edsteva --- EDS-TeVa provides a set of tools that aims
 at modeling the adoption over time and across space of the Electronic Health
 Records. ## Requirements EDS-TeVa stands on the shoulders of [Spark 2.4](https:
 //spark.apache.org/docs/2.4.8/index.html) which requires: - Python ~3.7.1 -
 Java 8 ## Installation You can install EDS-TeVa through ``pip``: ```shell pip
 install edsteva ``` We recommend pinning the library version in your projects,
 or use a strict package manager like [Poetry](https://python-poetry.org/). ```
-pip install edsteva==0.2.3 ``` ## Example A scientific paper is currently being
+pip install edsteva==0.2.4 ``` ## Example A scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients. ## Contributing Contributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given. ## Acknowledgement We would like to thank [Assistance
 Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation]
 (https://fondationrechercheaphp.fr/) for funding this project.
```

### Comparing `edsteva-0.2.3/edsteva/__init__.py` & `edsteva-0.2.4/edsteva/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 
 import importlib
 import os
 import sys
 import time
 from distutils.version import LooseVersion
```

### Comparing `edsteva-0.2.3/edsteva/io/files.py` & `edsteva-0.2.4/edsteva/io/files.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/io/hive.py` & `edsteva-0.2.4/edsteva/io/hive.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/io/i2b2_mapping.py` & `edsteva-0.2.4/edsteva/io/i2b2_mapping.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/io/postgres.py` & `edsteva-0.2.4/edsteva/io/postgres.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/io/settings.py` & `edsteva-0.2.4/edsteva/io/settings.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/io/synthetic/biology.py` & `edsteva-0.2.4/edsteva/io/synthetic/biology.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/io/synthetic/care_site.py` & `edsteva-0.2.4/edsteva/io/synthetic/care_site.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/io/synthetic/note.py` & `edsteva-0.2.4/edsteva/io/synthetic/note.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     note_date_col,
     id_visit_col,
     note_type_col,
     t0_visit,
 ):
     t_end = visit_care_site[date_col].max()
     t0 = generator.integers(t0_visit, t_end)
-    c_before = generator.uniform(0, 0.2)
+    c_before = generator.uniform(0, 0.01)
     c_after = generator.uniform(0.8, 1)
     note_before_t0_visit = (
         visit_care_site[visit_care_site[date_col] <= t0_visit][[id_visit_col, date_col]]
         .sample(frac=c_before)
         .rename(columns={date_col: note_date_col})
     )
     # Stratify visit between t0_visit and t0 to
```

### Comparing `edsteva-0.2.3/edsteva/io/synthetic/synthetic.py` & `edsteva-0.2.4/edsteva/io/synthetic/synthetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
         if self.mode not in ["step", "rect"]:
             raise AttributeError(
                 f"Unknown mode {self.mode}, options are ('step', 'rect')"
             )
 
     def generate(self):
         if self.seed:
+            np.random.seed(self.seed)
             self.generator = np.random.default_rng(self.seed)
         else:
             self.generator = np.random.default_rng()
 
         care_site, fact_relationship, hospital_ids = self._generate_care_site_tables()
         visit_occurrence = self._generate_visit_occurrence(hospital_ids)
         visit_detail = self._generate_visit_detail(visit_occurrence, care_site)
@@ -626,15 +627,18 @@
                 )
                 measurement = generate_bio(**params)
                 visit_care_site = visit_occurrence[
                     visit_occurrence.care_site_id == care_site_id
                 ]
                 measurement[self.id_visit_col] = (
                     visit_care_site[self.id_visit_col]
-                    .sample(n=measurement.shape[0], replace=True)
+                    .sample(
+                        n=measurement.shape[0],
+                        replace=True,
+                    )
                     .reset_index(drop=True)
                 )
                 measurement["value_as_number"] = [None] * missing_value + list(
                     self.generator.normal(
                         mean_value, std_value, measurement.shape[0] - missing_value
                     )
                 )
```

### Comparing `edsteva-0.2.3/edsteva/io/synthetic/utils.py` & `edsteva-0.2.4/edsteva/io/synthetic/utils.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/io/synthetic/visit.py` & `edsteva-0.2.4/edsteva/io/synthetic/visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/metrics/error.py` & `edsteva-0.2.4/edsteva/metrics/error.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/metrics/error_after_t0.py` & `edsteva-0.2.4/edsteva/metrics/error_after_t0.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/metrics/error_between_t0_t1.py` & `edsteva-0.2.4/edsteva/metrics/error_between_t0_t1.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/base.py` & `edsteva-0.2.4/edsteva/models/base.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/rectangle_function/algos/loss_minimization.py` & `edsteva-0.2.4/edsteva/models/rectangle_function/algos/loss_minimization.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/rectangle_function/rectangle_function.py` & `edsteva-0.2.4/edsteva/models/rectangle_function/rectangle_function.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/__init__.py` & `edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/defaults.py` & `edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,27 +65,28 @@
         value=predictor.t_1.astype(str).min(),
     )
     t_1_min_filter = alt.datum.t_1 >= t_1_selection.t_1
     return t_1_selection, t_1_min_filter
 
 
 normalized_probe_line = dict(
+    legend_title="Mean",
     encode=dict(
         strokeDash=alt.StrokeDash(
             "legend_predictor",
             title="Predictor line",
             legend=alt.Legend(
                 symbolType="stroke",
                 symbolStrokeColor="steelblue",
                 labelFontSize=12,
                 labelFontStyle="bold",
                 orient="top",
             ),
         )
-    )
+    ),
 )
 probe_line = dict(
     encode=dict(
         strokeDash=alt.StrokeDash(
             "legend_predictor",
             title="",
             legend=alt.Legend(
@@ -151,14 +152,33 @@
             max_t0="max(t_0)",
             groupby=["value", "date"],
         ),
     ],
     filters=[dict(filter=alt.datum.t_0 == alt.datum.max_t0)],
 )
 
+error_line = dict(
+    legend_title="Standard deviation",
+    mark_errorband=dict(
+        extent="stdev",
+    ),
+    encode=dict(
+        stroke=alt.Stroke(
+            "legend_error_band",
+            title="Error band",
+            legend=alt.Legend(
+                symbolType="square",
+                orient="top",
+                labelFontSize=12,
+                labelFontStyle="bold",
+            ),
+        ),
+    ),
+)
+
 horizontal_min_c0 = dict(
     x=alt.X(
         "min(c_0):Q",
         title="Min(c₀)",
     ),
     tooltip=alt.Tooltip("min(c_0):Q", format=".2"),
     sort={
```

### Comparing `edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py` & `edsteva-0.2.4/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 from edsteva.utils.typing import DataFrame
 
 from .defaults import (
+    error_line,
     get_c_0_min_selection,
     get_error_max_selection,
     get_t_0_selection,
-    get_t_1_selection,
     horizontal_max_error,
     horizontal_min_c0,
     normalized_model_line,
     normalized_probe_line,
 )
 
 
 def get_normalized_probe_dashboard_config(self, predictor: DataFrame):
     c_0_min_selection, c_0_min_filter = get_c_0_min_selection(predictor=predictor)
     t_0_selection, t_0_min_filter = get_t_0_selection(predictor=predictor)
-    t_1_selection, t_1_min_filter = get_t_1_selection(predictor=predictor)
     error_max_selection, error_max_filter = get_error_max_selection(predictor=predictor)
     return dict(
-        estimates_selections=[
-            t_0_selection,
-            t_1_selection,
-            c_0_min_selection,
-            error_max_selection,
-        ],
-        estimates_filters=[
-            t_0_min_filter,
-            t_1_min_filter,
-            c_0_min_filter,
-            error_max_filter,
-        ],
+        estimates_selections=[c_0_min_selection, t_0_selection, error_max_selection],
+        estimates_filters=[c_0_min_filter, t_0_min_filter, error_max_filter],
+        error_line=error_line,
         probe_line=normalized_probe_line,
         model_line=normalized_model_line,
         extra_horizontal_bar_charts=[horizontal_min_c0, horizontal_max_error],
         extra_vertical_bar_charts=[],
     )
```

### Comparing `edsteva-0.2.3/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py` & `edsteva-0.2.4/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from edsteva.utils.typing import DataFrame
 
 from .defaults import (
+    error_line,
     get_c_0_min_selection,
     get_error_max_selection,
     get_t_0_selection,
     get_t_1_selection,
     normalized_model_line,
     normalized_probe_line,
 )
@@ -24,10 +25,11 @@
         ],
         estimates_filters=[
             t_0_min_filter,
             t_1_min_filter,
             c_0_min_filter,
             error_max_filter,
         ],
-        probe_line=normalized_probe_line,
+        error_line=error_line,
         model_line=normalized_model_line,
+        probe_line=normalized_probe_line,
     )
```

### Comparing `edsteva-0.2.3/edsteva/models/step_function/algos/loss_minimization.py` & `edsteva-0.2.4/edsteva/models/step_function/algos/loss_minimization.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/step_function/algos/quantile.py` & `edsteva-0.2.4/edsteva/models/step_function/algos/quantile.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/step_function/step_function.py` & `edsteva-0.2.4/edsteva/models/step_function/step_function.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/step_function/viz_configs/__init__.py` & `edsteva-0.2.4/edsteva/models/step_function/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/models/step_function/viz_configs/defaults.py` & `edsteva-0.2.4/edsteva/models/step_function/viz_configs/defaults.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,28 +50,30 @@
         value=predictor.t_0.astype(str).max(),
     )
     t_0_min_filter = alt.datum.t_0 <= t_0_selection.t_0
     return t_0_selection, t_0_min_filter
 
 
 normalized_probe_line = dict(
+    legend_title="Mean",
     encode=dict(
         strokeDash=alt.StrokeDash(
             "legend_predictor",
             title="Predictor line",
             legend=alt.Legend(
                 symbolType="stroke",
                 symbolStrokeColor="steelblue",
                 labelFontSize=12,
                 labelFontStyle="bold",
                 orient="top",
             ),
         )
-    )
+    ),
 )
+
 probe_line = dict(
     encode=dict(
         strokeDash=alt.StrokeDash(
             "legend_predictor",
             title="",
             legend=alt.Legend(
                 symbolType="stroke",
@@ -79,14 +81,15 @@
                 labelFontSize=12,
                 labelFontStyle="bold",
                 orient="left",
             ),
         )
     )
 )
+
 normalized_model_line = dict(
     mark_line=dict(
         color="black",
         interpolate="step-after",
         strokeDash=[5, 5],
     ),
     encode=dict(
@@ -136,14 +139,33 @@
             max_t0="max(t_0)",
             groupby=["value", "date"],
         ),
     ],
     filters=[dict(filter=alt.datum.t_0 == alt.datum.max_t0)],
 )
 
+error_line = dict(
+    legend_title="Standard deviation",
+    mark_errorband=dict(
+        extent="stdev",
+    ),
+    encode=dict(
+        stroke=alt.Stroke(
+            "legend_error_band",
+            title="Error band",
+            legend=alt.Legend(
+                symbolType="square",
+                orient="top",
+                labelFontSize=12,
+                labelFontStyle="bold",
+            ),
+        ),
+    ),
+)
+
 horizontal_min_c0 = dict(
     x=alt.X(
         "min(c_0):Q",
         title="Min(c₀)",
     ),
     tooltip=alt.Tooltip("min(c_0):Q", format=".2"),
     sort={
```

### Comparing `edsteva-0.2.3/edsteva/models/step_function/viz_configs/normalized_probe_plot.py` & `edsteva-0.2.4/edsteva/models/step_function/viz_configs/normalized_probe_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from edsteva.utils.typing import DataFrame
 
 from .defaults import (
+    error_line,
     get_c_0_min_selection,
     get_error_max_selection,
     get_t_0_selection,
     normalized_model_line,
     normalized_probe_line,
 )
 
@@ -12,10 +13,11 @@
 def get_normalized_probe_plot_config(self, predictor: DataFrame):
     c_0_min_selection, c_0_min_filter = get_c_0_min_selection(predictor=predictor)
     t_0_selection, t_0_min_filter = get_t_0_selection(predictor=predictor)
     error_max_selection, error_max_filter = get_error_max_selection(predictor=predictor)
     return dict(
         estimates_selections=[c_0_min_selection, t_0_selection, error_max_selection],
         estimates_filters=[c_0_min_filter, t_0_min_filter, error_max_filter],
+        error_line=error_line,
         probe_line=normalized_probe_line,
         model_line=normalized_model_line,
     )
```

### Comparing `edsteva-0.2.3/edsteva/probes/base.py` & `edsteva-0.2.4/edsteva/probes/base.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/biology/biology.py` & `edsteva-0.2.4/edsteva/probes/biology/biology.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/per_measurement.py` & `edsteva-0.2.4/edsteva/probes/biology/completeness_predictors/per_measurement.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/biology/completeness_predictors/per_visit.py` & `edsteva-0.2.4/edsteva/probes/biology/completeness_predictors/per_visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/__init__.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/defaults.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,14 @@
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
```

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .defaults import (
     chart_style,
-    error_line,
     get_horizontal_bar_charts,
     normalized_main_chart,
     normalized_time_line,
     vertical_bar_charts,
 )
 
 
@@ -12,11 +11,10 @@
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
     return dict(
         chart_style=chart_style,
         main_chart=normalized_main_chart,
         time_line=normalized_time_line,
-        error_line=error_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
```

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/defaults.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,46 +100,45 @@
         ),
         dict(
             max_measurement="max(sum_measurement)",
             groupby=["value"],
         ),
     ],
     calculates=[
-        dict(completeness=alt.datum.sum_measurement / alt.datum.max_measurement),
+        dict(c=alt.datum.sum_measurement / alt.datum.max_measurement),
     ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
+            "c:Q",
             title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={"field": "n_measurement", "op": "sum", "order": "descending"},
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip("c:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
```

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .defaults import (
     chart_style,
-    error_line,
     get_horizontal_bar_charts,
     normalized_main_chart,
     normalized_time_line,
     vertical_bar_charts,
 )
 
 
@@ -12,11 +11,10 @@
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
     return dict(
         chart_style=chart_style,
         main_chart=normalized_main_chart,
         time_line=normalized_time_line,
-        error_line=error_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
```

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/defaults.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,46 +100,45 @@
         ),
         dict(
             sum_visit_with_measurement="sum(n_visit_with_measurement)",
             groupby=["value", "date"],
         ),
     ],
     calculates=[
-        dict(completeness=alt.datum.sum_visit_with_measurement / alt.datum.sum_visit),
+        dict(c=alt.datum.sum_visit_with_measurement / alt.datum.sum_visit),
     ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
+            "c:Q",
             title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={"field": "n_visit", "op": "sum", "order": "descending"},
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip("c:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
```

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .defaults import (
     chart_style,
-    error_line,
     get_horizontal_bar_charts,
     normalized_main_chart,
     normalized_time_line,
     vertical_bar_charts,
 )
 
 
@@ -12,11 +11,10 @@
     horizontal_bar_charts = get_horizontal_bar_charts(
         standard_terminologies=self._standard_terminologies.copy()
     )
     return dict(
         chart_style=chart_style,
         main_chart=normalized_main_chart,
         time_line=normalized_time_line,
-        error_line=error_line,
         vertical_bar_charts=vertical_bar_charts,
         horizontal_bar_charts=horizontal_bar_charts,
     )
```

### Comparing `edsteva-0.2.3/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py` & `edsteva-0.2.4/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/per_condition.py` & `edsteva-0.2.4/edsteva/probes/condition/completeness_predictors/per_condition.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/condition/completeness_predictors/per_visit.py` & `edsteva-0.2.4/edsteva/probes/condition/completeness_predictors/per_visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/condition/condition.py` & `edsteva-0.2.4/edsteva/probes/condition/condition.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/condition/viz_configs/__init__.py` & `edsteva-0.2.4/edsteva/probes/condition/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/condition/viz_configs/n_condition/defaults.py` & `edsteva-0.2.4/edsteva/probes/condition/viz_configs/n_condition/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
```

### Comparing `edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_condition/defaults.py` & `edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_condition/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
@@ -134,24 +133,24 @@
         ),
         dict(
             max_condition="max(sum_condition)",
             groupby=["value"],
         ),
     ],
     calculates=[
-        dict(completeness=alt.datum.sum_condition / alt.datum.max_condition),
+        dict(c=alt.datum.sum_condition / alt.datum.max_condition),
     ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
+            "c:Q",
             title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={
                 "field": "n_condition",
@@ -159,15 +158,15 @@
                 "order": "descending",
             },
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip("c:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.3/edsteva/probes/condition/viz_configs/per_visit/defaults.py` & `edsteva-0.2.4/edsteva/probes/condition/viz_configs/per_visit/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
@@ -150,24 +149,24 @@
         ),
         dict(
             sum_visit_with_condition="sum(n_visit_with_condition)",
             groupby=["value", "date"],
         ),
     ],
     calculates=[
-        dict(completeness=alt.datum.sum_visit_with_condition / alt.datum.sum_visit),
+        dict(c=alt.datum.sum_visit_with_condition / alt.datum.sum_visit),
     ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
+            "c:Q",
             title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={
                 "field": "n_visit_with_condition",
@@ -175,15 +174,15 @@
                 "order": "descending",
             },
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip("c:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.3/edsteva/probes/note/completeness_predictors/per_note.py` & `edsteva-0.2.4/edsteva/probes/note/completeness_predictors/per_note.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/note/completeness_predictors/per_visit.py` & `edsteva-0.2.4/edsteva/probes/note/completeness_predictors/per_visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/note/note.py` & `edsteva-0.2.4/edsteva/probes/note/note.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/note/viz_configs/__init__.py` & `edsteva-0.2.4/edsteva/probes/note/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/note/viz_configs/n_note/defaults.py` & `edsteva-0.2.4/edsteva/probes/note/viz_configs/n_note/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
```

### Comparing `edsteva-0.2.3/edsteva/probes/note/viz_configs/per_note/defaults.py` & `edsteva-0.2.4/edsteva/probes/note/viz_configs/per_note/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
@@ -122,24 +121,24 @@
         ),
         dict(
             max_note="max(sum_note)",
             groupby=["value"],
         ),
     ],
     calculates=[
-        dict(completeness=alt.datum.sum_note / alt.datum.max_note),
+        dict(c=alt.datum.sum_note / alt.datum.max_note),
     ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
+            "c:Q",
             title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={
                 "field": "n_note",
@@ -147,15 +146,15 @@
                 "order": "descending",
             },
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip("c:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.3/edsteva/probes/note/viz_configs/per_visit/defaults.py` & `edsteva-0.2.4/edsteva/probes/note/viz_configs/per_visit/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
@@ -138,24 +137,24 @@
         ),
         dict(
             sum_visit_with_note="sum(n_visit_with_note)",
             groupby=["value", "date"],
         ),
     ],
     calculates=[
-        dict(completeness=alt.datum.sum_visit_with_note / alt.datum.sum_visit),
+        dict(c=alt.datum.sum_visit_with_note / alt.datum.sum_visit),
     ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
+            "c:Q",
             title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={
                 "field": "n_visit_with_note",
@@ -163,15 +162,15 @@
                 "order": "descending",
             },
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip("c:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.3/edsteva/probes/utils/filter_df.py` & `edsteva-0.2.4/edsteva/probes/utils/filter_df.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/utils/prepare_df.py` & `edsteva-0.2.4/edsteva/probes/utils/prepare_df.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/utils/utils.py` & `edsteva-0.2.4/edsteva/probes/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,23 +25,25 @@
 def impute_missing_dates(
     start_date: datetime,
     end_date: datetime,
     predictor: DataFrame,
     partition_cols: List[str],
 ):
     # Generate all available dates
+    closed = "left"
     if not start_date:
         start_date = predictor["date"].min()
     if not end_date:
         end_date = predictor["date"].max()
+        closed = None
     date_index = pd.date_range(
         start=start_date,
         end=end_date,
         freq="MS",
-        closed="left",
+        closed=closed,
     )
     date_index = pd.DataFrame({"date": date_index})
 
     # Generate all available partitions
     all_partitions = (
         predictor[list(set(partition_cols) - {"date"})]
         .drop_duplicates()
```

### Comparing `edsteva-0.2.3/edsteva/probes/visit/completeness_predictors/per_visit.py` & `edsteva-0.2.4/edsteva/probes/visit/completeness_predictors/per_visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/visit/visit.py` & `edsteva-0.2.4/edsteva/probes/visit/visit.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/visit/viz_configs/__init__.py` & `edsteva-0.2.4/edsteva/probes/visit/viz_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/probes/visit/viz_configs/n_visit/defaults.py` & `edsteva-0.2.4/edsteva/probes/visit/viz_configs/n_visit/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
```

### Comparing `edsteva-0.2.3/edsteva/probes/visit/viz_configs/per_visit/defaults.py` & `edsteva-0.2.4/edsteva/probes/visit/viz_configs/per_visit/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
                 "order": "descending",
             },
         ),
     ],
 )
 
 normalized_main_chart = dict(
-    legend_title="Mean",
     encode=dict(
         x=alt.X(
             "normalized_date:Q",
             title="Δt = (t - t₀) months",
             scale=alt.Scale(nice=False),
         ),
         y=alt.Y(
@@ -112,36 +111,36 @@
         ),
         dict(
             max_visit="max(sum_visit)",
             groupby=["value"],
         ),
     ],
     calculates=[
-        dict(completeness=alt.datum.sum_visit / alt.datum.max_visit),
+        dict(c=alt.datum.sum_visit / alt.datum.max_visit),
     ],
     encode=dict(
         x=alt.X(
             "yearmonth(date):T",
             title="Time (Month Year)",
             axis=alt.Axis(tickCount="month", labelAngle=0, grid=True),
         ),
         y=alt.Y(
-            "completeness:Q",
+            "c:Q",
             title="Completeness predictor c(t)",
             axis=alt.Axis(grid=True),
         ),
         color=alt.Color(
             "value:N",
             sort={"field": "n_visit", "op": "sum", "order": "descending"},
             title=None,
         ),
         tooltip=[
             alt.Tooltip("value:N", title="Index"),
             alt.Tooltip("yearmonth(date):T", title="Date"),
-            alt.Tooltip("completeness:Q", title="c(t)", format=".2f"),
+            alt.Tooltip("c:Q", title="c(t)", format=".2f"),
         ],
     ),
     properties=dict(
         height=300,
         width=900,
     ),
 )
```

### Comparing `edsteva-0.2.3/edsteva/utils/checks.py` & `edsteva-0.2.4/edsteva/utils/checks.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/utils/file_management.py` & `edsteva-0.2.4/edsteva/utils/file_management.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/utils/framework.py` & `edsteva-0.2.4/edsteva/utils/framework.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/viz/dashboards/normalized_probe/normalized_probe.py` & `edsteva-0.2.4/edsteva/viz/dashboards/normalized_probe/normalized_probe.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from edsteva.probes.utils.utils import CARE_SITE_LEVEL_NAMES
 from edsteva.viz.utils import (
     add_estimates_filters,
     add_interactive_selection,
     concatenate_charts,
     configure_style,
     create_groupby_selection,
-    filter_predictor,
+    filter_data,
     generate_error_line,
     generate_horizontal_bar_charts,
     generate_main_chart,
     generate_model_line,
     generate_probe_line,
     generate_time_line,
     generate_vertical_bar_charts,
@@ -114,54 +114,56 @@
             predictor[estimate] = predictor[estimate].dt.strftime("%Y-%m")
     predictor["normalized_c"] = predictor["c"].where(
         (predictor["normalized_date"] < 0) | (predictor["c_0"] == 0),
         predictor["c"] / predictor["c_0"],
     )
     predictor["model"] = 1
     predictor["model"] = predictor["model"].where(predictor["normalized_date"] >= 0, 0)
-    predictor["legend_model"] = type(fitted_model).__name__
-    predictor = filter_predictor(
-        predictor=predictor, care_site_level=care_site_level, **kwargs
-    )
+    predictor = filter_data(data=predictor, care_site_level=care_site_level, **kwargs)
 
     # Get viz config
     probe_config = deepcopy(probe.get_viz_config("normalized_probe_dashboard"))
     model_config = deepcopy(
         fitted_model.get_viz_config("normalized_probe_dashboard", predictor=predictor)
     )
-    if not main_chart_config:
+    if main_chart_config is None:
         main_chart_config = probe_config["main_chart"]
-    if not time_line_config:
+    if time_line_config is None:
         time_line_config = probe_config["time_line"]
-    if not error_line_config:
-        error_line_config = probe_config["error_line"]
-    if not vertical_bar_charts_config:
+    if vertical_bar_charts_config is None:
         vertical_bar_charts_config = probe_config["vertical_bar_charts"]
         vertical_bar_charts_config["y"] = (
             vertical_bar_charts_config["y"] + model_config["extra_vertical_bar_charts"]
         )
-    if not horizontal_bar_charts_config:
+    if horizontal_bar_charts_config is None:
         horizontal_bar_charts_config = probe_config["horizontal_bar_charts"]
         horizontal_bar_charts_config["x"] = (
             horizontal_bar_charts_config["x"]
             + model_config["extra_horizontal_bar_charts"]
         )
-    if not chart_style:
+    if chart_style is None:
         chart_style = probe_config["chart_style"]
-    if not probe_line_config:
+    if probe_line_config is None:
         probe_line_config = model_config["probe_line"]
-    if not model_line_config:
+    if model_line_config is None:
         model_line_config = model_config["model_line"]
-    if not estimates_selections:
+    if error_line_config is None:
+        error_line_config = model_config["error_line"]
+    if estimates_selections is None:
         estimates_selections = model_config["estimates_selections"]
-    if not estimates_filters:
+    if estimates_filters is None:
         estimates_filters = model_config["estimates_filters"]
 
     # Viz
-    predictor["legend_predictor"] = main_chart_config["legend_title"]
+    predictor["legend_model"] = (
+        model_line_config.get("legend_title")
+        if model_line_config.get("legend_title")
+        else type(fitted_model).__name__
+    )
+    predictor["legend_predictor"] = probe_line_config["legend_title"]
     predictor["legend_error_band"] = error_line_config["legend_title"]
     base = alt.Chart(predictor)
     time_line, time_selection = generate_time_line(
         base=base,
         time_line_config=time_line_config,
     )
```

### Comparing `edsteva-0.2.3/edsteva/viz/dashboards/probe/fitted_probe.py` & `edsteva-0.2.4/edsteva/viz/dashboards/probe/fitted_probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/viz/dashboards/probe/probe.py` & `edsteva-0.2.4/edsteva/viz/dashboards/probe/probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/viz/dashboards/probe/wrapper.py` & `edsteva-0.2.4/edsteva/viz/dashboards/probe/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import altair as alt
 from IPython.display import HTML, display
 
 from edsteva.models.base import BaseModel
 from edsteva.probes.base import BaseProbe
 from edsteva.viz.dashboards.probe.fitted_probe import fitted_probe_dashboard
 from edsteva.viz.dashboards.probe.probe import probe_only_dashboard
-from edsteva.viz.utils import filter_predictor, save_html
+from edsteva.viz.utils import filter_data, save_html
 
 
 def probe_dashboard(
     probe: BaseProbe,
     fitted_model: BaseModel = None,
     care_site_level: str = None,
     save_path: str = None,
@@ -75,42 +75,42 @@
 
     alt.data_transformers.enable("default")
     alt.data_transformers.disable_max_rows()
 
     probe_config = deepcopy(probe.get_viz_config("probe_dashboard"))
     if fitted_model:
         model_config = deepcopy(fitted_model.get_viz_config("probe_dashboard"))
-        if not model_line_config:
+        if model_line_config is None:
             model_line_config = model_config["model_line"]
-        if not probe_line_config:
+        if probe_line_config is None:
             probe_line_config = model_config["probe_line"]
-    if not main_chart_config:
+    if main_chart_config is None:
         main_chart_config = probe_config["main_chart"]
-    if not time_line_config:
+    if time_line_config is None:
         time_line_config = probe_config["time_line"]
-    if not vertical_bar_charts_config:
+    if vertical_bar_charts_config is None:
         vertical_bar_charts_config = probe_config["vertical_bar_charts"]
         if fitted_model:
             vertical_bar_charts_config["y"] = (
                 vertical_bar_charts_config["y"]
                 + model_config["extra_vertical_bar_charts"]
             )
-    if not horizontal_bar_charts_config:
+    if horizontal_bar_charts_config is None:
         horizontal_bar_charts_config = probe_config["horizontal_bar_charts"]
         if fitted_model:
             horizontal_bar_charts_config["x"] = (
                 horizontal_bar_charts_config["x"]
                 + model_config["extra_horizontal_bar_charts"]
             )
-    if not chart_style:
+    if chart_style is None:
         chart_style = probe_config["chart_style"]
 
     predictor = fitted_model.predict(probe) if fitted_model else probe.predictor.copy()
-    predictor = filter_predictor(
-        predictor=predictor,
+    predictor = filter_data(
+        data=predictor,
         care_site_level=care_site_level,
         **kwargs,
     )
 
     if fitted_model:
         chart = fitted_probe_dashboard(
             predictor=predictor,
```

### Comparing `edsteva-0.2.3/edsteva/viz/plots/estimates_densities/estimates_densities.py` & `edsteva-0.2.4/edsteva/viz/plots/estimates_densities/estimates_densities.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 from edsteva.models import BaseModel
 from edsteva.probes import BaseProbe
 from edsteva.viz.utils import (
     add_interactive_selection,
     concatenate_charts,
     configure_style,
-    filter_predictor,
+    filter_data,
     generate_horizontal_bar_charts,
     generate_vertical_bar_charts,
     save_html,
 )
 
 
 def estimates_densities_plot(
-    probe: BaseProbe,
     fitted_model: BaseModel,
+    probe: BaseProbe = None,
     care_site_level: str = None,
     stay_type: List[str] = None,
     care_site_id: List[int] = None,
     start_date: Union[datetime, str] = None,
     end_date: Union[datetime, str] = None,
     care_site_short_name: List[int] = None,
     save_path: str = None,
@@ -66,39 +66,44 @@
         Configuration used to configure the chart style.
         **EXAMPLE**: `{"labelFontSize": 13, "titleFontSize": 14}`
     y_axis_title: str, optional,
         Label name for the y axis.
     """
     alt.data_transformers.disable_max_rows()
 
-    predictor = probe.predictor.copy()
-    predictor = filter_predictor(
-        predictor=predictor,
+    estimates = fitted_model.estimates.copy()
+    estimates = filter_data(
+        data=estimates,
+        table_name="estimates",
         care_site_level=care_site_level,
         stay_type=stay_type,
         care_site_id=care_site_id,
         care_site_short_name=care_site_short_name,
-        start_date=start_date,
-        end_date=end_date,
         **kwargs,
     )
-    estimates = fitted_model.estimates.copy()
-    estimates = estimates.merge(
-        predictor[
-            predictor.columns.intersection(set([*probe._index, "care_site_short_name"]))
-        ].drop_duplicates(),
-        on=list(predictor.columns.intersection(set(probe._index))),
-    )
-    probe_config = deepcopy(probe.get_viz_config("estimates_densities_plot"))
-    if not vertical_bar_charts_config:
-        vertical_bar_charts_config = probe_config["vertical_bar_charts"]
-    if not horizontal_bar_charts_config:
-        horizontal_bar_charts_config = probe_config["horizontal_bar_charts"]
-    if not chart_style:
-        chart_style = probe_config["chart_style"]
+    if probe is not None:
+        predictor = probe.predictor.copy()
+        # Filter data in predictor not in estimates
+        predictor = predictor.merge(
+            estimates[list(estimates.columns.intersection(set(predictor.columns)))],
+            on=list(estimates.columns.intersection(set(predictor.columns))),
+        )
+        predictor = filter_data(
+            data=predictor,
+            start_date=start_date,
+            end_date=end_date,
+        )
+        estimates = probe.add_names_columns(estimates)
+        probe_config = deepcopy(probe.get_viz_config("estimates_densities_plot"))
+        if vertical_bar_charts_config is None:
+            vertical_bar_charts_config = probe_config["vertical_bar_charts"]
+        if horizontal_bar_charts_config is None:
+            horizontal_bar_charts_config = probe_config["horizontal_bar_charts"]
+        if chart_style is None:
+            chart_style = probe_config["chart_style"]
 
     quantitative_estimates = []
     time_estimates = []
 
     base_estimate = alt.Chart(estimates)
     for estimate in fitted_model._coefs + fitted_model._metrics:
         if estimates[estimate].dtype == float or estimates[estimate].dtype == int:
@@ -178,52 +183,54 @@
         options=estimates["care_site_level"].unique(), name="Care site level : "
     )
     care_site_level_selection = alt.selection_point(
         fields=["care_site_level"],
         bind=care_site_level_dropdwon,
         value=estimates["care_site_level"].unique()[0],
     )
-    main_chart = reduce(
+    chart = reduce(
         lambda estimate_density_1, estimate_density_2: estimate_density_1
         & estimate_density_2,
         estimates_densities,
     )
-    base = alt.Chart(predictor).add_params(care_site_level_selection)
+    if probe is not None:
+        base = alt.Chart(predictor).add_params(care_site_level_selection)
 
-    horizontal_bar_charts, y_variables_selections = generate_horizontal_bar_charts(
-        base=base,
-        horizontal_bar_charts_config=horizontal_bar_charts_config,
-        predictor=predictor,
-    )
-    vertical_bar_charts, x_variables_selections = generate_vertical_bar_charts(
-        base=base,
-        vertical_bar_charts_config=vertical_bar_charts_config,
-        predictor=predictor,
-    )
+        horizontal_bar_charts, y_variables_selections = generate_horizontal_bar_charts(
+            base=base,
+            horizontal_bar_charts_config=horizontal_bar_charts_config,
+            predictor=predictor,
+        )
+        vertical_bar_charts, x_variables_selections = generate_vertical_bar_charts(
+            base=base,
+            vertical_bar_charts_config=vertical_bar_charts_config,
+            predictor=predictor,
+        )
 
-    selections = dict(
-        y_variables_selections,
-        **x_variables_selections,
-        **dict(cares_site_level=care_site_level_selection),
-    )
-    selection_charts = dict(
-        horizontal_bar_charts,
-        **vertical_bar_charts,
-    )
-    main_chart = add_interactive_selection(
-        base=main_chart, selection_charts=selection_charts, selections=selections
-    )
+        selections = dict(
+            y_variables_selections,
+            **x_variables_selections,
+            **dict(cares_site_level=care_site_level_selection),
+        )
+        selection_charts = dict(
+            horizontal_bar_charts,
+            **vertical_bar_charts,
+        )
+        chart = add_interactive_selection(
+            base=chart, selection_charts=selection_charts, selections=selections
+        )
 
-    chart = concatenate_charts(
-        main_chart=main_chart,
-        horizontal_bar_charts=horizontal_bar_charts,
-        vertical_bar_charts=vertical_bar_charts,
-        spacing=0,
-    )
-    chart = configure_style(chart=chart, chart_style=chart_style)
+        chart = concatenate_charts(
+            main_chart=chart,
+            horizontal_bar_charts=horizontal_bar_charts,
+            vertical_bar_charts=vertical_bar_charts,
+            spacing=0,
+        )
+    if chart_style:
+        chart = configure_style(chart=chart, chart_style=chart_style)
     if save_path:
         save_html(
             obj=chart,
             filename=save_path,
         )
 
     return chart
```

### Comparing `edsteva-0.2.3/edsteva/viz/plots/normalized_probe/normalized_probe.py` & `edsteva-0.2.4/edsteva/viz/plots/normalized_probe/normalized_probe.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from edsteva.models.base import BaseModel
 from edsteva.probes.base import BaseProbe
 from edsteva.viz.utils import (
     add_estimates_filters,
     configure_style,
     create_groupby_selection,
-    filter_predictor,
+    filter_data,
     generate_error_line,
     generate_main_chart,
     generate_model_line,
     generate_probe_line,
     get_indexes_to_groupby,
     month_diff,
     save_html,
@@ -119,17 +119,16 @@
             predictor[estimate] = predictor[estimate].dt.strftime("%Y-%m")
     predictor["normalized_c"] = predictor["c"].where(
         (predictor["normalized_date"] < 0) | (predictor["c_0"] == 0),
         predictor["c"] / predictor["c_0"],
     )
     predictor["model"] = 1
     predictor["model"] = predictor["model"].where(predictor["normalized_date"] >= 0, 0)
-    predictor["legend_model"] = type(fitted_model).__name__
-    predictor = filter_predictor(
-        predictor=predictor,
+    predictor = filter_data(
+        data=predictor,
         care_site_level=care_site_level,
         stay_type=stay_type,
         care_site_id=care_site_id,
         care_site_short_name=care_site_short_name,
         start_date=start_date,
         end_date=end_date,
         **kwargs,
@@ -140,31 +139,36 @@
         predictor = predictor[predictor.normalized_date <= t_max]
 
     # Get viz config
     probe_config = deepcopy(probe.get_viz_config("normalized_probe_plot"))
     model_config = deepcopy(
         fitted_model.get_viz_config("normalized_probe_plot", predictor=predictor)
     )
-    if not probe_line_config:
+    if probe_line_config is None:
         probe_line_config = model_config["probe_line"]
-    if not model_line_config:
+    if model_line_config is None:
         model_line_config = model_config["model_line"]
-    if not estimates_selections:
+    if error_line_config is None:
+        error_line_config = model_config["error_line"]
+    if estimates_selections is None:
         estimates_selections = model_config["estimates_selections"]
-    if not estimates_filters:
+    if estimates_filters is None:
         estimates_filters = model_config["estimates_filters"]
-    if not main_chart_config:
+    if main_chart_config is None:
         main_chart_config = probe_config["main_chart"]
-    if not error_line_config:
-        error_line_config = probe_config["error_line"]
-    if not chart_style:
+    if chart_style is None:
         chart_style = probe_config["chart_style"]
 
     # Viz
-    predictor["legend_predictor"] = main_chart_config["legend_title"]
+    predictor["legend_model"] = (
+        model_line_config.get("legend_title")
+        if model_line_config.get("legend_title")
+        else type(fitted_model).__name__
+    )
+    predictor["legend_predictor"] = probe_line_config["legend_title"]
     predictor["legend_error_band"] = error_line_config["legend_title"]
     index_selection, index_fields = create_groupby_selection(
         indexes=indexes,
         predictor=predictor,
     )
     base = alt.Chart(predictor)
     base = add_estimates_filters(
```

### Comparing `edsteva-0.2.3/edsteva/viz/plots/probe/fitted_probe.py` & `edsteva-0.2.4/edsteva/viz/plots/probe/fitted_probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/viz/plots/probe/probe.py` & `edsteva-0.2.4/edsteva/viz/plots/probe/probe.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.2.3/edsteva/viz/plots/probe/wrapper.py` & `edsteva-0.2.4/edsteva/viz/plots/probe/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import altair as alt
 
 from edsteva.models.base import BaseModel
 from edsteva.probes.base import BaseProbe
 from edsteva.viz.plots.probe.fitted_probe import fitted_probe_line
 from edsteva.viz.plots.probe.probe import probe_line
-from edsteva.viz.utils import configure_style, filter_predictor, save_html
+from edsteva.viz.utils import configure_style, filter_data, save_html
 
 
 def probe_plot(
     probe: BaseProbe,
     fitted_model: BaseModel = None,
     care_site_level: str = None,
     stay_type: List[str] = None,
@@ -77,31 +77,31 @@
     indexes_to_remove: List[str], optional
         indexes to remove from the groupby selection.
     """
     alt.data_transformers.enable("default")
     alt.data_transformers.disable_max_rows()
 
     probe_config = deepcopy(probe.get_viz_config("probe_plot"))
-    if not main_chart_config:
+    if main_chart_config is None:
         main_chart_config = probe_config["main_chart"]
-    if not chart_style:
+    if chart_style is None:
         chart_style = probe_config["chart_style"]
     predictor = probe.predictor.copy()
     cols_to_remove = ["date", *probe._metrics]
     if indexes_to_remove:
         cols_to_remove.extend(indexes_to_remove)
     indexes = list(set(predictor.columns).difference(cols_to_remove))
 
     if fitted_model:
         predictor = fitted_model.predict(probe).copy()
     else:
         predictor = probe.predictor.copy()
 
-    predictor = filter_predictor(
-        predictor=predictor,
+    predictor = filter_data(
+        data=predictor,
         care_site_level=care_site_level,
         stay_type=stay_type,
         care_site_id=care_site_id,
         care_site_short_name=care_site_short_name,
         start_date=start_date,
         end_date=end_date,
         **kwargs,
@@ -111,17 +111,17 @@
         {"field": variable, "title": variable.replace("_", " ").capitalize()}
         for variable in indexes
         if variable in predictor.columns and len(predictor[variable].unique()) >= 2
     ]
 
     if fitted_model:
         model_config = deepcopy(fitted_model.get_viz_config("probe_plot"))
-        if not model_line_config:
+        if model_line_config is None:
             model_line_config = model_config["model_line"]
-        if not probe_line_config:
+        if probe_line_config is None:
             probe_line_config = model_config["probe_line"]
         chart = fitted_probe_line(
             predictor=predictor,
             indexes=indexes,
             legend_predictor=legend_predictor,
             legend_model=legend_model,
             x_axis_title=x_axis_title,
```

### Comparing `edsteva-0.2.3/edsteva/viz/utils.py` & `edsteva-0.2.4/edsteva/viz/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -394,97 +394,105 @@
 
 def scale_it(x: float):
     if x == 0:
         return 1
     return 10 ** ceil(log10(x))
 
 
-def filter_predictor(
-    predictor: pd.DataFrame,
+def filter_data(
+    data: pd.DataFrame,
+    table_name: str = "predictor",
     care_site_level: str = None,
     stay_type: List[str] = None,
     care_site_id: List[int] = None,
     care_site_short_name: List[int] = None,
     start_date: Union[datetime, str] = None,
     end_date: Union[datetime, str] = None,
     **kwargs
 ):
     # Time
-    predictor = filter_table_by_date(
-        table=predictor,
-        table_name="predictor",
-        start_date=start_date,
-        end_date=end_date,
-    )
+    if "date" in data.columns:
+        data = filter_table_by_date(
+            table=data,
+            table_name=table_name,
+            start_date=start_date,
+            end_date=end_date,
+        )
 
     # Care site level
     if care_site_level:
         if not isinstance(care_site_level, list):
             care_site_level = [care_site_level]
         care_site_levels = []
         for care_site_lvl in care_site_level:
             if care_site_lvl in CARE_SITE_LEVEL_NAMES.keys():
                 care_site_lvl = CARE_SITE_LEVEL_NAMES[care_site_lvl]
-            if care_site_lvl not in predictor.care_site_level.unique():
+            if care_site_lvl not in data.care_site_level.unique():
                 raise AttributeError(
                     "The selected care site level {} is not part of the computed care site levels {}".format(
-                        care_site_level, list(predictor.care_site_level.unique())
+                        care_site_level, list(data.care_site_level.unique())
                     )
                 )
             care_site_levels.append(care_site_lvl)
-        predictor = predictor[predictor.care_site_level.isin(care_site_levels)]
+        data = data[data.care_site_level.isin(care_site_levels)]
         logger.debug(
-            "Predictor has been filtered on the selected care site level : {}",
+            "{} has been filtered on the selected care site level : {}",
+            table_name.capitalize(),
             care_site_levels,
         )
 
     # Stay type
     if stay_type:
         if not isinstance(stay_type, list):
             stay_type = [stay_type]
-        predictor = predictor[predictor.stay_type.isin(stay_type)]
+        data = data[data.stay_type.isin(stay_type)]
         logger.debug(
-            "Predictor has been filtered on the selected stay type : {}",
+            "{} has been filtered on the selected stay type : {}",
+            table_name.capitalize(),
             stay_type,
         )
 
     # Care site id
     if care_site_id:
         if not isinstance(care_site_id, list):
             care_site_id = [care_site_id]
-        predictor = predictor[predictor.care_site_id.isin(care_site_id)]
+        data = data[data.care_site_id.isin(care_site_id)]
         logger.debug(
-            "Predictor has been filtered on the selected care site id : {}",
+            "{} has been filtered on the selected care site id : {}",
+            table_name.capitalize(),
             care_site_id,
         )
 
     # Care site short name
     if care_site_short_name:
         if not isinstance(care_site_short_name, list):
             care_site_short_name = [care_site_short_name]
-        predictor = predictor[predictor.care_site_short_name.isin(care_site_short_name)]
+        data = data[data.care_site_short_name.isin(care_site_short_name)]
         logger.debug(
-            "Predictor has been filtered on the selected care site short name : {}",
+            "{} has been filtered on the selected care site short name : {}",
+            table_name.capitalize(),
             care_site_short_name,
         )
 
     # Others
     for key, value in kwargs.items():
         if not isinstance(value, list):
             value = [value]
-        predictor = predictor[predictor[key].isin(value)]
-        logger.debug(
-            "Predictor has been filtered on the selected {} : {}",
-            key,
-            value,
-        )
+        if key in data.columns:
+            data = data[data[key].isin(value)]
+            logger.debug(
+                "{} has been filtered on the selected {} : {}",
+                table_name.capitalize(),
+                key,
+                value,
+            )
 
     # Care site specialty
     if (
-        "care_site_specialty" in predictor.columns
-        and predictor[~(predictor.care_site_specialty == "Non renseigné")].empty
+        "care_site_specialty" in data.columns
+        and data[~(data.care_site_specialty == "Non renseigné")].empty
     ):
-        predictor = predictor.drop(columns="care_site_specialty")
+        data = data.drop(columns="care_site_specialty")
 
-    if predictor.empty:
-        raise TypeError("Empty predictor: no data to plot.")
-    return predictor
+    if data.empty:
+        raise TypeError("Empty {}: no data to plot.".format(table_name))
+    return data
```

### Comparing `edsteva-0.2.3/pyproject.toml` & `edsteva-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edsteva"
-version = "0.2.3"
+version = "0.2.4"
 description = "EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records."
 authors = ["Adam Remaki <adam.remaki@aphp.fr>", "Vicent Maladiere <vincent.maladiere-ext@aphp.fr>", "Benoit Playe <benoit.playe@aphp.fr>", "Romain Bey <romain.bey@aphp.fr>", "Paul Bernard <paul.bernard@aphp.fr>"]
 keywords = ["OMOP", "Data Analysis", "Electronic health record"]
 readme = "README.md"
 maintainers = ["Adam Remaki <adam.remaki@aphp.fr>", "Vicent Maladiere <vincent.maladiere-ext@aphp.fr>", "Thomas Petit-Jean <thomas.petitjean@aphp.fr>", "Romain Bey <romain.bey@aphp.fr>"]
 homepage = "https://github.com/aphp/edsteva"
 repository = "https://github.com/aphp/edsteva"
@@ -43,14 +43,15 @@
 ipykernel = "^6.15.3"
 jupyterlab-rise = "0.2.0"
 jupyterlab = "^3.0.0"
 
 [tool.poetry.group.docs.dependencies]
 pypandoc = "1.7.5"
 markdown = "^3.3.4"
+mkdocs = "<1.5.0"
 mkdocs-autorefs = "0.4.1"
 mkdocs-bibtex = "^2.0.1"
 mkdocs-charts-plugin = "0.0.9"
 mkdocs-gen-files = "0.3.5"
 mkdocs-img2fig-plugin = "0.9.3"
 mkdocs-literate-nav = "0.4.1"
 mkdocs-material = "^9.0.0"
@@ -69,15 +70,15 @@
 pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 pytest-html = "^3.1.1"
 pylic = "^3.4.0"
 
 [tool.ruff]
 select = ["E", "F", "I", "W", "B", "RUF", "NPY", "PD", "ERA", "PTH", "SIM", "RET", "RSE", "T20", "PIE"]
-ignore = ["E501", "B006", "B905", "B017", "W605", "RUF001", "RUF013", "PD901", "SIM118", "RET503"]
+ignore = ["E501", "B006", "B905", "B017", "W605", "RUF001", "RUF013", "NPY002", "PD901", "SIM118", "RET503"]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".eggs",
     ".git",
     ".gitignore",
     ".ruff_cache",
     ".tox",
```

### Comparing `edsteva-0.2.3/setup.py` & `edsteva-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
  'pgpasslib>=1.1.0,<2.0.0',
  'psycopg2-binary>=2.9.3,<3.0.0',
  'pyarrow>=0.15,<0.17.0',
  'pyspark>=2.4.3,<2.5.0']
 
 setup_kwargs = {
     'name': 'edsteva',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.',
-    'long_description': '<p align="center">\n<b>DISCLAIMER: </b>EDS-TeVa is intended to be a module of <a href="https://github.com/aphp/EDS-Scikit">EDS-Scikit</a>\n</p>\n\n<div align="center">\n\n<p align="center">\n  <a href="https://aphp.github.io/edsteva/latest/"><img src="https://aphp.github.io/edsteva/latest/assets/logo/edsteva_logo_small.svg" alt="EDS-TeVa"></a>\n</p>\n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)\n\n<p align="center">\n<a href="https://aphp.github.io/edsteva/latest/" target="_blank">\n    <img src="https://img.shields.io/github/actions/workflow/status/aphp/edsteva/documentation.yaml?branch=main&label=docs&style=flat" alt="Documentation">\n</a>\n<a href="https://pypi.org/project/edsteva/" target="_blank">\n    <img src="https://img.shields.io/pypi/v/edsteva?color=blue&style=flat" alt="PyPI">\n</a>\n<a href="https://codecov.io/github/aphp/edsteva?branch=main" target="_blank">\n    <img src="https://codecov.io/github/aphp/edsteva/coverage.svg?branch=main" alt="Codecov">\n</a>\n<a href="https://github.com/psf/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n</a>\n<a href="https://python-poetry.org/" target="_blank">\n    <img src="https://img.shields.io/badge/reproducibility-poetry-blue" alt="Poetry">\n</a>\n<a href="https://www.python.org/" target="_blank">\n    <img src="https://img.shields.io/badge/python-~3.7.1-brightgreen" alt="Supported Python versions">\n</a>\n<a href="https://github.com/astral-sh/ruff" target="_blank">\n    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff">\n</a>\n</p>\n</div>\n\n**Documentation**: <a href="https://aphp.github.io/edsteva/latest/" target="_blank">https://aphp.github.io/edsteva/latest/</a>\n\n**Source Code**: <a href="https://github.com/aphp/edsteva" target="_blank">https://github.com/aphp/edsteva</a>\n\n---\n\nEDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:\n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).\n\n```\npip install edsteva==0.2.3\n```\n## Example\n\nA scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are welcome, and they are greatly appreciated! Every little bit helps, and credit will always be given.\n\n## Acknowledgement\n\nWe would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
+    'long_description': '<p align="center">\n<b>DISCLAIMER: </b>EDS-TeVa is intended to be a module of <a href="https://github.com/aphp/EDS-Scikit">EDS-Scikit</a>\n</p>\n\n<div align="center">\n\n<p align="center">\n  <a href="https://aphp.github.io/edsteva/latest/"><img src="https://aphp.github.io/edsteva/latest/assets/logo/edsteva_logo_small.svg" alt="EDS-TeVa"></a>\n</p>\n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)\n\n<p align="center">\n<a href="https://aphp.github.io/edsteva/latest/" target="_blank">\n    <img src="https://img.shields.io/github/actions/workflow/status/aphp/edsteva/documentation.yaml?branch=main&label=docs&style=flat" alt="Documentation">\n</a>\n<a href="https://pypi.org/project/edsteva/" target="_blank">\n    <img src="https://img.shields.io/pypi/v/edsteva?color=blue&style=flat" alt="PyPI">\n</a>\n<a href="https://codecov.io/github/aphp/edsteva?branch=main" target="_blank">\n    <img src="https://codecov.io/github/aphp/edsteva/coverage.svg?branch=main" alt="Codecov">\n</a>\n<a href="https://github.com/psf/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n</a>\n<a href="https://python-poetry.org/" target="_blank">\n    <img src="https://img.shields.io/badge/reproducibility-poetry-blue" alt="Poetry">\n</a>\n<a href="https://www.python.org/" target="_blank">\n    <img src="https://img.shields.io/badge/python-~3.7.1-brightgreen" alt="Supported Python versions">\n</a>\n<a href="https://github.com/astral-sh/ruff" target="_blank">\n    <img src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json" alt="Ruff">\n</a>\n</p>\n</div>\n\n**Documentation**: <a href="https://aphp.github.io/edsteva/latest/" target="_blank">https://aphp.github.io/edsteva/latest/</a>\n\n**Source Code**: <a href="https://github.com/aphp/edsteva" target="_blank">https://github.com/aphp/edsteva</a>\n\n---\n\nEDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:\n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).\n\n```\npip install edsteva==0.2.4\n```\n## Example\n\nA scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are welcome, and they are greatly appreciated! Every little bit helps, and credit will always be given.\n\n## Acknowledgement\n\nWe would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
     'author': 'Adam Remaki',
     'author_email': 'adam.remaki@aphp.fr',
     'maintainer': 'Adam Remaki',
     'maintainer_email': 'adam.remaki@aphp.fr',
     'url': 'https://github.com/aphp/edsteva',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 'edsteva.viz.dashboards.probe', 'edsteva.viz.plots',
 'edsteva.viz.plots.estimates_densities', 'edsteva.viz.plots.normalized_probe',
 'edsteva.viz.plots.probe'] package_data = \ {'': ['*']} install_requires = \
 ['altair>=5.0,<6.0', 'catalogue>=2.0.8,<3.0.0', 'ipython>=7.31.0,<8.0.0',
 'koalas>=1.8.2,<2.0.0', 'loguru==0.7.0', 'numpy<1.20.0', 'pandas>=1.3,<2.0',
 'pgpasslib>=1.1.0,<2.0.0', 'psycopg2-binary>=2.9.3,<3.0.0',
 'pyarrow>=0.15,<0.17.0', 'pyspark>=2.4.3,<2.5.0'] setup_kwargs = { 'name':
-'edsteva', 'version': '0.2.3', 'description': 'EDS-TeVa provides a set of tools
+'edsteva', 'version': '0.2.4', 'description': 'EDS-TeVa provides a set of tools
 that aims at modeling the adoption over time and across space of the Electronic
 Health Records.', 'long_description': '
        \nDISCLAIMER:EDS-TeVa is intended to be a module of EDS-Scikit\n
 \n\n
                                      \n\n
                                 \n [EDS-TeVa]\n
    \n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://
@@ -47,15 +47,15 @@
 tools that aims at modeling the adoption over time and across space of the
 Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders
 of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:
 \n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa
 through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning
 the library version in your projects, or use a strict package manager like
 [Poetry](https://python-poetry.org/).\n\n```\npip install
-edsteva==0.2.3\n```\n## Example\n\nA scientific paper is currently being
+edsteva==0.2.4\n```\n## Example\n\nA scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given.\n\n## Acknowledgement\n\nWe would like to thank
 [Assistance Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP
 Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
 'author': 'Adam Remaki', 'author_email': 'adam.remaki@aphp.fr', 'maintainer':
```

### Comparing `edsteva-0.2.3/PKG-INFO` & `edsteva-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edsteva
-Version: 0.2.3
+Version: 0.2.4
 Summary: EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.
 Home-page: https://github.com/aphp/edsteva
 License: BSD 3-Clause
 Keywords: OMOP,Data Analysis,Electronic health record
 Author: Adam Remaki
 Author-email: adam.remaki@aphp.fr
 Maintainer: Adam Remaki
@@ -92,15 +92,15 @@
 
 ```shell
 pip install edsteva
 ```
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```
-pip install edsteva==0.2.3
+pip install edsteva==0.2.4
 ```
 ## Example
 
 A scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: edsteva Version: 0.2.3 Summary: EDS-TeVa provides a
+Metadata-Version: 2.1 Name: edsteva Version: 0.2.4 Summary: EDS-TeVa provides a
 set of tools that aims at modeling the adoption over time and across space of
 the Electronic Health Records. Home-page: https://github.com/aphp/edsteva
 License: BSD 3-Clause Keywords: OMOP,Data Analysis,Electronic health record
 Author: Adam Remaki Author-email: adam.remaki@aphp.fr Maintainer: Adam Remaki
 Maintainer-email: adam.remaki@aphp.fr Requires-Python: >=3.7.1,<3.8.0
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
@@ -29,14 +29,14 @@
 https://github.com/aphp/edsteva --- EDS-TeVa provides a set of tools that aims
 at modeling the adoption over time and across space of the Electronic Health
 Records. ## Requirements EDS-TeVa stands on the shoulders of [Spark 2.4](https:
 //spark.apache.org/docs/2.4.8/index.html) which requires: - Python ~3.7.1 -
 Java 8 ## Installation You can install EDS-TeVa through ``pip``: ```shell pip
 install edsteva ``` We recommend pinning the library version in your projects,
 or use a strict package manager like [Poetry](https://python-poetry.org/). ```
-pip install edsteva==0.2.3 ``` ## Example A scientific paper is currently being
+pip install edsteva==0.2.4 ``` ## Example A scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients. ## Contributing Contributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given. ## Acknowledgement We would like to thank [Assistance
 Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation]
 (https://fondationrechercheaphp.fr/) for funding this project.
```

