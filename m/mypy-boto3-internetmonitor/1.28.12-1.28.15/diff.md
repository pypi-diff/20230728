# Comparing `tmp/mypy-boto3-internetmonitor-1.28.12.tar.gz` & `tmp/mypy-boto3-internetmonitor-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-internetmonitor-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
+gzip compressed data, was "mypy-boto3-internetmonitor-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
```

## Comparing `mypy-boto3-internetmonitor-1.28.12.tar` & `mypy-boto3-internetmonitor-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.560489 mypy-boto3-internetmonitor-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-07-27 05:34:47.560489 mypy-boto3-internetmonitor-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.556489 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-07-27 05:23:40.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13326 2023-07-27 05:23:40.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:39.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.560489 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:47.000000 mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.560489 mypy-boto3-internetmonitor-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-27 05:23:38.000000 mypy-boto3-internetmonitor-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.409215 mypy-boto3-internetmonitor-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-28 20:42:56.409215 mypy-boto3-internetmonitor-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12957 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.409215 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-07-28 20:27:52.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.409215 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-28 20:42:56.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:42:56.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:56.000000 mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.409215 mypy-boto3-internetmonitor-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-28 20:27:51.000000 mypy-boto3-internetmonitor-1.28.15/setup.py
```

### Comparing `mypy-boto3-internetmonitor-1.28.12/LICENSE` & `mypy-boto3-internetmonitor-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.12/PKG-INFO` & `mypy-boto3-internetmonitor-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,42 +330,39 @@
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
-    CreateMonitorOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
-    HealthEventsConfigOutputTypeDef,
-    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHealthEventsInputRequestTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     NetworkTypeDef,
-    PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CreateMonitorOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    GetMonitorOutputTypeDef,
     CreateMonitorInputRequestTypeDef,
+    GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.12/README.md` & `mypy-boto3-internetmonitor-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,42 +298,39 @@
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
-    CreateMonitorOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
-    HealthEventsConfigOutputTypeDef,
-    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHealthEventsInputRequestTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     NetworkTypeDef,
-    PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CreateMonitorOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    GetMonitorOutputTypeDef,
     CreateMonitorInputRequestTypeDef,
+    GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__init__.py` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__init__.pyi` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/__main__.py` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
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

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/client.py` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/client.pyi` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/literals.py` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/literals.pyi` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/paginator.py` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,28 +55,28 @@
     def paginate(
         self,
         *,
         MonitorName: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         EventStatus: HealthEventStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHealthEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listhealtheventspaginator)
         """
 
 
 class ListMonitorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listmonitorspaginator)
     """
 
     def paginate(
-        self, *, MonitorStatus: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MonitorStatus: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMonitorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listmonitorspaginator)
         """
```

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/paginator.pyi` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,27 +52,27 @@
     def paginate(
         self,
         *,
         MonitorName: str,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         EventStatus: HealthEventStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHealthEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listhealtheventspaginator)
         """
 
 class ListMonitorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listmonitorspaginator)
     """
 
     def paginate(
-        self, *, MonitorStatus: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MonitorStatus: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMonitorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/paginators/#listmonitorspaginator)
         """
```

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/type_defs.py` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,42 +29,39 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AvailabilityMeasurementTypeDef",
     "HealthEventsConfigTypeDef",
-    "CreateMonitorOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
-    "HealthEventsConfigOutputTypeDef",
-    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
-    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListHealthEventsInputRequestTypeDef",
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "NetworkTypeDef",
-    "PaginatorConfigTypeDef",
     "RoundTripTimeTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "CreateMonitorOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
-    "InternetMeasurementsLogDeliveryOutputTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
+    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
-    "GetMonitorOutputTypeDef",
     "CreateMonitorInputRequestTypeDef",
+    "GetMonitorOutputTypeDef",
     "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
     "ImpactedLocationTypeDef",
     "GetHealthEventOutputTypeDef",
     "HealthEventTypeDef",
     "ListHealthEventsOutputTypeDef",
 )
@@ -84,20 +81,22 @@
     {
         "AvailabilityScoreThreshold": float,
         "PerformanceScoreThreshold": float,
     },
     total=False,
 )
 
-CreateMonitorOutputTypeDef = TypedDict(
-    "CreateMonitorOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "Status": MonitorConfigStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteMonitorInputRequestTypeDef = TypedDict(
     "DeleteMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
@@ -115,68 +114,34 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
-HealthEventsConfigOutputTypeDef = TypedDict(
-    "HealthEventsConfigOutputTypeDef",
-    {
-        "AvailabilityScoreThreshold": float,
-        "PerformanceScoreThreshold": float,
-    },
-    total=False,
-)
-
-S3ConfigOutputTypeDef = TypedDict(
-    "S3ConfigOutputTypeDef",
-    {
-        "BucketName": str,
-        "BucketPrefix": str,
-        "LogDeliveryStatus": LogDeliveryStatusType,
-    },
-    total=False,
-)
-
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
     total=False,
 )
 
-_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
-    "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
-    "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "EventStatus": HealthEventStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListHealthEventsInputListHealthEventsPaginateTypeDef(
-    _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
-    _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListHealthEventsInputRequestTypeDef = TypedDict(
     "_RequiredListHealthEventsInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalListHealthEventsInputRequestTypeDef = TypedDict(
@@ -194,23 +159,14 @@
 
 class ListHealthEventsInputRequestTypeDef(
     _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
 ):
     pass
 
 
-ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
-    {
-        "MonitorStatus": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMonitorsInputRequestTypeDef = TypedDict(
     "ListMonitorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "MonitorStatus": str,
     },
@@ -241,61 +197,32 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkTypeDef = TypedDict(
     "NetworkTypeDef",
     {
         "ASName": str,
         "ASNumber": int,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 RoundTripTimeTypeDef = TypedDict(
     "RoundTripTimeTypeDef",
     {
         "P50": float,
         "P90": float,
         "P95": float,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -304,45 +231,88 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+CreateMonitorOutputTypeDef = TypedDict(
+    "CreateMonitorOutputTypeDef",
+    {
+        "Arn": str,
+        "Status": MonitorConfigStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateMonitorOutputTypeDef = TypedDict(
     "UpdateMonitorOutputTypeDef",
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InternetMeasurementsLogDeliveryOutputTypeDef = TypedDict(
-    "InternetMeasurementsLogDeliveryOutputTypeDef",
+InternetMeasurementsLogDeliveryTypeDef = TypedDict(
+    "InternetMeasurementsLogDeliveryTypeDef",
     {
-        "S3Config": S3ConfigOutputTypeDef,
+        "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
 
-InternetMeasurementsLogDeliveryTypeDef = TypedDict(
-    "InternetMeasurementsLogDeliveryTypeDef",
+_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
+    "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
     {
-        "S3Config": S3ConfigTypeDef,
+        "MonitorName": str,
+    },
+)
+_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
+    "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "EventStatus": HealthEventStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListHealthEventsInputListHealthEventsPaginateTypeDef(
+    _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
+    _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
+):
+    pass
+
+
+ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    {
+        "MonitorStatus": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMonitorsOutputTypeDef = TypedDict(
     "ListMonitorsOutputTypeDef",
     {
         "Monitors": List[MonitorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkImpairmentTypeDef = TypedDict(
     "NetworkImpairmentTypeDef",
     {
         "Networks": List[NetworkTypeDef],
@@ -358,34 +328,14 @@
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
         "RoundTripTime": RoundTripTimeTypeDef,
     },
     total=False,
 )
 
-GetMonitorOutputTypeDef = TypedDict(
-    "GetMonitorOutputTypeDef",
-    {
-        "MonitorName": str,
-        "MonitorArn": str,
-        "Resources": List[str],
-        "Status": MonitorConfigStateType,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "ProcessingStatus": MonitorProcessingStatusCodeType,
-        "ProcessingStatusInfo": str,
-        "Tags": Dict[str, str],
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryOutputTypeDef,
-        "TrafficPercentageToMonitor": int,
-        "HealthEventsConfig": HealthEventsConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalCreateMonitorInputRequestTypeDef = TypedDict(
@@ -405,14 +355,34 @@
 
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
     pass
 
 
+GetMonitorOutputTypeDef = TypedDict(
+    "GetMonitorOutputTypeDef",
+    {
+        "MonitorName": str,
+        "MonitorArn": str,
+        "Resources": List[str],
+        "Status": MonitorConfigStateType,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "ProcessingStatus": MonitorProcessingStatusCodeType,
+        "ProcessingStatusInfo": str,
+        "Tags": Dict[str, str],
+        "MaxCityNetworksToMonitor": int,
+        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
+        "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalUpdateMonitorInputRequestTypeDef = TypedDict(
@@ -487,15 +457,15 @@
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "ImpactedLocations": List[ImpactedLocationTypeDef],
         "Status": HealthEventStatusType,
         "PercentOfTotalTrafficImpacted": float,
         "ImpactType": HealthEventImpactTypeType,
         "HealthScoreThreshold": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHealthEventTypeDef = TypedDict(
     "_RequiredHealthEventTypeDef",
     {
         "EventArn": str,
@@ -524,10 +494,10 @@
 
 
 ListHealthEventsOutputTypeDef = TypedDict(
     "ListHealthEventsOutputTypeDef",
     {
         "HealthEvents": List[HealthEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor/type_defs.pyi` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -28,42 +28,39 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AvailabilityMeasurementTypeDef",
     "HealthEventsConfigTypeDef",
-    "CreateMonitorOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
-    "HealthEventsConfigOutputTypeDef",
-    "S3ConfigOutputTypeDef",
     "S3ConfigTypeDef",
-    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListHealthEventsInputRequestTypeDef",
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "NetworkTypeDef",
-    "PaginatorConfigTypeDef",
     "RoundTripTimeTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "CreateMonitorOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
-    "InternetMeasurementsLogDeliveryOutputTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
+    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
-    "GetMonitorOutputTypeDef",
     "CreateMonitorInputRequestTypeDef",
+    "GetMonitorOutputTypeDef",
     "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
     "ImpactedLocationTypeDef",
     "GetHealthEventOutputTypeDef",
     "HealthEventTypeDef",
     "ListHealthEventsOutputTypeDef",
 )
@@ -83,20 +80,22 @@
     {
         "AvailabilityScoreThreshold": float,
         "PerformanceScoreThreshold": float,
     },
     total=False,
 )
 
-CreateMonitorOutputTypeDef = TypedDict(
-    "CreateMonitorOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "Status": MonitorConfigStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteMonitorInputRequestTypeDef = TypedDict(
     "DeleteMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
@@ -114,66 +113,34 @@
 GetMonitorInputRequestTypeDef = TypedDict(
     "GetMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 
-HealthEventsConfigOutputTypeDef = TypedDict(
-    "HealthEventsConfigOutputTypeDef",
-    {
-        "AvailabilityScoreThreshold": float,
-        "PerformanceScoreThreshold": float,
-    },
-    total=False,
-)
-
-S3ConfigOutputTypeDef = TypedDict(
-    "S3ConfigOutputTypeDef",
-    {
-        "BucketName": str,
-        "BucketPrefix": str,
-        "LogDeliveryStatus": LogDeliveryStatusType,
-    },
-    total=False,
-)
-
 S3ConfigTypeDef = TypedDict(
     "S3ConfigTypeDef",
     {
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
     total=False,
 )
 
-_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
-    "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
-    "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "EventStatus": HealthEventStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListHealthEventsInputListHealthEventsPaginateTypeDef(
-    _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
-    _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredListHealthEventsInputRequestTypeDef = TypedDict(
     "_RequiredListHealthEventsInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalListHealthEventsInputRequestTypeDef = TypedDict(
@@ -189,23 +156,14 @@
 )
 
 class ListHealthEventsInputRequestTypeDef(
     _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
 ):
     pass
 
-ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
-    {
-        "MonitorStatus": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMonitorsInputRequestTypeDef = TypedDict(
     "ListMonitorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "MonitorStatus": str,
     },
@@ -234,61 +192,32 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkTypeDef = TypedDict(
     "NetworkTypeDef",
     {
         "ASName": str,
         "ASNumber": int,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 RoundTripTimeTypeDef = TypedDict(
     "RoundTripTimeTypeDef",
     {
         "P50": float,
         "P90": float,
         "P95": float,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -297,45 +226,86 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+CreateMonitorOutputTypeDef = TypedDict(
+    "CreateMonitorOutputTypeDef",
+    {
+        "Arn": str,
+        "Status": MonitorConfigStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateMonitorOutputTypeDef = TypedDict(
     "UpdateMonitorOutputTypeDef",
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InternetMeasurementsLogDeliveryOutputTypeDef = TypedDict(
-    "InternetMeasurementsLogDeliveryOutputTypeDef",
+InternetMeasurementsLogDeliveryTypeDef = TypedDict(
+    "InternetMeasurementsLogDeliveryTypeDef",
     {
-        "S3Config": S3ConfigOutputTypeDef,
+        "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
 
-InternetMeasurementsLogDeliveryTypeDef = TypedDict(
-    "InternetMeasurementsLogDeliveryTypeDef",
+_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
+    "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
     {
-        "S3Config": S3ConfigTypeDef,
+        "MonitorName": str,
+    },
+)
+_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
+    "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
+    {
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "EventStatus": HealthEventStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListHealthEventsInputListHealthEventsPaginateTypeDef(
+    _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
+    _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
+):
+    pass
+
+ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    {
+        "MonitorStatus": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMonitorsOutputTypeDef = TypedDict(
     "ListMonitorsOutputTypeDef",
     {
         "Monitors": List[MonitorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkImpairmentTypeDef = TypedDict(
     "NetworkImpairmentTypeDef",
     {
         "Networks": List[NetworkTypeDef],
@@ -351,34 +321,14 @@
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
         "RoundTripTime": RoundTripTimeTypeDef,
     },
     total=False,
 )
 
-GetMonitorOutputTypeDef = TypedDict(
-    "GetMonitorOutputTypeDef",
-    {
-        "MonitorName": str,
-        "MonitorArn": str,
-        "Resources": List[str],
-        "Status": MonitorConfigStateType,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-        "ProcessingStatus": MonitorProcessingStatusCodeType,
-        "ProcessingStatusInfo": str,
-        "Tags": Dict[str, str],
-        "MaxCityNetworksToMonitor": int,
-        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryOutputTypeDef,
-        "TrafficPercentageToMonitor": int,
-        "HealthEventsConfig": HealthEventsConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredCreateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalCreateMonitorInputRequestTypeDef = TypedDict(
@@ -396,14 +346,34 @@
 )
 
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
     pass
 
+GetMonitorOutputTypeDef = TypedDict(
+    "GetMonitorOutputTypeDef",
+    {
+        "MonitorName": str,
+        "MonitorArn": str,
+        "Resources": List[str],
+        "Status": MonitorConfigStateType,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+        "ProcessingStatus": MonitorProcessingStatusCodeType,
+        "ProcessingStatusInfo": str,
+        "Tags": Dict[str, str],
+        "MaxCityNetworksToMonitor": int,
+        "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
+        "TrafficPercentageToMonitor": int,
+        "HealthEventsConfig": HealthEventsConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
     },
 )
 _OptionalUpdateMonitorInputRequestTypeDef = TypedDict(
@@ -474,15 +444,15 @@
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "ImpactedLocations": List[ImpactedLocationTypeDef],
         "Status": HealthEventStatusType,
         "PercentOfTotalTrafficImpacted": float,
         "ImpactType": HealthEventImpactTypeType,
         "HealthScoreThreshold": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHealthEventTypeDef = TypedDict(
     "_RequiredHealthEventTypeDef",
     {
         "EventArn": str,
@@ -509,10 +479,10 @@
     pass
 
 ListHealthEventsOutputTypeDef = TypedDict(
     "ListHealthEventsOutputTypeDef",
     {
         "HealthEvents": List[HealthEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/PKG-INFO` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-internetmonitor
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudWatchInternetMonitor 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-internetmonitor.svg?color=blue)](https://pypi.org/project/mypy-boto3-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-internetmonitor)](https://pepy.tech/project/mypy-boto3-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchInternetMonitor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
+[boto3.CloudWatchInternetMonitor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [mypy-boto3-internetmonitor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_internetmonitor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,42 +330,39 @@
 `mypy_boto3_internetmonitor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
     HealthEventsConfigTypeDef,
-    CreateMonitorOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
-    HealthEventsConfigOutputTypeDef,
-    S3ConfigOutputTypeDef,
     S3ConfigTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHealthEventsInputRequestTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     NetworkTypeDef,
-    PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CreateMonitorOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
-    InternetMeasurementsLogDeliveryOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListMonitorsInputListMonitorsPaginateTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
-    GetMonitorOutputTypeDef,
     CreateMonitorInputRequestTypeDef,
+    GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
```

### Comparing `mypy-boto3-internetmonitor-1.28.12/mypy_boto3_internetmonitor.egg-info/SOURCES.txt` & `mypy-boto3-internetmonitor-1.28.15/mypy_boto3_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-internetmonitor-1.28.12/setup.py` & `mypy-boto3-internetmonitor-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-internetmonitor",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CloudWatchInternetMonitor 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

