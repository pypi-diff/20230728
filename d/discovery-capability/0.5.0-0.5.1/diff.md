# Comparing `tmp/discovery-capability-0.5.0.tar.gz` & `tmp/discovery-capability-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.5.0.tar", last modified: Thu Jul 27 20:10:14 2023, max compression
+gzip compressed data, was "discovery-capability-0.5.1.tar", last modified: Thu Jul 27 22:07:54 2023, max compression
```

## Comparing `discovery-capability-0.5.0.tar` & `discovery-capability-0.5.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.089218 discovery-capability-0.5.0/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.0/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.0/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 20:10:14.089477 discovery-capability-0.5.0/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.0/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.914532 discovery-capability-0.5.0/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-27 20:10:13.000000 discovery-capability-0.5.0/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.914960 discovery-capability-0.5.0/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-27 16:53:34.000000 discovery-capability-0.5.0/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.918783 discovery-capability-0.5.0/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.0/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14475 2023-07-27 16:49:58.000000 discovery-capability-0.5.0/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.0/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)    10419 2023-07-27 18:38:24.000000 discovery-capability-0.5.0/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.0/ds_capability/components/feature_build.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.919791 discovery-capability-0.5.0/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.0/ds_capability/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.923784 discovery-capability-0.5.0/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.0/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.0/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.0/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.5.0/ds_capability/intent/feature_build_correlate_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    67984 2023-07-27 20:04:19.000000 discovery-capability-0.5.0/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.5.0/ds_capability/intent/feature_build_model_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:13.927507 discovery-capability-0.5.0/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.0/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.0/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.0/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.0/ds_capability/managers/feature_select_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.081872 discovery-capability-0.5.0/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.0/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.0/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-27 20:10:14.090286 discovery-capability-0.5.0/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.0/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.082897 discovery-capability-0.5.0/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.0/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.084371 discovery-capability-0.5.0/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.0/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2986 2023-07-27 16:26:58.000000 discovery-capability-0.5.0/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.0/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.085205 discovery-capability-0.5.0/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.0/test/handlers/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 20:10:14.088155 discovery-capability-0.5.0/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.0/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.0/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.0/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-27 20:05:03.000000 discovery-capability-0.5.0/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.0/test/intent/fb_model_intent_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.476600 discovery-capability-0.5.1/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.5.1/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.5.1/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 22:07:54.476837 discovery-capability-0.5.1/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.5.1/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.311444 discovery-capability-0.5.1/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     2313 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)      103 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-07-27 22:07:54.000000 discovery-capability-0.5.1/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.311968 discovery-capability-0.5.1/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      175 2023-07-27 20:11:45.000000 discovery-capability-0.5.1/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.314744 discovery-capability-0.5.1/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.5.1/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14475 2023-07-27 16:49:58.000000 discovery-capability-0.5.1/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3007 2023-07-27 15:44:19.000000 discovery-capability-0.5.1/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    10567 2023-07-27 21:55:26.000000 discovery-capability-0.5.1/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7120 2023-07-06 13:21:32.000000 discovery-capability-0.5.1/ds_capability/components/feature_build.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.315818 discovery-capability-0.5.1/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.5.1/ds_capability/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.320032 discovery-capability-0.5.1/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.5.1/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11404 2023-07-17 00:09:46.000000 discovery-capability-0.5.1/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5952 2023-07-01 22:05:04.000000 discovery-capability-0.5.1/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7128 2023-07-03 22:57:08.000000 discovery-capability-0.5.1/ds_capability/intent/feature_build_correlate_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    68036 2023-07-27 21:19:07.000000 discovery-capability-0.5.1/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15830 2023-07-21 22:27:17.000000 discovery-capability-0.5.1/ds_capability/intent/feature_build_model_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.323302 discovery-capability-0.5.1/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.5.1/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.5.1/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      871 2023-07-01 21:40:07.000000 discovery-capability-0.5.1/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3965 2023-07-01 21:40:07.000000 discovery-capability-0.5.1/ds_capability/managers/feature_select_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.464525 discovery-capability-0.5.1/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.5.1/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25756 2023-06-29 15:03:02.000000 discovery-capability-0.5.1/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-07-27 22:07:54.477535 discovery-capability-0.5.1/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2289 2023-07-03 16:47:21.000000 discovery-capability-0.5.1/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.468546 discovery-capability-0.5.1/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.5.1/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.470077 discovery-capability-0.5.1/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.5.1/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3000 2023-07-27 21:49:45.000000 discovery-capability-0.5.1/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2149 2023-07-01 22:50:31.000000 discovery-capability-0.5.1/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.471174 discovery-capability-0.5.1/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.5.1/test/handlers/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-27 22:07:54.475674 discovery-capability-0.5.1/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.5.1/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4991 2023-07-19 16:13:04.000000 discovery-capability-0.5.1/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14582 2023-07-06 13:56:21.000000 discovery-capability-0.5.1/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2920 2023-07-27 20:05:03.000000 discovery-capability-0.5.1/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11610 2023-07-23 23:20:52.000000 discovery-capability-0.5.1/test/intent/fb_model_intent_test.py
```

### Comparing `discovery-capability-0.5.0/LICENSE.txt` & `discovery-capability-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/PKG-INFO` & `discovery-capability-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.0
+Version: 0.5.1
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.0/README.rst` & `discovery-capability-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.5.1/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.5.0
+Version: 0.5.1
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.5.0/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.5.1/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.5.1/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/components/commons.py` & `discovery-capability-0.5.1/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/components/discovery.py` & `discovery-capability-0.5.1/ds_capability/components/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,25 +107,28 @@
 
         :param canonical: The canonical to interpret
         :param table_cast: attempt to cast columns to the content
         :param display_width: the width of the display
         :param stylise: if the output is stylised for jupyter display
         :return: a pa.Table or stylised pandas
         """
-        display_width = display_width if isinstance(display_width, int) else 80
+        display_width = display_width if isinstance(display_width, int) else 50
         stylise = stylise if isinstance(stylise, bool) else False
         record = []
         labels = [f'Attributes', 'DataType', 'Nulls', 'Dominate', 'Valid', 'Unique', 'Observations']
         # attempt cast
         if isinstance(table_cast, bool) and table_cast:
             canonical = Commons.table_cast(canonical)
         for c in canonical.column_names:
             column = canonical.column(c).combine_chunks()
             if pa.types.is_nested(column.type):
-                record.append([c,'nested',0,0,0,0,''])
+                s = str(column.slice(0,20).to_pylist())
+                if len(s) > display_width:
+                    s = s[:display_width] + "..."
+                record.append([c,'nested',0,0,1,1,s])
                 continue
             # data type
             line = [c,
                     'category' if pc.starts_with(str(column.type), 'dict').as_py() else str(column.type),
                     # null percentage
                     round(column.null_count / canonical.num_rows, 3)]
             # dominant percentage
```

### Comparing `discovery-capability-0.5.0/ds_capability/components/feature_build.py` & `discovery-capability-0.5.1/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.5.1/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/intent/common_intent.py` & `discovery-capability-0.5.1/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/intent/feature_build_correlate_intent.py` & `discovery-capability-0.5.1/ds_capability/intent/feature_build_correlate_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.5.1/ds_capability/intent/feature_build_intent.py`

 * *Files 0% similar despite different names*

```diff
@@ -908,17 +908,14 @@
         # date
         _ = self.get_datetime(start='2022-12-01', until='2023-03-31', ordered=True, size=size, seed=seed,
                               column_name='date', save_intent=False)
         canonical = Commons.table_append(canonical, _)
         # string
         _ = self.get_sample(sample_name='us_street_names', size=size, seed=seed, column_name='string',  save_intent=False)
         canonical = Commons.table_append(canonical, _)
-        # binary
-        _ = self.get_string_pattern(pattern='cccccccc', as_binary=True, size=size, seed=seed, column_name='binary', save_intent=False)
-        canonical = Commons.table_append(canonical, _)
 
         if isinstance(inc_nulls, bool) and inc_nulls:
             gen = np.random.default_rng()
             # cat_null
             prob_nulls = (gen.integers(1, 10, 1) * 0.001)[0] + prob_nulls
             _ = self.get_category(selection=['M', 'F', 'U'], relative_freq=[9,8,4], quantity=1 - prob_nulls,
                                   column_name='cat_null', size=size, seed=seed, save_intent=False)
@@ -956,14 +953,18 @@
             canonical = Commons.table_append(canonical, _)
             # nulls_str
             _ = pa.table([pa.array(pa.nulls(size), pa.string())], names=['nulls_str'])
             canonical = Commons.table_append(canonical, _)
             # nulls
             _ = pa.table([pa.nulls(size)], names=['nulls'])
             canonical = Commons.table_append(canonical, _)
+            # binary
+            _ = self.get_string_pattern(pattern='cccccccc', as_binary=True, size=size, seed=seed, column_name='binary',
+                                        save_intent=False)
+            canonical = Commons.table_append(canonical, _)
             # list array
             _ = pa.array(list(zip(canonical.column('num').to_pylist(), canonical.column('num_null').to_pylist())))
             _ = pa.table([_], names=['nest_list'])
             canonical = Commons.table_append(canonical, _)
             # struct array
             shuffle_int = pa.Array.from_pandas(canonical.column('int').to_pandas().sample(frac=1))
             shuffle_num = pa.Array.from_pandas(canonical.column('num').to_pandas().sample(frac=1))
```

### Comparing `discovery-capability-0.5.0/ds_capability/intent/feature_build_model_intent.py` & `discovery-capability-0.5.1/ds_capability/intent/feature_build_model_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.5.1/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.5.1/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.5.1/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.5.1/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.5.1/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.5.1/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.5.1/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.5.1/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.5.1/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.5.1/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.5.1/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.5.1/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.5.1/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.5.1/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.5.1/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/ds_capability/sample/sample_data.py` & `discovery-capability-0.5.1/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/setup.py` & `discovery-capability-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/test/component/discovery_test.py` & `discovery-capability-0.5.1/test/component/discovery_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         self.assertEqual(1_000, tbl.num_rows)
         self.assertEqual(17, tbl.num_columns)
 
     def test_data_dictionary(self):
         sb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = sb.tools
         tbl = tools.get_synthetic_data_types(1000, inc_nulls=True)
-        result = DataDiscovery.data_dictionary(tbl)
-        print(result.column_names)
+        result = DataDiscovery.data_dictionary(tbl, stylise=True)
+        pprint(result.to_string())
 
     def test_data_quality(self):
         sb = FeatureBuild.from_memory()
         tools: FeatureBuildIntentModel = sb.tools
         tbl = tools.get_synthetic_data_types(1000, inc_nulls=True)
         result = DataDiscovery.data_quality(tbl)
         print(result.column_names)
```

### Comparing `discovery-capability-0.5.0/test/component/synthetic_test.py` & `discovery-capability-0.5.1/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.5.1/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.5.1/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/test/intent/fb_intent_test.py` & `discovery-capability-0.5.1/test/intent/fb_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.5.0/test/intent/fb_model_intent_test.py` & `discovery-capability-0.5.1/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

