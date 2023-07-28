# Comparing `tmp/mypy-boto3-iot1click-projects-1.28.12.tar.gz` & `tmp/mypy-boto3-iot1click-projects-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot1click-projects-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
+gzip compressed data, was "mypy-boto3-iot1click-projects-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
```

## Comparing `mypy-boto3-iot1click-projects-1.28.12.tar` & `mypy-boto3-iot1click-projects-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:57.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.832488 mypy-boto3-iot1click-projects-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-projects-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.513216 mypy-boto3-iot1click-projects-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-28 20:42:56.509216 mypy-boto3-iot1click-projects-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.505216 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-28 20:28:14.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-07-28 20:28:14.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-28 20:28:14.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-28 20:28:14.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-28 20:28:14.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-28 20:28:14.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-28 20:28:14.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.509216 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.513216 mypy-boto3-iot1click-projects-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-projects-1.28.15/setup.py
```

### Comparing `mypy-boto3-iot1click-projects-1.28.12/LICENSE` & `mypy-boto3-iot1click-projects-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.12/PKG-INFO` & `mypy-boto3-iot1click-projects-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-projects
-Version: 1.28.12
-Summary: Type annotations for boto3.IoT1ClickProjects 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoT1ClickProjects 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,36 +328,36 @@
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ProjectDescriptionTypeDef,
     CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iot1click-projects-1.28.12/README.md` & `mypy-boto3-iot1click-projects-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,36 +296,36 @@
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ProjectDescriptionTypeDef,
     CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__init__.py` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__init__.pyi` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/__main__.py` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT1ClickProjects 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoT1ClickProjects 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects\nOther"
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

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/client.py` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/client.pyi` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/literals.py` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/literals.pyi` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/paginator.py` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListPlacementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listplacementspaginator)
     """
 
     def paginate(
-        self, *, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlacementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listplacementspaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/paginator.pyi` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListPlacementsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listplacementspaginator)
     """
 
     def paginate(
-        self, *, projectName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, projectName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPlacementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listplacementspaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/type_defs.py` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,36 +24,36 @@
 __all__ = (
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DeviceTemplateOutputTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
-    "GetDevicesInPlacementResponseTypeDef",
-    "ListPlacementsRequestListPlacementsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
+    "GetDevicesInPlacementResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PlacementTemplateOutputTypeDef",
     "PlacementTemplateTypeDef",
+    "ListPlacementsRequestListPlacementsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ProjectDescriptionTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
@@ -120,14 +120,25 @@
         "placementName": str,
         "attributes": Dict[str, str],
         "createdDate": datetime,
         "updatedDate": datetime,
     },
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
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
@@ -162,44 +173,24 @@
     "GetDevicesInPlacementRequestRequestTypeDef",
     {
         "projectName": str,
         "placementName": str,
     },
 )
 
-GetDevicesInPlacementResponseTypeDef = TypedDict(
-    "GetDevicesInPlacementResponseTypeDef",
-    {
-        "devices": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListPlacementsRequestListPlacementsPaginateTypeDef(
-    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
-    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPlacementsRequestRequestTypeDef = TypedDict(
     "_RequiredListPlacementsRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListPlacementsRequestRequestTypeDef = TypedDict(
@@ -224,22 +215,14 @@
         "projectName": str,
         "placementName": str,
         "createdDate": datetime,
         "updatedDate": datetime,
     },
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -270,43 +253,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -341,15 +295,31 @@
     pass
 
 
 DescribePlacementResponseTypeDef = TypedDict(
     "DescribePlacementResponseTypeDef",
     {
         "placement": PlacementDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDevicesInPlacementResponseTypeDef = TypedDict(
+    "GetDevicesInPlacementResponseTypeDef",
+    {
+        "devices": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PlacementTemplateOutputTypeDef = TypedDict(
     "PlacementTemplateOutputTypeDef",
     {
         "defaultAttributes": Dict[str, str],
@@ -363,29 +333,59 @@
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
 )
 
+_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPlacementsRequestListPlacementsPaginateTypeDef(
+    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
+    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
+):
+    pass
+
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPlacementsResponseTypeDef = TypedDict(
     "ListPlacementsResponseTypeDef",
     {
         "placements": List[PlacementSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredProjectDescriptionTypeDef = TypedDict(
     "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
@@ -456,10 +456,10 @@
     pass
 
 
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "project": ProjectDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects/type_defs.pyi` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,36 +23,36 @@
 __all__ = (
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "DeviceTemplateOutputTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
-    "GetDevicesInPlacementResponseTypeDef",
-    "ListPlacementsRequestListPlacementsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
+    "GetDevicesInPlacementResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PlacementTemplateOutputTypeDef",
     "PlacementTemplateTypeDef",
+    "ListPlacementsRequestListPlacementsPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
     "ProjectDescriptionTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
@@ -117,14 +117,25 @@
         "placementName": str,
         "attributes": Dict[str, str],
         "createdDate": datetime,
         "updatedDate": datetime,
     },
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
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
@@ -159,42 +170,24 @@
     "GetDevicesInPlacementRequestRequestTypeDef",
     {
         "projectName": str,
         "placementName": str,
     },
 )
 
-GetDevicesInPlacementResponseTypeDef = TypedDict(
-    "GetDevicesInPlacementResponseTypeDef",
-    {
-        "devices": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
-    {
-        "projectName": str,
-    },
-)
-_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
-    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListPlacementsRequestListPlacementsPaginateTypeDef(
-    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
-    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPlacementsRequestRequestTypeDef = TypedDict(
     "_RequiredListPlacementsRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalListPlacementsRequestRequestTypeDef = TypedDict(
@@ -217,22 +210,14 @@
         "projectName": str,
         "placementName": str,
         "createdDate": datetime,
         "updatedDate": datetime,
     },
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -261,43 +246,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -330,15 +286,31 @@
 ):
     pass
 
 DescribePlacementResponseTypeDef = TypedDict(
     "DescribePlacementResponseTypeDef",
     {
         "placement": PlacementDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDevicesInPlacementResponseTypeDef = TypedDict(
+    "GetDevicesInPlacementResponseTypeDef",
+    {
+        "devices": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PlacementTemplateOutputTypeDef = TypedDict(
     "PlacementTemplateOutputTypeDef",
     {
         "defaultAttributes": Dict[str, str],
@@ -352,29 +324,57 @@
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
 )
 
+_RequiredListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_RequiredListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "projectName": str,
+    },
+)
+_OptionalListPlacementsRequestListPlacementsPaginateTypeDef = TypedDict(
+    "_OptionalListPlacementsRequestListPlacementsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPlacementsRequestListPlacementsPaginateTypeDef(
+    _RequiredListPlacementsRequestListPlacementsPaginateTypeDef,
+    _OptionalListPlacementsRequestListPlacementsPaginateTypeDef,
+):
+    pass
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPlacementsResponseTypeDef = TypedDict(
     "ListPlacementsResponseTypeDef",
     {
         "placements": List[PlacementSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredProjectDescriptionTypeDef = TypedDict(
     "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
@@ -439,10 +439,10 @@
 ):
     pass
 
 DescribeProjectResponseTypeDef = TypedDict(
     "DescribeProjectResponseTypeDef",
     {
         "project": ProjectDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/PKG-INFO` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-projects
-Version: 1.28.12
-Summary: Type annotations for boto3.IoT1ClickProjects 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoT1ClickProjects 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-projects.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-projects)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-projects)](https://pepy.tech/project/mypy-boto3-iot1click-projects)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickProjects 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
+[boto3.IoT1ClickProjects 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
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
 [mypy-boto3-iot1click-projects docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,36 +328,36 @@
 from mypy_boto3_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
     CreatePlacementRequestRequestTypeDef,
     DeletePlacementRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DescribePlacementRequestRequestTypeDef,
     PlacementDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     DescribeProjectRequestRequestTypeDef,
     DeviceTemplateOutputTypeDef,
     DeviceTemplateTypeDef,
     DisassociateDeviceFromPlacementRequestRequestTypeDef,
     GetDevicesInPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPlacementsRequestRequestTypeDef,
     PlacementSummaryTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdatePlacementRequestRequestTypeDef,
     DescribePlacementResponseTypeDef,
+    GetDevicesInPlacementResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PlacementTemplateOutputTypeDef,
     PlacementTemplateTypeDef,
+    ListPlacementsRequestListPlacementsPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ProjectDescriptionTypeDef,
     CreateProjectRequestRequestTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeProjectResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iot1click-projects-1.28.12/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt` & `mypy-boto3-iot1click-projects-1.28.15/mypy_boto3_iot1click_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-projects-1.28.12/setup.py` & `mypy-boto3-iot1click-projects-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot1click-projects",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iot1click_projects"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT1ClickProjects 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IoT1ClickProjects 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

