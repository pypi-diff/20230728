# Comparing `tmp/mypy-boto3-simspaceweaver-1.28.12.tar.gz` & `tmp/mypy-boto3-simspaceweaver-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-simspaceweaver-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
+gzip compressed data, was "mypy-boto3-simspaceweaver-1.28.15.tar", last modified: Fri Jul 28 20:43:46 2023, max compression
```

## Comparing `mypy-boto3-simspaceweaver-1.28.12.tar` & `mypy-boto3-simspaceweaver-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-27 11:47:02.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 11:49:40.000000 mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.045314 mypy-boto3-simspaceweaver-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 11:47:01.000000 mypy-boto3-simspaceweaver-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:46.041896 mypy-boto3-simspaceweaver-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-07-28 20:43:46.037896 mypy-boto3-simspaceweaver-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:46.033896 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-07-28 20:39:34.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8737 2023-07-28 20:39:34.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-28 20:39:34.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-28 20:39:34.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:46.037896 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13627 2023-07-28 20:43:45.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-28 20:43:45.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:45.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:45.000000 mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:46.041896 mypy-boto3-simspaceweaver-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:39:33.000000 mypy-boto3-simspaceweaver-1.28.15/setup.py
```

### Comparing `mypy-boto3-simspaceweaver-1.28.12/LICENSE` & `mypy-boto3-simspaceweaver-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.12/PKG-INFO` & `mypy-boto3-simspaceweaver-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-simspaceweaver
-Version: 1.28.12
-Summary: Type annotations for boto3.SimSpaceWeaver 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SimSpaceWeaver 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-simspaceweaver)](https://pepy.tech/project/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,41 +312,40 @@
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesOutputTypeDef,
     ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     DomainTypeDef,
     LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     SimulationClockTypeDef,
-    S3LocationTypeDef,
     SimulationAppPortMappingTypeDef,
     StartClockInputRequestTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
+    StartSimulationInputRequestTypeDef,
     StartAppInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
-    StartSimulationInputRequestTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.12/README.md` & `mypy-boto3-simspaceweaver-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-simspaceweaver)](https://pepy.tech/project/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,41 +280,40 @@
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesOutputTypeDef,
     ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     DomainTypeDef,
     LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     SimulationClockTypeDef,
-    S3LocationTypeDef,
     SimulationAppPortMappingTypeDef,
     StartClockInputRequestTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
+    StartSimulationInputRequestTypeDef,
     StartAppInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
-    StartSimulationInputRequestTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/__main__.py` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SimSpaceWeaver 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.SimSpaceWeaver 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver\nOther"
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

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/client.py` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/client.pyi` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/literals.py` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/literals.pyi` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/type_defs.py` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,41 +36,40 @@
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
     "LaunchOverridesOutputTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
-    "S3LocationOutputTypeDef",
+    "S3LocationTypeDef",
     "DomainTypeDef",
     "LaunchOverridesTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "SimulationClockTypeDef",
-    "S3LocationTypeDef",
     "SimulationAppPortMappingTypeDef",
     "StartClockInputRequestTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
     "CreateSnapshotInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "StartAppOutputTypeDef",
     "StartSimulationOutputTypeDef",
+    "StartSimulationInputRequestTypeDef",
     "StartAppInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
-    "StartSimulationInputRequestTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
     "DescribeSimulationOutputTypeDef",
 )
 
 CloudWatchLogsLogGroupTypeDef = TypedDict(
@@ -137,16 +136,16 @@
 DescribeSimulationInputRequestTypeDef = TypedDict(
     "DescribeSimulationInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
@@ -235,23 +234,14 @@
     {
         "Status": ClockStatusType,
         "TargetStatus": ClockTargetStatusType,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKey": str,
-    },
-    total=False,
-)
-
 SimulationAppPortMappingTypeDef = TypedDict(
     "SimulationAppPortMappingTypeDef",
     {
         "Actual": int,
         "Declared": int,
     },
     total=False,
@@ -343,14 +333,41 @@
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartSimulationInputRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationInputRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalStartSimulationInputRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "MaximumDuration": str,
+        "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class StartSimulationInputRequestTypeDef(
+    _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
+):
+    pass
+
+
 _RequiredStartAppInputRequestTypeDef = TypedDict(
     "_RequiredStartAppInputRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
     },
@@ -395,41 +412,14 @@
     {
         "Clocks": List[SimulationClockTypeDef],
         "Domains": List[DomainTypeDef],
     },
     total=False,
 )
 
-_RequiredStartSimulationInputRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationInputRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-    },
-)
-_OptionalStartSimulationInputRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-        "MaximumDuration": str,
-        "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class StartSimulationInputRequestTypeDef(
-    _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
-):
-    pass
-
-
 SimulationAppEndpointInfoTypeDef = TypedDict(
     "SimulationAppEndpointInfoTypeDef",
     {
         "Address": str,
         "IngressPortMappings": List[SimulationAppPortMappingTypeDef],
     },
     total=False,
@@ -467,15 +457,15 @@
         "ExecutionId": str,
         "LiveSimulationState": LiveSimulationStateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaximumDuration": str,
         "Name": str,
         "RoleArn": str,
         "SchemaError": str,
-        "SchemaS3Location": S3LocationOutputTypeDef,
-        "SnapshotS3Location": S3LocationOutputTypeDef,
+        "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
         "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver/type_defs.pyi` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,41 +35,40 @@
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
     "LaunchOverridesOutputTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
-    "S3LocationOutputTypeDef",
+    "S3LocationTypeDef",
     "DomainTypeDef",
     "LaunchOverridesTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "SimulationClockTypeDef",
-    "S3LocationTypeDef",
     "SimulationAppPortMappingTypeDef",
     "StartClockInputRequestTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
     "CreateSnapshotInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "StartAppOutputTypeDef",
     "StartSimulationOutputTypeDef",
+    "StartSimulationInputRequestTypeDef",
     "StartAppInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
-    "StartSimulationInputRequestTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
     "DescribeSimulationOutputTypeDef",
 )
 
 CloudWatchLogsLogGroupTypeDef = TypedDict(
@@ -136,16 +135,16 @@
 DescribeSimulationInputRequestTypeDef = TypedDict(
     "DescribeSimulationInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
@@ -232,23 +231,14 @@
     {
         "Status": ClockStatusType,
         "TargetStatus": ClockTargetStatusType,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "BucketName": str,
-        "ObjectKey": str,
-    },
-    total=False,
-)
-
 SimulationAppPortMappingTypeDef = TypedDict(
     "SimulationAppPortMappingTypeDef",
     {
         "Actual": int,
         "Declared": int,
     },
     total=False,
@@ -340,14 +330,39 @@
         "Arn": str,
         "CreationTime": datetime,
         "ExecutionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStartSimulationInputRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationInputRequestTypeDef",
+    {
+        "Name": str,
+        "RoleArn": str,
+    },
+)
+_OptionalStartSimulationInputRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "MaximumDuration": str,
+        "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartSimulationInputRequestTypeDef(
+    _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
+):
+    pass
+
 _RequiredStartAppInputRequestTypeDef = TypedDict(
     "_RequiredStartAppInputRequestTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
     },
@@ -390,39 +405,14 @@
     {
         "Clocks": List[SimulationClockTypeDef],
         "Domains": List[DomainTypeDef],
     },
     total=False,
 )
 
-_RequiredStartSimulationInputRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationInputRequestTypeDef",
-    {
-        "Name": str,
-        "RoleArn": str,
-    },
-)
-_OptionalStartSimulationInputRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-        "MaximumDuration": str,
-        "SchemaS3Location": S3LocationTypeDef,
-        "SnapshotS3Location": S3LocationTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class StartSimulationInputRequestTypeDef(
-    _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
-):
-    pass
-
 SimulationAppEndpointInfoTypeDef = TypedDict(
     "SimulationAppEndpointInfoTypeDef",
     {
         "Address": str,
         "IngressPortMappings": List[SimulationAppPortMappingTypeDef],
     },
     total=False,
@@ -460,15 +450,15 @@
         "ExecutionId": str,
         "LiveSimulationState": LiveSimulationStateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaximumDuration": str,
         "Name": str,
         "RoleArn": str,
         "SchemaError": str,
-        "SchemaS3Location": S3LocationOutputTypeDef,
-        "SnapshotS3Location": S3LocationOutputTypeDef,
+        "SchemaS3Location": S3LocationTypeDef,
+        "SnapshotS3Location": S3LocationTypeDef,
         "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/PKG-INFO` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-simspaceweaver
-Version: 1.28.12
-Summary: Type annotations for boto3.SimSpaceWeaver 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SimSpaceWeaver 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-simspaceweaver.svg?color=blue)](https://pypi.org/project/mypy-boto3-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-simspaceweaver)](https://pepy.tech/project/mypy-boto3-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SimSpaceWeaver 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
+[boto3.SimSpaceWeaver 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [mypy-boto3-simspaceweaver docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_simspaceweaver/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,41 +312,40 @@
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
     LaunchOverridesOutputTypeDef,
     ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     DomainTypeDef,
     LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     SimulationClockTypeDef,
-    S3LocationTypeDef,
     SimulationAppPortMappingTypeDef,
     StartClockInputRequestTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
+    StartSimulationInputRequestTypeDef,
     StartAppInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
-    StartSimulationInputRequestTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
```

### Comparing `mypy-boto3-simspaceweaver-1.28.12/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt` & `mypy-boto3-simspaceweaver-1.28.15/mypy_boto3_simspaceweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-simspaceweaver-1.28.12/setup.py` & `mypy-boto3-simspaceweaver-1.28.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-simspaceweaver",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_simspaceweaver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SimSpaceWeaver 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SimSpaceWeaver 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

