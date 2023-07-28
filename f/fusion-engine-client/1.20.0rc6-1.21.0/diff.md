# Comparing `tmp/fusion-engine-client-1.20.0rc6.tar.gz` & `tmp/fusion-engine-client-1.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion-engine-client-1.20.0rc6.tar", last modified: Wed Jul 12 14:53:01 2023, max compression
+gzip compressed data, was "fusion-engine-client-1.21.0.tar", last modified: Fri Jul 28 20:52:12 2023, max compression
```

## Comparing `fusion-engine-client-1.20.0rc6.tar` & `fusion-engine-client-1.21.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.255403 fusion-engine-client-1.20.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-12 14:53:01.255403 fusion-engine-client-1.20.0rc6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.239403 fusion-engine-client-1.20.0rc6/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/bin/p1_display
--rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/bin/p1_extract
--rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/bin/p1_print
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.239403 fusion-engine-client-1.20.0rc6/fusion_engine_client/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.243403 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   114807 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/attitude.py
--rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/data_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.247403 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56721 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    25370 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/control.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    26231 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/fault_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/gnss_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/measurement_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/ros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/signal_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35596 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.247403 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/mixed_log_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.251403 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/bin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/time_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.243403 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-12 14:53:01.000000 fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:53:01.255403 fusion-engine-client-1.20.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:53:01.255403 fusion-engine-client-1.20.0rc6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_construct_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_enum_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_file_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_message_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_mixed_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-12 14:52:20.000000 fusion-engine-client-1.20.0rc6/tests/test_time_range.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.429172 fusion-engine-client-1.21.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-28 20:52:12.429172 fusion-engine-client-1.21.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.417172 fusion-engine-client-1.21.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      472 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/bin/p1_display
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4679 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/bin/p1_extract
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13937 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/bin/p1_print
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.417172 fusion-engine-client-1.21.0/fusion_engine_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.417172 fusion-engine-client-1.21.0/fusion_engine_client/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/analysis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   116442 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/analysis/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/analysis/attitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41758 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/analysis/data_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.421172 fusion-engine-client-1.21.0/fusion_engine_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57914 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25370 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26231 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/fault_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/gnss_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/measurement_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39947 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15258 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/signal_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35596 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/messages/timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.425172 fusion-engine-client-1.21.0/fusion_engine_client/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/parsers/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/parsers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22963 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/parsers/file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31146 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/parsers/mixed_log_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.429172 fusion-engine-client-1.21.0/fusion_engine_client/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/bin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24860 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/time_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/fusion_engine_client/utils/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.417172 fusion-engine-client-1.21.0/fusion_engine_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-28 20:52:12.000000 fusion-engine-client-1.21.0/fusion_engine_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-28 20:52:12.000000 fusion-engine-client-1.21.0/fusion_engine_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:52:12.000000 fusion-engine-client-1.21.0/fusion_engine_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 20:52:12.000000 fusion-engine-client-1.21.0/fusion_engine_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:52:12.000000 fusion-engine-client-1.21.0/fusion_engine_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:52:12.429172 fusion-engine-client-1.21.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:52:12.429172 fusion-engine-client-1.21.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_construct_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20962 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_enum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_file_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_message_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_mixed_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-07-28 20:51:34.000000 fusion-engine-client-1.21.0/tests/test_time_range.py
```

### Comparing `fusion-engine-client-1.20.0rc6/PKG-INFO` & `fusion-engine-client-1.21.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc6
+Version: 1.21.0
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc6/README.md` & `fusion-engine-client-1.21.0/README.md`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/bin/p1_extract` & `fusion-engine-client-1.21.0/bin/p1_extract`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/bin/p1_print` & `fusion-engine-client-1.21.0/bin/p1_print`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/analyzer.py` & `fusion-engine-client-1.21.0/fusion_engine_client/analysis/analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1059,14 +1059,53 @@
             'xanchor': 'left',
             'y': 1.1,
             'yanchor': 'top'
         }]
 
         self._add_figure(name=filename, figure=figure, title=figure_title)
 
+    def plot_dop(self):
+        """!
+        @brief Plot dilution of precision (DOP).
+
+        This includes geometric, position, horizontal, and vertical DOP.
+        """
+        result = self.reader.read(message_types=[GNSSInfoMessage], **self.params)
+        data = result[GNSSInfoMessage.MESSAGE_TYPE]
+
+        if len(data.p1_time) == 0:
+            self.logger.info('No GNSS info data available. Skipping dilution of precision plot.')
+            return
+
+        # # Setup the figure.
+        figure = make_subplots(
+            rows=1, cols=1,  print_grid=False, shared_xaxes=True,
+            subplot_titles=['Dilution of Precision (DOP)'])
+
+        figure['layout'].update(showlegend=True, modebar_add=['v1hovermode'])
+        figure['layout']['xaxis'].update(title=self.p1_time_label)
+
+        dops = [('GDOP', data.gdop), ('PDOP', data.pdop), ('HDOP', data.hdop), ('VDOP', data.vdop)]
+
+        # Assign colors to each DOP type.
+        color_by_dop = self._assign_colors([entry[0] for entry in dops])
+
+        # Plot each DOP type.
+        for entry in dops:
+            name, dop = entry
+
+            text = ['P1: %.1f sec' % t for t in data.p1_time]
+            time = data.p1_time - float(self.t0)
+            figure.add_trace(go.Scattergl(x=time, y=dop, text=text,
+                                          name=name, hoverlabel={'namelength': -1},
+                                          mode='markers', marker={'color': color_by_dop[name]}),
+                             1, 1)
+
+        self._add_figure(name='dilution_of_precision', figure=figure, title='Dilution of Precision vs. Time')
+
     def plot_gnss_corrections_status(self):
         """!
         @brief Plot GNSS corrections status (baseline distance, age, etc.).
         """
         result = self.reader.read(message_types=[GNSSInfoMessage], **self.params)
         data = result[GNSSInfoMessage.MESSAGE_TYPE]
 
@@ -2375,14 +2414,15 @@
         analyzer.plot_relative_position()
         analyzer.plot_map(mapbox_token=options.mapbox_token)
         analyzer.plot_calibration()
         analyzer.plot_gnss_cn0()
         analyzer.plot_gnss_signal_status()
         analyzer.plot_gnss_skyplot()
         analyzer.plot_gnss_corrections_status()
+        analyzer.plot_dop()
 
         # By default, we always plot heading measurements (i.e., output from a secondary heading device like an
         # LG69T-AH), separate from other sensor measurements controlled by --measurements.
         analyzer.plot_heading_measurements()
 
         if options.measurements:
             analyzer.plot_imu()
```

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/attitude.py` & `fusion-engine-client-1.21.0/fusion_engine_client/analysis/attitude.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/analysis/data_loader.py` & `fusion-engine-client-1.21.0/fusion_engine_client/analysis/data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/configuration.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     INTERFACE_CONFIG = 200
     UART1_BAUD = 256
     UART2_BAUD = 257
     UART1_OUTPUT_DIAGNOSTICS_MESSAGES = 258
     UART2_OUTPUT_DIAGNOSTICS_MESSAGES = 259
     ENABLE_WATCHDOG_TIMER = 300
     USER_DEVICE_ID = 301
+    LBAND_PARAMETERS = 1024
 
 
 class InterfaceConfigType(IntEnum):
   INVALID = 0
   OUTPUT_DIAGNOSTICS_MESSAGES = 1
   BAUD_RATE = 2
   REMOTE_ADDRESS = 3
@@ -622,14 +623,43 @@
         tropo_delay_model: TropoDelayModel = TropoDelayModel.AUTO
 
     TroposphereConfigConstruct = Struct(
         "tropo_delay_model" / AutoEnum(Int8ul, TropoDelayModel),
         Padding(3),
     )
 
+    class LBandConfig(NamedTuple):
+        """!
+        @brief Configuration of the L-band demodulator parameters.
+        """
+        ## The center frequency of the L-band beam (Hz).
+        center_frequency_hz: float
+
+        ## The size of the signal acquisition search space (in Hz) around the center
+        ## frequency.
+        ##
+        ## For example, a value of 6000 will search +/- 3 kHz around the center
+        ## frequency.
+        search_window_hz: float
+        ## Service ID of the provider.
+        pmp_service_id: int
+        ## Data rate of the provider (bps).
+        pmp_data_rate_bps: int
+        ## Unique word of the provider.
+        pmp_unique_word: int
+
+    LBandConfigConstruct = Struct(
+        "center_frequency_hz" / Float32l,
+        "search_window_hz" / Float32l,
+        "pmp_service_id" / Int32ul,
+        "pmp_data_rate_bps" / Int16ul,
+        Padding(2),
+        "pmp_unique_word" / Int32ul,
+    )
+
     class Empty(NamedTuple):
         """!
         @brief Dummy specifier for empty config.
         """
         pass
 
     # Empty construct
@@ -713,22 +743,31 @@
 @_conf_gen.create_config_class(ConfigType.IONOSPHERE_CONFIG, _conf_gen.IonosphereConfigConstruct)
 class IonosphereConfig(_conf_gen.IonosphereConfig):
     """!
     @brief Ionospheric delay model configuration.
     """
     pass
 
+
 @_conf_gen.create_config_class(ConfigType.TROPOSPHERE_CONFIG, _conf_gen.TroposphereConfigConstruct)
 class TroposphereConfig(_conf_gen.TroposphereConfig):
     """!
     @brief Tropospheric delay model configuration.
     """
     pass
 
 
+@_conf_gen.create_config_class(ConfigType.LBAND_PARAMETERS, _conf_gen.LBandConfigConstruct)
+class LBandConfig(_conf_gen.LBandConfig):
+    """!
+    @brief Configuration of the L-band demodulator parameters.
+    """
+    pass
+
+
 @_conf_gen.create_config_class(ConfigType.UART1_BAUD, _conf_gen.UInt32Construct)
 class Uart1BaudConfig(_conf_gen.IntegerVal):
     """!
     @brief The UART1 serial baud rate (in bits/second).
     """
     pass
```

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/control.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/defs.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/device.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/device.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/fault_control.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/fault_control.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/gnss_corrections.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/gnss_corrections.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..utils.construct_utils import construct_message_to_string
 from .defs import *
 
 
 class LBandFrameMessage(MessagePayload):
     """!
-    @brief L-Band frame message.
+    @brief L-band frame message.
     """
     MESSAGE_TYPE = MessageType.LBAND_FRAME
     MESSAGE_VERSION = 0
 
     LBandFrameMessageConstruct = Struct(
         "system_time_ns" / Int64sl,
         "user_data_size_bytes" / Int16ul,
@@ -45,15 +45,15 @@
 
     def __repr__(self):
         result = super().__repr__()[:-1]
         result += f', errors={self.bit_error_count}, power={self.signal_power_db}, doppler={self.doppler_hz}]'
         return result
 
     def __str__(self):
-        string = f'L-Band Frame @ %s\n' % system_time_to_str(self.system_time_ns)
+        string = f'L-band Frame @ %s\n' % system_time_to_str(self.system_time_ns)
         string += f'  Bit Error Count: {self.bit_error_count}\n'
         string += f'  Signal Power: {self.signal_power_db} dB\n'
         string += f'  Doppler: {self.doppler_hz} Hz'
         return string
 
     def calcsize(self) -> int:
         return len(self.pack())
```

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/measurement_details.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/measurement_details.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/measurements.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/measurements.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/ros.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/ros.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/signal_defs.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/signal_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/solution.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/solution.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/messages/timestamp.py` & `fusion-engine-client-1.21.0/fusion_engine_client/messages/timestamp.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/decoder.py` & `fusion-engine-client-1.21.0/fusion_engine_client/parsers/decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/encoder.py` & `fusion-engine-client-1.21.0/fusion_engine_client/parsers/encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/file_index.py` & `fusion-engine-client-1.21.0/fusion_engine_client/parsers/file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/parsers/mixed_log_reader.py` & `fusion-engine-client-1.21.0/fusion_engine_client/parsers/mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/argument_parser.py` & `fusion-engine-client-1.21.0/fusion_engine_client/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/bin_utils.py` & `fusion-engine-client-1.21.0/fusion_engine_client/utils/bin_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/construct_utils.py` & `fusion-engine-client-1.21.0/fusion_engine_client/utils/construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/enum_utils.py` & `fusion-engine-client-1.21.0/fusion_engine_client/utils/enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/log.py` & `fusion-engine-client-1.21.0/fusion_engine_client/utils/log.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/numpy_utils.py` & `fusion-engine-client-1.21.0/fusion_engine_client/utils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/time_range.py` & `fusion-engine-client-1.21.0/fusion_engine_client/utils/time_range.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client/utils/trace.py` & `fusion-engine-client-1.21.0/fusion_engine_client/utils/trace.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/PKG-INFO` & `fusion-engine-client-1.21.0/fusion_engine_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-engine-client
-Version: 1.20.0rc6
+Version: 1.21.0
 Summary: Point One FusionEngine Library
 Home-page: https://github.com/PointOneNav/fusion-engine-client
 Author: Point One Navigation
 Author-email: support@pointonenav.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `fusion-engine-client-1.20.0rc6/fusion_engine_client.egg-info/SOURCES.txt` & `fusion-engine-client-1.21.0/fusion_engine_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/setup.py` & `fusion-engine-client-1.21.0/setup.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_config.py` & `fusion-engine-client-1.21.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_construct_utils.py` & `fusion-engine-client-1.21.0/tests/test_construct_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_data_loader.py` & `fusion-engine-client-1.21.0/tests/test_data_loader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_decoder.py` & `fusion-engine-client-1.21.0/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_encoder.py` & `fusion-engine-client-1.21.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_enum_utils.py` & `fusion-engine-client-1.21.0/tests/test_enum_utils.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_file_index.py` & `fusion-engine-client-1.21.0/tests/test_file_index.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_message_defs.py` & `fusion-engine-client-1.21.0/tests/test_message_defs.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_mixed_log_reader.py` & `fusion-engine-client-1.21.0/tests/test_mixed_log_reader.py`

 * *Files identical despite different names*

### Comparing `fusion-engine-client-1.20.0rc6/tests/test_time_range.py` & `fusion-engine-client-1.21.0/tests/test_time_range.py`

 * *Files identical despite different names*

