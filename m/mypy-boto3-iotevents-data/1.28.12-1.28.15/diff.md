# Comparing `tmp/mypy-boto3-iotevents-data-1.28.12.tar.gz` & `tmp/mypy-boto3-iotevents-data-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotevents-data-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
+gzip compressed data, was "mypy-boto3-iotevents-data-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
```

## Comparing `mypy-boto3-iotevents-data-1.28.12.tar` & `mypy-boto3-iotevents-data-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.428483 mypy-boto3-iotevents-data-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-data-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-07-27 05:34:49.428483 mypy-boto3-iotevents-data-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-data-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.428483 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-07-27 05:24:04.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-27 05:24:04.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-07-27 05:24:04.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-27 05:24:04.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-07-27 05:24:04.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18821 2023-07-27 05:24:04.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.428483 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:49.000000 mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.428483 mypy-boto3-iotevents-data-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 05:24:03.000000 mypy-boto3-iotevents-data-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.457257 mypy-boto3-iotevents-data-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-07-28 20:42:59.457257 mypy-boto3-iotevents-data-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12855 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.449257 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-07-28 20:28:25.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-28 20:28:25.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-07-28 20:28:25.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18797 2023-07-28 20:28:25.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.457257 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:59.000000 mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.457257 mypy-boto3-iotevents-data-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:28:24.000000 mypy-boto3-iotevents-data-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotevents-data-1.28.12/LICENSE` & `mypy-boto3-iotevents-data-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.28.12/PKG-INFO` & `mypy-boto3-iotevents-data-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents-data
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTEventsData 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTEventsData 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents-data)](https://pepy.tech/project/mypy-boto3-iotevents-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEventsData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
+[boto3.IoTEventsData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotevents-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,14 +306,15 @@
 
 ```python
 from mypy_boto3_iotevents_data.type_defs import (
     AcknowledgeActionConfigurationTypeDef,
     AcknowledgeAlarmActionRequestTypeDef,
     AlarmSummaryTypeDef,
     BatchAlarmActionErrorEntryTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteDetectorErrorEntryTypeDef,
     DeleteDetectorRequestTypeDef,
     DisableAlarmActionRequestTypeDef,
     EnableAlarmActionRequestTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     ResetAlarmActionRequestTypeDef,
     SnoozeAlarmActionRequestTypeDef,
@@ -328,24 +329,23 @@
     VariableDefinitionTypeDef,
     DetectorStateSummaryTypeDef,
     TimerTypeDef,
     VariableTypeDef,
     ListAlarmsRequestRequestTypeDef,
     ListDetectorsRequestRequestTypeDef,
     TimestampValueTypeDef,
-    ResponseMetadataTypeDef,
     SimpleRuleEvaluationTypeDef,
     StateChangeConfigurationTypeDef,
     BatchAcknowledgeAlarmRequestRequestTypeDef,
-    ListAlarmsResponseTypeDef,
     BatchAcknowledgeAlarmResponseTypeDef,
     BatchDisableAlarmResponseTypeDef,
     BatchEnableAlarmResponseTypeDef,
     BatchResetAlarmResponseTypeDef,
     BatchSnoozeAlarmResponseTypeDef,
+    ListAlarmsResponseTypeDef,
     BatchDeleteDetectorResponseTypeDef,
     BatchDeleteDetectorRequestRequestTypeDef,
     BatchDisableAlarmRequestRequestTypeDef,
     BatchEnableAlarmRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchResetAlarmRequestRequestTypeDef,
     BatchSnoozeAlarmRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iotevents-data-1.28.12/README.md` & `mypy-boto3-iotevents-data-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents-data)](https://pepy.tech/project/mypy-boto3-iotevents-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEventsData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
+[boto3.IoTEventsData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotevents-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,14 +274,15 @@
 
 ```python
 from mypy_boto3_iotevents_data.type_defs import (
     AcknowledgeActionConfigurationTypeDef,
     AcknowledgeAlarmActionRequestTypeDef,
     AlarmSummaryTypeDef,
     BatchAlarmActionErrorEntryTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteDetectorErrorEntryTypeDef,
     DeleteDetectorRequestTypeDef,
     DisableAlarmActionRequestTypeDef,
     EnableAlarmActionRequestTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     ResetAlarmActionRequestTypeDef,
     SnoozeAlarmActionRequestTypeDef,
@@ -296,24 +297,23 @@
     VariableDefinitionTypeDef,
     DetectorStateSummaryTypeDef,
     TimerTypeDef,
     VariableTypeDef,
     ListAlarmsRequestRequestTypeDef,
     ListDetectorsRequestRequestTypeDef,
     TimestampValueTypeDef,
-    ResponseMetadataTypeDef,
     SimpleRuleEvaluationTypeDef,
     StateChangeConfigurationTypeDef,
     BatchAcknowledgeAlarmRequestRequestTypeDef,
-    ListAlarmsResponseTypeDef,
     BatchAcknowledgeAlarmResponseTypeDef,
     BatchDisableAlarmResponseTypeDef,
     BatchEnableAlarmResponseTypeDef,
     BatchResetAlarmResponseTypeDef,
     BatchSnoozeAlarmResponseTypeDef,
+    ListAlarmsResponseTypeDef,
     BatchDeleteDetectorResponseTypeDef,
     BatchDeleteDetectorRequestRequestTypeDef,
     BatchDisableAlarmRequestRequestTypeDef,
     BatchEnableAlarmRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchResetAlarmRequestRequestTypeDef,
     BatchSnoozeAlarmRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/__main__.py` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTEventsData 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTEventsData 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/client.py` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/client.pyi` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/literals.py` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/literals.pyi` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/type_defs.py` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 
 __all__ = (
     "AcknowledgeActionConfigurationTypeDef",
     "AcknowledgeAlarmActionRequestTypeDef",
     "AlarmSummaryTypeDef",
     "BatchAlarmActionErrorEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteDetectorErrorEntryTypeDef",
     "DeleteDetectorRequestTypeDef",
     "DisableAlarmActionRequestTypeDef",
     "EnableAlarmActionRequestTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "ResetAlarmActionRequestTypeDef",
     "SnoozeAlarmActionRequestTypeDef",
@@ -57,24 +58,23 @@
     "VariableDefinitionTypeDef",
     "DetectorStateSummaryTypeDef",
     "TimerTypeDef",
     "VariableTypeDef",
     "ListAlarmsRequestRequestTypeDef",
     "ListDetectorsRequestRequestTypeDef",
     "TimestampValueTypeDef",
-    "ResponseMetadataTypeDef",
     "SimpleRuleEvaluationTypeDef",
     "StateChangeConfigurationTypeDef",
     "BatchAcknowledgeAlarmRequestRequestTypeDef",
-    "ListAlarmsResponseTypeDef",
     "BatchAcknowledgeAlarmResponseTypeDef",
     "BatchDisableAlarmResponseTypeDef",
     "BatchEnableAlarmResponseTypeDef",
     "BatchResetAlarmResponseTypeDef",
     "BatchSnoozeAlarmResponseTypeDef",
+    "ListAlarmsResponseTypeDef",
     "BatchDeleteDetectorResponseTypeDef",
     "BatchDeleteDetectorRequestRequestTypeDef",
     "BatchDisableAlarmRequestRequestTypeDef",
     "BatchEnableAlarmRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "BatchResetAlarmRequestRequestTypeDef",
     "BatchSnoozeAlarmRequestRequestTypeDef",
@@ -147,14 +147,25 @@
         "requestId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 BatchDeleteDetectorErrorEntryTypeDef = TypedDict(
     "BatchDeleteDetectorErrorEntryTypeDef",
     {
         "messageId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
@@ -460,25 +471,14 @@
     "TimestampValueTypeDef",
     {
         "timeInMillis": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 SimpleRuleEvaluationTypeDef = TypedDict(
     "SimpleRuleEvaluationTypeDef",
     {
         "inputPropertyValue": str,
         "operator": ComparisonOperatorType,
         "thresholdValue": str,
     },
@@ -496,68 +496,68 @@
 BatchAcknowledgeAlarmRequestRequestTypeDef = TypedDict(
     "BatchAcknowledgeAlarmRequestRequestTypeDef",
     {
         "acknowledgeActionRequests": Sequence[AcknowledgeAlarmActionRequestTypeDef],
     },
 )
 
-ListAlarmsResponseTypeDef = TypedDict(
-    "ListAlarmsResponseTypeDef",
-    {
-        "alarmSummaries": List[AlarmSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchAcknowledgeAlarmResponseTypeDef = TypedDict(
     "BatchAcknowledgeAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisableAlarmResponseTypeDef = TypedDict(
     "BatchDisableAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEnableAlarmResponseTypeDef = TypedDict(
     "BatchEnableAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchResetAlarmResponseTypeDef = TypedDict(
     "BatchResetAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchSnoozeAlarmResponseTypeDef = TypedDict(
     "BatchSnoozeAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlarmsResponseTypeDef = TypedDict(
+    "ListAlarmsResponseTypeDef",
+    {
+        "alarmSummaries": List[AlarmSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteDetectorResponseTypeDef = TypedDict(
     "BatchDeleteDetectorResponseTypeDef",
     {
         "batchDeleteDetectorErrorEntries": List[BatchDeleteDetectorErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteDetectorRequestRequestTypeDef = TypedDict(
     "BatchDeleteDetectorRequestRequestTypeDef",
     {
         "detectors": Sequence[DeleteDetectorRequestTypeDef],
@@ -578,15 +578,15 @@
     },
 )
 
 BatchPutMessageResponseTypeDef = TypedDict(
     "BatchPutMessageResponseTypeDef",
     {
         "BatchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchResetAlarmRequestRequestTypeDef = TypedDict(
     "BatchResetAlarmRequestRequestTypeDef",
     {
         "resetActionRequests": Sequence[ResetAlarmActionRequestTypeDef],
@@ -600,15 +600,15 @@
     },
 )
 
 BatchUpdateDetectorResponseTypeDef = TypedDict(
     "BatchUpdateDetectorResponseTypeDef",
     {
         "batchUpdateDetectorErrorEntries": List[BatchUpdateDetectorErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomerActionTypeDef = TypedDict(
     "CustomerActionTypeDef",
     {
         "actionName": CustomerActionNameType,
@@ -714,15 +714,15 @@
 
 
 ListDetectorsResponseTypeDef = TypedDict(
     "ListDetectorsResponseTypeDef",
     {
         "detectorSummaries": List[DetectorSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectorTypeDef = TypedDict(
     "DetectorTypeDef",
     {
         "detectorModelName": str,
@@ -760,15 +760,15 @@
     },
 )
 
 DescribeDetectorResponseTypeDef = TypedDict(
     "DescribeDetectorResponseTypeDef",
     {
         "detector": DetectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "alarmModelName": str,
@@ -782,10 +782,10 @@
     total=False,
 )
 
 DescribeAlarmResponseTypeDef = TypedDict(
     "DescribeAlarmResponseTypeDef",
     {
         "alarm": AlarmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data/type_defs.pyi` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcknowledgeActionConfigurationTypeDef",
     "AcknowledgeAlarmActionRequestTypeDef",
     "AlarmSummaryTypeDef",
     "BatchAlarmActionErrorEntryTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteDetectorErrorEntryTypeDef",
     "DeleteDetectorRequestTypeDef",
     "DisableAlarmActionRequestTypeDef",
     "EnableAlarmActionRequestTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "ResetAlarmActionRequestTypeDef",
     "SnoozeAlarmActionRequestTypeDef",
@@ -56,24 +57,23 @@
     "VariableDefinitionTypeDef",
     "DetectorStateSummaryTypeDef",
     "TimerTypeDef",
     "VariableTypeDef",
     "ListAlarmsRequestRequestTypeDef",
     "ListDetectorsRequestRequestTypeDef",
     "TimestampValueTypeDef",
-    "ResponseMetadataTypeDef",
     "SimpleRuleEvaluationTypeDef",
     "StateChangeConfigurationTypeDef",
     "BatchAcknowledgeAlarmRequestRequestTypeDef",
-    "ListAlarmsResponseTypeDef",
     "BatchAcknowledgeAlarmResponseTypeDef",
     "BatchDisableAlarmResponseTypeDef",
     "BatchEnableAlarmResponseTypeDef",
     "BatchResetAlarmResponseTypeDef",
     "BatchSnoozeAlarmResponseTypeDef",
+    "ListAlarmsResponseTypeDef",
     "BatchDeleteDetectorResponseTypeDef",
     "BatchDeleteDetectorRequestRequestTypeDef",
     "BatchDisableAlarmRequestRequestTypeDef",
     "BatchEnableAlarmRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "BatchResetAlarmRequestRequestTypeDef",
     "BatchSnoozeAlarmRequestRequestTypeDef",
@@ -144,14 +144,25 @@
         "requestId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 BatchDeleteDetectorErrorEntryTypeDef = TypedDict(
     "BatchDeleteDetectorErrorEntryTypeDef",
     {
         "messageId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
@@ -439,25 +450,14 @@
     "TimestampValueTypeDef",
     {
         "timeInMillis": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 SimpleRuleEvaluationTypeDef = TypedDict(
     "SimpleRuleEvaluationTypeDef",
     {
         "inputPropertyValue": str,
         "operator": ComparisonOperatorType,
         "thresholdValue": str,
     },
@@ -475,68 +475,68 @@
 BatchAcknowledgeAlarmRequestRequestTypeDef = TypedDict(
     "BatchAcknowledgeAlarmRequestRequestTypeDef",
     {
         "acknowledgeActionRequests": Sequence[AcknowledgeAlarmActionRequestTypeDef],
     },
 )
 
-ListAlarmsResponseTypeDef = TypedDict(
-    "ListAlarmsResponseTypeDef",
-    {
-        "alarmSummaries": List[AlarmSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchAcknowledgeAlarmResponseTypeDef = TypedDict(
     "BatchAcknowledgeAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisableAlarmResponseTypeDef = TypedDict(
     "BatchDisableAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEnableAlarmResponseTypeDef = TypedDict(
     "BatchEnableAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchResetAlarmResponseTypeDef = TypedDict(
     "BatchResetAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchSnoozeAlarmResponseTypeDef = TypedDict(
     "BatchSnoozeAlarmResponseTypeDef",
     {
         "errorEntries": List[BatchAlarmActionErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlarmsResponseTypeDef = TypedDict(
+    "ListAlarmsResponseTypeDef",
+    {
+        "alarmSummaries": List[AlarmSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteDetectorResponseTypeDef = TypedDict(
     "BatchDeleteDetectorResponseTypeDef",
     {
         "batchDeleteDetectorErrorEntries": List[BatchDeleteDetectorErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteDetectorRequestRequestTypeDef = TypedDict(
     "BatchDeleteDetectorRequestRequestTypeDef",
     {
         "detectors": Sequence[DeleteDetectorRequestTypeDef],
@@ -557,15 +557,15 @@
     },
 )
 
 BatchPutMessageResponseTypeDef = TypedDict(
     "BatchPutMessageResponseTypeDef",
     {
         "BatchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchResetAlarmRequestRequestTypeDef = TypedDict(
     "BatchResetAlarmRequestRequestTypeDef",
     {
         "resetActionRequests": Sequence[ResetAlarmActionRequestTypeDef],
@@ -579,15 +579,15 @@
     },
 )
 
 BatchUpdateDetectorResponseTypeDef = TypedDict(
     "BatchUpdateDetectorResponseTypeDef",
     {
         "batchUpdateDetectorErrorEntries": List[BatchUpdateDetectorErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomerActionTypeDef = TypedDict(
     "CustomerActionTypeDef",
     {
         "actionName": CustomerActionNameType,
@@ -689,15 +689,15 @@
     pass
 
 ListDetectorsResponseTypeDef = TypedDict(
     "ListDetectorsResponseTypeDef",
     {
         "detectorSummaries": List[DetectorSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectorTypeDef = TypedDict(
     "DetectorTypeDef",
     {
         "detectorModelName": str,
@@ -735,15 +735,15 @@
     },
 )
 
 DescribeDetectorResponseTypeDef = TypedDict(
     "DescribeDetectorResponseTypeDef",
     {
         "detector": DetectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "alarmModelName": str,
@@ -757,10 +757,10 @@
     total=False,
 )
 
 DescribeAlarmResponseTypeDef = TypedDict(
     "DescribeAlarmResponseTypeDef",
     {
         "alarm": AlarmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/PKG-INFO` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotevents-data
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTEventsData 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTEventsData 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotevents-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotevents-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotevents-data)](https://pepy.tech/project/mypy-boto3-iotevents-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTEventsData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
+[boto3.IoTEventsData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#IoTEventsData)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotevents-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotevents_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,14 +306,15 @@
 
 ```python
 from mypy_boto3_iotevents_data.type_defs import (
     AcknowledgeActionConfigurationTypeDef,
     AcknowledgeAlarmActionRequestTypeDef,
     AlarmSummaryTypeDef,
     BatchAlarmActionErrorEntryTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteDetectorErrorEntryTypeDef,
     DeleteDetectorRequestTypeDef,
     DisableAlarmActionRequestTypeDef,
     EnableAlarmActionRequestTypeDef,
     BatchPutMessageErrorEntryTypeDef,
     ResetAlarmActionRequestTypeDef,
     SnoozeAlarmActionRequestTypeDef,
@@ -328,24 +329,23 @@
     VariableDefinitionTypeDef,
     DetectorStateSummaryTypeDef,
     TimerTypeDef,
     VariableTypeDef,
     ListAlarmsRequestRequestTypeDef,
     ListDetectorsRequestRequestTypeDef,
     TimestampValueTypeDef,
-    ResponseMetadataTypeDef,
     SimpleRuleEvaluationTypeDef,
     StateChangeConfigurationTypeDef,
     BatchAcknowledgeAlarmRequestRequestTypeDef,
-    ListAlarmsResponseTypeDef,
     BatchAcknowledgeAlarmResponseTypeDef,
     BatchDisableAlarmResponseTypeDef,
     BatchEnableAlarmResponseTypeDef,
     BatchResetAlarmResponseTypeDef,
     BatchSnoozeAlarmResponseTypeDef,
+    ListAlarmsResponseTypeDef,
     BatchDeleteDetectorResponseTypeDef,
     BatchDeleteDetectorRequestRequestTypeDef,
     BatchDisableAlarmRequestRequestTypeDef,
     BatchEnableAlarmRequestRequestTypeDef,
     BatchPutMessageResponseTypeDef,
     BatchResetAlarmRequestRequestTypeDef,
     BatchSnoozeAlarmRequestRequestTypeDef,
```

### Comparing `mypy-boto3-iotevents-data-1.28.12/mypy_boto3_iotevents_data.egg-info/SOURCES.txt` & `mypy-boto3-iotevents-data-1.28.15/mypy_boto3_iotevents_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotevents-data-1.28.12/setup.py` & `mypy-boto3-iotevents-data-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotevents-data",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotevents_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTEventsData 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTEventsData 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

