# Comparing `tmp/autopilot_tools-0.1.0.tar.gz` & `tmp/autopilot_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopilot_tools-0.1.0.tar", last modified: Tue Jul 18 18:03:21 2023, max compression
+gzip compressed data, was "autopilot_tools-0.3.0.tar", last modified: Fri Jul 28 17:39:06 2023, max compression
```

## Comparing `autopilot_tools-0.1.0.tar` & `autopilot_tools-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/
--rw-rw-r--   0 nex       (1000) nex       (1000)     1078 2023-07-18 17:51:06.000000 autopilot_tools-0.1.0/LICENSE
--rw-rw-r--   0 nex       (1000) nex       (1000)     3150 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/PKG-INFO
--rw-rw-r--   0 nex       (1000) nex       (1000)     2625 2023-07-18 17:59:28.000000 autopilot_tools-0.1.0/README.md
--rw-rw-r--   0 nex       (1000) nex       (1000)      698 2023-07-18 17:38:33.000000 autopilot_tools-0.1.0/pyproject.toml
--rw-rw-r--   0 nex       (1000) nex       (1000)       43 2023-05-16 20:44:57.000000 autopilot_tools-0.1.0/requirements.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)       38 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/setup.cfg
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/src/
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/src/autopilot_tools/
--rwxrwxr-x   0 nex       (1000) nex       (1000)       85 2023-07-18 17:17:55.000000 autopilot_tools-0.1.0/src/autopilot_tools/analyzer.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/src/autopilot_tools/configurator/
--rwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/configurator/__init__.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1412 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/configurator/mavlink_params.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/
--rwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/__init__.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1586 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/airspeed.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1781 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/altitude.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)      695 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/color_logging.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1353 2023-07-15 21:25:27.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/device_id_parser.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     2037 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/esc_status.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     5225 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/extract.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     7645 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/flight_distance.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     3708 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/ice.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     3254 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/uorb_topics.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1530 2023-05-16 20:02:01.000000 autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/utils.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/src/autopilot_tools/px4/
--rwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 13:51:18.000000 autopilot_tools-0.1.0/src/autopilot_tools/px4/__init__.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)    40414 2023-07-18 13:49:20.000000 autopilot_tools-0.1.0/src/autopilot_tools/px4/px_uploader.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     9212 2023-07-18 17:28:41.000000 autopilot_tools-0.1.0/src/autopilot_tools/vehicle.py
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/src/autopilot_tools.egg-info/
--rw-rw-r--   0 nex       (1000) nex       (1000)     3150 2023-07-18 18:03:21.000000 autopilot_tools-0.1.0/src/autopilot_tools.egg-info/PKG-INFO
--rw-rw-r--   0 nex       (1000) nex       (1000)     1059 2023-07-18 18:03:21.000000 autopilot_tools-0.1.0/src/autopilot_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)        1 2023-07-18 18:03:21.000000 autopilot_tools-0.1.0/src/autopilot_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)       44 2023-07-18 18:03:21.000000 autopilot_tools-0.1.0/src/autopilot_tools.egg-info/requires.txt
--rw-rw-r--   0 nex       (1000) nex       (1000)       16 2023-07-18 18:03:21.000000 autopilot_tools-0.1.0/src/autopilot_tools.egg-info/top_level.txt
-drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 18:03:21.342521 autopilot_tools-0.1.0/tests/
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1530 2023-07-18 17:08:42.000000 autopilot_tools-0.1.0/tests/test_mavlink_params.py
--rwxrwxr-x   0 nex       (1000) nex       (1000)     1540 2023-07-18 17:22:37.000000 autopilot_tools-0.1.0/tests/test_vehicle.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-28 17:39:06.815915 autopilot_tools-0.3.0/
+-rw-rw-r--   0 nex       (1000) nex       (1000)     1078 2023-07-18 17:51:06.000000 autopilot_tools-0.3.0/LICENSE
+-rw-rw-r--   0 nex       (1000) nex       (1000)     3180 2023-07-28 17:39:06.815915 autopilot_tools-0.3.0/PKG-INFO
+-rw-rw-r--   0 nex       (1000) nex       (1000)     2643 2023-07-27 16:33:22.000000 autopilot_tools-0.3.0/README.md
+-rw-rw-r--   0 nex       (1000) nex       (1000)      709 2023-07-28 17:35:02.000000 autopilot_tools-0.3.0/pyproject.toml
+-rw-rw-r--   0 nex       (1000) nex       (1000)       48 2023-07-28 17:11:43.000000 autopilot_tools-0.3.0/requirements.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)       38 2023-07-28 17:39:06.815915 autopilot_tools-0.3.0/setup.cfg
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-28 17:39:06.811915 autopilot_tools-0.3.0/src/
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-28 17:39:06.811915 autopilot_tools-0.3.0/src/autopilot_tools/
+-rw-rw-r--   0 nex       (1000) nex       (1000)        0 2023-07-28 17:11:43.000000 autopilot_tools-0.3.0/src/autopilot_tools/__init__.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)       85 2023-07-18 17:17:55.000000 autopilot_tools-0.3.0/src/autopilot_tools/analyzer.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-28 17:39:06.811915 autopilot_tools-0.3.0/src/autopilot_tools/configurator/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-05-16 20:02:01.000000 autopilot_tools-0.3.0/src/autopilot_tools/configurator/__init__.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)     4482 2023-07-28 17:11:43.000000 autopilot_tools-0.3.0/src/autopilot_tools/configurator/ftp_filesystem.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)     8820 2023-07-28 17:11:43.000000 autopilot_tools-0.3.0/src/autopilot_tools/configurator/mavftputils.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1414 2023-07-28 17:11:43.000000 autopilot_tools-0.3.0/src/autopilot_tools/configurator/mavlink_params.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)     9918 2023-07-28 17:11:43.000000 autopilot_tools-0.3.0/src/autopilot_tools/configurator/mission_file.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)      584 2023-07-28 17:11:43.000000 autopilot_tools-0.3.0/src/autopilot_tools/configurator/mission_result.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)      588 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/exceptions.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-28 17:39:06.811915 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-05-16 20:02:01.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/__init__.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1577 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/airspeed.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1747 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/altitude.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)      701 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/color_logging.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1341 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/device_id_parser.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     2037 2023-05-16 20:02:01.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/esc_status.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     5231 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/extract.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     7663 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/flight_distance.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     3713 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/ice.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     3268 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/uorb_topics.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1534 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/utils.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-28 17:39:06.811915 autopilot_tools-0.3.0/src/autopilot_tools/px4/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-18 13:51:18.000000 autopilot_tools-0.3.0/src/autopilot_tools/px4/__init__.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)    40414 2023-07-18 13:49:20.000000 autopilot_tools-0.3.0/src/autopilot_tools/px4/px_uploader.py
+-rw-rw-r--   0 nex       (1000) nex       (1000)      568 2023-07-28 17:11:44.000000 autopilot_tools-0.3.0/src/autopilot_tools/utils.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)    15789 2023-07-28 17:35:57.000000 autopilot_tools-0.3.0/src/autopilot_tools/vehicle.py
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-28 17:39:06.811915 autopilot_tools-0.3.0/src/autopilot_tools.egg-info/
+-rw-rw-r--   0 nex       (1000) nex       (1000)     3180 2023-07-28 17:39:06.000000 autopilot_tools-0.3.0/src/autopilot_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 nex       (1000) nex       (1000)     1353 2023-07-28 17:39:06.000000 autopilot_tools-0.3.0/src/autopilot_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)        1 2023-07-28 17:39:06.000000 autopilot_tools-0.3.0/src/autopilot_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)       49 2023-07-28 17:39:06.000000 autopilot_tools-0.3.0/src/autopilot_tools.egg-info/requires.txt
+-rw-rw-r--   0 nex       (1000) nex       (1000)       16 2023-07-28 17:39:06.000000 autopilot_tools-0.3.0/src/autopilot_tools.egg-info/top_level.txt
+drwxrwxr-x   0 nex       (1000) nex       (1000)        0 2023-07-28 17:39:06.811915 autopilot_tools-0.3.0/tests/
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1530 2023-07-27 07:21:47.000000 autopilot_tools-0.3.0/tests/test_mavlink_params.py
+-rwxrwxr-x   0 nex       (1000) nex       (1000)     1540 2023-07-18 17:22:37.000000 autopilot_tools-0.3.0/tests/test_vehicle.py
```

### Comparing `autopilot_tools-0.1.0/LICENSE` & `autopilot_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autopilot_tools-0.1.0/PKG-INFO` & `autopilot_tools-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: autopilot_tools
-Version: 0.1.0
-Summary: PX4/ArduPilot MAVLink usefull tools
-Author-email: Dmitry Ponomarev <PonomarevDA96@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PX4/ArduPilot Autopilot tools ![](https://badge.fury.io/py/autopilot-tools.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/build_package.yml/badge.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/pylint.yml/badge.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/tests.yml/badge.svg)
+# PX4/ArduPilot Autopilot tools ![](https://badge.fury.io/py/autopilot-tools.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/build_package.yml/badge.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/pylint.yml/badge.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/tests.yml/badge.svg)
 
 This repository is a collection of scripts created to facilitate automated work with the PX4/ArduPilot, such as:
 1. Upload a specific firmware to the autopilot via a link or given binaries
 2. Reset the autopilot to default and configure the required parameters
 3. Upload and run a mission
 4. Download the last flight log
 5. Analyze the flight log
@@ -39,14 +25,15 @@
 The script below could be used as part of a CI process and it illustrates the main functionality of the package:
 
 ```python
 from autopilot_tools.vehicle import Vehicle
 from autopilot_tools.analyzer import Analyzer
 
 vehicle = Vehicle()
+vehicle.connect(device="serial")
 vehicle.upload_firmware(firmware_path_or_url)
 vehicle.configure(params_path)
 vehicle.load_mission(mission_path)
 
 res = vehicle.run_mission(mission_path)
 print(res)
```

### Comparing `autopilot_tools-0.1.0/README.md` & `autopilot_tools-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-# PX4/ArduPilot Autopilot tools ![](https://badge.fury.io/py/autopilot-tools.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/build_package.yml/badge.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/pylint.yml/badge.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/tests.yml/badge.svg)
+Metadata-Version: 2.1
+Name: autopilot_tools
+Version: 0.3.0
+Summary: PX4/ArduPilot autopilot tools
+Author-email: Dmitry Ponomarev <PonomarevDA96@gmail.com>
+Project-URL: Homepage, https://github.com/PonomarevDA/autopilot_tools
+Project-URL: Bug Tracker, https://github.com/PonomarevDA/autopilot_tools/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PX4/ArduPilot Autopilot tools ![](https://badge.fury.io/py/autopilot-tools.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/build_package.yml/badge.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/pylint.yml/badge.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/tests.yml/badge.svg)
 
 This repository is a collection of scripts created to facilitate automated work with the PX4/ArduPilot, such as:
 1. Upload a specific firmware to the autopilot via a link or given binaries
 2. Reset the autopilot to default and configure the required parameters
 3. Upload and run a mission
 4. Download the last flight log
 5. Analyze the flight log
@@ -25,14 +39,15 @@
 The script below could be used as part of a CI process and it illustrates the main functionality of the package:
 
 ```python
 from autopilot_tools.vehicle import Vehicle
 from autopilot_tools.analyzer import Analyzer
 
 vehicle = Vehicle()
+vehicle.connect(device="serial")
 vehicle.upload_firmware(firmware_path_or_url)
 vehicle.configure(params_path)
 vehicle.load_mission(mission_path)
 
 res = vehicle.run_mission(mission_path)
 print(res)
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/configurator/mavlink_params.py` & `autopilot_tools-0.3.0/src/autopilot_tools/configurator/mavlink_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 #!/usr/bin/env python3
 import struct
 from pymavlink import mavutil
 
 MAV_PARAM_TYPE_INT8 = 2
 MAV_PARAM_TYPE_INT16 = 4
 PARAM_TYPE_TO_STRING = {
-    MAV_PARAM_TYPE_INT8 : "INT8",
-    MAV_PARAM_TYPE_INT16 : "INT16",
-    mavutil.mavlink.MAV_PARAM_TYPE_INT32 : "INT32",
-    mavutil.mavlink.MAV_PARAM_TYPE_REAL32 : "FLOAT"
+    MAV_PARAM_TYPE_INT8: "INT8",
+    MAV_PARAM_TYPE_INT16: "INT16",
+    mavutil.mavlink.MAV_PARAM_TYPE_INT32: "INT32",
+    mavutil.mavlink.MAV_PARAM_TYPE_REAL32: "FLOAT"
 }
 INTEGER_TYPES = [
     MAV_PARAM_TYPE_INT8,
     MAV_PARAM_TYPE_INT16,
     mavutil.mavlink.MAV_PARAM_TYPE_INT32
 ]
 
+
 def float_to_integer(float_number):
     return struct.unpack('!I', struct.pack('!f', float_number))[0]
 
+
 def integer_to_float(int_number):
     return struct.unpack('!f', struct.pack('!I', int_number))[0]
 
+
 def is_integer_param(param_type):
     return param_type in INTEGER_TYPES
 
+
 def param_value_to_type(param_value):
     if isinstance(param_value, int):
         return mavutil.mavlink.MAV_PARAM_TYPE_INT32
     return mavutil.mavlink.MAV_PARAM_TYPE_REAL32
 
+
 def deserialize_param_value(msg):
     param_name = msg.param_id
     param_type = PARAM_TYPE_TO_STRING[msg.param_type]
     if is_integer_param(msg.param_type):
         param_value = float_to_integer(msg.param_value)
     else:
         param_value = msg.param_value
 
     return param_name, param_type, param_value
 
+
 def serialize_param_value(param_value):
     param_type = param_value_to_type(param_value)
     if isinstance(param_value, int):
         param_value = integer_to_float(param_value)
     return param_value, param_type
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/airspeed.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/airspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python3
 import matplotlib.pyplot as plt
 
 from .extract import extract_args
 from .device_id_parser import parse_device_id
 from .utils import log_name_from_full_path
 
+
 def airspeed(log_path, output_path, output_report_path):
     log_name = log_name_from_full_path(log_path)
     # 1. Extract data
     expected_data_list = [
-        ("differential_pressure_0", "device_id",        "differential_pressure_pa"),
-        ("differential_pressure_1", "device_id",        "differential_pressure_pa"),
+        ("differential_pressure_0", "device_id", "differential_pressure_pa"),
+        ("differential_pressure_1", "device_id", "differential_pressure_pa"),
     ]
     extracted_data = []
     for idx, expected_data in enumerate(expected_data_list):
         data = extract_args(log_path=f"{log_path}/{log_name}.ulg",
                             output_path=output_path,
                             msg=expected_data[0],
                             msg_fields=expected_data[1:])
@@ -29,14 +30,14 @@
     parsed_data_list.append(parse_device_id(device_id, verbose=True))
 
     device_id = int(extracted_data[1][0][0])
     parsed_data_list.append(parse_device_id(device_id, verbose=True))
 
     label = "diff_pressure"
     plt.cla()
-    plt.plot(extracted_data[0][1], label="node_id="+str(parsed_data_list[0]["address"]))
-    plt.plot(extracted_data[1][1], label="node_id="+str(parsed_data_list[1]["address"]))
+    plt.plot(extracted_data[0][1], label="node_id=" + str(parsed_data_list[0]["address"]))
+    plt.plot(extracted_data[1][1], label="node_id=" + str(parsed_data_list[1]["address"]))
     plt.legend()
     plt.title(log_name)
     plt.ylabel("Differential pressure, Pa")
     plt.grid()
     plt.savefig(f'{output_report_path}/{label}.png')
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/altitude.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/altitude.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
 import matplotlib.pyplot as plt
 
 from .extract import extract_args
 from .uorb_topics import UorbTopic, DistanceSensor, EstimatorLocalPositionRefAlt, \
-                         VehicleGpsPosition, VehicleAirDataBaroAltMeter, SensorGps
+    VehicleGpsPosition, VehicleAirDataBaroAltMeter, SensorGps
 from .utils import log_name_from_full_path
 
 UORB_TOPICS = {
-    "vehicle_local_position_0"      : UorbTopic(["z"], True),
-    "distance_sensor_0"             : DistanceSensor(["current_distance"], True),
-    "estimator_local_position_0"    : EstimatorLocalPositionRefAlt(["ref_alt"]),
-    "vehicle_gps_position_0"        : VehicleGpsPosition(["alt"]),
-    "vehicle_air_data_0"            : VehicleAirDataBaroAltMeter(["baro_alt_meter"], True),
-    "sensor_gps_0"                  : SensorGps(["alt", "device_id"], True),
-    "sensor_gps_1"                  : SensorGps(["alt", "device_id"], True),
+    "vehicle_local_position_0":     UorbTopic(["z"], True),
+    "distance_sensor_0":            DistanceSensor(["current_distance"], True),
+    "estimator_local_position_0":   EstimatorLocalPositionRefAlt(["ref_alt"]),
+    "vehicle_gps_position_0":       VehicleGpsPosition(["alt"]),
+    "vehicle_air_data_0":           VehicleAirDataBaroAltMeter(["baro_alt_meter"], True),
+    "sensor_gps_0":                 SensorGps(["alt", "device_id"], True),
+    "sensor_gps_1":                 SensorGps(["alt", "device_id"], True),
 }
 
+
 def altitude(log_path, output_path, output_report_path):
     log_name = log_name_from_full_path(log_path)
 
     # 1. Extract and process data
     for topic, uorb in UORB_TOPICS.items():
         data_args = uorb.args
         tss_and_data = extract_args(log_path=f"{log_path}/{log_name}.ulg",
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/color_logging.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/color_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 #!/usr/bin/env python3
 from enum import Enum
 
+
 class Colors(Enum):
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
+
 def log_info(log_str):
     print(f"INFO: {log_str}")
 
+
 def log_warn(log_str):
     print(f"{Colors.WARNING.value}WARN: {log_str}{Colors.ENDC.value}")
 
+
 def log_err(log_str):
     print(f"{Colors.FAIL.value}ERR: {log_str}{Colors.ENDC.value}")
 
+
 def log_green(log_str):
     print(f"{Colors.OKGREEN.value}{log_str}{Colors.ENDC.value}")
 
+
 def log_cyan(log_str):
     print(f"{Colors.OKCYAN.value}{log_str}{Colors.ENDC.value}")
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/esc_status.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/esc_status.py`

 * *Files identical despite different names*

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/extract.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,56 +3,61 @@
 Set of functions to extract usefull data from .ulg logs.
 """
 import csv
 import subprocess
 import os
 from .color_logging import log_info, log_err
 
+
 def convert_relative_path_to_absolute(path):
     if len(path) == 0:
         path = ""
     elif path[0] == '/':
-        pass # is already absolute
+        pass  # is already absolute
     else:
         path = f"{os.getcwd()}/{path}"
     return path
 
+
 def ulog2csv(output_path, log_path):
     """
     Process bash command: ulog2csv
     """
     output_path = convert_relative_path_to_absolute(output_path)
     bash_command_log_to_csv = f"ulog2csv -o {output_path} {log_path}"
     log_info(bash_command_log_to_csv)
     process = subprocess.Popen(bash_command_log_to_csv.split(),
-                                stderr=subprocess.PIPE,
-                                stdout=subprocess.PIPE)
-    _,_ = process.communicate()
+                               stderr=subprocess.PIPE,
+                               stdout=subprocess.PIPE)
+    _, _ = process.communicate()
+
 
 def ulog_params(ulog_full_path):
     """
     Process bash command: ulog_params
     """
     bash_command_extract_params = f"ulog_params {ulog_full_path}"
     process = subprocess.Popen(bash_command_extract_params.split(), stdout=subprocess.PIPE)
     params_raw, _ = process.communicate()
     params_raw = params_raw.decode("utf-8")
     params_raw = params_raw.split('\n')
     return params_raw
 
+
 def read_csv_file(csv_file_path):
     """
     Open and read given file
     csv_file_path - relative or absolute
     """
     path = convert_relative_path_to_absolute(csv_file_path)
     csvfile = open(path, newline='', encoding="utf8")
     reader = csv.reader(csvfile, delimiter=',')
     return reader
 
+
 def parse_ulog_if_it_is_not_parsed_and_read_csv_file(log_path, output_path, msg):
     """
     log_path    String of relative or absolute path to log file.
                 Example: data_set/fw/log_172_2022-1-14-18-07-00.ulg
     output_path String of relative or absolute path to output folder.
                 Example: data_set/fw/output
     msg         String of uorb topic name.
@@ -130,14 +135,15 @@
     for row_with_values in csv_fd:
         for idx in range(msg_fields_amount):
             data = data_idx[idx]
             new_data = float(row_with_values[data])
             parsed_data[idx].append(new_data)
     return parsed_data
 
+
 def extract_params(log_path):
     """
     log_path    String with log path.
                 Example: data_set/fw/log_79_2021-12-5-06-22-20.ulg
     """
     params_raw = ulog_params(log_path)
     params_parsed = {}
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/flight_distance.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/flight_distance.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,55 +5,61 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 from .extract import extract_args
 from .utils import get_log_names, extract_date_from_date_string, extract_date_from_log_path
 from .color_logging import log_info, log_warn
 
+
 def extract_vehicle_local_position(log_name, output_path):
     extracted_data = extract_args(log_path=log_name,
                                   output_path=output_path,
                                   msg="vehicle_local_position_0",
                                   msg_fields=("x", "y", "z", "xy_valid", "z_valid", "timestamp"))
     pos_x_y_z = (extracted_data[0], extracted_data[1], extracted_data[2])
     xy_valid = extracted_data[3]
     z_valid = extracted_data[4]
     timestamp = extracted_data[5]
     pos_xyz_valid = np.multiply(xy_valid, z_valid)
     flight_time_minutes = (timestamp[-1] - timestamp[0]) / 1000000 / 60
     return pos_x_y_z[0], pos_x_y_z[1], pos_x_y_z[2], pos_xyz_valid, flight_time_minutes
 
+
 def estimate_distance(pos_x, pos_y, pos_z, pos_xyz_valid):
     total_dist_m = 0
     last_index = -2
     for valid_index in np.argwhere(pos_xyz_valid > 0):
         index = valid_index[0]
         if index == last_index + 1:
             dx = pos_x[index] - pos_x[last_index]
             dy = pos_y[index] - pos_y[last_index]
             dz = pos_z[index] - pos_z[last_index]
-            total_dist_m += math.sqrt(dx*dx + dy*dy + dz*dz)
+            total_dist_m += math.sqrt(dx * dx + dy * dy + dz * dz)
         last_index = index
 
     return total_dist_m
 
+
 class BasePlotter:
     def __init__(self) -> None:
         self.x_label_name = ""
         self.y_label_name = ""
         self.title = ""
+
     def crease_plot_template(self):
         plt.clf()
         plt.grid()
         plt.xlabel(self.x_label_name)
         plt.ylabel(self.y_label_name)
         plt.title(self.title)
+
     def create(self, total):
         pass
 
+
 class MonthDistancesPlotter(BasePlotter):
     def __init__(self, output_report_path, dates) -> None:
         super().__init__()
         self.output_report_path = f"{output_report_path}/distance.png"
         self.x_label_name = f"logs from {dates[0]} to {dates[-1]}"
         self.y_label_name = "total distance, km"
 
@@ -71,14 +77,15 @@
 
         lists = sorted(self.month_distances.items())
         x, y = zip(*lists)
         plt.bar(x, y)
 
         plt.savefig(self.output_report_path)
 
+
 class MonthFlightTimePlotter(BasePlotter):
     def __init__(self, output_report_path, dates) -> None:
         super().__init__()
         self.output_report_path = f'{output_report_path}/month_flight_time.png'
         self.x_label_name = f"logs from {dates[0]} to {dates[-1]}"
         self.y_label_name = "total flight time, hours"
 
@@ -96,14 +103,15 @@
 
         lists = sorted(self.month_flight_time.items())
         x, y = zip(*lists)
         plt.bar(x, y)
 
         plt.savefig(self.output_report_path)
 
+
 class CrashDistancePlotter(BasePlotter):
     def __init__(self, output_report_path, dates) -> None:
         super().__init__()
         self.output_report_path = f'{output_report_path}/distance_between_crashes.png'
         self.x_label_name = f"logs from {dates[0]} to {dates[-1]}"
         self.y_label_name = "total distance, km"
         self.title = ""
@@ -169,31 +177,32 @@
 
     def get_total_distance(self):
         return self.total_dist_from_all_logs_km
 
     def get_total_flight_time(self):
         return self.total_flight_time_minutes
 
+
 def flight_distance(input_logs_path, dates, output_build_path, output_report_path):
     log_info(f"The script config:\n- Input {input_logs_path},\n- Output is {output_build_path}.")
     logs_pathes = get_log_names(input_logs_path, verbose=False)
 
     stats_estimator = FlightStatsEstimator(len(logs_pathes), output_build_path)
     month_distances_plotter = MonthDistancesPlotter(output_report_path, dates)
     month_flight_time_plotter = MonthFlightTimePlotter(output_report_path, dates)
     crash_distance_plotter = CrashDistancePlotter(output_report_path, dates)
 
     for log_path in logs_pathes:
         month_num, day_num = extract_date_from_log_path(log_path)
 
         dist_km, flight_time_minutes = stats_estimator.process_log(log_path)
         month_distances_plotter.process(month_num, dist_km)
-        month_flight_time_plotter.process(month_num, flight_time_minutes/60)
+        month_flight_time_plotter.process(month_num, flight_time_minutes / 60)
         crash_distance_plotter.process(day_num, dist_km)
-    print("") # new line
+    print("")  # new line
 
     total_dist_km = int(stats_estimator.get_total_distance())
     if total_dist_km == 0:
         log_warn("There is no any log or total distance is 0. Skip plot creating.")
         sys.exit()
 
     month_distances_plotter.create(total_dist_km)
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/ice.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/ice.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 import matplotlib.pyplot as plt
 from .extract import extract_args
 from .uorb_topics import ActuatorOutputs
 
 MINIMAL_DURATION_SEC = 5.0
 
+
 def get_desired_time_limit(state_timestamps, states):
     first_work_timestamp = state_timestamps[-1]
     for idx, state in enumerate(states):
         if state == 2:
             first_work_timestamp = state_timestamps[idx]
             break
     last_work_timestamp = state_timestamps[0]
@@ -20,14 +21,15 @@
 
     if last_work_timestamp < first_work_timestamp:
         print(f'Wrong timestamp. From {first_work_timestamp} to {last_work_timestamp}')
         return None, None
 
     return first_work_timestamp, last_work_timestamp
 
+
 def get_most_useful_time_limit(state_timestamps, states):
     longest_repeating_counter = 0
     longest_repeating_last_idx = 0
     repeating_counter = 0
     for idx, state in enumerate(states):
         if state == 2:
             repeating_counter += 1
@@ -42,32 +44,35 @@
 
     duration_sec = (last_work_timestamp - first_work_timestamp) * 1e-6
     if duration_sec < MINIMAL_DURATION_SEC:
         print(f'Wrong timestamp. From {first_work_timestamp} to {last_work_timestamp}.')
         return None, None
     return first_work_timestamp, last_work_timestamp
 
+
 def clamp_dataset(timestamps, data, first_work_timestamp, last_work_timestamp):
     first_rpm_idx = len(timestamps) - 1
     for idx, timestamp in enumerate(timestamps):
         if timestamp > first_work_timestamp:
             first_rpm_idx = idx
             break
     last_rpm_idx = len(timestamps) - 1
 
     for idx, timestamp in reversed(list(enumerate(timestamps))):
         if timestamps[idx] < last_work_timestamp:
             last_rpm_idx = idx
             break
-    timestamps = timestamps[first_rpm_idx : last_rpm_idx]
-    data = data[first_rpm_idx : last_rpm_idx]
+    timestamps = timestamps[first_rpm_idx: last_rpm_idx]
+    data = data[first_rpm_idx: last_rpm_idx]
     return timestamps, data
 
+
 def fit_func(x, b, c):
-    return b * x**2 + c * x
+    return b * x ** 2 + c * x
+
 
 def ice(in_log_path, out_path, out_report_path):
     if in_log_path is None or len(in_log_path) == 0:
         return
 
     log_path_splitted = in_log_path.split('/')
     log_name = f"{log_path_splitted[-2]}/{log_path_splitted[-1]}"[0:-4]
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/uorb_topics.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/uorb_topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,76 +1,88 @@
 #!/usr/bin/env python3
 from .device_id_parser import parse_device_id
 
+
 class UorbTopic:
     ref_alt = 0
+
     def __init__(self, args, need_plot=False) -> None:
         self.args = args
         self.need_plot = need_plot
         self.data = tuple([] for _ in range(len(args)))
+
     def append_data(self, data):
         self.data = data
 
+
 class EstimatorLocalPositionRefAlt(UorbTopic):
     def append_data(self, data):
         self.data = data
         UorbTopic.ref_alt = self.data[1][0]
 
+
 class DistanceSensor(UorbTopic):
     def append_data(self, data):
         self.data = data
         for idx in range(len(self.data[1])):
             if self.data[1][idx] > 70:
                 self.data[1][idx] = 0
             self.data[1][idx] *= -1
 
+
 class VehicleGpsPosition(UorbTopic):
     def append_data(self, data):
         self.data = data
         for idx in range(len(self.data[1])):
             self.data[1][idx] /= 1000
             self.data[1][idx] = UorbTopic.ref_alt - self.data[1][idx]
 
+
 class VehicleAirDataBaroAltMeter(UorbTopic):
     def append_data(self, data):
         self.data = data
         baro_offset = self.data[1][0]
         for idx in range(len(self.data[1])):
             self.data[1][idx] -= baro_offset
             self.data[1][idx] *= -1
 
+
 class SensorGps(UorbTopic):
     def append_data(self, data):
         if len(data[2]) == 0:
             return
 
         self.data = data
         device_id = int(sum(self.data[2]) / len(self.data[2]))
         parse_device_id(device_id, verbose=True)
         for idx in range(len(self.data[1])):
             self.data[1][idx] /= 1000
             self.data[1][idx] = UorbTopic.ref_alt - self.data[1][idx]
 
+
 class ActuatorOutputs(UorbTopic):
     def __init__(self, args=("timestamp", "output[7]"), need_plot=False) -> None:
         super().__init__(args, need_plot)
         self.msg = "actuator_outputs_0"
         self.values = {}
         for arg in self.args:
             self.values[arg] = []
+
     def fill_values(self):
         for idx, arg in enumerate(self.args):
             self.values[arg] = self.data[idx]
+
     def append_data(self, data):
         self.data = data
         for idx in range(len(self.data[1])):
             if self.data[1][idx] == 65535:
                 self.data[1][idx] = 0
         self.fill_values()
 
+
 class EscStatus(UorbTopic):
     def __init__(self, args=("timestamp",
                              "esc[0].esc_rpm",
                              "esc[1].esc_rpm",
                              "esc[2].esc_rpm",
                              "esc[3].esc_rpm",
                              "esc[0].esc_voltage",
@@ -78,16 +90,18 @@
                              "esc[2].esc_voltage",
                              "esc[3].esc_voltage"), need_plot=False) -> None:
         super().__init__(args, need_plot)
         self.msg = "esc_status_0"
         self.values = {}
         for arg in self.args:
             self.values[arg] = []
+
     def fill_values(self):
         for idx, arg in enumerate(self.args):
             self.values[arg] = self.data[idx]
+
     def append_data(self, data):
         self.data = data
         for idx in range(len(self.data[1])):
             if self.data[1][idx] == 65535:
                 self.data[1][idx] = 0
         self.fill_values()
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/log_analyzer/utils.py` & `autopilot_tools-0.3.0/src/autopilot_tools/log_analyzer/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 #!/usr/bin/env python3
 import sys
 import os
 from glob import glob
 from .color_logging import log_info, log_warn
 
+
 def get_log_names(path, verbose=False):
     result = [y for x in os.walk(path) for y in glob(os.path.join(x[0], '*.ulg'))]
     result.sort()
     if verbose:
         log_info("List of log pathes:")
         for log_idx, log_res in enumerate(result):
             log_info(f"{log_idx}. {log_res}")
         print("")
 
     return result
 
+
 def extract_date_from_date_string(date_string):
     """Example: `2021.12.31`"""
     try:
         splitted_date = date_string.split(".")
         year = int(splitted_date[0])
         month = int(splitted_date[1])
         day = int(splitted_date[2])
         month_num = (year - 2021) * 12 + month
         day_num = month_num * 31 + day
     except ValueError as err:
         log_warn(f"Can't extract the date from the log {err}.")
         sys.exit()
     return month_num, day_num
 
+
 def extract_date_from_log_path(path):
     """assume that every month has 31 days to simplify the model"""
     date_string = path.split("/")[-2]
     return extract_date_from_date_string(date_string)
 
+
 # def log_name_from_full_path(log_path):
 #     splited_log_path = log_path.split("/", 10)
 #     log_name = splited_log_path[-1]
 #     log_name_without_extension = os.path.splitext(log_name)[0]
 #     return log_name_without_extension
 
 def log_name_from_full_path(log_path):
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools/px4/px_uploader.py` & `autopilot_tools-0.3.0/src/autopilot_tools/px4/px_uploader.py`

 * *Files identical despite different names*

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools.egg-info/PKG-INFO` & `autopilot_tools-0.3.0/src/autopilot_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: autopilot-tools
-Version: 0.1.0
-Summary: PX4/ArduPilot MAVLink usefull tools
+Version: 0.3.0
+Summary: PX4/ArduPilot autopilot tools
 Author-email: Dmitry Ponomarev <PonomarevDA96@gmail.com>
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/PonomarevDA/autopilot_tools
+Project-URL: Bug Tracker, https://github.com/PonomarevDA/autopilot_tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PX4/ArduPilot Autopilot tools ![](https://badge.fury.io/py/autopilot-tools.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/build_package.yml/badge.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/pylint.yml/badge.svg) ![badge](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/tests.yml/badge.svg)
+# PX4/ArduPilot Autopilot tools ![](https://badge.fury.io/py/autopilot-tools.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/build_package.yml/badge.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/pylint.yml/badge.svg) ![](https://github.com/PonomarevDA/autopilot_tools/actions/workflows/tests.yml/badge.svg)
 
 This repository is a collection of scripts created to facilitate automated work with the PX4/ArduPilot, such as:
 1. Upload a specific firmware to the autopilot via a link or given binaries
 2. Reset the autopilot to default and configure the required parameters
 3. Upload and run a mission
 4. Download the last flight log
 5. Analyze the flight log
@@ -39,14 +39,15 @@
 The script below could be used as part of a CI process and it illustrates the main functionality of the package:
 
 ```python
 from autopilot_tools.vehicle import Vehicle
 from autopilot_tools.analyzer import Analyzer
 
 vehicle = Vehicle()
+vehicle.connect(device="serial")
 vehicle.upload_firmware(firmware_path_or_url)
 vehicle.configure(params_path)
 vehicle.load_mission(mission_path)
 
 res = vehicle.run_mission(mission_path)
 print(res)
```

### Comparing `autopilot_tools-0.1.0/src/autopilot_tools.egg-info/SOURCES.txt` & `autopilot_tools-0.3.0/src/autopilot_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
+src/autopilot_tools/__init__.py
 src/autopilot_tools/analyzer.py
+src/autopilot_tools/exceptions.py
+src/autopilot_tools/utils.py
 src/autopilot_tools/vehicle.py
 src/autopilot_tools.egg-info/PKG-INFO
 src/autopilot_tools.egg-info/SOURCES.txt
 src/autopilot_tools.egg-info/dependency_links.txt
 src/autopilot_tools.egg-info/requires.txt
 src/autopilot_tools.egg-info/top_level.txt
 src/autopilot_tools/configurator/__init__.py
+src/autopilot_tools/configurator/ftp_filesystem.py
+src/autopilot_tools/configurator/mavftputils.py
 src/autopilot_tools/configurator/mavlink_params.py
+src/autopilot_tools/configurator/mission_file.py
+src/autopilot_tools/configurator/mission_result.py
 src/autopilot_tools/log_analyzer/__init__.py
 src/autopilot_tools/log_analyzer/airspeed.py
 src/autopilot_tools/log_analyzer/altitude.py
 src/autopilot_tools/log_analyzer/color_logging.py
 src/autopilot_tools/log_analyzer/device_id_parser.py
 src/autopilot_tools/log_analyzer/esc_status.py
 src/autopilot_tools/log_analyzer/extract.py
```

### Comparing `autopilot_tools-0.1.0/tests/test_mavlink_params.py` & `autopilot_tools-0.3.0/tests/test_mavlink_params.py`

 * *Files identical despite different names*

### Comparing `autopilot_tools-0.1.0/tests/test_vehicle.py` & `autopilot_tools-0.3.0/tests/test_vehicle.py`

 * *Files identical despite different names*

