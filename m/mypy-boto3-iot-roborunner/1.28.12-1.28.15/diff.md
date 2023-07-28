# Comparing `tmp/mypy-boto3-iot-roborunner-1.28.12.tar.gz` & `tmp/mypy-boto3-iot-roborunner-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-roborunner-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-roborunner-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
```

## Comparing `mypy-boto3-iot-roborunner-1.28.12.tar` & `mypy-boto3-iot-roborunner-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.000484 mypy-boto3-iot-roborunner-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-27 05:34:48.992484 mypy-boto3-iot-roborunner-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.992484 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21802 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:54.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.992484 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:48.000000 mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.000484 mypy-boto3-iot-roborunner-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-27 05:23:53.000000 mypy-boto3-iot-roborunner-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.349255 mypy-boto3-iot-roborunner-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-28 20:42:59.349255 mypy-boto3-iot-roborunner-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.349255 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20216 2023-07-28 20:28:12.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20177 2023-07-28 20:28:12.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.349255 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-28 20:42:59.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:59.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:59.000000 mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.349255 mypy-boto3-iot-roborunner-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-28 20:28:11.000000 mypy-boto3-iot-roborunner-1.28.15/setup.py
```

### Comparing `mypy-boto3-iot-roborunner-1.28.12/LICENSE` & `mypy-boto3-iot-roborunner-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.12/PKG-INFO` & `mypy-boto3-iot-roborunner-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-roborunner
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTRoboRunner 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTRoboRunner 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,72 +332,68 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
-    CartesianCoordinatesOutputTypeDef,
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    CreateDestinationResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
-    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
-    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
-    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
-    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
-    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    OrientationOutputTypeDef,
-    VendorPropertiesOutputTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDestinationsRequestRequestTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
-    UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
-    UpdateWorkerFleetResponseTypeDef,
-    PositionCoordinatesOutputTypeDef,
     PositionCoordinatesTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateSiteResponseTypeDef,
+    CreateWorkerFleetResponseTypeDef,
+    CreateWorkerResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetSiteResponseTypeDef,
+    GetWorkerFleetResponseTypeDef,
+    UpdateDestinationResponseTypeDef,
+    UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetResponseTypeDef,
     ListDestinationsResponseTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
+    CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
+    UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
-    CreateWorkerRequestRequestTypeDef,
-    UpdateWorkerRequestRequestTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesOutputTypeDef:
+def get_structure() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.12/README.md` & `mypy-boto3-iot-roborunner-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,72 +300,68 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
-    CartesianCoordinatesOutputTypeDef,
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    CreateDestinationResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
-    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
-    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
-    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
-    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
-    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    OrientationOutputTypeDef,
-    VendorPropertiesOutputTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDestinationsRequestRequestTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
-    UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
-    UpdateWorkerFleetResponseTypeDef,
-    PositionCoordinatesOutputTypeDef,
     PositionCoordinatesTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateSiteResponseTypeDef,
+    CreateWorkerFleetResponseTypeDef,
+    CreateWorkerResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetSiteResponseTypeDef,
+    GetWorkerFleetResponseTypeDef,
+    UpdateDestinationResponseTypeDef,
+    UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetResponseTypeDef,
     ListDestinationsResponseTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
+    CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
+    UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
-    CreateWorkerRequestRequestTypeDef,
-    UpdateWorkerRequestRequestTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesOutputTypeDef:
+def get_structure() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__init__.py` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__init__.pyi` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/__main__.py` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTRoboRunner 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTRoboRunner 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner\nOther"
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

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/client.py` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/client.pyi` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/literals.py` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/literals.pyi` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/paginator.py` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,80 +41,74 @@
 __all__ = (
     "ListDestinationsPaginator",
     "ListSitesPaginator",
     "ListWorkerFleetsPaginator",
     "ListWorkersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listdestinationspaginator)
     """
 
     def paginate(
         self,
         *,
         site: str,
         state: DestinationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listdestinationspaginator)
         """
 
-
 class ListSitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listsitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listsitespaginator)
         """
 
-
 class ListWorkerFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerfleetspaginator)
     """
 
     def paginate(
-        self, *, site: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, site: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkerFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerfleetspaginator)
         """
 
-
 class ListWorkersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerspaginator)
     """
 
     def paginate(
-        self, *, site: str, fleet: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, site: str, fleet: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerspaginator)
         """
```

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/paginator.pyi` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,74 +41,80 @@
 __all__ = (
     "ListDestinationsPaginator",
     "ListSitesPaginator",
     "ListWorkerFleetsPaginator",
     "ListWorkersPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listdestinationspaginator)
     """
 
     def paginate(
         self,
         *,
         site: str,
         state: DestinationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listdestinationspaginator)
         """
 
+
 class ListSitesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listsitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listsitespaginator)
         """
 
+
 class ListWorkerFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerfleetspaginator)
     """
 
     def paginate(
-        self, *, site: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, site: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkerFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerfleetspaginator)
         """
 
+
 class ListWorkersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerspaginator)
     """
 
     def paginate(
-        self, *, site: str, fleet: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, site: str, fleet: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/paginators/#listworkerspaginator)
         """
```

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/type_defs.py` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,110 +2,83 @@
 Type annotations for iot-roborunner service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesOutputTypeDef
+    from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
 
-    data: CartesianCoordinatesOutputTypeDef = {...}
+    data: CartesianCoordinatesTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import DestinationStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "CartesianCoordinatesOutputTypeDef",
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "CreateDestinationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSiteRequestRequestTypeDef",
-    "CreateSiteResponseTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
-    "CreateWorkerFleetResponseTypeDef",
     "OrientationTypeDef",
     "VendorPropertiesTypeDef",
-    "CreateWorkerResponseTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteSiteRequestRequestTypeDef",
     "DeleteWorkerFleetRequestRequestTypeDef",
     "DeleteWorkerRequestRequestTypeDef",
     "DestinationTypeDef",
     "GetDestinationRequestRequestTypeDef",
-    "GetDestinationResponseTypeDef",
     "GetSiteRequestRequestTypeDef",
-    "GetSiteResponseTypeDef",
     "GetWorkerFleetRequestRequestTypeDef",
-    "GetWorkerFleetResponseTypeDef",
     "GetWorkerRequestRequestTypeDef",
-    "OrientationOutputTypeDef",
-    "VendorPropertiesOutputTypeDef",
-    "ListDestinationsRequestListDestinationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDestinationsRequestRequestTypeDef",
-    "ListSitesRequestListSitesPaginateTypeDef",
     "ListSitesRequestRequestTypeDef",
     "SiteTypeDef",
-    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
     "ListWorkerFleetsRequestRequestTypeDef",
     "WorkerFleetTypeDef",
-    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListWorkersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
-    "UpdateDestinationResponseTypeDef",
     "UpdateSiteRequestRequestTypeDef",
-    "UpdateSiteResponseTypeDef",
     "UpdateWorkerFleetRequestRequestTypeDef",
-    "UpdateWorkerFleetResponseTypeDef",
-    "PositionCoordinatesOutputTypeDef",
     "PositionCoordinatesTypeDef",
+    "CreateDestinationResponseTypeDef",
+    "CreateSiteResponseTypeDef",
+    "CreateWorkerFleetResponseTypeDef",
+    "CreateWorkerResponseTypeDef",
+    "GetDestinationResponseTypeDef",
+    "GetSiteResponseTypeDef",
+    "GetWorkerFleetResponseTypeDef",
+    "UpdateDestinationResponseTypeDef",
+    "UpdateSiteResponseTypeDef",
+    "UpdateWorkerFleetResponseTypeDef",
     "ListDestinationsResponseTypeDef",
+    "ListDestinationsRequestListDestinationsPaginateTypeDef",
+    "ListSitesRequestListSitesPaginateTypeDef",
+    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListSitesResponseTypeDef",
     "ListWorkerFleetsResponseTypeDef",
+    "CreateWorkerRequestRequestTypeDef",
     "GetWorkerResponseTypeDef",
+    "UpdateWorkerRequestRequestTypeDef",
     "UpdateWorkerResponseTypeDef",
     "WorkerTypeDef",
-    "CreateWorkerRequestRequestTypeDef",
-    "UpdateWorkerRequestRequestTypeDef",
     "ListWorkersResponseTypeDef",
 )
 
-_RequiredCartesianCoordinatesOutputTypeDef = TypedDict(
-    "_RequiredCartesianCoordinatesOutputTypeDef",
-    {
-        "x": float,
-        "y": float,
-    },
-)
-_OptionalCartesianCoordinatesOutputTypeDef = TypedDict(
-    "_OptionalCartesianCoordinatesOutputTypeDef",
-    {
-        "z": float,
-    },
-    total=False,
-)
-
-
-class CartesianCoordinatesOutputTypeDef(
-    _RequiredCartesianCoordinatesOutputTypeDef, _OptionalCartesianCoordinatesOutputTypeDef
-):
-    pass
-
-
 _RequiredCartesianCoordinatesTypeDef = TypedDict(
     "_RequiredCartesianCoordinatesTypeDef",
     {
         "x": float,
         "y": float,
     },
 )
@@ -113,21 +86,19 @@
     "_OptionalCartesianCoordinatesTypeDef",
     {
         "z": float,
     },
     total=False,
 )
 
-
 class CartesianCoordinatesTypeDef(
     _RequiredCartesianCoordinatesTypeDef, _OptionalCartesianCoordinatesTypeDef
 ):
     pass
 
-
 _RequiredCreateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDestinationRequestRequestTypeDef",
     {
         "name": str,
         "site": str,
     },
 )
@@ -137,30 +108,27 @@
         "clientToken": str,
         "state": DestinationStateType,
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
-
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
-
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSiteRequestRequestTypeDef",
     {
         "name": str,
@@ -172,32 +140,19 @@
     {
         "clientToken": str,
         "description": str,
     },
     total=False,
 )
 
-
 class CreateSiteRequestRequestTypeDef(
     _RequiredCreateSiteRequestRequestTypeDef, _OptionalCreateSiteRequestRequestTypeDef
 ):
     pass
 
-
-CreateSiteResponseTypeDef = TypedDict(
-    "CreateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerFleetRequestRequestTypeDef",
     {
         "name": str,
         "site": str,
     },
 )
@@ -206,32 +161,19 @@
     {
         "clientToken": str,
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
-
 class CreateWorkerFleetRequestRequestTypeDef(
     _RequiredCreateWorkerFleetRequestRequestTypeDef, _OptionalCreateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
-
-CreateWorkerFleetResponseTypeDef = TypedDict(
-    "CreateWorkerFleetResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OrientationTypeDef = TypedDict(
     "OrientationTypeDef",
     {
         "degrees": float,
     },
     total=False,
 )
@@ -248,31 +190,17 @@
         "vendorWorkerIpAddress": str,
         "vendorAdditionalTransientProperties": str,
         "vendorAdditionalFixedProperties": str,
     },
     total=False,
 )
 
-
 class VendorPropertiesTypeDef(_RequiredVendorPropertiesTypeDef, _OptionalVendorPropertiesTypeDef):
     pass
 
-
-CreateWorkerResponseTypeDef = TypedDict(
-    "CreateWorkerResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "site": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -313,144 +241,55 @@
     "_OptionalDestinationTypeDef",
     {
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
-
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
-
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSiteRequestRequestTypeDef = TypedDict(
     "GetSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetSiteResponseTypeDef = TypedDict(
-    "GetSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkerFleetRequestRequestTypeDef = TypedDict(
     "GetWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetWorkerFleetResponseTypeDef = TypedDict(
-    "GetWorkerFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkerRequestRequestTypeDef = TypedDict(
     "GetWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-OrientationOutputTypeDef = TypedDict(
-    "OrientationOutputTypeDef",
-    {
-        "degrees": float,
-    },
-    total=False,
-)
-
-_RequiredVendorPropertiesOutputTypeDef = TypedDict(
-    "_RequiredVendorPropertiesOutputTypeDef",
-    {
-        "vendorWorkerId": str,
-    },
-)
-_OptionalVendorPropertiesOutputTypeDef = TypedDict(
-    "_OptionalVendorPropertiesOutputTypeDef",
-    {
-        "vendorWorkerIpAddress": str,
-        "vendorAdditionalTransientProperties": str,
-        "vendorAdditionalFixedProperties": str,
-    },
-    total=False,
-)
-
-
-class VendorPropertiesOutputTypeDef(
-    _RequiredVendorPropertiesOutputTypeDef, _OptionalVendorPropertiesOutputTypeDef
-):
-    pass
-
-
-_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "state": DestinationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDestinationsRequestListDestinationsPaginateTypeDef(
-    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
-    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListDestinationsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListDestinationsRequestRequestTypeDef = TypedDict(
@@ -459,29 +298,19 @@
         "maxResults": int,
         "nextToken": str,
         "state": DestinationStateType,
     },
     total=False,
 )
 
-
 class ListDestinationsRequestRequestTypeDef(
     _RequiredListDestinationsRequestRequestTypeDef, _OptionalListDestinationsRequestRequestTypeDef
 ):
     pass
 
-
-ListSitesRequestListSitesPaginateTypeDef = TypedDict(
-    "ListSitesRequestListSitesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSitesRequestRequestTypeDef = TypedDict(
     "ListSitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -493,36 +322,14 @@
         "arn": str,
         "name": str,
         "countryCode": str,
         "createdAt": datetime,
     },
 )
 
-_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
-    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkerFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkerFleetsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkerFleetsRequestRequestTypeDef = TypedDict(
@@ -530,21 +337,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListWorkerFleetsRequestRequestTypeDef(
     _RequiredListWorkerFleetsRequestRequestTypeDef, _OptionalListWorkerFleetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredWorkerFleetTypeDef = TypedDict(
     "_RequiredWorkerFleetTypeDef",
     {
         "arn": str,
         "id": str,
         "name": str,
         "site": str,
@@ -556,42 +361,17 @@
     "_OptionalWorkerFleetTypeDef",
     {
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
-
 class WorkerFleetTypeDef(_RequiredWorkerFleetTypeDef, _OptionalWorkerFleetTypeDef):
     pass
 
-
-_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "fleet": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkersRequestListWorkersPaginateTypeDef(
-    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
-    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkersRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkersRequestRequestTypeDef = TypedDict(
@@ -600,42 +380,19 @@
         "maxResults": int,
         "nextToken": str,
         "fleet": str,
     },
     total=False,
 )
 
-
 class ListWorkersRequestRequestTypeDef(
     _RequiredListWorkersRequestRequestTypeDef, _OptionalListWorkersRequestRequestTypeDef
 ):
     pass
 
-
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
 _RequiredUpdateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateDestinationRequestRequestTypeDef = TypedDict(
@@ -644,34 +401,19 @@
         "name": str,
         "state": DestinationStateType,
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
-
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
-
-UpdateDestinationResponseTypeDef = TypedDict(
-    "UpdateDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateSiteRequestRequestTypeDef = TypedDict(
@@ -680,34 +422,19 @@
         "name": str,
         "countryCode": str,
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateSiteRequestRequestTypeDef(
     _RequiredUpdateSiteRequestRequestTypeDef, _OptionalUpdateSiteRequestRequestTypeDef
 ):
     pass
 
-
-UpdateSiteResponseTypeDef = TypedDict(
-    "UpdateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
@@ -715,140 +442,250 @@
     {
         "name": str,
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
-
 class UpdateWorkerFleetRequestRequestTypeDef(
     _RequiredUpdateWorkerFleetRequestRequestTypeDef, _OptionalUpdateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
+PositionCoordinatesTypeDef = TypedDict(
+    "PositionCoordinatesTypeDef",
+    {
+        "cartesianCoordinates": CartesianCoordinatesTypeDef,
+    },
+    total=False,
+)
 
-UpdateWorkerFleetResponseTypeDef = TypedDict(
-    "UpdateWorkerFleetResponseTypeDef",
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
     {
         "arn": str,
         "id": str,
-        "name": str,
+        "createdAt": datetime,
         "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "state": DestinationStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PositionCoordinatesOutputTypeDef = TypedDict(
-    "PositionCoordinatesOutputTypeDef",
+CreateSiteResponseTypeDef = TypedDict(
+    "CreateSiteResponseTypeDef",
     {
-        "cartesianCoordinates": CartesianCoordinatesOutputTypeDef,
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-PositionCoordinatesTypeDef = TypedDict(
-    "PositionCoordinatesTypeDef",
+CreateWorkerFleetResponseTypeDef = TypedDict(
+    "CreateWorkerFleetResponseTypeDef",
     {
-        "cartesianCoordinates": CartesianCoordinatesTypeDef,
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListDestinationsResponseTypeDef = TypedDict(
-    "ListDestinationsResponseTypeDef",
+CreateWorkerResponseTypeDef = TypedDict(
+    "CreateWorkerResponseTypeDef",
     {
-        "nextToken": str,
-        "destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "site": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListSitesResponseTypeDef = TypedDict(
-    "ListSitesResponseTypeDef",
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
     {
-        "nextToken": str,
-        "sites": List[SiteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "id": str,
+        "name": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListWorkerFleetsResponseTypeDef = TypedDict(
-    "ListWorkerFleetsResponseTypeDef",
+GetSiteResponseTypeDef = TypedDict(
+    "GetSiteResponseTypeDef",
     {
-        "nextToken": str,
-        "workerFleets": List[WorkerFleetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetWorkerResponseTypeDef = TypedDict(
-    "GetWorkerResponseTypeDef",
+GetWorkerFleetResponseTypeDef = TypedDict(
+    "GetWorkerFleetResponseTypeDef",
     {
-        "arn": str,
         "id": str,
-        "fleet": str,
+        "arn": str,
+        "name": str,
         "site": str,
         "createdAt": datetime,
         "updatedAt": datetime,
-        "name": str,
-        "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesOutputTypeDef,
-        "position": PositionCoordinatesOutputTypeDef,
-        "orientation": OrientationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWorkerResponseTypeDef = TypedDict(
-    "UpdateWorkerResponseTypeDef",
+UpdateDestinationResponseTypeDef = TypedDict(
+    "UpdateDestinationResponseTypeDef",
     {
         "arn": str,
         "id": str,
-        "fleet": str,
-        "updatedAt": datetime,
         "name": str,
-        "additionalTransientProperties": str,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
         "additionalFixedProperties": str,
-        "orientation": OrientationOutputTypeDef,
-        "vendorProperties": VendorPropertiesOutputTypeDef,
-        "position": PositionCoordinatesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredWorkerTypeDef = TypedDict(
-    "_RequiredWorkerTypeDef",
+UpdateSiteResponseTypeDef = TypedDict(
+    "UpdateSiteResponseTypeDef",
     {
         "arn": str,
         "id": str,
-        "fleet": str,
-        "createdAt": datetime,
+        "name": str,
+        "countryCode": str,
+        "description": str,
         "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkerFleetResponseTypeDef = TypedDict(
+    "UpdateWorkerFleetResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
         "name": str,
+        "updatedAt": datetime,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDestinationsResponseTypeDef = TypedDict(
+    "ListDestinationsResponseTypeDef",
+    {
+        "nextToken": str,
+        "destinations": List[DestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
+    {
         "site": str,
     },
 )
-_OptionalWorkerTypeDef = TypedDict(
-    "_OptionalWorkerTypeDef",
+_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
     {
-        "additionalTransientProperties": str,
-        "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesOutputTypeDef,
-        "position": PositionCoordinatesOutputTypeDef,
-        "orientation": OrientationOutputTypeDef,
+        "state": DestinationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class ListDestinationsRequestListDestinationsPaginateTypeDef(
+    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
+    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
+):
+    pass
 
-class WorkerTypeDef(_RequiredWorkerTypeDef, _OptionalWorkerTypeDef):
+ListSitesRequestListSitesPaginateTypeDef = TypedDict(
+    "ListSitesRequestListSitesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
+    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+):
     pass
 
+_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "fleet": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListWorkersRequestListWorkersPaginateTypeDef(
+    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
+    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
+):
+    pass
+
+ListSitesResponseTypeDef = TypedDict(
+    "ListSitesResponseTypeDef",
+    {
+        "nextToken": str,
+        "sites": List[SiteTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListWorkerFleetsResponseTypeDef = TypedDict(
+    "ListWorkerFleetsResponseTypeDef",
+    {
+        "nextToken": str,
+        "workerFleets": List[WorkerFleetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerRequestRequestTypeDef",
     {
         "name": str,
         "fleet": str,
     },
@@ -862,20 +699,37 @@
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
     },
     total=False,
 )
 
-
 class CreateWorkerRequestRequestTypeDef(
     _RequiredCreateWorkerRequestRequestTypeDef, _OptionalCreateWorkerRequestRequestTypeDef
 ):
     pass
 
+GetWorkerResponseTypeDef = TypedDict(
+    "GetWorkerResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "fleet": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "name": str,
+        "additionalTransientProperties": str,
+        "additionalFixedProperties": str,
+        "vendorProperties": VendorPropertiesTypeDef,
+        "position": PositionCoordinatesTypeDef,
+        "orientation": OrientationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -888,22 +742,64 @@
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateWorkerRequestRequestTypeDef(
     _RequiredUpdateWorkerRequestRequestTypeDef, _OptionalUpdateWorkerRequestRequestTypeDef
 ):
     pass
 
+UpdateWorkerResponseTypeDef = TypedDict(
+    "UpdateWorkerResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "fleet": str,
+        "updatedAt": datetime,
+        "name": str,
+        "additionalTransientProperties": str,
+        "additionalFixedProperties": str,
+        "orientation": OrientationTypeDef,
+        "vendorProperties": VendorPropertiesTypeDef,
+        "position": PositionCoordinatesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredWorkerTypeDef = TypedDict(
+    "_RequiredWorkerTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "fleet": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "name": str,
+        "site": str,
+    },
+)
+_OptionalWorkerTypeDef = TypedDict(
+    "_OptionalWorkerTypeDef",
+    {
+        "additionalTransientProperties": str,
+        "additionalFixedProperties": str,
+        "vendorProperties": VendorPropertiesTypeDef,
+        "position": PositionCoordinatesTypeDef,
+        "orientation": OrientationTypeDef,
+    },
+    total=False,
+)
+
+class WorkerTypeDef(_RequiredWorkerTypeDef, _OptionalWorkerTypeDef):
+    pass
 
 ListWorkersResponseTypeDef = TypedDict(
     "ListWorkersResponseTypeDef",
     {
         "nextToken": str,
         "workers": List[WorkerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner/type_defs.pyi` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,107 +2,84 @@
 Type annotations for iot-roborunner service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesOutputTypeDef
+    from mypy_boto3_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
 
-    data: CartesianCoordinatesOutputTypeDef = {...}
+    data: CartesianCoordinatesTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import DestinationStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "CartesianCoordinatesOutputTypeDef",
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "CreateDestinationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSiteRequestRequestTypeDef",
-    "CreateSiteResponseTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
-    "CreateWorkerFleetResponseTypeDef",
     "OrientationTypeDef",
     "VendorPropertiesTypeDef",
-    "CreateWorkerResponseTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteSiteRequestRequestTypeDef",
     "DeleteWorkerFleetRequestRequestTypeDef",
     "DeleteWorkerRequestRequestTypeDef",
     "DestinationTypeDef",
     "GetDestinationRequestRequestTypeDef",
-    "GetDestinationResponseTypeDef",
     "GetSiteRequestRequestTypeDef",
-    "GetSiteResponseTypeDef",
     "GetWorkerFleetRequestRequestTypeDef",
-    "GetWorkerFleetResponseTypeDef",
     "GetWorkerRequestRequestTypeDef",
-    "OrientationOutputTypeDef",
-    "VendorPropertiesOutputTypeDef",
-    "ListDestinationsRequestListDestinationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDestinationsRequestRequestTypeDef",
-    "ListSitesRequestListSitesPaginateTypeDef",
     "ListSitesRequestRequestTypeDef",
     "SiteTypeDef",
-    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
     "ListWorkerFleetsRequestRequestTypeDef",
     "WorkerFleetTypeDef",
-    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListWorkersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
-    "UpdateDestinationResponseTypeDef",
     "UpdateSiteRequestRequestTypeDef",
-    "UpdateSiteResponseTypeDef",
     "UpdateWorkerFleetRequestRequestTypeDef",
-    "UpdateWorkerFleetResponseTypeDef",
-    "PositionCoordinatesOutputTypeDef",
     "PositionCoordinatesTypeDef",
+    "CreateDestinationResponseTypeDef",
+    "CreateSiteResponseTypeDef",
+    "CreateWorkerFleetResponseTypeDef",
+    "CreateWorkerResponseTypeDef",
+    "GetDestinationResponseTypeDef",
+    "GetSiteResponseTypeDef",
+    "GetWorkerFleetResponseTypeDef",
+    "UpdateDestinationResponseTypeDef",
+    "UpdateSiteResponseTypeDef",
+    "UpdateWorkerFleetResponseTypeDef",
     "ListDestinationsResponseTypeDef",
+    "ListDestinationsRequestListDestinationsPaginateTypeDef",
+    "ListSitesRequestListSitesPaginateTypeDef",
+    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListSitesResponseTypeDef",
     "ListWorkerFleetsResponseTypeDef",
+    "CreateWorkerRequestRequestTypeDef",
     "GetWorkerResponseTypeDef",
+    "UpdateWorkerRequestRequestTypeDef",
     "UpdateWorkerResponseTypeDef",
     "WorkerTypeDef",
-    "CreateWorkerRequestRequestTypeDef",
-    "UpdateWorkerRequestRequestTypeDef",
     "ListWorkersResponseTypeDef",
 )
 
-_RequiredCartesianCoordinatesOutputTypeDef = TypedDict(
-    "_RequiredCartesianCoordinatesOutputTypeDef",
-    {
-        "x": float,
-        "y": float,
-    },
-)
-_OptionalCartesianCoordinatesOutputTypeDef = TypedDict(
-    "_OptionalCartesianCoordinatesOutputTypeDef",
-    {
-        "z": float,
-    },
-    total=False,
-)
-
-class CartesianCoordinatesOutputTypeDef(
-    _RequiredCartesianCoordinatesOutputTypeDef, _OptionalCartesianCoordinatesOutputTypeDef
-):
-    pass
-
 _RequiredCartesianCoordinatesTypeDef = TypedDict(
     "_RequiredCartesianCoordinatesTypeDef",
     {
         "x": float,
         "y": float,
     },
 )
@@ -110,19 +87,21 @@
     "_OptionalCartesianCoordinatesTypeDef",
     {
         "z": float,
     },
     total=False,
 )
 
+
 class CartesianCoordinatesTypeDef(
     _RequiredCartesianCoordinatesTypeDef, _OptionalCartesianCoordinatesTypeDef
 ):
     pass
 
+
 _RequiredCreateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDestinationRequestRequestTypeDef",
     {
         "name": str,
         "site": str,
     },
 )
@@ -132,28 +111,29 @@
         "clientToken": str,
         "state": DestinationStateType,
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
+
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSiteRequestRequestTypeDef",
     {
         "name": str,
@@ -165,29 +145,20 @@
     {
         "clientToken": str,
         "description": str,
     },
     total=False,
 )
 
+
 class CreateSiteRequestRequestTypeDef(
     _RequiredCreateSiteRequestRequestTypeDef, _OptionalCreateSiteRequestRequestTypeDef
 ):
     pass
 
-CreateSiteResponseTypeDef = TypedDict(
-    "CreateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerFleetRequestRequestTypeDef",
     {
         "name": str,
         "site": str,
     },
@@ -197,29 +168,20 @@
     {
         "clientToken": str,
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
+
 class CreateWorkerFleetRequestRequestTypeDef(
     _RequiredCreateWorkerFleetRequestRequestTypeDef, _OptionalCreateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
-CreateWorkerFleetResponseTypeDef = TypedDict(
-    "CreateWorkerFleetResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 OrientationTypeDef = TypedDict(
     "OrientationTypeDef",
     {
         "degrees": float,
     },
     total=False,
@@ -237,28 +199,18 @@
         "vendorWorkerIpAddress": str,
         "vendorAdditionalTransientProperties": str,
         "vendorAdditionalFixedProperties": str,
     },
     total=False,
 )
 
+
 class VendorPropertiesTypeDef(_RequiredVendorPropertiesTypeDef, _OptionalVendorPropertiesTypeDef):
     pass
 
-CreateWorkerResponseTypeDef = TypedDict(
-    "CreateWorkerResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "site": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -300,138 +252,57 @@
     "_OptionalDestinationTypeDef",
     {
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
+
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
+
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSiteRequestRequestTypeDef = TypedDict(
     "GetSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetSiteResponseTypeDef = TypedDict(
-    "GetSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkerFleetRequestRequestTypeDef = TypedDict(
     "GetWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetWorkerFleetResponseTypeDef = TypedDict(
-    "GetWorkerFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkerRequestRequestTypeDef = TypedDict(
     "GetWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-OrientationOutputTypeDef = TypedDict(
-    "OrientationOutputTypeDef",
-    {
-        "degrees": float,
-    },
-    total=False,
-)
-
-_RequiredVendorPropertiesOutputTypeDef = TypedDict(
-    "_RequiredVendorPropertiesOutputTypeDef",
-    {
-        "vendorWorkerId": str,
-    },
-)
-_OptionalVendorPropertiesOutputTypeDef = TypedDict(
-    "_OptionalVendorPropertiesOutputTypeDef",
-    {
-        "vendorWorkerIpAddress": str,
-        "vendorAdditionalTransientProperties": str,
-        "vendorAdditionalFixedProperties": str,
-    },
-    total=False,
-)
-
-class VendorPropertiesOutputTypeDef(
-    _RequiredVendorPropertiesOutputTypeDef, _OptionalVendorPropertiesOutputTypeDef
-):
-    pass
-
-_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "state": DestinationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDestinationsRequestListDestinationsPaginateTypeDef(
-    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
-    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListDestinationsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListDestinationsRequestRequestTypeDef = TypedDict(
@@ -440,26 +311,20 @@
         "maxResults": int,
         "nextToken": str,
         "state": DestinationStateType,
     },
     total=False,
 )
 
+
 class ListDestinationsRequestRequestTypeDef(
     _RequiredListDestinationsRequestRequestTypeDef, _OptionalListDestinationsRequestRequestTypeDef
 ):
     pass
 
-ListSitesRequestListSitesPaginateTypeDef = TypedDict(
-    "ListSitesRequestListSitesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListSitesRequestRequestTypeDef = TypedDict(
     "ListSitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
@@ -472,34 +337,14 @@
         "arn": str,
         "name": str,
         "countryCode": str,
         "createdAt": datetime,
     },
 )
 
-_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
-    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkerFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkerFleetsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkerFleetsRequestRequestTypeDef = TypedDict(
@@ -507,19 +352,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListWorkerFleetsRequestRequestTypeDef(
     _RequiredListWorkerFleetsRequestRequestTypeDef, _OptionalListWorkerFleetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredWorkerFleetTypeDef = TypedDict(
     "_RequiredWorkerFleetTypeDef",
     {
         "arn": str,
         "id": str,
         "name": str,
         "site": str,
@@ -531,37 +378,18 @@
     "_OptionalWorkerFleetTypeDef",
     {
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
+
 class WorkerFleetTypeDef(_RequiredWorkerFleetTypeDef, _OptionalWorkerFleetTypeDef):
     pass
 
-_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "fleet": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkersRequestListWorkersPaginateTypeDef(
-    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
-    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
-):
-    pass
 
 _RequiredListWorkersRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersRequestRequestTypeDef",
     {
         "site": str,
     },
 )
@@ -571,39 +399,20 @@
         "maxResults": int,
         "nextToken": str,
         "fleet": str,
     },
     total=False,
 )
 
+
 class ListWorkersRequestRequestTypeDef(
     _RequiredListWorkersRequestRequestTypeDef, _OptionalListWorkersRequestRequestTypeDef
 ):
     pass
 
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
 
 _RequiredUpdateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -613,31 +422,20 @@
         "name": str,
         "state": DestinationStateType,
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
+
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
-UpdateDestinationResponseTypeDef = TypedDict(
-    "UpdateDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -647,31 +445,20 @@
         "name": str,
         "countryCode": str,
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateSiteRequestRequestTypeDef(
     _RequiredUpdateSiteRequestRequestTypeDef, _OptionalUpdateSiteRequestRequestTypeDef
 ):
     pass
 
-UpdateSiteResponseTypeDef = TypedDict(
-    "UpdateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -680,137 +467,259 @@
     {
         "name": str,
         "additionalFixedProperties": str,
     },
     total=False,
 )
 
+
 class UpdateWorkerFleetRequestRequestTypeDef(
     _RequiredUpdateWorkerFleetRequestRequestTypeDef, _OptionalUpdateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
-UpdateWorkerFleetResponseTypeDef = TypedDict(
-    "UpdateWorkerFleetResponseTypeDef",
+
+PositionCoordinatesTypeDef = TypedDict(
+    "PositionCoordinatesTypeDef",
+    {
+        "cartesianCoordinates": CartesianCoordinatesTypeDef,
+    },
+    total=False,
+)
+
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
     {
         "arn": str,
         "id": str,
-        "name": str,
+        "createdAt": datetime,
         "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "state": DestinationStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PositionCoordinatesOutputTypeDef = TypedDict(
-    "PositionCoordinatesOutputTypeDef",
+CreateSiteResponseTypeDef = TypedDict(
+    "CreateSiteResponseTypeDef",
     {
-        "cartesianCoordinates": CartesianCoordinatesOutputTypeDef,
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-PositionCoordinatesTypeDef = TypedDict(
-    "PositionCoordinatesTypeDef",
+CreateWorkerFleetResponseTypeDef = TypedDict(
+    "CreateWorkerFleetResponseTypeDef",
     {
-        "cartesianCoordinates": CartesianCoordinatesTypeDef,
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListDestinationsResponseTypeDef = TypedDict(
-    "ListDestinationsResponseTypeDef",
+CreateWorkerResponseTypeDef = TypedDict(
+    "CreateWorkerResponseTypeDef",
     {
-        "nextToken": str,
-        "destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "site": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListSitesResponseTypeDef = TypedDict(
-    "ListSitesResponseTypeDef",
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
     {
-        "nextToken": str,
-        "sites": List[SiteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "id": str,
+        "name": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListWorkerFleetsResponseTypeDef = TypedDict(
-    "ListWorkerFleetsResponseTypeDef",
+GetSiteResponseTypeDef = TypedDict(
+    "GetSiteResponseTypeDef",
     {
-        "nextToken": str,
-        "workerFleets": List[WorkerFleetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetWorkerResponseTypeDef = TypedDict(
-    "GetWorkerResponseTypeDef",
+GetWorkerFleetResponseTypeDef = TypedDict(
+    "GetWorkerFleetResponseTypeDef",
     {
-        "arn": str,
         "id": str,
-        "fleet": str,
+        "arn": str,
+        "name": str,
         "site": str,
         "createdAt": datetime,
         "updatedAt": datetime,
-        "name": str,
-        "additionalTransientProperties": str,
         "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesOutputTypeDef,
-        "position": PositionCoordinatesOutputTypeDef,
-        "orientation": OrientationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWorkerResponseTypeDef = TypedDict(
-    "UpdateWorkerResponseTypeDef",
+UpdateDestinationResponseTypeDef = TypedDict(
+    "UpdateDestinationResponseTypeDef",
     {
         "arn": str,
         "id": str,
-        "fleet": str,
-        "updatedAt": datetime,
         "name": str,
-        "additionalTransientProperties": str,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
         "additionalFixedProperties": str,
-        "orientation": OrientationOutputTypeDef,
-        "vendorProperties": VendorPropertiesOutputTypeDef,
-        "position": PositionCoordinatesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredWorkerTypeDef = TypedDict(
-    "_RequiredWorkerTypeDef",
+UpdateSiteResponseTypeDef = TypedDict(
+    "UpdateSiteResponseTypeDef",
     {
         "arn": str,
         "id": str,
-        "fleet": str,
-        "createdAt": datetime,
+        "name": str,
+        "countryCode": str,
+        "description": str,
         "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkerFleetResponseTypeDef = TypedDict(
+    "UpdateWorkerFleetResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
         "name": str,
+        "updatedAt": datetime,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDestinationsResponseTypeDef = TypedDict(
+    "ListDestinationsResponseTypeDef",
+    {
+        "nextToken": str,
+        "destinations": List[DestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
+    {
         "site": str,
     },
 )
-_OptionalWorkerTypeDef = TypedDict(
-    "_OptionalWorkerTypeDef",
+_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
     {
-        "additionalTransientProperties": str,
-        "additionalFixedProperties": str,
-        "vendorProperties": VendorPropertiesOutputTypeDef,
-        "position": PositionCoordinatesOutputTypeDef,
-        "orientation": OrientationOutputTypeDef,
+        "state": DestinationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class WorkerTypeDef(_RequiredWorkerTypeDef, _OptionalWorkerTypeDef):
+
+class ListDestinationsRequestListDestinationsPaginateTypeDef(
+    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
+    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
+):
     pass
 
+
+ListSitesRequestListSitesPaginateTypeDef = TypedDict(
+    "ListSitesRequestListSitesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
+    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "fleet": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWorkersRequestListWorkersPaginateTypeDef(
+    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
+    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
+):
+    pass
+
+
+ListSitesResponseTypeDef = TypedDict(
+    "ListSitesResponseTypeDef",
+    {
+        "nextToken": str,
+        "sites": List[SiteTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListWorkerFleetsResponseTypeDef = TypedDict(
+    "ListWorkerFleetsResponseTypeDef",
+    {
+        "nextToken": str,
+        "workerFleets": List[WorkerFleetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerRequestRequestTypeDef",
     {
         "name": str,
         "fleet": str,
     },
 )
@@ -823,19 +732,40 @@
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
     },
     total=False,
 )
 
+
 class CreateWorkerRequestRequestTypeDef(
     _RequiredCreateWorkerRequestRequestTypeDef, _OptionalCreateWorkerRequestRequestTypeDef
 ):
     pass
 
+
+GetWorkerResponseTypeDef = TypedDict(
+    "GetWorkerResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "fleet": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "name": str,
+        "additionalTransientProperties": str,
+        "additionalFixedProperties": str,
+        "vendorProperties": VendorPropertiesTypeDef,
+        "position": PositionCoordinatesTypeDef,
+        "orientation": OrientationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateWorkerRequestRequestTypeDef = TypedDict(
@@ -847,20 +777,68 @@
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateWorkerRequestRequestTypeDef(
     _RequiredUpdateWorkerRequestRequestTypeDef, _OptionalUpdateWorkerRequestRequestTypeDef
 ):
     pass
 
+
+UpdateWorkerResponseTypeDef = TypedDict(
+    "UpdateWorkerResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "fleet": str,
+        "updatedAt": datetime,
+        "name": str,
+        "additionalTransientProperties": str,
+        "additionalFixedProperties": str,
+        "orientation": OrientationTypeDef,
+        "vendorProperties": VendorPropertiesTypeDef,
+        "position": PositionCoordinatesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredWorkerTypeDef = TypedDict(
+    "_RequiredWorkerTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "fleet": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "name": str,
+        "site": str,
+    },
+)
+_OptionalWorkerTypeDef = TypedDict(
+    "_OptionalWorkerTypeDef",
+    {
+        "additionalTransientProperties": str,
+        "additionalFixedProperties": str,
+        "vendorProperties": VendorPropertiesTypeDef,
+        "position": PositionCoordinatesTypeDef,
+        "orientation": OrientationTypeDef,
+    },
+    total=False,
+)
+
+
+class WorkerTypeDef(_RequiredWorkerTypeDef, _OptionalWorkerTypeDef):
+    pass
+
+
 ListWorkersResponseTypeDef = TypedDict(
     "ListWorkersResponseTypeDef",
     {
         "nextToken": str,
         "workers": List[WorkerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/PKG-INFO` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-roborunner
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTRoboRunner 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTRoboRunner 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-roborunner.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-roborunner)](https://pepy.tech/project/mypy-boto3-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTRoboRunner 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
+[boto3.IoTRoboRunner 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [mypy-boto3-iot-roborunner docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_roborunner/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,72 +332,68 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot_roborunner.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_roborunner.type_defs import (
-    CartesianCoordinatesOutputTypeDef,
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    CreateDestinationResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
-    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
-    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
-    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
-    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
-    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    OrientationOutputTypeDef,
-    VendorPropertiesOutputTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDestinationsRequestRequestTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
-    UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
-    UpdateWorkerFleetResponseTypeDef,
-    PositionCoordinatesOutputTypeDef,
     PositionCoordinatesTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateSiteResponseTypeDef,
+    CreateWorkerFleetResponseTypeDef,
+    CreateWorkerResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetSiteResponseTypeDef,
+    GetWorkerFleetResponseTypeDef,
+    UpdateDestinationResponseTypeDef,
+    UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetResponseTypeDef,
     ListDestinationsResponseTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
+    CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
+    UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
-    CreateWorkerRequestRequestTypeDef,
-    UpdateWorkerRequestRequestTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesOutputTypeDef:
+def get_structure() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-roborunner-1.28.12/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt` & `mypy-boto3-iot-roborunner-1.28.15/mypy_boto3_iot_roborunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-roborunner-1.28.12/setup.py` & `mypy-boto3-iot-roborunner-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot-roborunner",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iot_roborunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTRoboRunner 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTRoboRunner 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

