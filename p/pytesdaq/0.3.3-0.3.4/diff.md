# Comparing `tmp/pytesdaq-0.3.3.tar.gz` & `tmp/pytesdaq-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytesdaq-0.3.3.tar", last modified: Wed Jul 26 22:35:29 2023, max compression
+gzip compressed data, was "pytesdaq-0.3.4.tar", last modified: Fri Jul 28 18:51:51 2023, max compression
```

## Comparing `pytesdaq-0.3.3.tar` & `pytesdaq-0.3.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:29.003694 pytesdaq-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-26 22:35:29.003694 pytesdaq-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27099 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/analyzer/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/config/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27052 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/daq/daq.py
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/daq/nidaqtask.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/daq/polaris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/display/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/display/series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    78796 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/instruments/feb/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/feb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/feb/feb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/instruments/imacrt/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/imacrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/imacrt/imacrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/imacrt/macrtmodule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq/instruments/keysight/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/keysight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/keysight/keysight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/instruments/lakeshore/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61202 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/lakeshore/lakeshore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/instruments/magnicon/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/magnicon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/magnicon/magnicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/instruments/niadc/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/niadc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/instruments/niadc/nidevice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/io/filter_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    70229 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/io/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/io/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63818 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/_iv_didv_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/_iv_didv_tools_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/_process_iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    65026 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/processing/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/scope/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/scope/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/scope/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/sequencer/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/sequencer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45457 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/sequencer/iv_didv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/sequencer/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/sequencer/tc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.999693 pytesdaq-0.3.3/pytesdaq/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/utils/arg_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/utils/connection_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/pytesdaq/utils/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 22:35:28.995693 pytesdaq-0.3.3/pytesdaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 22:35:28.000000 pytesdaq-0.3.3/pytesdaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 22:35:29.003694 pytesdaq-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-26 22:35:17.000000 pytesdaq-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.292005 pytesdaq-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 18:51:51.292005 pytesdaq-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27099 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/analyzer/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27052 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/daq/daq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/daq/nidaqtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/daq/polaris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/display/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20524 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/display/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78796 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/instruments/feb/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/feb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25655 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/feb/feb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/instruments/imacrt/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/imacrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18154 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/imacrt/imacrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/imacrt/macrtmodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq/instruments/keysight/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/keysight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/keysight/keysight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/instruments/lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61202 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/lakeshore/lakeshore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/instruments/magnicon/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/magnicon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50731 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/magnicon/magnicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/instruments/niadc/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/niadc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/instruments/niadc/nidevice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/io/filter_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70229 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/io/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/io/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63818 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/_iv_didv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24567 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/_iv_didv_tools_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13187 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/_process_iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65026 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/processing/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38417 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/scope/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67331 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/scope/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/sequencer/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/sequencer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45457 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/sequencer/iv_didv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16666 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/sequencer/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/sequencer/tc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.288004 pytesdaq-0.3.4/pytesdaq/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/utils/arg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/utils/connection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/pytesdaq/utils/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:51:51.284005 pytesdaq-0.3.4/pytesdaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 18:51:51.000000 pytesdaq-0.3.4/pytesdaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:51:51.292005 pytesdaq-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-28 18:51:42.000000 pytesdaq-0.3.4/setup.py
```

### Comparing `pytesdaq-0.3.3/PKG-INFO` & `pytesdaq-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.3
+Version: 0.3.4
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 
 # `pytesdaq`
```

### Comparing `pytesdaq-0.3.3/README.md` & `pytesdaq-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/analyzer/analyzer.py` & `pytesdaq-0.3.4/pytesdaq/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/config/settings.py` & `pytesdaq-0.3.4/pytesdaq/config/settings.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/daq/daq.py` & `pytesdaq-0.3.4/pytesdaq/daq/daq.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/daq/nidaqtask.py` & `pytesdaq-0.3.4/pytesdaq/daq/nidaqtask.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/daq/polaris.py` & `pytesdaq-0.3.4/pytesdaq/daq/polaris.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/display/series.py` & `pytesdaq-0.3.4/pytesdaq/display/series.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/communication.py` & `pytesdaq-0.3.4/pytesdaq/instruments/communication.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/control.py` & `pytesdaq-0.3.4/pytesdaq/instruments/control.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/feb/feb.py` & `pytesdaq-0.3.4/pytesdaq/instruments/feb/feb.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/imacrt/imacrt.py` & `pytesdaq-0.3.4/pytesdaq/instruments/imacrt/imacrt.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/imacrt/macrtmodule.py` & `pytesdaq-0.3.4/pytesdaq/instruments/imacrt/macrtmodule.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/keysight/keysight.py` & `pytesdaq-0.3.4/pytesdaq/instruments/keysight/keysight.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/lakeshore/lakeshore.py` & `pytesdaq-0.3.4/pytesdaq/instruments/lakeshore/lakeshore.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/magnicon/magnicon.py` & `pytesdaq-0.3.4/pytesdaq/instruments/magnicon/magnicon.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/instruments/niadc/nidevice.py` & `pytesdaq-0.3.4/pytesdaq/instruments/niadc/nidevice.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/io/filter_hdf5.py` & `pytesdaq-0.3.4/pytesdaq/io/filter_hdf5.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/io/hdf5.py` & `pytesdaq-0.3.4/pytesdaq/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/io/redis.py` & `pytesdaq-0.3.4/pytesdaq/io/redis.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/processing/_iv_didv_tools.py` & `pytesdaq-0.3.4/pytesdaq/processing/_iv_didv_tools.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/processing/_iv_didv_tools_plotting.py` & `pytesdaq-0.3.4/pytesdaq/processing/_iv_didv_tools_plotting.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/processing/_process_iv_didv.py` & `pytesdaq-0.3.4/pytesdaq/processing/_process_iv_didv.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/processing/trigger.py` & `pytesdaq-0.3.4/pytesdaq/processing/trigger.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/scope/readout.py` & `pytesdaq-0.3.4/pytesdaq/scope/readout.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/scope/scope.py` & `pytesdaq-0.3.4/pytesdaq/scope/scope.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/sequencer/iv_didv.py` & `pytesdaq-0.3.4/pytesdaq/sequencer/iv_didv.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/sequencer/sequencer.py` & `pytesdaq-0.3.4/pytesdaq/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/sequencer/tc.py` & `pytesdaq-0.3.4/pytesdaq/sequencer/tc.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/utils/arg_utils.py` & `pytesdaq-0.3.4/pytesdaq/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/utils/connection_utils.py` & `pytesdaq-0.3.4/pytesdaq/utils/connection_utils.py`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/pytesdaq/utils/remote.py` & `pytesdaq-0.3.4/pytesdaq/utils/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import socket
 import termios
 import time
 import traceback
 import getpass
 from binascii import hexlify
 import paramiko
-from paramiko.py3compat import input, u
+from paramiko.util import u
 
 
 
 class Remote(object):
     """
     Use ssh connection to remote computer, using Python paramiko library
     """
```

### Comparing `pytesdaq-0.3.3/pytesdaq.egg-info/PKG-INFO` & `pytesdaq-0.3.4/pytesdaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytesdaq
-Version: 0.3.3
+Version: 0.3.4
 Summary: DAQ and Intruments control for TES development
 Home-page: https://github.com/spice-herald/pytesdaq
 Author: Bruno Serfass
 Author-email: serfass@berkeley.edu
 Description-Content-Type: text/markdown
 
 # `pytesdaq`
```

### Comparing `pytesdaq-0.3.3/pytesdaq.egg-info/SOURCES.txt` & `pytesdaq-0.3.4/pytesdaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytesdaq-0.3.3/setup.py` & `pytesdaq-0.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
       long_description = f.read()
 
 
 setup(name='pytesdaq',
-      version='0.3.3',
+      version='0.3.4',
       description='DAQ and Intruments control for TES development',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Bruno Serfass',
       author_email='serfass@berkeley.edu',
       url="https://github.com/spice-herald/pytesdaq",
       zip_safe = False,
@@ -24,15 +24,15 @@
       install_requires=[
           'PyQt5',
           'matplotlib',
           'lakeshore',
           'pandas',
           'nidaqmx',
           'pyvisa',
-          'paramiko',
+          'paramiko>=3.2.0',
           'walrus',
           'h5py',
           'qetpy>=1.6.3',
           'scipy',
           'seaborn',
           'astropy',
           'lmfit',
```

