# Comparing `tmp/co2mpas_driver-1.3.3.tar.gz` & `tmp/co2mpas_driver-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "co2mpas_driver-1.3.3.tar", last modified: Mon May  8 12:10:23 2023, max compression
+gzip compressed data, was "co2mpas_driver-1.3.4.tar", last modified: Fri Jul 28 08:44:30 2023, max compression
```

## Comparing `co2mpas_driver-1.3.3.tar` & `co2mpas_driver-1.3.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.220894 co2mpas_driver-1.3.3/
--rw-rw-rw-   0        0        0     1096 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/AUTHORS.rst
--rw-rw-rw-   0        0        0    13407 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0    11983 2023-05-08 12:10:23.220390 co2mpas_driver-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0    10795 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.157581 co2mpas_driver-1.3.3/co2mpas_driver/
--rw-rw-rw-   0        0        0     2142 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/README.md
--rw-rw-rw-   0        0        0     1903 2023-05-08 08:07:10.000000 co2mpas_driver-1.3.3/co2mpas_driver/__init__.py
--rw-rw-rw-   0        0        0      104 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.189455 co2mpas_driver-1.3.3/co2mpas_driver/common/
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/__init__.py
--rw-rw-rw-   0        0        0    21259 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/defaults.py
--rw-rw-rw-   0        0        0    13600 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/functions.py
--rw-rw-rw-   0        0        0     5342 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/gear_functions.py
--rw-rw-rw-   0        0        0     3436 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/generic_co2mpas.py
--rw-rw-rw-   0        0        0     1028 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/plot_templates.py
--rw-rw-rw-   0        0        0     1870 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/reading_n_organizing.py
--rw-rw-rw-   0        0        0     1500 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/simulation_part.py
--rw-rw-rw-   0        0        0     9313 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/utils.py
--rw-rw-rw-   0        0        0    14718 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/vehicle_functions.py
--rw-rw-rw-   0        0        0     7883 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/common/vehicle_specs_class.py
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.193231 co2mpas_driver-1.3.3/co2mpas_driver/db/
--rw-rw-rw-   0        0        0    60717 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar.csv
--rw-rw-rw-   0        0        0    42723 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar_cleaned.csv
--rw-rw-rw-   0        0        0    42723 2023-04-10 21:50:10.000000 co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar_cleaned_yl.csv
--rw-rw-rw-   0        0        0      790 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/euro_segment.py
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.207205 co2mpas_driver-1.3.3/co2mpas_driver/examples/
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/Sim_Kat_for_Jaime_2.py
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/__init__.py
--rw-rw-rw-   0        0        0     1212 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/calculate_on_existing_example.py
--rw-rw-rw-   0        0        0     9263 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/mfc_post_proc_trajectory.py
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/new_test.py
--rw-rw-rw-   0        0        0     5178 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py
--rw-rw-rw-   0        0        0     2896 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_gear_shifting.py
--rw-rw-rw-   0        0        0     3398 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_light_co2mpas.py
--rw-rw-rw-   0        0        0     3961 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_simulation.py
--rw-rw-rw-   0        0        0     8119 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_varying_des_speed.py
--rw-rw-rw-   0        0        0    11012 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_varying_des_speed_yl_2.py
--rw-rw-rw-   0        0        0     2976 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_veh_specs_collection.py
--rw-rw-rw-   0        0        0     2302 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/examples/test.py
--rw-rw-rw-   0        0        0     7770 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/load.py
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.212869 co2mpas_driver-1.3.3/co2mpas_driver/model/
--rw-rw-rw-   0        0        0    41159 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/model/__init__.py
--rw-rw-rw-   0        0        0     8227 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/model/co2mpas.py
--rw-rw-rw-   0        0        0    16433 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/model/driver.py
--rw-rw-rw-   0        0        0     4983 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/co2mpas_driver/model/simulation.py
--rw-rw-rw-   0        0        0     3361 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/plot.py
--rw-rw-rw-   0        0        0     2745 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/sample_simulation.py
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.213869 co2mpas_driver-1.3.3/co2mpas_driver/template/
--rw-rw-rw-   0        0        0    15512 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/co2mpas_driver/template/sample.xlsx
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.177758 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/
--rw-rw-rw-   0        0        0    11983 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1964 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      113 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 12:10:23.000000 co2mpas_driver-1.3.3/co2mpas_driver.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-05-08 12:10:23.217870 co2mpas_driver-1.3.3/model_validation/
--rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/model_validation/__init__.py
--rw-rw-rw-   0        0        0      996 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/model_validation/test_core.py
--rw-rw-rw-   0        0        0     5659 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/model_validation/test_model.py
--rw-rw-rw-   0        0        0     1123 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.3/model_validation/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-08 12:10:23.220894 co2mpas_driver-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     3037 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.739172 co2mpas_driver-1.3.4/
+-rw-rw-rw-   0        0        0     1096 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0    13407 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    11983 2023-07-28 08:44:30.738170 co2mpas_driver-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10795 2023-07-28 08:25:56.000000 co2mpas_driver-1.3.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.669889 co2mpas_driver-1.3.4/co2mpas_driver/
+-rw-rw-rw-   0        0        0     2142 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/README.md
+-rw-rw-rw-   0        0        0     1903 2023-05-08 08:07:10.000000 co2mpas_driver-1.3.4/co2mpas_driver/__init__.py
+-rw-rw-rw-   0        0        0      104 2023-07-28 08:25:56.000000 co2mpas_driver-1.3.4/co2mpas_driver/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.703807 co2mpas_driver-1.3.4/co2mpas_driver/common/
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/__init__.py
+-rw-rw-rw-   0        0        0    21259 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/defaults.py
+-rw-rw-rw-   0        0        0    13600 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/functions.py
+-rw-rw-rw-   0        0        0     5342 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/gear_functions.py
+-rw-rw-rw-   0        0        0     3436 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/generic_co2mpas.py
+-rw-rw-rw-   0        0        0     1028 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/plot_templates.py
+-rw-rw-rw-   0        0        0     1870 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/reading_n_organizing.py
+-rw-rw-rw-   0        0        0     1500 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/simulation_part.py
+-rw-rw-rw-   0        0        0     9313 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/utils.py
+-rw-rw-rw-   0        0        0    14718 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/vehicle_functions.py
+-rw-rw-rw-   0        0        0     7883 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/common/vehicle_specs_class.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.707188 co2mpas_driver-1.3.4/co2mpas_driver/db/
+-rw-rw-rw-   0        0        0    60717 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/db/EuroSegmentCar.csv
+-rw-rw-rw-   0        0        0    42723 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/db/EuroSegmentCar_cleaned.csv
+-rw-rw-rw-   0        0        0    42723 2023-04-10 21:50:10.000000 co2mpas_driver-1.3.4/co2mpas_driver/db/EuroSegmentCar_cleaned_yl.csv
+-rw-rw-rw-   0        0        0      790 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/euro_segment.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.721783 co2mpas_driver-1.3.4/co2mpas_driver/examples/
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/Sim_Kat_for_Jaime_2.py
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/__init__.py
+-rw-rw-rw-   0        0        0     1212 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/calculate_on_existing_example.py
+-rw-rw-rw-   0        0        0     9263 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/mfc_post_proc_trajectory.py
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/new_test.py
+-rw-rw-rw-   0        0        0     5178 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py
+-rw-rw-rw-   0        0        0     2896 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_gear_shifting.py
+-rw-rw-rw-   0        0        0     3398 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_light_co2mpas.py
+-rw-rw-rw-   0        0        0     3961 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_simulation.py
+-rw-rw-rw-   0        0        0     8119 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_varying_des_speed.py
+-rw-rw-rw-   0        0        0    11018 2023-06-08 11:59:45.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_varying_des_speed_yl_2.py
+-rw-rw-rw-   0        0        0     2976 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_veh_specs_collection.py
+-rw-rw-rw-   0        0        0     2302 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/examples/test.py
+-rw-rw-rw-   0        0        0     7770 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/load.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.732093 co2mpas_driver-1.3.4/co2mpas_driver/model/
+-rw-rw-rw-   0        0        0    41159 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/model/__init__.py
+-rw-rw-rw-   0        0        0     8174 2023-07-28 07:23:24.000000 co2mpas_driver-1.3.4/co2mpas_driver/model/co2mpas.py
+-rw-rw-rw-   0        0        0    16433 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/model/driver.py
+-rw-rw-rw-   0        0        0     4983 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/co2mpas_driver/model/simulation.py
+-rw-rw-rw-   0        0        0     3361 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/plot.py
+-rw-rw-rw-   0        0        0     2745 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/sample_simulation.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.733758 co2mpas_driver-1.3.4/co2mpas_driver/template/
+-rw-rw-rw-   0        0        0    15512 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/co2mpas_driver/template/sample.xlsx
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.692685 co2mpas_driver-1.3.4/co2mpas_driver.egg-info/
+-rw-rw-rw-   0        0        0    11983 2023-07-28 08:44:30.000000 co2mpas_driver-1.3.4/co2mpas_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1964 2023-07-28 08:44:30.000000 co2mpas_driver-1.3.4/co2mpas_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 08:44:30.000000 co2mpas_driver-1.3.4/co2mpas_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-07-28 08:44:30.000000 co2mpas_driver-1.3.4/co2mpas_driver.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      113 2023-07-28 08:44:30.000000 co2mpas_driver-1.3.4/co2mpas_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-28 08:44:30.000000 co2mpas_driver-1.3.4/co2mpas_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-28 08:44:30.000000 co2mpas_driver-1.3.4/co2mpas_driver.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-28 08:44:30.737165 co2mpas_driver-1.3.4/model_validation/
+-rw-rw-rw-   0        0        0        0 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/model_validation/__init__.py
+-rw-rw-rw-   0        0        0      996 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/model_validation/test_core.py
+-rw-rw-rw-   0        0        0     5659 2023-05-08 11:51:40.000000 co2mpas_driver-1.3.4/model_validation/test_model.py
+-rw-rw-rw-   0        0        0     1123 2022-10-14 10:27:15.000000 co2mpas_driver-1.3.4/model_validation/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 08:44:30.740172 co2mpas_driver-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     3037 2023-07-28 08:41:59.000000 co2mpas_driver-1.3.4/setup.py
```

### Comparing `co2mpas_driver-1.3.3/AUTHORS.rst` & `co2mpas_driver-1.3.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/LICENSE.txt` & `co2mpas_driver-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/PKG-INFO` & `co2mpas_driver-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: co2mpas_driver
-Version: 1.3.3
+Version: 1.3.4
 Summary: A lightweight microsimulation free-flow acceleration model(MFC) or co2mpas_driver is a model that is able to capture the vehicle acceleration dynamics accurately and consistently
 License: European Union Public Licence 1.1 or later (EUPL 1.1+)
 Project-URL: Sources, https://code.europa.eu/jrc-ldv/co2mpas_driver
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -278,19 +278,19 @@
 .. _end-usage:
 
 .. _start-sub:
 
 .. |python-ver| image::  https://img.shields.io/badge/PyPi%20python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20-informational
     :alt: Supported Python versions of latest release in PyPi
 
-.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.3-orange
+.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.4-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: Latest version in GitHub
 
-.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/05/08-orange
+.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/07/28-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: release date
 
 .. |br| image:: https://img.shields.io/badge/docs-working%20on%20that-red
     :alt: GitHub page documentation
 
 .. |doc| image:: https://img.shields.io/badge/docs-passing-success
@@ -304,15 +304,15 @@
     :target: https://github.com/ambv/black
     :alt: Code Style
 
 .. |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/JRCSTU/co2mpas_driver/master?urlpath=lab/tree/examples
     :alt: JupyterLab for co2mpas_driver (stable)
 
-.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.1-informational
+.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.4-informational
     :target: https://pypi.org/project/co2mpas-driver/
     :alt: pip installation
 
 .. |JRC-image| image:: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/raw/master/doc/_static/images/co2mpas_driver_logo.png
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver
     :alt: GitLab repository
```

### Comparing `co2mpas_driver-1.3.3/README.rst` & `co2mpas_driver-1.3.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -253,19 +253,19 @@
 .. _end-usage:
 
 .. _start-sub:
 
 .. |python-ver| image::  https://img.shields.io/badge/PyPi%20python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20-informational
     :alt: Supported Python versions of latest release in PyPi
 
-.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.3-orange
+.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.4-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: Latest version in GitHub
 
-.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/05/08-orange
+.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/07/28-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: release date
 
 .. |br| image:: https://img.shields.io/badge/docs-working%20on%20that-red
     :alt: GitHub page documentation
 
 .. |doc| image:: https://img.shields.io/badge/docs-passing-success
@@ -279,15 +279,15 @@
     :target: https://github.com/ambv/black
     :alt: Code Style
 
 .. |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/JRCSTU/co2mpas_driver/master?urlpath=lab/tree/examples
     :alt: JupyterLab for co2mpas_driver (stable)
 
-.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.1-informational
+.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.4-informational
     :target: https://pypi.org/project/co2mpas-driver/
     :alt: pip installation
 
 .. |JRC-image| image:: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/raw/master/doc/_static/images/co2mpas_driver_logo.png
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver
     :alt: GitLab repository
```

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/README.md` & `co2mpas_driver-1.3.4/co2mpas_driver/README.md`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/__init__.py` & `co2mpas_driver-1.3.4/co2mpas_driver/__init__.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/defaults.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/defaults.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/functions.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/functions.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/gear_functions.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/gear_functions.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/generic_co2mpas.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/generic_co2mpas.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/plot_templates.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/plot_templates.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/reading_n_organizing.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/reading_n_organizing.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/simulation_part.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/simulation_part.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/utils.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/utils.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/vehicle_functions.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/vehicle_functions.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/common/vehicle_specs_class.py` & `co2mpas_driver-1.3.4/co2mpas_driver/common/vehicle_specs_class.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar.csv` & `co2mpas_driver-1.3.4/co2mpas_driver/db/EuroSegmentCar.csv`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar_cleaned.csv` & `co2mpas_driver-1.3.4/co2mpas_driver/db/EuroSegmentCar_cleaned.csv`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/db/EuroSegmentCar_cleaned_yl.csv` & `co2mpas_driver-1.3.4/co2mpas_driver/db/EuroSegmentCar_cleaned_yl.csv`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/euro_segment.py` & `co2mpas_driver-1.3.4/co2mpas_driver/euro_segment.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/calculate_on_existing_example.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/calculate_on_existing_example.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/mfc_post_proc_trajectory.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/mfc_post_proc_trajectory.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_acc_dec_bounds_per_gear.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_gear_shifting.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_gear_shifting.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_light_co2mpas.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_light_co2mpas.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_simulation.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_simulation.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_varying_des_speed.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_varying_des_speed.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_varying_des_speed_yl_2.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_varying_des_speed_yl_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
             final_drive_power_in,
             gear_box_power_in,
         ) = my_veh(sim_step, res["v_des"][-1])
 
         if car_id in car_id_db["electric_engine"]:
             fc = 0
         else:
-            fc, p_engine, p_motor, soc = my_veh.calculate_fuel_consumption(
+            fc, p_engine, p_motor, soc, _, _ = my_veh.calculate_fuel_consumption(
                 gear, sim_step, gear_box_speeds_in, gear_box_power_in
             )
 
         res["accel"].append(acc)
         res["speed"].append(next_velocity)
         res["gear"].append(gear)
         res["veh_wheel_torque"].append(veh_wheel_torque)
```

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/sample_veh_specs_collection.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/sample_veh_specs_collection.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/examples/test.py` & `co2mpas_driver-1.3.4/co2mpas_driver/examples/test.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/load.py` & `co2mpas_driver-1.3.4/co2mpas_driver/load.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/model/__init__.py` & `co2mpas_driver-1.3.4/co2mpas_driver/model/__init__.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/model/co2mpas.py` & `co2mpas_driver-1.3.4/co2mpas_driver/model/co2mpas.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
         return sh.NONE
     #     xp = [0, 0]; fp = [0, 0]
     # else:
     xp, fp = defaults.dfl.functions.get_full_load.FULL_LOAD[ignition_type]
     fp = np.array(fp)
     fp *= engine_max_power
     xp = np.array(xp)
-    idle = idle_engine_speed[0]
-    xp = xp * (engine_max_speed_at_max_power - idle) + idle
+    xp *= engine_max_speed_at_max_power
 
     func = functools.partial(np.interp, xp=xp, fp=fp, left=0, right=0)
 
     return func
 
 
 def calculate_full_load_speeds_and_powers(
```

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/model/driver.py` & `co2mpas_driver-1.3.4/co2mpas_driver/model/driver.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/model/simulation.py` & `co2mpas_driver-1.3.4/co2mpas_driver/model/simulation.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/plot.py` & `co2mpas_driver-1.3.4/co2mpas_driver/plot.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/sample_simulation.py` & `co2mpas_driver-1.3.4/co2mpas_driver/sample_simulation.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver/template/sample.xlsx` & `co2mpas_driver-1.3.4/co2mpas_driver/template/sample.xlsx`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver.egg-info/PKG-INFO` & `co2mpas_driver-1.3.4/co2mpas_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: co2mpas-driver
-Version: 1.3.3
+Version: 1.3.4
 Summary: A lightweight microsimulation free-flow acceleration model(MFC) or co2mpas_driver is a model that is able to capture the vehicle acceleration dynamics accurately and consistently
 License: European Union Public Licence 1.1 or later (EUPL 1.1+)
 Project-URL: Sources, https://code.europa.eu/jrc-ldv/co2mpas_driver
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -278,19 +278,19 @@
 .. _end-usage:
 
 .. _start-sub:
 
 .. |python-ver| image::  https://img.shields.io/badge/PyPi%20python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20-informational
     :alt: Supported Python versions of latest release in PyPi
 
-.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.3-orange
+.. |gh-version| image::  https://img.shields.io/badge/GitLab%20-1.3.4-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: Latest version in GitHub
 
-.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/05/08-orange
+.. |rel-date| image:: https://img.shields.io/badge/rel--date-2023/07/28-orange
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/releases
     :alt: release date
 
 .. |br| image:: https://img.shields.io/badge/docs-working%20on%20that-red
     :alt: GitHub page documentation
 
 .. |doc| image:: https://img.shields.io/badge/docs-passing-success
@@ -304,15 +304,15 @@
     :target: https://github.com/ambv/black
     :alt: Code Style
 
 .. |binder| image:: https://mybinder.org/badge_logo.svg
     :target: https://mybinder.org/v2/gh/JRCSTU/co2mpas_driver/master?urlpath=lab/tree/examples
     :alt: JupyterLab for co2mpas_driver (stable)
 
-.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.1-informational
+.. |pypi-ins| image:: https://img.shields.io/badge/pypi-v1.3.4-informational
     :target: https://pypi.org/project/co2mpas-driver/
     :alt: pip installation
 
 .. |JRC-image| image:: https://code.europa.eu/jrc-ldv/co2mpas-driver/-/raw/master/doc/_static/images/co2mpas_driver_logo.png
     :target: https://code.europa.eu/jrc-ldv/co2mpas-driver
     :alt: GitLab repository
```

### Comparing `co2mpas_driver-1.3.3/co2mpas_driver.egg-info/SOURCES.txt` & `co2mpas_driver-1.3.4/co2mpas_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/model_validation/test_core.py` & `co2mpas_driver-1.3.4/model_validation/test_core.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/model_validation/test_model.py` & `co2mpas_driver-1.3.4/model_validation/test_model.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/model_validation/utils.py` & `co2mpas_driver-1.3.4/model_validation/utils.py`

 * *Files identical despite different names*

### Comparing `co2mpas_driver-1.3.3/setup.py` & `co2mpas_driver-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     test_deps = ["pytest"]
 
     url = "https://code.europa.eu/jrc-ldv/%s" % name
 
     setup(
         name=name,
-        version="1.3.3",
+        version="1.3.4",
         packages=find_packages(
             exclude=[
                 "test",
                 "test.*",
             ]
         ),
         license="European Union Public Licence 1.1 or later (EUPL 1.1+)",
```

