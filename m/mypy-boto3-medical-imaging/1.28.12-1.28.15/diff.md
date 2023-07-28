# Comparing `tmp/mypy-boto3-medical-imaging-1.28.12.tar.gz` & `tmp/mypy-boto3-medical-imaging-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medical-imaging-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
+gzip compressed data, was "mypy-boto3-medical-imaging-1.28.15.tar", last modified: Fri Jul 28 20:43:18 2023, max compression
```

## Comparing `mypy-boto3-medical-imaging-1.28.12.tar` & `mypy-boto3-medical-imaging-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.120437 mypy-boto3-medical-imaging-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-07-27 05:35:02.120437 mypy-boto3-medical-imaging-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.120437 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-27 05:26:29.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-07-27 05:26:31.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24194 2023-07-27 05:26:29.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.120437 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-07-27 05:35:01.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:35:02.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:01.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:35:01.000000 mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.120437 mypy-boto3-medical-imaging-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-27 05:26:28.000000 mypy-boto3-medical-imaging-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.069512 mypy-boto3-medical-imaging-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:45.000000 mypy-boto3-medical-imaging-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-07-28 20:43:18.069512 mypy-boto3-medical-imaging-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14335 2023-07-28 20:31:45.000000 mypy-boto3-medical-imaging-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.061512 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-28 20:31:45.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-28 20:31:45.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:31:45.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-07-28 20:31:46.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16194 2023-07-28 20:31:46.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-07-28 20:31:46.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-07-28 20:31:46.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-07-28 20:31:46.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-28 20:31:46.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:45.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24194 2023-07-28 20:31:47.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24154 2023-07-28 20:31:46.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:45.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.069512 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15852 2023-07-28 20:43:17.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:43:17.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:17.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:17.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:17.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:17.000000 mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:18.069512 mypy-boto3-medical-imaging-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-28 20:31:45.000000 mypy-boto3-medical-imaging-1.28.15/setup.py
```

### Comparing `mypy-boto3-medical-imaging-1.28.12/LICENSE` & `mypy-boto3-medical-imaging-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.12/PKG-INFO` & `mypy-boto3-medical-imaging-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medical-imaging
-Version: 1.28.12
-Summary: Type annotations for boto3.HealthImaging 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.HealthImaging 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,62 +343,62 @@
 
 ```python
 from mypy_boto3_medical_imaging.type_defs import (
     CopyDestinationImageSetPropertiesTypeDef,
     CopyDestinationImageSetTypeDef,
     CopySourceImageSetInformationTypeDef,
     CopySourceImageSetPropertiesTypeDef,
+    ResponseMetadataTypeDef,
     CreateDatastoreRequestRequestTypeDef,
-    CreateDatastoreResponseTypeDef,
     DICOMImportJobPropertiesTypeDef,
     DICOMImportJobSummaryTypeDef,
     DICOMStudyDateAndTimeTypeDef,
     DICOMTagsTypeDef,
     DICOMUpdatesTypeDef,
     DatastorePropertiesTypeDef,
     DatastoreSummaryTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
-    DeleteDatastoreResponseTypeDef,
     DeleteImageSetRequestRequestTypeDef,
-    DeleteImageSetResponseTypeDef,
     GetDICOMImportJobRequestRequestTypeDef,
     GetDatastoreRequestRequestTypeDef,
     ImageFrameInformationTypeDef,
-    GetImageFrameResponseTypeDef,
     GetImageSetMetadataRequestRequestTypeDef,
-    GetImageSetMetadataResponseTypeDef,
     GetImageSetRequestRequestTypeDef,
-    GetImageSetResponseTypeDef,
     ImageSetPropertiesTypeDef,
-    ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDICOMImportJobsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
     ListImageSetVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartDICOMImportJobRequestRequestTypeDef,
-    StartDICOMImportJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateImageSetMetadataResponseTypeDef,
     CopyImageSetInformationTypeDef,
     CopyImageSetResponseTypeDef,
+    CreateDatastoreResponseTypeDef,
+    DeleteDatastoreResponseTypeDef,
+    DeleteImageSetResponseTypeDef,
+    GetImageFrameResponseTypeDef,
+    GetImageSetMetadataResponseTypeDef,
+    GetImageSetResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDICOMImportJobResponseTypeDef,
+    UpdateImageSetMetadataResponseTypeDef,
     GetDICOMImportJobResponseTypeDef,
     ListDICOMImportJobsResponseTypeDef,
     SearchByAttributeValueTypeDef,
     ImageSetsMetadataSummaryTypeDef,
     MetadataUpdatesTypeDef,
     GetDatastoreResponseTypeDef,
     ListDatastoresResponseTypeDef,
     GetImageFrameRequestRequestTypeDef,
     ListImageSetVersionsResponseTypeDef,
+    ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
     CopyImageSetRequestRequestTypeDef,
     SearchFilterTypeDef,
     SearchImageSetsResponseTypeDef,
     UpdateImageSetMetadataRequestRequestTypeDef,
     SearchCriteriaTypeDef,
     SearchImageSetsRequestRequestTypeDef,
     SearchImageSetsRequestSearchImageSetsPaginateTypeDef,
```

### Comparing `mypy-boto3-medical-imaging-1.28.12/README.md` & `mypy-boto3-medical-imaging-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,62 +311,62 @@
 
 ```python
 from mypy_boto3_medical_imaging.type_defs import (
     CopyDestinationImageSetPropertiesTypeDef,
     CopyDestinationImageSetTypeDef,
     CopySourceImageSetInformationTypeDef,
     CopySourceImageSetPropertiesTypeDef,
+    ResponseMetadataTypeDef,
     CreateDatastoreRequestRequestTypeDef,
-    CreateDatastoreResponseTypeDef,
     DICOMImportJobPropertiesTypeDef,
     DICOMImportJobSummaryTypeDef,
     DICOMStudyDateAndTimeTypeDef,
     DICOMTagsTypeDef,
     DICOMUpdatesTypeDef,
     DatastorePropertiesTypeDef,
     DatastoreSummaryTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
-    DeleteDatastoreResponseTypeDef,
     DeleteImageSetRequestRequestTypeDef,
-    DeleteImageSetResponseTypeDef,
     GetDICOMImportJobRequestRequestTypeDef,
     GetDatastoreRequestRequestTypeDef,
     ImageFrameInformationTypeDef,
-    GetImageFrameResponseTypeDef,
     GetImageSetMetadataRequestRequestTypeDef,
-    GetImageSetMetadataResponseTypeDef,
     GetImageSetRequestRequestTypeDef,
-    GetImageSetResponseTypeDef,
     ImageSetPropertiesTypeDef,
-    ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDICOMImportJobsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
     ListImageSetVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartDICOMImportJobRequestRequestTypeDef,
-    StartDICOMImportJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateImageSetMetadataResponseTypeDef,
     CopyImageSetInformationTypeDef,
     CopyImageSetResponseTypeDef,
+    CreateDatastoreResponseTypeDef,
+    DeleteDatastoreResponseTypeDef,
+    DeleteImageSetResponseTypeDef,
+    GetImageFrameResponseTypeDef,
+    GetImageSetMetadataResponseTypeDef,
+    GetImageSetResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDICOMImportJobResponseTypeDef,
+    UpdateImageSetMetadataResponseTypeDef,
     GetDICOMImportJobResponseTypeDef,
     ListDICOMImportJobsResponseTypeDef,
     SearchByAttributeValueTypeDef,
     ImageSetsMetadataSummaryTypeDef,
     MetadataUpdatesTypeDef,
     GetDatastoreResponseTypeDef,
     ListDatastoresResponseTypeDef,
     GetImageFrameRequestRequestTypeDef,
     ListImageSetVersionsResponseTypeDef,
+    ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
     CopyImageSetRequestRequestTypeDef,
     SearchFilterTypeDef,
     SearchImageSetsResponseTypeDef,
     UpdateImageSetMetadataRequestRequestTypeDef,
     SearchCriteriaTypeDef,
     SearchImageSetsRequestRequestTypeDef,
     SearchImageSetsRequestSearchImageSetsPaginateTypeDef,
```

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/__init__.py` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/__init__.pyi` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/__main__.py` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.HealthImaging 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.HealthImaging 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging\nOther"
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

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/client.py` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/client.pyi` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/literals.py` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/literals.pyi` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/paginator.py` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,87 +42,81 @@
 __all__ = (
     "ListDICOMImportJobsPaginator",
     "ListDatastoresPaginator",
     "ListImageSetVersionsPaginator",
     "SearchImageSetsPaginator",
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
 class ListDICOMImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdicomimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDICOMImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdicomimportjobspaginator)
         """
 
-
 class ListDatastoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdatastorespaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdatastorespaginator)
         """
 
-
 class ListImageSetVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListImageSetVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listimagesetversionspaginator)
     """
 
     def paginate(
-        self, *, datastoreId: str, imageSetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, datastoreId: str, imageSetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImageSetVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListImageSetVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listimagesetversionspaginator)
         """
 
-
 class SearchImageSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#searchimagesetspaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchImageSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#searchimagesetspaginator)
         """
```

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/paginator.pyi` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,81 +42,87 @@
 __all__ = (
     "ListDICOMImportJobsPaginator",
     "ListDatastoresPaginator",
     "ListImageSetVersionsPaginator",
     "SearchImageSetsPaginator",
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
 class ListDICOMImportJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdicomimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         jobStatus: JobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDICOMImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDICOMImportJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdicomimportjobspaginator)
         """
 
+
 class ListDatastoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdatastorespaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreStatus: DatastoreStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListDatastores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listdatastorespaginator)
         """
 
+
 class ListImageSetVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListImageSetVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listimagesetversionspaginator)
     """
 
     def paginate(
-        self, *, datastoreId: str, imageSetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, datastoreId: str, imageSetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImageSetVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.ListImageSetVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#listimagesetversionspaginator)
         """
 
+
 class SearchImageSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#searchimagesetspaginator)
     """
 
     def paginate(
         self,
         *,
         datastoreId: str,
         searchCriteria: SearchCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchImageSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging.Paginator.SearchImageSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/paginators/#searchimagesetspaginator)
         """
```

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/type_defs.py` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,62 +32,62 @@
 
 
 __all__ = (
     "CopyDestinationImageSetPropertiesTypeDef",
     "CopyDestinationImageSetTypeDef",
     "CopySourceImageSetInformationTypeDef",
     "CopySourceImageSetPropertiesTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
-    "CreateDatastoreResponseTypeDef",
     "DICOMImportJobPropertiesTypeDef",
     "DICOMImportJobSummaryTypeDef",
     "DICOMStudyDateAndTimeTypeDef",
     "DICOMTagsTypeDef",
     "DICOMUpdatesTypeDef",
     "DatastorePropertiesTypeDef",
     "DatastoreSummaryTypeDef",
     "DeleteDatastoreRequestRequestTypeDef",
-    "DeleteDatastoreResponseTypeDef",
     "DeleteImageSetRequestRequestTypeDef",
-    "DeleteImageSetResponseTypeDef",
     "GetDICOMImportJobRequestRequestTypeDef",
     "GetDatastoreRequestRequestTypeDef",
     "ImageFrameInformationTypeDef",
-    "GetImageFrameResponseTypeDef",
     "GetImageSetMetadataRequestRequestTypeDef",
-    "GetImageSetMetadataResponseTypeDef",
     "GetImageSetRequestRequestTypeDef",
-    "GetImageSetResponseTypeDef",
     "ImageSetPropertiesTypeDef",
-    "ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDICOMImportJobsRequestRequestTypeDef",
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
-    "ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
     "ListImageSetVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDICOMImportJobRequestRequestTypeDef",
-    "StartDICOMImportJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateImageSetMetadataResponseTypeDef",
     "CopyImageSetInformationTypeDef",
     "CopyImageSetResponseTypeDef",
+    "CreateDatastoreResponseTypeDef",
+    "DeleteDatastoreResponseTypeDef",
+    "DeleteImageSetResponseTypeDef",
+    "GetImageFrameResponseTypeDef",
+    "GetImageSetMetadataResponseTypeDef",
+    "GetImageSetResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDICOMImportJobResponseTypeDef",
+    "UpdateImageSetMetadataResponseTypeDef",
     "GetDICOMImportJobResponseTypeDef",
     "ListDICOMImportJobsResponseTypeDef",
     "SearchByAttributeValueTypeDef",
     "ImageSetsMetadataSummaryTypeDef",
     "MetadataUpdatesTypeDef",
     "GetDatastoreResponseTypeDef",
     "ListDatastoresResponseTypeDef",
     "GetImageFrameRequestRequestTypeDef",
     "ListImageSetVersionsResponseTypeDef",
+    "ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    "ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
     "CopyImageSetRequestRequestTypeDef",
     "SearchFilterTypeDef",
     "SearchImageSetsResponseTypeDef",
     "UpdateImageSetMetadataRequestRequestTypeDef",
     "SearchCriteriaTypeDef",
     "SearchImageSetsRequestRequestTypeDef",
     "SearchImageSetsRequestSearchImageSetsPaginateTypeDef",
@@ -157,14 +157,25 @@
 
 class CopySourceImageSetPropertiesTypeDef(
     _RequiredCopySourceImageSetPropertiesTypeDef, _OptionalCopySourceImageSetPropertiesTypeDef
 ):
     pass
 
 
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
 _RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatastoreRequestRequestTypeDef",
     {
         "clientToken": str,
     },
 )
 _OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
@@ -180,23 +191,14 @@
 
 class CreateDatastoreRequestRequestTypeDef(
     _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
 ):
     pass
 
 
-CreateDatastoreResponseTypeDef = TypedDict(
-    "CreateDatastoreResponseTypeDef",
-    {
-        "datastoreId": str,
-        "datastoreStatus": DatastoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDICOMImportJobPropertiesTypeDef = TypedDict(
     "_RequiredDICOMImportJobPropertiesTypeDef",
     {
         "jobId": str,
         "jobName": str,
         "jobStatus": JobStatusType,
         "datastoreId": str,
@@ -350,42 +352,22 @@
 DeleteDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteDatastoreRequestRequestTypeDef",
     {
         "datastoreId": str,
     },
 )
 
-DeleteDatastoreResponseTypeDef = TypedDict(
-    "DeleteDatastoreResponseTypeDef",
-    {
-        "datastoreId": str,
-        "datastoreStatus": DatastoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageSetRequestRequestTypeDef = TypedDict(
     "DeleteImageSetRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
     },
 )
 
-DeleteImageSetResponseTypeDef = TypedDict(
-    "DeleteImageSetResponseTypeDef",
-    {
-        "datastoreId": str,
-        "imageSetId": str,
-        "imageSetState": ImageSetStateType,
-        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDICOMImportJobRequestRequestTypeDef = TypedDict(
     "GetDICOMImportJobRequestRequestTypeDef",
     {
         "datastoreId": str,
         "jobId": str,
     },
 )
@@ -400,23 +382,14 @@
 ImageFrameInformationTypeDef = TypedDict(
     "ImageFrameInformationTypeDef",
     {
         "imageFrameId": str,
     },
 )
 
-GetImageFrameResponseTypeDef = TypedDict(
-    "GetImageFrameResponseTypeDef",
-    {
-        "imageFrameBlob": StreamingBody,
-        "contentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetImageSetMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetImageSetMetadataRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
     },
 )
@@ -432,24 +405,14 @@
 class GetImageSetMetadataRequestRequestTypeDef(
     _RequiredGetImageSetMetadataRequestRequestTypeDef,
     _OptionalGetImageSetMetadataRequestRequestTypeDef,
 ):
     pass
 
 
-GetImageSetMetadataResponseTypeDef = TypedDict(
-    "GetImageSetMetadataResponseTypeDef",
-    {
-        "imageSetMetadataBlob": StreamingBody,
-        "contentType": str,
-        "contentEncoding": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetImageSetRequestRequestTypeDef = TypedDict(
     "_RequiredGetImageSetRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
     },
 )
@@ -464,31 +427,14 @@
 
 class GetImageSetRequestRequestTypeDef(
     _RequiredGetImageSetRequestRequestTypeDef, _OptionalGetImageSetRequestRequestTypeDef
 ):
     pass
 
 
-GetImageSetResponseTypeDef = TypedDict(
-    "GetImageSetResponseTypeDef",
-    {
-        "datastoreId": str,
-        "imageSetId": str,
-        "versionId": str,
-        "imageSetState": ImageSetStateType,
-        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "deletedAt": datetime,
-        "message": str,
-        "imageSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImageSetPropertiesTypeDef = TypedDict(
     "_RequiredImageSetPropertiesTypeDef",
     {
         "imageSetId": str,
         "versionId": str,
         "imageSetState": ImageSetStateType,
     },
@@ -508,37 +454,24 @@
 
 class ImageSetPropertiesTypeDef(
     _RequiredImageSetPropertiesTypeDef, _OptionalImageSetPropertiesTypeDef
 ):
     pass
 
 
-_RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
-    {
-        "datastoreId": str,
-    },
-)
-_OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "jobStatus": JobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef(
-    _RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
-    _OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDICOMImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListDICOMImportJobsRequestRequestTypeDef",
     {
         "datastoreId": str,
     },
 )
 _OptionalListDICOMImportJobsRequestRequestTypeDef = TypedDict(
@@ -555,56 +488,24 @@
 class ListDICOMImportJobsRequestRequestTypeDef(
     _RequiredListDICOMImportJobsRequestRequestTypeDef,
     _OptionalListDICOMImportJobsRequestRequestTypeDef,
 ):
     pass
 
 
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    {
-        "datastoreStatus": DatastoreStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatastoresRequestRequestTypeDef = TypedDict(
     "ListDatastoresRequestRequestTypeDef",
     {
         "datastoreStatus": DatastoreStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
-    {
-        "datastoreId": str,
-        "imageSetId": str,
-    },
-)
-_OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef(
-    _RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
-    _OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListImageSetVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListImageSetVersionsRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
     },
 )
@@ -628,43 +529,14 @@
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
 _RequiredStartDICOMImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDICOMImportJobRequestRequestTypeDef",
     {
         "dataAccessRoleArn": str,
         "clientToken": str,
         "datastoreId": str,
         "inputS3Uri": str,
@@ -683,25 +555,14 @@
 class StartDICOMImportJobRequestRequestTypeDef(
     _RequiredStartDICOMImportJobRequestRequestTypeDef,
     _OptionalStartDICOMImportJobRequestRequestTypeDef,
 ):
     pass
 
 
-StartDICOMImportJobResponseTypeDef = TypedDict(
-    "StartDICOMImportJobResponseTypeDef",
-    {
-        "datastoreId": str,
-        "jobId": str,
-        "jobStatus": JobStatusType,
-        "submittedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -710,29 +571,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateImageSetMetadataResponseTypeDef = TypedDict(
-    "UpdateImageSetMetadataResponseTypeDef",
-    {
-        "datastoreId": str,
-        "imageSetId": str,
-        "latestVersionId": str,
-        "imageSetState": ImageSetStateType,
-        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCopyImageSetInformationTypeDef = TypedDict(
     "_RequiredCopyImageSetInformationTypeDef",
     {
         "sourceImageSet": CopySourceImageSetInformationTypeDef,
     },
 )
 _OptionalCopyImageSetInformationTypeDef = TypedDict(
@@ -752,32 +598,131 @@
 
 CopyImageSetResponseTypeDef = TypedDict(
     "CopyImageSetResponseTypeDef",
     {
         "datastoreId": str,
         "sourceImageSetProperties": CopySourceImageSetPropertiesTypeDef,
         "destinationImageSetProperties": CopyDestinationImageSetPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatastoreResponseTypeDef = TypedDict(
+    "CreateDatastoreResponseTypeDef",
+    {
+        "datastoreId": str,
+        "datastoreStatus": DatastoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDatastoreResponseTypeDef = TypedDict(
+    "DeleteDatastoreResponseTypeDef",
+    {
+        "datastoreId": str,
+        "datastoreStatus": DatastoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageSetResponseTypeDef = TypedDict(
+    "DeleteImageSetResponseTypeDef",
+    {
+        "datastoreId": str,
+        "imageSetId": str,
+        "imageSetState": ImageSetStateType,
+        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageFrameResponseTypeDef = TypedDict(
+    "GetImageFrameResponseTypeDef",
+    {
+        "imageFrameBlob": StreamingBody,
+        "contentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageSetMetadataResponseTypeDef = TypedDict(
+    "GetImageSetMetadataResponseTypeDef",
+    {
+        "imageSetMetadataBlob": StreamingBody,
+        "contentType": str,
+        "contentEncoding": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageSetResponseTypeDef = TypedDict(
+    "GetImageSetResponseTypeDef",
+    {
+        "datastoreId": str,
+        "imageSetId": str,
+        "versionId": str,
+        "imageSetState": ImageSetStateType,
+        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "deletedAt": datetime,
+        "message": str,
+        "imageSetArn": str,
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
+StartDICOMImportJobResponseTypeDef = TypedDict(
+    "StartDICOMImportJobResponseTypeDef",
+    {
+        "datastoreId": str,
+        "jobId": str,
+        "jobStatus": JobStatusType,
+        "submittedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateImageSetMetadataResponseTypeDef = TypedDict(
+    "UpdateImageSetMetadataResponseTypeDef",
+    {
+        "datastoreId": str,
+        "imageSetId": str,
+        "latestVersionId": str,
+        "imageSetState": ImageSetStateType,
+        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDICOMImportJobResponseTypeDef = TypedDict(
     "GetDICOMImportJobResponseTypeDef",
     {
         "jobProperties": DICOMImportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDICOMImportJobsResponseTypeDef = TypedDict(
     "ListDICOMImportJobsResponseTypeDef",
     {
         "jobSummaries": List[DICOMImportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchByAttributeValueTypeDef = TypedDict(
     "SearchByAttributeValueTypeDef",
     {
         "DICOMPatientId": str,
@@ -822,24 +767,24 @@
     total=False,
 )
 
 GetDatastoreResponseTypeDef = TypedDict(
     "GetDatastoreResponseTypeDef",
     {
         "datastoreProperties": DatastorePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImageFrameRequestRequestTypeDef = TypedDict(
     "GetImageFrameRequestRequestTypeDef",
     {
         "datastoreId": str,
@@ -849,18 +794,73 @@
 )
 
 ListImageSetVersionsResponseTypeDef = TypedDict(
     "ListImageSetVersionsResponseTypeDef",
     {
         "imageSetPropertiesList": List[ImageSetPropertiesTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+    {
+        "datastoreId": str,
+    },
+)
+_OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+    {
+        "jobStatus": JobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef(
+    _RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+    _OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+):
+    pass
+
+
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "datastoreStatus": DatastoreStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
+    {
+        "datastoreId": str,
+        "imageSetId": str,
+    },
+)
+_OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef(
+    _RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
+    _OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
+):
+    pass
+
+
 CopyImageSetRequestRequestTypeDef = TypedDict(
     "CopyImageSetRequestRequestTypeDef",
     {
         "datastoreId": str,
         "sourceImageSetId": str,
         "copyImageSetInformation": CopyImageSetInformationTypeDef,
     },
@@ -875,15 +875,15 @@
 )
 
 SearchImageSetsResponseTypeDef = TypedDict(
     "SearchImageSetsResponseTypeDef",
     {
         "imageSetsMetadataSummaries": List[ImageSetsMetadataSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateImageSetMetadataRequestRequestTypeDef = TypedDict(
     "UpdateImageSetMetadataRequestRequestTypeDef",
     {
         "datastoreId": str,
@@ -930,15 +930,15 @@
         "datastoreId": str,
     },
 )
 _OptionalSearchImageSetsRequestSearchImageSetsPaginateTypeDef = TypedDict(
     "_OptionalSearchImageSetsRequestSearchImageSetsPaginateTypeDef",
     {
         "searchCriteria": SearchCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchImageSetsRequestSearchImageSetsPaginateTypeDef(
     _RequiredSearchImageSetsRequestSearchImageSetsPaginateTypeDef,
```

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging/type_defs.pyi` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,62 +31,62 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "CopyDestinationImageSetPropertiesTypeDef",
     "CopyDestinationImageSetTypeDef",
     "CopySourceImageSetInformationTypeDef",
     "CopySourceImageSetPropertiesTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
-    "CreateDatastoreResponseTypeDef",
     "DICOMImportJobPropertiesTypeDef",
     "DICOMImportJobSummaryTypeDef",
     "DICOMStudyDateAndTimeTypeDef",
     "DICOMTagsTypeDef",
     "DICOMUpdatesTypeDef",
     "DatastorePropertiesTypeDef",
     "DatastoreSummaryTypeDef",
     "DeleteDatastoreRequestRequestTypeDef",
-    "DeleteDatastoreResponseTypeDef",
     "DeleteImageSetRequestRequestTypeDef",
-    "DeleteImageSetResponseTypeDef",
     "GetDICOMImportJobRequestRequestTypeDef",
     "GetDatastoreRequestRequestTypeDef",
     "ImageFrameInformationTypeDef",
-    "GetImageFrameResponseTypeDef",
     "GetImageSetMetadataRequestRequestTypeDef",
-    "GetImageSetMetadataResponseTypeDef",
     "GetImageSetRequestRequestTypeDef",
-    "GetImageSetResponseTypeDef",
     "ImageSetPropertiesTypeDef",
-    "ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDICOMImportJobsRequestRequestTypeDef",
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
-    "ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
     "ListImageSetVersionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDICOMImportJobRequestRequestTypeDef",
-    "StartDICOMImportJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateImageSetMetadataResponseTypeDef",
     "CopyImageSetInformationTypeDef",
     "CopyImageSetResponseTypeDef",
+    "CreateDatastoreResponseTypeDef",
+    "DeleteDatastoreResponseTypeDef",
+    "DeleteImageSetResponseTypeDef",
+    "GetImageFrameResponseTypeDef",
+    "GetImageSetMetadataResponseTypeDef",
+    "GetImageSetResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDICOMImportJobResponseTypeDef",
+    "UpdateImageSetMetadataResponseTypeDef",
     "GetDICOMImportJobResponseTypeDef",
     "ListDICOMImportJobsResponseTypeDef",
     "SearchByAttributeValueTypeDef",
     "ImageSetsMetadataSummaryTypeDef",
     "MetadataUpdatesTypeDef",
     "GetDatastoreResponseTypeDef",
     "ListDatastoresResponseTypeDef",
     "GetImageFrameRequestRequestTypeDef",
     "ListImageSetVersionsResponseTypeDef",
+    "ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    "ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
     "CopyImageSetRequestRequestTypeDef",
     "SearchFilterTypeDef",
     "SearchImageSetsResponseTypeDef",
     "UpdateImageSetMetadataRequestRequestTypeDef",
     "SearchCriteriaTypeDef",
     "SearchImageSetsRequestRequestTypeDef",
     "SearchImageSetsRequestSearchImageSetsPaginateTypeDef",
@@ -152,14 +152,25 @@
 )
 
 class CopySourceImageSetPropertiesTypeDef(
     _RequiredCopySourceImageSetPropertiesTypeDef, _OptionalCopySourceImageSetPropertiesTypeDef
 ):
     pass
 
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
 _RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatastoreRequestRequestTypeDef",
     {
         "clientToken": str,
     },
 )
 _OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
@@ -173,23 +184,14 @@
 )
 
 class CreateDatastoreRequestRequestTypeDef(
     _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
 ):
     pass
 
-CreateDatastoreResponseTypeDef = TypedDict(
-    "CreateDatastoreResponseTypeDef",
-    {
-        "datastoreId": str,
-        "datastoreStatus": DatastoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDICOMImportJobPropertiesTypeDef = TypedDict(
     "_RequiredDICOMImportJobPropertiesTypeDef",
     {
         "jobId": str,
         "jobName": str,
         "jobStatus": JobStatusType,
         "datastoreId": str,
@@ -333,42 +335,22 @@
 DeleteDatastoreRequestRequestTypeDef = TypedDict(
     "DeleteDatastoreRequestRequestTypeDef",
     {
         "datastoreId": str,
     },
 )
 
-DeleteDatastoreResponseTypeDef = TypedDict(
-    "DeleteDatastoreResponseTypeDef",
-    {
-        "datastoreId": str,
-        "datastoreStatus": DatastoreStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageSetRequestRequestTypeDef = TypedDict(
     "DeleteImageSetRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
     },
 )
 
-DeleteImageSetResponseTypeDef = TypedDict(
-    "DeleteImageSetResponseTypeDef",
-    {
-        "datastoreId": str,
-        "imageSetId": str,
-        "imageSetState": ImageSetStateType,
-        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDICOMImportJobRequestRequestTypeDef = TypedDict(
     "GetDICOMImportJobRequestRequestTypeDef",
     {
         "datastoreId": str,
         "jobId": str,
     },
 )
@@ -383,23 +365,14 @@
 ImageFrameInformationTypeDef = TypedDict(
     "ImageFrameInformationTypeDef",
     {
         "imageFrameId": str,
     },
 )
 
-GetImageFrameResponseTypeDef = TypedDict(
-    "GetImageFrameResponseTypeDef",
-    {
-        "imageFrameBlob": StreamingBody,
-        "contentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetImageSetMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredGetImageSetMetadataRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
     },
 )
@@ -413,24 +386,14 @@
 
 class GetImageSetMetadataRequestRequestTypeDef(
     _RequiredGetImageSetMetadataRequestRequestTypeDef,
     _OptionalGetImageSetMetadataRequestRequestTypeDef,
 ):
     pass
 
-GetImageSetMetadataResponseTypeDef = TypedDict(
-    "GetImageSetMetadataResponseTypeDef",
-    {
-        "imageSetMetadataBlob": StreamingBody,
-        "contentType": str,
-        "contentEncoding": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetImageSetRequestRequestTypeDef = TypedDict(
     "_RequiredGetImageSetRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
     },
 )
@@ -443,31 +406,14 @@
 )
 
 class GetImageSetRequestRequestTypeDef(
     _RequiredGetImageSetRequestRequestTypeDef, _OptionalGetImageSetRequestRequestTypeDef
 ):
     pass
 
-GetImageSetResponseTypeDef = TypedDict(
-    "GetImageSetResponseTypeDef",
-    {
-        "datastoreId": str,
-        "imageSetId": str,
-        "versionId": str,
-        "imageSetState": ImageSetStateType,
-        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "deletedAt": datetime,
-        "message": str,
-        "imageSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImageSetPropertiesTypeDef = TypedDict(
     "_RequiredImageSetPropertiesTypeDef",
     {
         "imageSetId": str,
         "versionId": str,
         "imageSetState": ImageSetStateType,
     },
@@ -485,35 +431,24 @@
 )
 
 class ImageSetPropertiesTypeDef(
     _RequiredImageSetPropertiesTypeDef, _OptionalImageSetPropertiesTypeDef
 ):
     pass
 
-_RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef = TypedDict(
-    "_RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
-    {
-        "datastoreId": str,
-    },
-)
-_OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef = TypedDict(
-    "_OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "jobStatus": JobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef(
-    _RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
-    _OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDICOMImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListDICOMImportJobsRequestRequestTypeDef",
     {
         "datastoreId": str,
     },
 )
 _OptionalListDICOMImportJobsRequestRequestTypeDef = TypedDict(
@@ -528,54 +463,24 @@
 
 class ListDICOMImportJobsRequestRequestTypeDef(
     _RequiredListDICOMImportJobsRequestRequestTypeDef,
     _OptionalListDICOMImportJobsRequestRequestTypeDef,
 ):
     pass
 
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    {
-        "datastoreStatus": DatastoreStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatastoresRequestRequestTypeDef = TypedDict(
     "ListDatastoresRequestRequestTypeDef",
     {
         "datastoreStatus": DatastoreStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
-    {
-        "datastoreId": str,
-        "imageSetId": str,
-    },
-)
-_OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef(
-    _RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
-    _OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListImageSetVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListImageSetVersionsRequestRequestTypeDef",
     {
         "datastoreId": str,
         "imageSetId": str,
     },
 )
@@ -597,43 +502,14 @@
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
 _RequiredStartDICOMImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDICOMImportJobRequestRequestTypeDef",
     {
         "dataAccessRoleArn": str,
         "clientToken": str,
         "datastoreId": str,
         "inputS3Uri": str,
@@ -650,25 +526,14 @@
 
 class StartDICOMImportJobRequestRequestTypeDef(
     _RequiredStartDICOMImportJobRequestRequestTypeDef,
     _OptionalStartDICOMImportJobRequestRequestTypeDef,
 ):
     pass
 
-StartDICOMImportJobResponseTypeDef = TypedDict(
-    "StartDICOMImportJobResponseTypeDef",
-    {
-        "datastoreId": str,
-        "jobId": str,
-        "jobStatus": JobStatusType,
-        "submittedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -677,29 +542,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateImageSetMetadataResponseTypeDef = TypedDict(
-    "UpdateImageSetMetadataResponseTypeDef",
-    {
-        "datastoreId": str,
-        "imageSetId": str,
-        "latestVersionId": str,
-        "imageSetState": ImageSetStateType,
-        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCopyImageSetInformationTypeDef = TypedDict(
     "_RequiredCopyImageSetInformationTypeDef",
     {
         "sourceImageSet": CopySourceImageSetInformationTypeDef,
     },
 )
 _OptionalCopyImageSetInformationTypeDef = TypedDict(
@@ -717,32 +567,131 @@
 
 CopyImageSetResponseTypeDef = TypedDict(
     "CopyImageSetResponseTypeDef",
     {
         "datastoreId": str,
         "sourceImageSetProperties": CopySourceImageSetPropertiesTypeDef,
         "destinationImageSetProperties": CopyDestinationImageSetPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatastoreResponseTypeDef = TypedDict(
+    "CreateDatastoreResponseTypeDef",
+    {
+        "datastoreId": str,
+        "datastoreStatus": DatastoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDatastoreResponseTypeDef = TypedDict(
+    "DeleteDatastoreResponseTypeDef",
+    {
+        "datastoreId": str,
+        "datastoreStatus": DatastoreStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageSetResponseTypeDef = TypedDict(
+    "DeleteImageSetResponseTypeDef",
+    {
+        "datastoreId": str,
+        "imageSetId": str,
+        "imageSetState": ImageSetStateType,
+        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageFrameResponseTypeDef = TypedDict(
+    "GetImageFrameResponseTypeDef",
+    {
+        "imageFrameBlob": StreamingBody,
+        "contentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageSetMetadataResponseTypeDef = TypedDict(
+    "GetImageSetMetadataResponseTypeDef",
+    {
+        "imageSetMetadataBlob": StreamingBody,
+        "contentType": str,
+        "contentEncoding": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageSetResponseTypeDef = TypedDict(
+    "GetImageSetResponseTypeDef",
+    {
+        "datastoreId": str,
+        "imageSetId": str,
+        "versionId": str,
+        "imageSetState": ImageSetStateType,
+        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "deletedAt": datetime,
+        "message": str,
+        "imageSetArn": str,
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
+StartDICOMImportJobResponseTypeDef = TypedDict(
+    "StartDICOMImportJobResponseTypeDef",
+    {
+        "datastoreId": str,
+        "jobId": str,
+        "jobStatus": JobStatusType,
+        "submittedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateImageSetMetadataResponseTypeDef = TypedDict(
+    "UpdateImageSetMetadataResponseTypeDef",
+    {
+        "datastoreId": str,
+        "imageSetId": str,
+        "latestVersionId": str,
+        "imageSetState": ImageSetStateType,
+        "imageSetWorkflowStatus": ImageSetWorkflowStatusType,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDICOMImportJobResponseTypeDef = TypedDict(
     "GetDICOMImportJobResponseTypeDef",
     {
         "jobProperties": DICOMImportJobPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDICOMImportJobsResponseTypeDef = TypedDict(
     "ListDICOMImportJobsResponseTypeDef",
     {
         "jobSummaries": List[DICOMImportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchByAttributeValueTypeDef = TypedDict(
     "SearchByAttributeValueTypeDef",
     {
         "DICOMPatientId": str,
@@ -785,24 +734,24 @@
     total=False,
 )
 
 GetDatastoreResponseTypeDef = TypedDict(
     "GetDatastoreResponseTypeDef",
     {
         "datastoreProperties": DatastorePropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetImageFrameRequestRequestTypeDef = TypedDict(
     "GetImageFrameRequestRequestTypeDef",
     {
         "datastoreId": str,
@@ -812,18 +761,69 @@
 )
 
 ListImageSetVersionsResponseTypeDef = TypedDict(
     "ListImageSetVersionsResponseTypeDef",
     {
         "imageSetPropertiesList": List[ImageSetPropertiesTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef = TypedDict(
+    "_RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+    {
+        "datastoreId": str,
+    },
+)
+_OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef = TypedDict(
+    "_OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef",
+    {
+        "jobStatus": JobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef(
+    _RequiredListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+    _OptionalListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+):
+    pass
+
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "datastoreStatus": DatastoreStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
+    {
+        "datastoreId": str,
+        "imageSetId": str,
+    },
+)
+_OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef(
+    _RequiredListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
+    _OptionalListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
+):
+    pass
+
 CopyImageSetRequestRequestTypeDef = TypedDict(
     "CopyImageSetRequestRequestTypeDef",
     {
         "datastoreId": str,
         "sourceImageSetId": str,
         "copyImageSetInformation": CopyImageSetInformationTypeDef,
     },
@@ -838,15 +838,15 @@
 )
 
 SearchImageSetsResponseTypeDef = TypedDict(
     "SearchImageSetsResponseTypeDef",
     {
         "imageSetsMetadataSummaries": List[ImageSetsMetadataSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateImageSetMetadataRequestRequestTypeDef = TypedDict(
     "UpdateImageSetMetadataRequestRequestTypeDef",
     {
         "datastoreId": str,
@@ -891,15 +891,15 @@
         "datastoreId": str,
     },
 )
 _OptionalSearchImageSetsRequestSearchImageSetsPaginateTypeDef = TypedDict(
     "_OptionalSearchImageSetsRequestSearchImageSetsPaginateTypeDef",
     {
         "searchCriteria": SearchCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchImageSetsRequestSearchImageSetsPaginateTypeDef(
     _RequiredSearchImageSetsRequestSearchImageSetsPaginateTypeDef,
     _OptionalSearchImageSetsRequestSearchImageSetsPaginateTypeDef,
```

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/PKG-INFO` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medical-imaging
-Version: 1.28.12
-Summary: Type annotations for boto3.HealthImaging 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.HealthImaging 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medical-imaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-medical-imaging)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medical-imaging)](https://pepy.tech/project/mypy-boto3-medical-imaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.HealthImaging 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
+[boto3.HealthImaging 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#HealthImaging)
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
 [mypy-boto3-medical-imaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medical_imaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,62 +343,62 @@
 
 ```python
 from mypy_boto3_medical_imaging.type_defs import (
     CopyDestinationImageSetPropertiesTypeDef,
     CopyDestinationImageSetTypeDef,
     CopySourceImageSetInformationTypeDef,
     CopySourceImageSetPropertiesTypeDef,
+    ResponseMetadataTypeDef,
     CreateDatastoreRequestRequestTypeDef,
-    CreateDatastoreResponseTypeDef,
     DICOMImportJobPropertiesTypeDef,
     DICOMImportJobSummaryTypeDef,
     DICOMStudyDateAndTimeTypeDef,
     DICOMTagsTypeDef,
     DICOMUpdatesTypeDef,
     DatastorePropertiesTypeDef,
     DatastoreSummaryTypeDef,
     DeleteDatastoreRequestRequestTypeDef,
-    DeleteDatastoreResponseTypeDef,
     DeleteImageSetRequestRequestTypeDef,
-    DeleteImageSetResponseTypeDef,
     GetDICOMImportJobRequestRequestTypeDef,
     GetDatastoreRequestRequestTypeDef,
     ImageFrameInformationTypeDef,
-    GetImageFrameResponseTypeDef,
     GetImageSetMetadataRequestRequestTypeDef,
-    GetImageSetMetadataResponseTypeDef,
     GetImageSetRequestRequestTypeDef,
-    GetImageSetResponseTypeDef,
     ImageSetPropertiesTypeDef,
-    ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDICOMImportJobsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
     ListImageSetVersionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartDICOMImportJobRequestRequestTypeDef,
-    StartDICOMImportJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateImageSetMetadataResponseTypeDef,
     CopyImageSetInformationTypeDef,
     CopyImageSetResponseTypeDef,
+    CreateDatastoreResponseTypeDef,
+    DeleteDatastoreResponseTypeDef,
+    DeleteImageSetResponseTypeDef,
+    GetImageFrameResponseTypeDef,
+    GetImageSetMetadataResponseTypeDef,
+    GetImageSetResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDICOMImportJobResponseTypeDef,
+    UpdateImageSetMetadataResponseTypeDef,
     GetDICOMImportJobResponseTypeDef,
     ListDICOMImportJobsResponseTypeDef,
     SearchByAttributeValueTypeDef,
     ImageSetsMetadataSummaryTypeDef,
     MetadataUpdatesTypeDef,
     GetDatastoreResponseTypeDef,
     ListDatastoresResponseTypeDef,
     GetImageFrameRequestRequestTypeDef,
     ListImageSetVersionsResponseTypeDef,
+    ListDICOMImportJobsRequestListDICOMImportJobsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListImageSetVersionsRequestListImageSetVersionsPaginateTypeDef,
     CopyImageSetRequestRequestTypeDef,
     SearchFilterTypeDef,
     SearchImageSetsResponseTypeDef,
     UpdateImageSetMetadataRequestRequestTypeDef,
     SearchCriteriaTypeDef,
     SearchImageSetsRequestRequestTypeDef,
     SearchImageSetsRequestSearchImageSetsPaginateTypeDef,
```

### Comparing `mypy-boto3-medical-imaging-1.28.12/mypy_boto3_medical_imaging.egg-info/SOURCES.txt` & `mypy-boto3-medical-imaging-1.28.15/mypy_boto3_medical_imaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medical-imaging-1.28.12/setup.py` & `mypy-boto3-medical-imaging-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medical-imaging",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_medical_imaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.HealthImaging 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.HealthImaging 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

