# Comparing `tmp/SPPRVAL-0.0.6.tar.gz` & `tmp/spprval-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPPRVAL-0.0.6.tar", max compression
+gzip compressed data, was "spprval-0.1.0.tar", max compression
```

## Comparing `SPPRVAL-0.0.6.tar` & `spprval-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,18 @@
--rw-r--r--   0        0        0      312 2023-03-30 10:36:52.693634 SPPRVAL-0.0.6/pyproject.toml
--rw-r--r--   0        0        0       87 2023-03-30 10:31:32.385856 SPPRVAL-0.0.6/spprval/Config_of_params.csv
--rw-r--r--   0        0        0    16903 2023-03-30 10:31:32.393829 SPPRVAL-0.0.6/spprval/data/brave_work_res.csv
--rw-r--r--   0        0        0    18493 2023-03-30 10:31:32.394826 SPPRVAL-0.0.6/spprval/data_for_val/electroline_bapl_evolution_schedule.json
--rw-r--r--   0        0        0    19346 2023-03-30 10:31:32.395825 SPPRVAL-0.0.6/spprval/data_for_val/electroline_baps_heft_add_end_schedule.json
--rw-r--r--   0        0        0    16027 2023-03-30 10:31:32.395825 SPPRVAL-0.0.6/spprval/data_for_val/transform25_bapl_heft_add_end_schedule.json
--rw-r--r--   0        0        0    19648 2023-03-30 10:31:32.395825 SPPRVAL-0.0.6/spprval/data_for_val/transform25_bapl_heft_add_end_schedule1.json
--rw-r--r--   0        0        0      228 2023-03-30 10:31:32.395825 SPPRVAL-0.0.6/spprval/requirements.txt
--rw-r--r--   0        0        0  1688999 2023-03-30 10:31:32.393829 SPPRVAL-0.0.6/spprval/Tutorial.ipynb
--rw-r--r--   0        0        0     3809 2023-03-30 10:31:32.395825 SPPRVAL-0.0.6/spprval/unique_tasks_dict.csv
--rw-r--r--   0        0        0  3405235 2023-03-30 10:31:32.403796 SPPRVAL-0.0.6/spprval/val_datasets/val_data_messoyaha.csv
--rw-r--r--   0        0        0 14135724 2023-03-30 10:31:32.433907 SPPRVAL-0.0.6/spprval/val_datasets/works_messoyaha_clustered_15kdict_and_glue_work_series_less_14_day.pkl
--rw-r--r--   0        0        0       77 2023-03-30 10:31:32.434903 SPPRVAL-0.0.6/spprval/validation/__init__.py
--rw-r--r--   0        0        0    10808 2023-03-30 10:31:32.435900 SPPRVAL-0.0.6/spprval/validation/__pycache__/aggregator.cpython-39.pyc
--rw-r--r--   0        0        0    17122 2023-03-30 10:31:32.436896 SPPRVAL-0.0.6/spprval/validation/__pycache__/dataset_wrapper.cpython-39.pyc
--rw-r--r--   0        0        0     1427 2023-03-30 10:31:32.436896 SPPRVAL-0.0.6/spprval/validation/__pycache__/rendering.cpython-39.pyc
--rw-r--r--   0        0        0     9539 2023-03-30 10:31:32.435900 SPPRVAL-0.0.6/spprval/validation/__pycache__/SPPRVal.cpython-39.pyc
--rw-r--r--   0        0        0    23473 2023-03-30 10:31:32.437893 SPPRVAL-0.0.6/spprval/validation/__pycache__/validator.cpython-39.pyc
--rw-r--r--   0        0        0     5551 2023-03-30 10:31:32.438938 SPPRVAL-0.0.6/spprval/validation/aggregator.py
--rw-r--r--   0        0        0    32010 2023-03-30 10:31:32.438938 SPPRVAL-0.0.6/spprval/validation/dataset_wrapper.py
--rw-r--r--   0        0        0     1410 2023-03-30 10:31:32.438938 SPPRVAL-0.0.6/spprval/validation/rendering.py
--rw-r--r--   0        0        0    17672 2023-03-30 10:31:32.434903 SPPRVAL-0.0.6/spprval/validation/SPPRVal.py
--rw-r--r--   0        0        0    21373 2023-03-30 10:31:32.439886 SPPRVAL-0.0.6/spprval/validation/validator.py
--rw-r--r--   0        0        0      573 2023-03-30 10:36:56.822046 SPPRVAL-0.0.6/setup.py
--rw-r--r--   0        0        0      241 2023-03-30 10:36:56.822046 SPPRVAL-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-07-28 10:03:38.977083 spprval-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-28 09:19:40.313251 spprval-0.1.0/spprval/__init__.py
+-rw-r--r--   0        0        0      853 2023-07-28 09:19:40.313360 spprval-0.1.0/spprval/database/DBWrapper.py
+-rw-r--r--   0        0        0      136 2023-07-28 09:19:40.313418 spprval-0.1.0/spprval/database/DataSource.py
+-rw-r--r--   0        0        0        0 2023-07-28 09:19:40.313440 spprval-0.1.0/spprval/database/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-28 09:19:40.313531 spprval-0.1.0/spprval/dataset/BaseDataset.py
+-rw-r--r--   0        0        0     1635 2023-07-28 09:19:40.313599 spprval-0.1.0/spprval/dataset/ObjectNameProcessor.py
+-rw-r--r--   0        0        0     3240 2023-07-28 09:19:40.313662 spprval-0.1.0/spprval/dataset/PlanDataset.py
+-rw-r--r--   0        0        0     4036 2023-07-28 09:19:40.313744 spprval-0.1.0/spprval/dataset/ValidationDataset.py
+-rw-r--r--   0        0        0     3758 2023-07-28 09:19:40.313806 spprval-0.1.0/spprval/dataset/utils.py
+-rw-r--r--   0        0        0    19329 2023-07-28 09:19:40.313939 spprval-0.1.0/spprval/validation/SPPRVal.py
+-rw-r--r--   0        0        0       73 2023-07-28 09:19:40.314001 spprval-0.1.0/spprval/validation/__init__.py
+-rw-r--r--   0        0        0     8159 2023-07-28 09:19:40.314082 spprval-0.1.0/spprval/validation/aggregator.py
+-rw-r--r--   0        0        0    32603 2023-07-28 09:19:40.314272 spprval-0.1.0/spprval/validation/dataset_wrapper.py
+-rw-r--r--   0        0        0     1311 2023-07-28 09:19:40.314338 spprval-0.1.0/spprval/validation/rendering.py
+-rw-r--r--   0        0        0     4872 2023-07-28 09:19:40.314403 spprval-0.1.0/spprval/validation/stats_calculator.py
+-rw-r--r--   0        0        0    15106 2023-07-28 09:19:40.314533 spprval-0.1.0/spprval/validation/validator.py
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 spprval-0.1.0/PKG-INFO
```

