# Comparing `tmp/profcomff_parse_lib-2023.7.20.1.tar.gz` & `tmp/profcomff_parse_lib-2023.7.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profcomff_parse_lib-2023.7.20.1.tar", last modified: Thu Jul 20 14:24:03 2023, max compression
+gzip compressed data, was "profcomff_parse_lib-2023.7.28.tar", last modified: Fri Jul 28 14:00:53 2023, max compression
```

## Comparing `profcomff_parse_lib-2023.7.20.1.tar` & `profcomff_parse_lib-2023.7.28.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.668391 profcomff_parse_lib-2023.7.20.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 14:24:03.668391 profcomff_parse_lib-2023.7.20.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.664391 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.664391 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/add_lessons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/delete_lessons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/id_instead_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.664391 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/calc_date.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.664391 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_teacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_timetable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/pretty_subjects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.668391 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/test_parse_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/test_parse_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/test_parse_subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/test_pretty_subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/manual_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/multiple_lessons.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/parse_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/semester_parse_timetable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.668391 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/utilities/ndim_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/utilities/urls_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.664391 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-20 14:24:03.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-20 14:24:03.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:24:03.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 14:24:03.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 14:24:03.000000 profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:24:03.668391 profcomff_parse_lib-2023.7.20.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:24:03.668391 profcomff_parse_lib-2023.7.20.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/tests/test_calc_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/tests/test_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/tests/test_manual_edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-20 14:23:49.000000 profcomff_parse_lib-2023.7.20.1/tests/test_multiple_lessons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.598977 profcomff_parse_lib-2023.7.28/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-28 14:00:53.598977 profcomff_parse_lib-2023.7.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.594977 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.594977 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/add_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/delete_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/groups_to_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/id_instead_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.594977 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/calc_date.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.594977 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_teacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_timetable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/pretty_subjects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.594977 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/test_parse_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/test_parse_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/test_parse_subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/test_pretty_subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/manual_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/multiple_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/parse_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/semester_parse_timetable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.598977 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/utilities/ndim_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib/utilities/urls_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.594977 profcomff_parse_lib-2023.7.28/profcomff_parse_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-28 14:00:53.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-28 14:00:53.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 14:00:53.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 14:00:53.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 14:00:53.000000 profcomff_parse_lib-2023.7.28/profcomff_parse_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 14:00:53.598977 profcomff_parse_lib-2023.7.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:53.598977 profcomff_parse_lib-2023.7.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/tests/test_calc_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/tests/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/tests/test_manual_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-28 14:00:42.000000 profcomff_parse_lib-2023.7.28/tests/test_multiple_lessons.py
```

### Comparing `profcomff_parse_lib-2023.7.20.1/LICENSE` & `profcomff_parse_lib-2023.7.28/LICENSE`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/add_lessons.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/add_lessons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 import requests
 from requests.exceptions import RequestException
 from retrying import retry
 
-from utilities import urls_api
+from profcomff_parse_lib.utilities import urls_api
 
 _logger = logging.getLogger(__name__)
 
 
 @retry(retry_on_exception=lambda e: isinstance(e, RequestException), wait_exponential_multiplier=1000,
        wait_exponential_max=30000, stop_max_attempt_number=30)
 def upload_event(event, headers, base):
@@ -21,14 +21,14 @@
     """
     _logger.info("Загружаю пары в базу данных...")
 
     for i, row in lessons.iterrows():
         event = {
             "name": row['subject'],
             "room_id": row['place'],
-            "group_id": [row['group']],
+            "group_id": row['group'],
             "lecturer_id": row['teacher'],
             "start_ts": row['start'],
             "end_ts": row['end']
         }
         upload_event(event, headers, base)
```

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/completion.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 import pandas as pd
 import requests
 
-from utilities import urls_api
+from profcomff_parse_lib.utilities import urls_api
 
 _logger = logging.getLogger(__name__)
 
 
 def completion_lecturers(new_lecturers, headers, base):
     """
     Добавляет лекторов в базу данных, которые появляются при парсинге, но в данный момент отсутсвуют в базе.
```

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/delete_lessons.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/delete_lessons.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import logging
 
 import requests
 from requests.exceptions import RequestException
 from retrying import retry
 from datetime import timedelta
-from utilities import urls_api
+from profcomff_parse_lib.utilities import urls_api
 
 _logger = logging.getLogger(__name__)
 
 
 @retry(retry_on_exception=lambda e: isinstance(e, RequestException), wait_exponential_multiplier=1000,
        wait_exponential_max=30000, stop_max_attempt_number=30)
 def delete_lessons(headers, start, end, base):
```

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/database/id_instead_name.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/database/id_instead_name.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import sys
 
 import requests
 
-from utilities import urls_api
+from profcomff_parse_lib.utilities import urls_api
 
 _logger = logging.getLogger(__name__)
 
 
 def room_to_id(lessons, headers, base):
     """
     Превращает названия комнат в расписании в id для базы данных.
@@ -40,24 +40,26 @@
     _logger.info("Превращаю названия групп в id...")
 
     response = requests.get(urls_api.get_url_group(urls_api.MODES_URL.get, base), headers=headers)
     groups = response.json()["items"]
 
     new_groups = lessons["group"].tolist()
     for i, row in lessons.iterrows():
-        b = False
-        for group in groups:
-            if row["group"] == group["number"]:
-                new_groups[i] = group["id"]
-                b = True
-                break
-        if not b:
-            _logger.critical("Ошибка, группа '{group}' не найдена. Завершение работы".format(group=row["group"]))
-            sys.exit()
+        for j in range(len(row["group"])):
+            b = False
+            for group in groups:
+                if row["group"][j] == group["number"]:
+                    new_groups[i][j] = group["id"]
+                    b = True
+                    break
+            if not b:
+                _logger.critical("Ошибка, группа '{group}' не найдена. Завершение работы".format(group=row["group"][j]))
+                sys.exit()
     lessons["group"] = new_groups
+
     return lessons
 
 
 def teacher_to_id(lessons, headers, base):
     """
     Превращает препов в расписании в id для базы данных.
     """
```

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/calc_date.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/calc_date.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_group.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_group.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_name.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_name.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_place.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_place.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_subjects.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_subjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import re
-from utilities.ndim_iterator import NDimIterator
+from profcomff_parse_lib.utilities.ndim_iterator import NDimIterator
 
 _logger = logging.getLogger(__name__)
 
 
 def _preprocessing(subject):
     """По сути, исправление опечаток в названии пар."""
     if subject == "309, 312 - 312Д/С, 309 С/К по выбору ":
```

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_teacher.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_teacher.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/parse_timetable.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/parse_timetable.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,23 +180,20 @@
 
 
 USER_AGENT = "Mozilla/5.0 (Linux; Android 7.0; SM-G930V Build/NRD90M) AppleWebKit/537.36 " \
              "(KHTML, like Gecko) Chrome/59.0.3071.125 Mobile Safari/537.36"
 HEADERS = {"User-Agent": USER_AGENT}
 
 
-def parse_timetable(course: int, stream: int, group: int):
+def parse_timetable(course: int, stream: int, group: int, conn):
     """
     Получает данные с сайта расписания.
     """
     results = pd.DataFrame()
     try:
-        # html = requests.get(f"http://ras.phys.msu.ru/table/{course}/{stream}/{group}.htm",
-        #                     headers=HEADERS).text
-        # results = pd.concat([results, pd.DataFrame(run(html))])
-        html = instead_request(course, stream, group)
+        html = instead_request(course, stream, group, conn)
         results = pd.concat([results, pd.DataFrame(run(html))])
     except Exception:
         _logger.warning(f"'{course}/{stream}/{group}' парсинг завершился ошибкой.")
         raise
 
     return results
```

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/pretty_subjects.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/pretty_subjects.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/test_parse_group.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/test_parse_group.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/test_parse_name.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/test_parse_name.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/core/tests/test_parse_subjects.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/core/tests/test_parse_subjects.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/flatten.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/flatten.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 
 import pandas as pd
 
 _logger = logging.getLogger(__name__)
 
 
-def _to_list(value):
+def flatten_to_list(value):
     if isinstance(value, list) or isinstance(value, tuple):
         result = []
         for item in value:
-            result += _to_list(item)
+            result += flatten_to_list(item)
         return result
 
     if value is None:
         return []
 
     if pd.isna(value):
         return []
@@ -23,16 +23,16 @@
 
 def flatten(lessons):
     """
     Единственное, что делает эта функция: это превращает каждый элемент из 'place' и 'teacher' в list.
     """
     _logger.info("Произвожу сглаживание...")
 
-    lessons["place"] = lessons["place"].map(_to_list)
-    lessons["teacher"] = lessons["teacher"].map(_to_list)
+    lessons["place"] = lessons["place"].map(flatten_to_list)
+    lessons["teacher"] = lessons["teacher"].map(flatten_to_list)
 
     return lessons
```

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/manual_edit.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/manual_edit.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/multiple_lessons.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/multiple_lessons.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/timetable/semester_parse_timetable.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/timetable/semester_parse_timetable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 
 import pandas as pd
 
-from timetable.core.parse_timetable import parse_timetable
+from .core.parse_timetable import parse_timetable
 
 _logger = logging.getLogger(__name__)
 
 
-def classical_parse_timetable(sources):  # sources: [[курс, поток, количество групп], ...]
+def classical_parse_timetable(sources, conn):  # sources: [[курс, поток, количество групп], ...]
     _logger.info("Начинаю парсинг сайта расписания...")
 
     results = pd.DataFrame()
     for index, source in enumerate(sources):
         for group in range(1, source[2] + 1):
-            results = pd.concat([results, parse_timetable(source[0], source[1], group)])
+            results = pd.concat([results, parse_timetable(source[0], source[1], group, conn)])
 
     return results
```

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/utilities/logger.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/utilities/ndim_iterator.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/utilities/ndim_iterator.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib/utilities/urls_api.py` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib/utilities/urls_api.py`

 * *Files identical despite different names*

### Comparing `profcomff_parse_lib-2023.7.20.1/profcomff_parse_lib.egg-info/SOURCES.txt` & `profcomff_parse_lib-2023.7.28/profcomff_parse_lib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 profcomff_parse_lib.egg-info/dependency_links.txt
 profcomff_parse_lib.egg-info/requires.txt
 profcomff_parse_lib.egg-info/top_level.txt
 profcomff_parse_lib/database/__init__.py
 profcomff_parse_lib/database/add_lessons.py
 profcomff_parse_lib/database/completion.py
 profcomff_parse_lib/database/delete_lessons.py
+profcomff_parse_lib/database/groups_to_array.py
 profcomff_parse_lib/database/id_instead_name.py
 profcomff_parse_lib/timetable/__init__.py
 profcomff_parse_lib/timetable/calc_date.py
 profcomff_parse_lib/timetable/flatten.py
 profcomff_parse_lib/timetable/manual_edit.py
 profcomff_parse_lib/timetable/multiple_lessons.py
 profcomff_parse_lib/timetable/parse_all.py
```

### Comparing `profcomff_parse_lib-2023.7.20.1/setup.py` & `profcomff_parse_lib-2023.7.28/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="profcomff_parse_lib",
-    version="2023.07.20.1",
+    version="2023.07.28",
     author="Sergey Zamyatin and Andrei Lukianov",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/preparation-timetable-data ",
     packages=find_packages(),
     install_requires=["requests", "pandas", "setuptools", "retrying", "beautifulsoup4"],
     classifiers=[
         "Programming Language :: Python :: 3.11",
     ],
-)
+)
```

### Comparing `profcomff_parse_lib-2023.7.20.1/tests/test_calc_date.py` & `profcomff_parse_lib-2023.7.28/tests/test_calc_date.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase
 
 import pandas as pd
 
-from timetable import calc_date
+from profcomff_parse_lib.timetable import calc_date
 
 
 class Test(TestCase):
     def test_calc_date(self):
         semester_begin = "09/01/2022"
         semester_end = "09/15/2022"
         df = pd.DataFrame(
```

### Comparing `profcomff_parse_lib-2023.7.20.1/tests/test_manual_edit.py` & `profcomff_parse_lib-2023.7.28/tests/test_manual_edit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase
 
 import pandas as pd
 
-from timetable.manual_edit import _delete_row
+from profcomff_parse_lib.timetable.manual_edit import _delete_row
 
 
 class Test(TestCase):
     def test__delete_row(self):
         data = pd.DataFrame({"1": [1, 1, 3, 4], "2": [3, 4, 2, 2]})
 
         new_data = _delete_row(data, {"1": 1})
```

### Comparing `profcomff_parse_lib-2023.7.20.1/tests/test_multiple_lessons.py` & `profcomff_parse_lib-2023.7.28/tests/test_multiple_lessons.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest import TestCase
 import pandas as pd
 
-from timetable.core import multiple_lessons
+from profcomff_parse_lib.timetable import multiple_lessons
 
 
 class Test(TestCase):
     def test_multiple_lessons(self):
         data = pd.DataFrame(
             {'weekday': [0, 2, 2, 1, 1],
              'group': [101, 103, 103, 107, 107],
```

