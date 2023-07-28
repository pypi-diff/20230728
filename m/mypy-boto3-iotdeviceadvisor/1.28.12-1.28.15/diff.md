# Comparing `tmp/mypy-boto3-iotdeviceadvisor-1.28.12.tar.gz` & `tmp/mypy-boto3-iotdeviceadvisor-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
+gzip compressed data, was "mypy-boto3-iotdeviceadvisor-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
```

## Comparing `mypy-boto3-iotdeviceadvisor-1.28.12.tar` & `mypy-boto3-iotdeviceadvisor-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-27 05:24:00.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-27 05:24:00.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-07-27 05:24:00.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-27 05:24:00.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:49.000000 mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.292483 mypy-boto3-iotdeviceadvisor-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-27 05:23:59.000000 mypy-boto3-iotdeviceadvisor-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.409256 mypy-boto3-iotdeviceadvisor-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-07-28 20:42:59.405256 mypy-boto3-iotdeviceadvisor-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.401256 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-07-28 20:28:20.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.405256 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:59.000000 mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.409256 mypy-boto3-iotdeviceadvisor-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-28 20:28:19.000000 mypy-boto3-iotdeviceadvisor-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/LICENSE` & `mypy-boto3-iotdeviceadvisor-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,55 +303,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
-    CreateSuiteDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
-    DeviceUnderTestOutputTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
-    GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
     ListSuiteDefinitionsRequestRequestTypeDef,
     ListSuiteRunsRequestRequestTypeDef,
     SuiteRunInformationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
-    StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateSuiteDefinitionResponseTypeDef,
+    GetEndpointResponseTypeDef,
+    GetSuiteRunReportResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSuiteRunResponseTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
     SuiteDefinitionConfigurationOutputTypeDef,
+    SuiteDefinitionConfigurationTypeDef,
     SuiteDefinitionInformationTypeDef,
     SuiteRunConfigurationOutputTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
     GetSuiteDefinitionResponseTypeDef,
-    ListSuiteDefinitionsResponseTypeDef,
     CreateSuiteDefinitionRequestRequestTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
+    ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> CreateSuiteDefinitionResponseTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/README.md` & `mypy-boto3-iotdeviceadvisor-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,55 +271,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
-    CreateSuiteDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
-    DeviceUnderTestOutputTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
-    GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
     ListSuiteDefinitionsRequestRequestTypeDef,
     ListSuiteRunsRequestRequestTypeDef,
     SuiteRunInformationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
-    StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateSuiteDefinitionResponseTypeDef,
+    GetEndpointResponseTypeDef,
+    GetSuiteRunReportResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSuiteRunResponseTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
     SuiteDefinitionConfigurationOutputTypeDef,
+    SuiteDefinitionConfigurationTypeDef,
     SuiteDefinitionInformationTypeDef,
     SuiteRunConfigurationOutputTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
     GetSuiteDefinitionResponseTypeDef,
-    ListSuiteDefinitionsResponseTypeDef,
     CreateSuiteDefinitionRequestRequestTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
+    ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> CreateSuiteDefinitionResponseTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/__main__.py` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTDeviceAdvisor 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor\nOther"
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

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/client.py` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/client.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/literals.py` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/literals.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/type_defs.py` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotdeviceadvisor service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotdeviceadvisor.type_defs import CreateSuiteDefinitionResponseTypeDef
+    from mypy_boto3_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
-    data: CreateSuiteDefinitionResponseTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -25,83 +25,71 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "CreateSuiteDefinitionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
-    "DeviceUnderTestOutputTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
-    "GetEndpointResponseTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
-    "GetSuiteRunReportResponseTypeDef",
     "GetSuiteRunRequestRequestTypeDef",
     "ListSuiteDefinitionsRequestRequestTypeDef",
     "ListSuiteRunsRequestRequestTypeDef",
     "SuiteRunInformationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartSuiteRunResponseTypeDef",
     "StopSuiteRunRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestCaseScenarioTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateSuiteDefinitionResponseTypeDef",
+    "GetEndpointResponseTypeDef",
+    "GetSuiteRunReportResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartSuiteRunResponseTypeDef",
     "UpdateSuiteDefinitionResponseTypeDef",
     "SuiteDefinitionConfigurationOutputTypeDef",
+    "SuiteDefinitionConfigurationTypeDef",
     "SuiteDefinitionInformationTypeDef",
     "SuiteRunConfigurationOutputTypeDef",
-    "SuiteDefinitionConfigurationTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
     "GetSuiteDefinitionResponseTypeDef",
-    "ListSuiteDefinitionsResponseTypeDef",
     "CreateSuiteDefinitionRequestRequestTypeDef",
     "UpdateSuiteDefinitionRequestRequestTypeDef",
+    "ListSuiteDefinitionsResponseTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
-CreateSuiteDefinitionResponseTypeDef = TypedDict(
-    "CreateSuiteDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionName": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
     },
 )
 
-DeviceUnderTestOutputTypeDef = TypedDict(
-    "DeviceUnderTestOutputTypeDef",
-    {
-        "thingArn": str,
-        "certificateArn": str,
-        "deviceRoleArn": str,
-    },
-    total=False,
-)
-
 DeviceUnderTestTypeDef = TypedDict(
     "DeviceUnderTestTypeDef",
     {
         "thingArn": str,
         "certificateArn": str,
         "deviceRoleArn": str,
     },
@@ -115,60 +103,42 @@
         "certificateArn": str,
         "deviceRoleArn": str,
         "authenticationMethod": AuthenticationMethodType,
     },
     total=False,
 )
 
-GetEndpointResponseTypeDef = TypedDict(
-    "GetEndpointResponseTypeDef",
-    {
-        "endpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
     },
 )
 _OptionalGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionVersion": str,
     },
     total=False,
 )
 
-
 class GetSuiteDefinitionRequestRequestTypeDef(
     _RequiredGetSuiteDefinitionRequestRequestTypeDef,
     _OptionalGetSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 GetSuiteRunReportRequestRequestTypeDef = TypedDict(
     "GetSuiteRunReportRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
 
-GetSuiteRunReportResponseTypeDef = TypedDict(
-    "GetSuiteRunReportResponseTypeDef",
-    {
-        "qualificationReportDownloadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSuiteRunRequestRequestTypeDef = TypedDict(
     "GetSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -213,44 +183,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
-StartSuiteRunResponseTypeDef = TypedDict(
-    "StartSuiteRunResponseTypeDef",
-    {
-        "suiteRunId": str,
-        "suiteRunArn": str,
-        "createdAt": datetime,
-        "endpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopSuiteRunRequestRequestTypeDef = TypedDict(
     "StopSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -279,116 +219,156 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CreateSuiteDefinitionResponseTypeDef = TypedDict(
+    "CreateSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionName": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEndpointResponseTypeDef = TypedDict(
+    "GetEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSuiteRunReportResponseTypeDef = TypedDict(
+    "GetSuiteRunReportResponseTypeDef",
+    {
+        "qualificationReportDownloadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSuiteRunResponseTypeDef = TypedDict(
+    "StartSuiteRunResponseTypeDef",
+    {
+        "suiteRunId": str,
+        "suiteRunArn": str,
+        "createdAt": datetime,
+        "endpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSuiteDefinitionResponseTypeDef = TypedDict(
     "UpdateSuiteDefinitionResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionArn": str,
         "suiteDefinitionName": str,
         "suiteDefinitionVersion": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
     "_RequiredSuiteDefinitionConfigurationOutputTypeDef",
     {
         "suiteDefinitionName": str,
         "rootGroup": str,
         "devicePermissionRoleArn": str,
     },
 )
 _OptionalSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
     "_OptionalSuiteDefinitionConfigurationOutputTypeDef",
     {
-        "devices": List[DeviceUnderTestOutputTypeDef],
+        "devices": List[DeviceUnderTestTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
     },
     total=False,
 )
 
-
 class SuiteDefinitionConfigurationOutputTypeDef(
     _RequiredSuiteDefinitionConfigurationOutputTypeDef,
     _OptionalSuiteDefinitionConfigurationOutputTypeDef,
 ):
     pass
 
+_RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
+    "_RequiredSuiteDefinitionConfigurationTypeDef",
+    {
+        "suiteDefinitionName": str,
+        "rootGroup": str,
+        "devicePermissionRoleArn": str,
+    },
+)
+_OptionalSuiteDefinitionConfigurationTypeDef = TypedDict(
+    "_OptionalSuiteDefinitionConfigurationTypeDef",
+    {
+        "devices": Sequence[DeviceUnderTestTypeDef],
+        "intendedForQualification": bool,
+        "isLongDurationTest": bool,
+        "protocol": ProtocolType,
+    },
+    total=False,
+)
+
+class SuiteDefinitionConfigurationTypeDef(
+    _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
+):
+    pass
 
 SuiteDefinitionInformationTypeDef = TypedDict(
     "SuiteDefinitionInformationTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionName": str,
-        "defaultDevices": List[DeviceUnderTestOutputTypeDef],
+        "defaultDevices": List[DeviceUnderTestTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
         "createdAt": datetime,
     },
     total=False,
 )
 
 _RequiredSuiteRunConfigurationOutputTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationOutputTypeDef",
     {
-        "primaryDevice": DeviceUnderTestOutputTypeDef,
+        "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationOutputTypeDef = TypedDict(
     "_OptionalSuiteRunConfigurationOutputTypeDef",
     {
         "selectedTestList": List[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
-
 class SuiteRunConfigurationOutputTypeDef(
     _RequiredSuiteRunConfigurationOutputTypeDef, _OptionalSuiteRunConfigurationOutputTypeDef
 ):
     pass
 
-
-_RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
-    "_RequiredSuiteDefinitionConfigurationTypeDef",
-    {
-        "suiteDefinitionName": str,
-        "rootGroup": str,
-        "devicePermissionRoleArn": str,
-    },
-)
-_OptionalSuiteDefinitionConfigurationTypeDef = TypedDict(
-    "_OptionalSuiteDefinitionConfigurationTypeDef",
-    {
-        "devices": Sequence[DeviceUnderTestTypeDef],
-        "intendedForQualification": bool,
-        "isLongDurationTest": bool,
-        "protocol": ProtocolType,
-    },
-    total=False,
-)
-
-
-class SuiteDefinitionConfigurationTypeDef(
-    _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
-):
-    pass
-
-
 _RequiredSuiteRunConfigurationTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationTypeDef",
     {
         "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationTypeDef = TypedDict(
@@ -396,27 +376,25 @@
     {
         "selectedTestList": Sequence[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
-
 class SuiteRunConfigurationTypeDef(
     _RequiredSuiteRunConfigurationTypeDef, _OptionalSuiteRunConfigurationTypeDef
 ):
     pass
 
-
 ListSuiteRunsResponseTypeDef = TypedDict(
     "ListSuiteRunsResponseTypeDef",
     {
         "suiteRunsList": List[SuiteRunInformationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestCaseRunTypeDef = TypedDict(
     "TestCaseRunTypeDef",
     {
         "testCaseRunId": str,
@@ -440,24 +418,15 @@
         "suiteDefinitionArn": str,
         "suiteDefinitionVersion": str,
         "latestVersion": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationOutputTypeDef,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSuiteDefinitionsResponseTypeDef = TypedDict(
-    "ListSuiteDefinitionsResponseTypeDef",
-    {
-        "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
@@ -467,30 +436,37 @@
     "_OptionalCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 
+ListSuiteDefinitionsResponseTypeDef = TypedDict(
+    "ListSuiteDefinitionsResponseTypeDef",
+    {
+        "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredStartSuiteRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
     },
 )
@@ -499,21 +475,19 @@
     {
         "suiteDefinitionVersion": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
-
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
@@ -538,10 +512,10 @@
         "suiteRunConfiguration": SuiteRunConfigurationOutputTypeDef,
         "testResult": TestResultTypeDef,
         "startTime": datetime,
         "endTime": datetime,
         "status": SuiteRunStatusType,
         "errorReason": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor/type_defs.pyi` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotdeviceadvisor service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iotdeviceadvisor.type_defs import CreateSuiteDefinitionResponseTypeDef
+    from mypy_boto3_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
-    data: CreateSuiteDefinitionResponseTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -25,82 +25,72 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "CreateSuiteDefinitionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
-    "DeviceUnderTestOutputTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
-    "GetEndpointResponseTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
-    "GetSuiteRunReportResponseTypeDef",
     "GetSuiteRunRequestRequestTypeDef",
     "ListSuiteDefinitionsRequestRequestTypeDef",
     "ListSuiteRunsRequestRequestTypeDef",
     "SuiteRunInformationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartSuiteRunResponseTypeDef",
     "StopSuiteRunRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestCaseScenarioTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateSuiteDefinitionResponseTypeDef",
+    "GetEndpointResponseTypeDef",
+    "GetSuiteRunReportResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartSuiteRunResponseTypeDef",
     "UpdateSuiteDefinitionResponseTypeDef",
     "SuiteDefinitionConfigurationOutputTypeDef",
+    "SuiteDefinitionConfigurationTypeDef",
     "SuiteDefinitionInformationTypeDef",
     "SuiteRunConfigurationOutputTypeDef",
-    "SuiteDefinitionConfigurationTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
     "GetSuiteDefinitionResponseTypeDef",
-    "ListSuiteDefinitionsResponseTypeDef",
     "CreateSuiteDefinitionRequestRequestTypeDef",
     "UpdateSuiteDefinitionRequestRequestTypeDef",
+    "ListSuiteDefinitionsResponseTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
-CreateSuiteDefinitionResponseTypeDef = TypedDict(
-    "CreateSuiteDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionName": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
     },
 )
 
-DeviceUnderTestOutputTypeDef = TypedDict(
-    "DeviceUnderTestOutputTypeDef",
-    {
-        "thingArn": str,
-        "certificateArn": str,
-        "deviceRoleArn": str,
-    },
-    total=False,
-)
-
 DeviceUnderTestTypeDef = TypedDict(
     "DeviceUnderTestTypeDef",
     {
         "thingArn": str,
         "certificateArn": str,
         "deviceRoleArn": str,
     },
@@ -114,58 +104,44 @@
         "certificateArn": str,
         "deviceRoleArn": str,
         "authenticationMethod": AuthenticationMethodType,
     },
     total=False,
 )
 
-GetEndpointResponseTypeDef = TypedDict(
-    "GetEndpointResponseTypeDef",
-    {
-        "endpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
     },
 )
 _OptionalGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionVersion": str,
     },
     total=False,
 )
 
+
 class GetSuiteDefinitionRequestRequestTypeDef(
     _RequiredGetSuiteDefinitionRequestRequestTypeDef,
     _OptionalGetSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 GetSuiteRunReportRequestRequestTypeDef = TypedDict(
     "GetSuiteRunReportRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
 
-GetSuiteRunReportResponseTypeDef = TypedDict(
-    "GetSuiteRunReportResponseTypeDef",
-    {
-        "qualificationReportDownloadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSuiteRunRequestRequestTypeDef = TypedDict(
     "GetSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -210,44 +186,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
-StartSuiteRunResponseTypeDef = TypedDict(
-    "StartSuiteRunResponseTypeDef",
-    {
-        "suiteRunId": str,
-        "suiteRunArn": str,
-        "createdAt": datetime,
-        "endpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopSuiteRunRequestRequestTypeDef = TypedDict(
     "StopSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -276,109 +222,161 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CreateSuiteDefinitionResponseTypeDef = TypedDict(
+    "CreateSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionName": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEndpointResponseTypeDef = TypedDict(
+    "GetEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSuiteRunReportResponseTypeDef = TypedDict(
+    "GetSuiteRunReportResponseTypeDef",
+    {
+        "qualificationReportDownloadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSuiteRunResponseTypeDef = TypedDict(
+    "StartSuiteRunResponseTypeDef",
+    {
+        "suiteRunId": str,
+        "suiteRunArn": str,
+        "createdAt": datetime,
+        "endpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSuiteDefinitionResponseTypeDef = TypedDict(
     "UpdateSuiteDefinitionResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionArn": str,
         "suiteDefinitionName": str,
         "suiteDefinitionVersion": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
     "_RequiredSuiteDefinitionConfigurationOutputTypeDef",
     {
         "suiteDefinitionName": str,
         "rootGroup": str,
         "devicePermissionRoleArn": str,
     },
 )
 _OptionalSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
     "_OptionalSuiteDefinitionConfigurationOutputTypeDef",
     {
-        "devices": List[DeviceUnderTestOutputTypeDef],
+        "devices": List[DeviceUnderTestTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
     },
     total=False,
 )
 
+
 class SuiteDefinitionConfigurationOutputTypeDef(
     _RequiredSuiteDefinitionConfigurationOutputTypeDef,
     _OptionalSuiteDefinitionConfigurationOutputTypeDef,
 ):
     pass
 
+
+_RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
+    "_RequiredSuiteDefinitionConfigurationTypeDef",
+    {
+        "suiteDefinitionName": str,
+        "rootGroup": str,
+        "devicePermissionRoleArn": str,
+    },
+)
+_OptionalSuiteDefinitionConfigurationTypeDef = TypedDict(
+    "_OptionalSuiteDefinitionConfigurationTypeDef",
+    {
+        "devices": Sequence[DeviceUnderTestTypeDef],
+        "intendedForQualification": bool,
+        "isLongDurationTest": bool,
+        "protocol": ProtocolType,
+    },
+    total=False,
+)
+
+
+class SuiteDefinitionConfigurationTypeDef(
+    _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
+):
+    pass
+
+
 SuiteDefinitionInformationTypeDef = TypedDict(
     "SuiteDefinitionInformationTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionName": str,
-        "defaultDevices": List[DeviceUnderTestOutputTypeDef],
+        "defaultDevices": List[DeviceUnderTestTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
         "createdAt": datetime,
     },
     total=False,
 )
 
 _RequiredSuiteRunConfigurationOutputTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationOutputTypeDef",
     {
-        "primaryDevice": DeviceUnderTestOutputTypeDef,
+        "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationOutputTypeDef = TypedDict(
     "_OptionalSuiteRunConfigurationOutputTypeDef",
     {
         "selectedTestList": List[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
+
 class SuiteRunConfigurationOutputTypeDef(
     _RequiredSuiteRunConfigurationOutputTypeDef, _OptionalSuiteRunConfigurationOutputTypeDef
 ):
     pass
 
-_RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
-    "_RequiredSuiteDefinitionConfigurationTypeDef",
-    {
-        "suiteDefinitionName": str,
-        "rootGroup": str,
-        "devicePermissionRoleArn": str,
-    },
-)
-_OptionalSuiteDefinitionConfigurationTypeDef = TypedDict(
-    "_OptionalSuiteDefinitionConfigurationTypeDef",
-    {
-        "devices": Sequence[DeviceUnderTestTypeDef],
-        "intendedForQualification": bool,
-        "isLongDurationTest": bool,
-        "protocol": ProtocolType,
-    },
-    total=False,
-)
-
-class SuiteDefinitionConfigurationTypeDef(
-    _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
-):
-    pass
 
 _RequiredSuiteRunConfigurationTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationTypeDef",
     {
         "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
@@ -387,25 +385,27 @@
     {
         "selectedTestList": Sequence[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
+
 class SuiteRunConfigurationTypeDef(
     _RequiredSuiteRunConfigurationTypeDef, _OptionalSuiteRunConfigurationTypeDef
 ):
     pass
 
+
 ListSuiteRunsResponseTypeDef = TypedDict(
     "ListSuiteRunsResponseTypeDef",
     {
         "suiteRunsList": List[SuiteRunInformationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestCaseRunTypeDef = TypedDict(
     "TestCaseRunTypeDef",
     {
         "testCaseRunId": str,
@@ -429,24 +429,15 @@
         "suiteDefinitionArn": str,
         "suiteDefinitionVersion": str,
         "latestVersion": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationOutputTypeDef,
         "createdAt": datetime,
         "lastModifiedAt": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSuiteDefinitionsResponseTypeDef = TypedDict(
-    "ListSuiteDefinitionsResponseTypeDef",
-    {
-        "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
@@ -456,28 +447,39 @@
     "_OptionalCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 
+ListSuiteDefinitionsResponseTypeDef = TypedDict(
+    "ListSuiteDefinitionsResponseTypeDef",
+    {
+        "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredStartSuiteRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
     },
 )
@@ -486,19 +488,21 @@
     {
         "suiteDefinitionVersion": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
+
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
@@ -523,10 +527,10 @@
         "suiteRunConfiguration": SuiteRunConfigurationOutputTypeDef,
         "testResult": TestResultTypeDef,
         "startTime": datetime,
         "endTime": datetime,
         "status": SuiteRunStatusType,
         "errorReason": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotdeviceadvisor
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotdeviceadvisor)](https://pepy.tech/project/mypy-boto3-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTDeviceAdvisor 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
+[boto3.IoTDeviceAdvisor 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [mypy-boto3-iotdeviceadvisor docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotdeviceadvisor/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,55 +303,54 @@
 ### Typed dictionaries
 
 `mypy_boto3_iotdeviceadvisor.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotdeviceadvisor.type_defs import (
-    CreateSuiteDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
-    DeviceUnderTestOutputTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
-    GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
     ListSuiteDefinitionsRequestRequestTypeDef,
     ListSuiteRunsRequestRequestTypeDef,
     SuiteRunInformationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
-    StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateSuiteDefinitionResponseTypeDef,
+    GetEndpointResponseTypeDef,
+    GetSuiteRunReportResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSuiteRunResponseTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
     SuiteDefinitionConfigurationOutputTypeDef,
+    SuiteDefinitionConfigurationTypeDef,
     SuiteDefinitionInformationTypeDef,
     SuiteRunConfigurationOutputTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
     GetSuiteDefinitionResponseTypeDef,
-    ListSuiteDefinitionsResponseTypeDef,
     CreateSuiteDefinitionRequestRequestTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
+    ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> CreateSuiteDefinitionResponseTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt` & `mypy-boto3-iotdeviceadvisor-1.28.15/mypy_boto3_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotdeviceadvisor-1.28.12/setup.py` & `mypy-boto3-iotdeviceadvisor-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotdeviceadvisor",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTDeviceAdvisor 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IoTDeviceAdvisor 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

