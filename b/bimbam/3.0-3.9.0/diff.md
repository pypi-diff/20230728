# Comparing `tmp/bimbam-3.0.tar.gz` & `tmp/bimbam-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimbam-3.0.tar", last modified: Thu Jul 27 21:23:26 2023, max compression
+gzip compressed data, was "bimbam-3.9.0.tar", last modified: Fri Jul 28 12:19:27 2023, max compression
```

## Comparing `bimbam-3.0.tar` & `bimbam-3.9.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.071947 bimbam-3.0/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-27 21:23:26.071947 bimbam-3.0/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.055947 bimbam-3.0/bimbam.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      664 2023-07-27 21:23:25.000000 bimbam-3.0/bimbam.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-27 21:23:26.000000 bimbam-3.0/bimbam.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-27 21:23:25.000000 bimbam-3.0/bimbam.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-27 21:23:25.000000 bimbam-3.0/bimbam.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-27 21:23:25.000000 bimbam-3.0/bimbam.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-27 21:23:26.071947 bimbam-3.0/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1961 2023-07-27 21:23:18.000000 bimbam-3.0/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.059947 bimbam-3.0/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1804 2023-07-26 19:04:33.000000 bimbam-3.0/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.059947 bimbam-3.0/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17887 2023-07-27 19:37:17.000000 bimbam-3.0/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-3.0/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-27 19:30:14.000000 bimbam-3.0/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-3.0/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7164 2023-07-27 19:31:40.000000 bimbam-3.0/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.063947 bimbam-3.0/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-3.0/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-3.0/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-3.0/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.063947 bimbam-3.0/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.067947 bimbam-3.0/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-3.0/thonnycontrib/docs/res/exception_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-3.0/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/failed_red_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-3.0/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/success_green_chip.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.067947 bimbam-3.0/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      408 2023-07-23 13:51:19.000000 bimbam-3.0/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    11803 2023-07-27 19:42:02.000000 bimbam-3.0/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-3.0/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-3.0/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-3.0/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.067947 bimbam-3.0/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-3.0/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.067947 bimbam-3.0/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-3.0/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-3.0/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-3.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-3.0/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23084 2023-07-27 21:21:22.000000 bimbam-3.0/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    39063 2023-07-27 20:38:47.000000 bimbam-3.0/thonnycontrib/l1test_frontend/l1test_treeview.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.067947 bimbam-3.0/thonnycontrib/main_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-3.0/thonnycontrib/main_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5295 2023-07-23 11:59:59.000000 bimbam-3.0/thonnycontrib/main_generator/main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5332 2023-07-23 16:18:24.000000 bimbam-3.0/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-3.0/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.071947 bimbam-3.0/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/tests/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-27 21:23:26.071947 bimbam-3.0/thonnycontrib/tests/fixtures/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-3.0/thonnycontrib/tests/fixtures/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-3.0/thonnycontrib/tests/fixtures/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-3.0/thonnycontrib/tests/fixtures/workbench_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1991 2023-07-24 19:13:49.000000 bimbam-3.0/thonnycontrib/tests/tests_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-3.0/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-3.0/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-3.0/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-3.0/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-3.0/thonnycontrib/tests/tests_main_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-3.0/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-3.0/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18025 2023-07-27 20:42:09.000000 bimbam-3.0/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.988488 bimbam-3.9.0/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      666 2023-07-28 12:19:27.988488 bimbam-3.9.0/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.976487 bimbam-3.9.0/bimbam.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      666 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2648 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-07-28 12:19:27.000000 bimbam-3.9.0/bimbam.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-07-28 12:19:27.988488 bimbam-3.9.0/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1963 2023-07-28 12:19:08.000000 bimbam-3.9.0/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.976487 bimbam-3.9.0/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1804 2023-07-26 19:04:33.000000 bimbam-3.9.0/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.980487 bimbam-3.9.0/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    17887 2023-07-27 19:37:17.000000 bimbam-3.9.0/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35564 2023-07-23 17:34:08.000000 bimbam-3.9.0/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5015 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4508 2023-07-27 19:33:34.000000 bimbam-3.9.0/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7164 2023-07-27 19:31:40.000000 bimbam-3.9.0/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.980487 bimbam-3.9.0/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2379 2023-07-22 13:45:44.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      475 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      735 2023-07-23 18:54:56.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      644 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      371 2023-07-22 11:09:20.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/PassedSetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      429 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.980487 bimbam-3.9.0/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.980487 bimbam-3.9.0/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1778 2023-07-27 18:28:42.000000 bimbam-3.9.0/thonnycontrib/docs/res/exception_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-07-27 19:02:02.000000 bimbam-3.9.0/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1647 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/failed_red_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-07-27 19:01:55.000000 bimbam-3.9.0/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1625 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/success_green_chip.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      408 2023-07-23 13:51:19.000000 bimbam-3.9.0/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    11803 2023-07-27 19:42:02.000000 bimbam-3.9.0/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7054 2023-07-22 09:12:15.000000 bimbam-3.9.0/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1058 2023-07-23 10:37:34.000000 bimbam-3.9.0/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-07-27 21:16:38.000000 bimbam-3.9.0/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2991 2023-07-23 10:41:36.000000 bimbam-3.9.0/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      754 2023-07-23 12:01:22.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2847 2023-07-20 20:39:26.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3986 2023-07-23 12:06:57.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2749 2023-07-23 16:34:32.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23084 2023-07-27 21:21:22.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    41453 2023-07-28 11:09:46.000000 bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_treeview.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/main_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-07-22 08:21:17.000000 bimbam-3.9.0/thonnycontrib/main_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5295 2023-07-23 11:59:59.000000 bimbam-3.9.0/thonnycontrib/main_generator/main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5332 2023-07-23 16:18:24.000000 bimbam-3.9.0/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2962 2023-07-27 19:06:48.000000 bimbam-3.9.0/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/tests/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-28 12:19:27.984488 bimbam-3.9.0/thonnycontrib/tests/fixtures/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-07-24 19:06:13.000000 bimbam-3.9.0/thonnycontrib/tests/fixtures/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-07-20 20:20:05.000000 bimbam-3.9.0/thonnycontrib/tests/fixtures/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1767 2023-07-22 09:17:05.000000 bimbam-3.9.0/thonnycontrib/tests/fixtures/workbench_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1991 2023-07-24 19:13:49.000000 bimbam-3.9.0/thonnycontrib/tests/tests_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5767 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16504 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    21862 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7935 2023-07-27 19:56:06.000000 bimbam-3.9.0/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2030 2023-07-26 07:37:26.000000 bimbam-3.9.0/thonnycontrib/tests/tests_main_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6202 2023-07-27 19:30:14.000000 bimbam-3.9.0/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14861 2023-07-24 19:26:54.000000 bimbam-3.9.0/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18025 2023-07-27 20:42:09.000000 bimbam-3.9.0/thonnycontrib/utils.py
```

### Comparing `bimbam-3.0/PKG-INFO` & `bimbam-3.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 3.0
+Version: 3.9.0
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-3.0/bimbam.egg-info/PKG-INFO` & `bimbam-3.9.0/bimbam.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimbam
-Version: 3.0
+Version: 3.9.0
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests
 Author: idtaleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `bimbam-3.0/bimbam.egg-info/SOURCES.txt` & `bimbam-3.9.0/bimbam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/setup.py` & `bimbam-3.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="bimbam",
-    version="3.0",
+    version="3.9.0",
     author="idtaleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests""",
     url="https://gitlab.univ-lille.fr/mirabelle.nebut/thonny-tests",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `bimbam-3.0/thonnycontrib/ThonnyLogsGenerator.py` & `bimbam-3.9.0/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/backend/ast_parser.py` & `bimbam-3.9.0/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/backend/doctest_parser.py` & `bimbam-3.9.0/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/backend/evaluator.py` & `bimbam-3.9.0/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/backend/l1test_backend.py` & `bimbam-3.9.0/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/backend/test_finder.py` & `bimbam-3.9.0/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `bimbam-3.9.0/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/backend/verdicts/FailedVerdict.py` & `bimbam-3.9.0/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `bimbam-3.9.0/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/error_icon.png` & `bimbam-3.9.0/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/exception_red_chip.png` & `bimbam-3.9.0/thonnycontrib/docs/res/exception_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/failed.png` & `bimbam-3.9.0/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/failed_red_chip.png` & `bimbam-3.9.0/thonnycontrib/docs/res/failed_red_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/l1test_icon.png` & `bimbam-3.9.0/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/l1test_icon_old.png` & `bimbam-3.9.0/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/outline_class.png` & `bimbam-3.9.0/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/outline_method.gif` & `bimbam-3.9.0/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/passed.png` & `bimbam-3.9.0/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/pending_icon.png` & `bimbam-3.9.0/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/restart_icon.png` & `bimbam-3.9.0/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/success_green_chip.png` & `bimbam-3.9.0/thonnycontrib/docs/res/success_green_chip.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docs/res/warning.png` & `bimbam-3.9.0/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docstring_generator/doc_generator.py` & `bimbam-3.9.0/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/docstring_generator/doc_template.py` & `bimbam-3.9.0/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/environement_vars.py` & `bimbam-3.9.0/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/exceptions.py` & `bimbam-3.9.0/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/l1test_configuration/l1test_options.py` & `bimbam-3.9.0/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/l1test_frontend/__init__.py` & `bimbam-3.9.0/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/l1test_frontend/l1test_error_view.py` & `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py` & `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_outliner_menu.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/l1test_frontend/l1test_reporter.py` & `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/l1test_frontend/l1test_runner.py` & `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/l1test_frontend/l1test_treeview.py` & `bimbam-3.9.0/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,16 +90,22 @@
         for color_name, color in COLORS.items():
             if color_name == "lightred":
                 self.treeview.tag_configure(color_name, background=color)
             else:
                 self.treeview.tag_configure(color_name, foreground=color)
         
         # définir un tag pour les test en exception: il faut les souligner (underline)
-        self.treeview.tag_configure("underline", font=tk_font.Font(underline=True))
-        
+        self.treeview.tag_configure("exception_as_link", foreground=COLORS["red"], 
+                                    font=tk_font.Font(underline=True, weight="normal", family=get_font_family_option(), size=get_font_size_option()))
+        self.treeview.tag_configure("exception_hovered", foreground=COLORS["red"], 
+                                    font=tk_font.Font(underline=True, 
+                                                    weight="bold", 
+                                                    family=get_font_family_option(), 
+                                                    size=get_font_size_option()))
+
         # définir un style par défault pour la treeview
         self.style = ttk.Style()
         self.style_mapping = self.style.map('Treeview')
         
         self.__update_tree_font(get_font_family_option(), get_font_size_option())
 
         # All the icons used in the treeview should be loaded here to keep thier references.
@@ -113,38 +119,65 @@
         self.image_references[SUCCESS_GREEN_CHIP] = get_photoImage(SUCCESS_GREEN_CHIP)
         
         # add a menu to the treeview 
         self.menu = tk.Menu(self.treeview, name="menu", tearoff=False)
         
         self.treeview.tag_bind("clickable", "<<TreeviewSelect>>", self._on_select)
         self.treeview.tag_bind("nonClickable", "<<TreeviewSelect>>", self._remove_highlight_selection_effect)
-        self.treeview.bind("<Motion>", self.change_cursor)
+        self.treeview.bind("<Motion>", self._on_hover_exception_test)
         self.treeview.bind("<Configure>", self.__wrap_tree_content) # Here we handle the motion event of the treeview 
         
         self.workbench.bind(ALT_I, self.increase_row_height, True)
         self.workbench.bind(ALT_D, self.decrease_row_height, True)
         self.workbench.bind(ALT_F, self.update_font, True)
         self.workbench.bind(ALT_U, self.expand_rows, True) 
         self.workbench.bind(ALT_O, self.fold_rows, True)
+
+        self.__init_special_attributes()
         
-        self.__old_height = -1
+    def __init_special_attributes(self):
+        """"
+        Initializes the special attributes of the treeview.
+        """
+        self.__old_height = -1 # utilisé pour savoir si la hauteur de la treeview a changé
         self.__max_lines = 1 # le nombre de lignes du texte le plus long de la treeview
-    
-    def change_cursor(self, event):
-        item = self.treeview.identify('item', event.x, event.y)
-        tags = self.treeview.item(item, "tags")
-        if "underline" in tags:
-            self.treeview.config(cursor="hand2")
-            # should show it as bold
-            self.treeview.tag_configure("underline", font=tk_font.Font(underline=True, weight="bold", family=get_font_family_option(), size=get_font_size_option()))
-            # should show it as link
-        else:
-            self.treeview.config(cursor="arrow")
-            self.treeview.tag_configure("underline", font=tk_font.Font(underline=True, weight="normal", family=get_font_family_option(), size=get_font_size_option()))
-        
+        self.__hovered_exception = None # l'exception test sur laquelle le curseur est en train de passer
+     
+    def _on_hover_exception_test(self, event):
+        """
+        Handles the motion event of the treeview. When the cursor is hovering over an exception test, 
+        the font of the test is changed to bold and underlined. The cursor is also changed to "hand".
+        """
+        if not self.is_empty():
+            item = self.treeview.identify('item', event.x, event.y)
+            tags = self.treeview.item(item, "tags")
+            if "exception_as_link" in tags:
+                if self.__hovered_exception and self.__hovered_exception != item:
+                    # If the cursor is hovering over a different item, revert the font and cursor to normal for the previously hovered item
+                    prev_item = self.__hovered_exception
+                    prev_tags = self.treeview.item(prev_item, "tags")
+                    new_tags = tuple(tag for tag in prev_tags if tag not in ("exception_hovered", "exception_cursor"))
+                    self.treeview.item(prev_item, tags=new_tags + ("exception_as_link",))
+                    self.treeview.configure(cursor="")
+                    self.__hovered_exception = None
+
+                # Change the font to bold and underlined and set the cursor to "hand" when the cursor enters the row with the "exception_as_link" tag
+                new_tags = tuple(tag for tag in tags if tag != "exception_as_link")
+                self.treeview.item(item, tags=new_tags + ("exception_hovered", "exception_cursor"))
+                self.treeview.configure(cursor="hand2")
+                self.__hovered_exception = item
+            elif self.__hovered_exception and self.__hovered_exception != item:
+                # If the cursor is not over any "exception_as_link" item, revert the font and cursor to normal for the previously hovered item
+                prev_item = self.__hovered_exception
+                prev_tags = self.treeview.item(prev_item, "tags")
+                new_tags = tuple(tag for tag in prev_tags if tag not in ("exception_hovered", "exception_cursor"))
+                self.treeview.item(prev_item, tags=new_tags + ("exception_as_link",))
+                self.treeview.configure(cursor="")
+                self.__hovered_exception = None
+
     # ------------------------------------
     # Fonctions pour le Header du treeview
     # ------------------------------------
     
     def init_header(self, row=0, column=0):
         """
         Initialize the header of the treeview. Initially, the header contains 
@@ -423,15 +456,15 @@
         self.resize_header_bar()
     
     def __update_tree_font(self, font_family, font_size):
         """
         Applies the new font to the treeview.
         """
         self.style.configure("Treeview", justify="left", font=(font_family, font_size), wrap=tk.WORD)  
-        self.treeview.tag_configure("underline", font=tk_font.Font(underline=True, family=font_family, size=font_size))
+        self.treeview.tag_configure("exception_as_link", font=tk_font.Font(underline=True, family=font_family, size=font_size))
     
     def __wrap_tree_content(self, event=None, margin=NORMAL_MARGIN):
         """
             This function wraps the text of treeview to follow its width.
         """
         widget = event.widget if event else self.treeview
         if (isinstance(widget, ttk.Treeview)): 
@@ -580,15 +613,15 @@
             verdict_tags = (verdict.get_color(), CLICKABLE_TAG)
             item_text = str(verdict)
 
             for verdict_type, (icon, is_exception) in verdicts_map.items():
                 if isinstance(verdict, verdict_type) and not isinstance(verdict, PassedSetupVerdict):                
                     if is_exception:
                         values = [verdict.get_lineno(), verdict.__class__.__name__, verdict.get_details()] 
-                        verdict_tags += ("underline", "lightred" if get_option(HIGHLIGHT_EXCEPTIONS) else "")
+                        verdict_tags += ("exception_as_link", "lightred" if get_option(HIGHLIGHT_EXCEPTIONS) else "")
                     else:
                         values = [verdict.get_lineno()]
                     # on insère le test dans la treeview   
                     current_test = self.insert_into_treeview(current_node, item_text, values, 
                                                         verdict_tags, icon, open=get_option(OPEN_RED_TEST_ROWS))
                     # on configure les tags pour insérer les détails de l'exception
                     if isinstance(verdict, FailedVerdict):
@@ -688,16 +721,15 @@
             get_l1test_runner().set_has_exception(False)
         if clear_all:
             self.clear_header_bar()  # on supprime le contenu du header
         if clear_errorview:
             error_view:L1TestErrorView = self.workbench.get_view(L1TestErrorView.__name__)
             error_view.clear()
         self.treeview.delete(*self.treeview.get_children())
-        self.__max_lines = 1
-        self.__old_height = -1
+        self.__init_special_attributes()
         self.disable_menu()
         
     def clear_header_bar(self):
         """Clears the header of the treeview."""
         if self.header_bar:
             self.header_bar.direct_delete("1.0", "end")
             self.resize_header_bar()
```

### Comparing `bimbam-3.0/thonnycontrib/main_generator/main_generator.py` & `bimbam-3.9.0/thonnycontrib/main_generator/main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/plugin_loader.py` & `bimbam-3.9.0/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/properties.py` & `bimbam-3.9.0/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/fixtures/workbench_mock.py` & `bimbam-3.9.0/thonnycontrib/tests/fixtures/workbench_mock.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/tests_doc_generator.py` & `bimbam-3.9.0/thonnycontrib/tests/tests_doc_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/tests_example_no_expected.py` & `bimbam-3.9.0/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/tests_example_with_exception.py` & `bimbam-3.9.0/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/tests_example_with_expected.py` & `bimbam-3.9.0/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/tests_l1TestRunner.py` & `bimbam-3.9.0/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/tests_main_generator.py` & `bimbam-3.9.0/thonnycontrib/tests/tests_main_generator.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/tests_test_finder.py` & `bimbam-3.9.0/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/tests/tests_view.py` & `bimbam-3.9.0/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `bimbam-3.0/thonnycontrib/utils.py` & `bimbam-3.9.0/thonnycontrib/utils.py`

 * *Files identical despite different names*

