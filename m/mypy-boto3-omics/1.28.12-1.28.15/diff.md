# Comparing `tmp/mypy-boto3-omics-1.28.12.tar.gz` & `tmp/mypy-boto3-omics-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-omics-1.28.12.tar", last modified: Thu Jul 27 05:44:17 2023, max compression
+gzip compressed data, was "mypy-boto3-omics-1.28.15.tar", last modified: Fri Jul 28 20:43:23 2023, max compression
```

## Comparing `mypy-boto3-omics-1.28.12.tar` & `mypy-boto3-omics-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29272 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27793 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/mypy_boto3_omics/
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61421 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61309 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   100219 2023-07-27 05:44:02.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100059 2023-07-27 05:44:01.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:43:59.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-27 05:44:00.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29272 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:44:17.000000 mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:44:17.379381 mypy-boto3-omics-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:43:58.000000 mypy-boto3-omics-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:23.885592 mypy-boto3-omics-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-07-28 20:43:23.881592 mypy-boto3-omics-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27547 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:23.877592 mypy-boto3-omics-1.28.15/mypy_boto3_omics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61421 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61309 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-07-28 20:32:43.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97914 2023-07-28 20:32:48.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97758 2023-07-28 20:32:46.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-28 20:32:42.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:23.881592 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29026 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:23.000000 mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:23.885592 mypy-boto3-omics-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:32:41.000000 mypy-boto3-omics-1.28.15/setup.py
```

### Comparing `mypy-boto3-omics-1.28.12/LICENSE` & `mypy-boto3-omics-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/PKG-INFO` & `mypy-boto3-omics-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.12
-Summary: Type annotations for boto3.Omics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -514,25 +514,23 @@
     AbortMultipartReadSetUploadRequestRequestTypeDef,
     ActivateReadSetFilterTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
-    ReferenceItemOutputTypeDef,
-    SseConfigOutputTypeDef,
+    ReferenceItemTypeDef,
+    SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
     ResponseMetadataTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    ReferenceItemTypeDef,
-    SseConfigTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
     CreateRunGroupRequestRequestTypeDef,
     WorkflowParameterTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
@@ -541,15 +539,14 @@
     DeleteVariantStoreRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     ExportReadSetDetailTypeDef,
     ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
-    VcfOptionsOutputTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
@@ -565,18 +562,17 @@
     GetRunRequestRequestTypeDef,
     GetRunTaskRequestRequestTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    WorkflowParameterOutputTypeDef,
     ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
-    SourceFilesOutputTypeDef,
+    SourceFilesTypeDef,
     ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
     PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
@@ -595,17 +591,15 @@
     SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    ReadOptionsOutputTypeDef,
     ReadOptionsTypeDef,
-    SourceFilesTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunRequestRequestTypeDef,
     VariantImportItemSourceTypeDef,
     TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -613,14 +607,17 @@
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     UploadReadSetPartRequestRequestTypeDef,
     ListReadSetActivationJobsRequestRequestTypeDef,
     AnnotationStoreItemTypeDef,
+    CreateReferenceStoreRequestRequestTypeDef,
+    CreateSequenceStoreRequestRequestTypeDef,
+    CreateVariantStoreRequestRequestTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
     BatchDeleteReadSetResponseTypeDef,
     CompleteMultipartReadSetUploadResponseTypeDef,
     CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
@@ -649,18 +646,16 @@
     StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
-    CreateReferenceStoreRequestRequestTypeDef,
-    CreateSequenceStoreRequestRequestTypeDef,
-    CreateVariantStoreRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
     ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
@@ -677,18 +672,18 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    GetWorkflowResponseTypeDef,
     ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
+    StartReadSetImportJobSourceItemTypeDef,
     ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
     ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
     ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
@@ -718,33 +713,30 @@
     ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
-    TsvOptionsOutputTypeDef,
     TsvOptionsTypeDef,
-    StartReadSetImportJobSourceItemTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
     StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
-    FormatOptionsOutputTypeDef,
-    FormatOptionsTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
+    FormatOptionsTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     CreateAnnotationStoreRequestRequestTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-omics-1.28.12/README.md` & `mypy-boto3-omics-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -482,25 +482,23 @@
     AbortMultipartReadSetUploadRequestRequestTypeDef,
     ActivateReadSetFilterTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
-    ReferenceItemOutputTypeDef,
-    SseConfigOutputTypeDef,
+    ReferenceItemTypeDef,
+    SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
     ResponseMetadataTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    ReferenceItemTypeDef,
-    SseConfigTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
     CreateRunGroupRequestRequestTypeDef,
     WorkflowParameterTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
@@ -509,15 +507,14 @@
     DeleteVariantStoreRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     ExportReadSetDetailTypeDef,
     ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
-    VcfOptionsOutputTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
@@ -533,18 +530,17 @@
     GetRunRequestRequestTypeDef,
     GetRunTaskRequestRequestTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    WorkflowParameterOutputTypeDef,
     ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
-    SourceFilesOutputTypeDef,
+    SourceFilesTypeDef,
     ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
     PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
@@ -563,17 +559,15 @@
     SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    ReadOptionsOutputTypeDef,
     ReadOptionsTypeDef,
-    SourceFilesTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunRequestRequestTypeDef,
     VariantImportItemSourceTypeDef,
     TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -581,14 +575,17 @@
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     UploadReadSetPartRequestRequestTypeDef,
     ListReadSetActivationJobsRequestRequestTypeDef,
     AnnotationStoreItemTypeDef,
+    CreateReferenceStoreRequestRequestTypeDef,
+    CreateSequenceStoreRequestRequestTypeDef,
+    CreateVariantStoreRequestRequestTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
     BatchDeleteReadSetResponseTypeDef,
     CompleteMultipartReadSetUploadResponseTypeDef,
     CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
@@ -617,18 +614,16 @@
     StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
-    CreateReferenceStoreRequestRequestTypeDef,
-    CreateSequenceStoreRequestRequestTypeDef,
-    CreateVariantStoreRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
     ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
@@ -645,18 +640,18 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    GetWorkflowResponseTypeDef,
     ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
+    StartReadSetImportJobSourceItemTypeDef,
     ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
     ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
     ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
@@ -686,33 +681,30 @@
     ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
-    TsvOptionsOutputTypeDef,
     TsvOptionsTypeDef,
-    StartReadSetImportJobSourceItemTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
     StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
-    FormatOptionsOutputTypeDef,
-    FormatOptionsTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
+    FormatOptionsTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     CreateAnnotationStoreRequestRequestTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/__init__.py` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/__init__.pyi` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/__main__.py` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Omics 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Omics 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
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

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/client.py` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/client.pyi` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/literals.py` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/literals.pyi` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/paginator.py` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/paginator.pyi` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/type_defs.py` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,25 +60,23 @@
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     "ActivateReadSetFilterTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
     "AnnotationImportItemDetailTypeDef",
     "AnnotationImportItemSourceTypeDef",
     "AnnotationImportJobItemTypeDef",
-    "ReferenceItemOutputTypeDef",
-    "SseConfigOutputTypeDef",
+    "ReferenceItemTypeDef",
+    "SseConfigTypeDef",
     "BatchDeleteReadSetRequestRequestTypeDef",
     "ReadSetBatchErrorTypeDef",
     "ResponseMetadataTypeDef",
     "CancelAnnotationImportRequestRequestTypeDef",
     "CancelRunRequestRequestTypeDef",
     "CancelVariantImportRequestRequestTypeDef",
     "CompleteReadSetUploadPartListItemTypeDef",
-    "ReferenceItemTypeDef",
-    "SseConfigTypeDef",
     "CreateMultipartReadSetUploadRequestRequestTypeDef",
     "CreateRunGroupRequestRequestTypeDef",
     "WorkflowParameterTypeDef",
     "DeleteAnnotationStoreRequestRequestTypeDef",
     "DeleteReferenceRequestRequestTypeDef",
     "DeleteReferenceStoreRequestRequestTypeDef",
     "DeleteRunGroupRequestRequestTypeDef",
@@ -87,15 +85,14 @@
     "DeleteVariantStoreRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "ExportReadSetDetailTypeDef",
     "ExportReadSetFilterTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
     "FileInformationTypeDef",
-    "VcfOptionsOutputTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
     "GetReadSetActivationJobRequestRequestTypeDef",
     "GetReadSetExportJobRequestRequestTypeDef",
     "GetReadSetImportJobRequestRequestTypeDef",
@@ -111,18 +108,17 @@
     "GetRunRequestRequestTypeDef",
     "GetRunTaskRequestRequestTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
-    "WorkflowParameterOutputTypeDef",
     "ImportReadSetFilterTypeDef",
     "ImportReadSetJobItemTypeDef",
-    "SourceFilesOutputTypeDef",
+    "SourceFilesTypeDef",
     "ImportReferenceFilterTypeDef",
     "ImportReferenceJobItemTypeDef",
     "ListAnnotationImportJobsFilterTypeDef",
     "PaginatorConfigTypeDef",
     "ListAnnotationStoresFilterTypeDef",
     "ListMultipartReadSetUploadsRequestRequestTypeDef",
     "MultipartReadSetUploadListItemTypeDef",
@@ -141,17 +137,15 @@
     "SequenceStoreFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVariantImportJobsFilterTypeDef",
     "VariantImportJobItemTypeDef",
     "ListVariantStoresFilterTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
-    "ReadOptionsOutputTypeDef",
     "ReadOptionsTypeDef",
-    "SourceFilesTypeDef",
     "StartReadSetActivationJobSourceItemTypeDef",
     "StartReferenceImportJobSourceItemTypeDef",
     "StartRunRequestRequestTypeDef",
     "VariantImportItemSourceTypeDef",
     "TsvStoreOptionsOutputTypeDef",
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -159,14 +153,17 @@
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "UploadReadSetPartRequestRequestTypeDef",
     "ListReadSetActivationJobsRequestRequestTypeDef",
     "AnnotationStoreItemTypeDef",
+    "CreateReferenceStoreRequestRequestTypeDef",
+    "CreateSequenceStoreRequestRequestTypeDef",
+    "CreateVariantStoreRequestRequestTypeDef",
     "ReferenceStoreDetailTypeDef",
     "SequenceStoreDetailTypeDef",
     "VariantStoreItemTypeDef",
     "BatchDeleteReadSetResponseTypeDef",
     "CompleteMultipartReadSetUploadResponseTypeDef",
     "CreateMultipartReadSetUploadResponseTypeDef",
     "CreateReferenceStoreResponseTypeDef",
@@ -195,18 +192,16 @@
     "StartReadSetImportJobResponseTypeDef",
     "StartReferenceImportJobResponseTypeDef",
     "StartRunResponseTypeDef",
     "StartVariantImportResponseTypeDef",
     "UpdateVariantStoreResponseTypeDef",
     "UploadReadSetPartResponseTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
-    "CreateReferenceStoreRequestRequestTypeDef",
-    "CreateSequenceStoreRequestRequestTypeDef",
-    "CreateVariantStoreRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
+    "GetWorkflowResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
     "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
     "ReadSetFilesTypeDef",
     "ReferenceFilesTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
@@ -223,18 +218,18 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetVariantImportResponseTypeDef",
-    "GetWorkflowResponseTypeDef",
     "ListReadSetImportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
+    "StartReadSetImportJobSourceItemTypeDef",
     "ListReferenceImportJobsRequestRequestTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
     "ListAnnotationImportJobsRequestRequestTypeDef",
     "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
     "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
@@ -264,33 +259,30 @@
     "ListSequenceStoresRequestRequestTypeDef",
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     "ListVariantImportJobsRequestRequestTypeDef",
     "ListVariantImportJobsResponseTypeDef",
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
-    "TsvOptionsOutputTypeDef",
     "TsvOptionsTypeDef",
-    "StartReadSetImportJobSourceItemTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
     "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
-    "FormatOptionsOutputTypeDef",
-    "FormatOptionsTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
+    "FormatOptionsTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
     "CreateAnnotationStoreRequestRequestTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
@@ -398,38 +390,38 @@
 
 class AnnotationImportJobItemTypeDef(
     _RequiredAnnotationImportJobItemTypeDef, _OptionalAnnotationImportJobItemTypeDef
 ):
     pass
 
 
-ReferenceItemOutputTypeDef = TypedDict(
-    "ReferenceItemOutputTypeDef",
+ReferenceItemTypeDef = TypedDict(
+    "ReferenceItemTypeDef",
     {
         "referenceArn": str,
     },
     total=False,
 )
 
-_RequiredSseConfigOutputTypeDef = TypedDict(
-    "_RequiredSseConfigOutputTypeDef",
+_RequiredSseConfigTypeDef = TypedDict(
+    "_RequiredSseConfigTypeDef",
     {
         "type": Literal["KMS"],
     },
 )
-_OptionalSseConfigOutputTypeDef = TypedDict(
-    "_OptionalSseConfigOutputTypeDef",
+_OptionalSseConfigTypeDef = TypedDict(
+    "_OptionalSseConfigTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
 
-class SseConfigOutputTypeDef(_RequiredSseConfigOutputTypeDef, _OptionalSseConfigOutputTypeDef):
+class SseConfigTypeDef(_RequiredSseConfigTypeDef, _OptionalSseConfigTypeDef):
     pass
 
 
 BatchDeleteReadSetRequestRequestTypeDef = TypedDict(
     "BatchDeleteReadSetRequestRequestTypeDef",
     {
         "ids": Sequence[str],
@@ -483,41 +475,14 @@
     {
         "partNumber": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
     },
 )
 
-ReferenceItemTypeDef = TypedDict(
-    "ReferenceItemTypeDef",
-    {
-        "referenceArn": str,
-    },
-    total=False,
-)
-
-_RequiredSseConfigTypeDef = TypedDict(
-    "_RequiredSseConfigTypeDef",
-    {
-        "type": Literal["KMS"],
-    },
-)
-_OptionalSseConfigTypeDef = TypedDict(
-    "_OptionalSseConfigTypeDef",
-    {
-        "keyArn": str,
-    },
-    total=False,
-)
-
-
-class SseConfigTypeDef(_RequiredSseConfigTypeDef, _OptionalSseConfigTypeDef):
-    pass
-
-
 _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sourceFileType": FileTypeType,
         "subjectId": str,
         "sampleId": str,
@@ -736,23 +701,14 @@
         "totalParts": int,
         "partSize": int,
         "contentLength": int,
     },
     total=False,
 )
 
-VcfOptionsOutputTypeDef = TypedDict(
-    "VcfOptionsOutputTypeDef",
-    {
-        "ignoreQualField": bool,
-        "ignoreFilterField": bool,
-    },
-    total=False,
-)
-
 VcfOptionsTypeDef = TypedDict(
     "VcfOptionsTypeDef",
     {
         "ignoreQualField": bool,
         "ignoreFilterField": bool,
     },
     total=False,
@@ -1016,23 +972,14 @@
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
 
-WorkflowParameterOutputTypeDef = TypedDict(
-    "WorkflowParameterOutputTypeDef",
-    {
-        "description": str,
-        "optional": bool,
-    },
-    total=False,
-)
-
 ImportReadSetFilterTypeDef = TypedDict(
     "ImportReadSetFilterTypeDef",
     {
         "status": ReadSetImportJobStatusType,
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
     },
@@ -1060,32 +1007,30 @@
 
 class ImportReadSetJobItemTypeDef(
     _RequiredImportReadSetJobItemTypeDef, _OptionalImportReadSetJobItemTypeDef
 ):
     pass
 
 
-_RequiredSourceFilesOutputTypeDef = TypedDict(
-    "_RequiredSourceFilesOutputTypeDef",
+_RequiredSourceFilesTypeDef = TypedDict(
+    "_RequiredSourceFilesTypeDef",
     {
         "source1": str,
     },
 )
-_OptionalSourceFilesOutputTypeDef = TypedDict(
-    "_OptionalSourceFilesOutputTypeDef",
+_OptionalSourceFilesTypeDef = TypedDict(
+    "_OptionalSourceFilesTypeDef",
     {
         "source2": str,
     },
     total=False,
 )
 
 
-class SourceFilesOutputTypeDef(
-    _RequiredSourceFilesOutputTypeDef, _OptionalSourceFilesOutputTypeDef
-):
+class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
     pass
 
 
 ImportReferenceFilterTypeDef = TypedDict(
     "ImportReferenceFilterTypeDef",
     {
         "status": ReferenceImportJobStatusType,
@@ -1475,30 +1420,14 @@
         "digest": str,
         "creationTime": datetime,
         "metadata": Dict[str, str],
     },
     total=False,
 )
 
-ReadOptionsOutputTypeDef = TypedDict(
-    "ReadOptionsOutputTypeDef",
-    {
-        "sep": str,
-        "encoding": str,
-        "quote": str,
-        "quoteAll": bool,
-        "escape": str,
-        "escapeQuotes": bool,
-        "comment": str,
-        "header": bool,
-        "lineSep": str,
-    },
-    total=False,
-)
-
 ReadOptionsTypeDef = TypedDict(
     "ReadOptionsTypeDef",
     {
         "sep": str,
         "encoding": str,
         "quote": str,
         "quoteAll": bool,
@@ -1507,33 +1436,14 @@
         "comment": str,
         "header": bool,
         "lineSep": str,
     },
     total=False,
 )
 
-_RequiredSourceFilesTypeDef = TypedDict(
-    "_RequiredSourceFilesTypeDef",
-    {
-        "source1": str,
-    },
-)
-_OptionalSourceFilesTypeDef = TypedDict(
-    "_OptionalSourceFilesTypeDef",
-    {
-        "source2": str,
-    },
-    total=False,
-)
-
-
-class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
-    pass
-
-
 StartReadSetActivationJobSourceItemTypeDef = TypedDict(
     "StartReadSetActivationJobSourceItemTypeDef",
     {
         "readSetId": str,
     },
 )
 
@@ -1762,42 +1672,118 @@
     pass
 
 
 AnnotationStoreItemTypeDef = TypedDict(
     "AnnotationStoreItemTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "storeFormat": StoreFormatType,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "statusMessage": str,
         "storeSizeBytes": int,
     },
 )
 
+_RequiredCreateReferenceStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReferenceStoreRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateReferenceStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReferenceStoreRequestRequestTypeDef",
+    {
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "tags": Mapping[str, str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateReferenceStoreRequestRequestTypeDef(
+    _RequiredCreateReferenceStoreRequestRequestTypeDef,
+    _OptionalCreateReferenceStoreRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSequenceStoreRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSequenceStoreRequestRequestTypeDef",
+    {
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "tags": Mapping[str, str],
+        "clientToken": str,
+        "fallbackLocation": str,
+    },
+    total=False,
+)
+
+
+class CreateSequenceStoreRequestRequestTypeDef(
+    _RequiredCreateSequenceStoreRequestRequestTypeDef,
+    _OptionalCreateSequenceStoreRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVariantStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+    },
+)
+_OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVariantStoreRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateVariantStoreRequestRequestTypeDef(
+    _RequiredCreateVariantStoreRequestRequestTypeDef,
+    _OptionalCreateVariantStoreRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredReferenceStoreDetailTypeDef = TypedDict(
     "_RequiredReferenceStoreDetailTypeDef",
     {
         "arn": str,
         "id": str,
         "creationTime": datetime,
     },
 )
 _OptionalReferenceStoreDetailTypeDef = TypedDict(
     "_OptionalReferenceStoreDetailTypeDef",
     {
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
     },
     total=False,
 )
 
 
 class ReferenceStoreDetailTypeDef(
     _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
@@ -1814,15 +1800,15 @@
     },
 )
 _OptionalSequenceStoreDetailTypeDef = TypedDict(
     "_OptionalSequenceStoreDetailTypeDef",
     {
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "fallbackLocation": str,
     },
     total=False,
 )
 
 
 class SequenceStoreDetailTypeDef(
@@ -1831,20 +1817,20 @@
     pass
 
 
 VariantStoreItemTypeDef = TypedDict(
     "VariantStoreItemTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "statusMessage": str,
         "storeSizeBytes": int,
     },
 )
 
@@ -1885,15 +1871,15 @@
 CreateReferenceStoreResponseTypeDef = TypedDict(
     "CreateReferenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRunGroupResponseTypeDef = TypedDict(
     "CreateRunGroupResponseTypeDef",
@@ -1908,26 +1894,26 @@
 CreateSequenceStoreResponseTypeDef = TypedDict(
     "CreateSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVariantStoreResponseTypeDef = TypedDict(
     "CreateVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1998,15 +1984,15 @@
 GetReferenceStoreResponseTypeDef = TypedDict(
     "GetReferenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRunGroupResponseTypeDef = TypedDict(
     "GetRunGroupResponseTypeDef",
@@ -2076,31 +2062,31 @@
 GetSequenceStoreResponseTypeDef = TypedDict(
     "GetSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariantStoreResponseTypeDef = TypedDict(
     "GetVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
         "statusMessage": str,
         "storeSizeBytes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2206,15 +2192,15 @@
     },
 )
 
 UpdateVariantStoreResponseTypeDef = TypedDict(
     "UpdateVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2233,90 +2219,14 @@
     {
         "sequenceStoreId": str,
         "uploadId": str,
         "parts": Sequence[CompleteReadSetUploadPartListItemTypeDef],
     },
 )
 
-_RequiredCreateReferenceStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReferenceStoreRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateReferenceStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReferenceStoreRequestRequestTypeDef",
-    {
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "tags": Mapping[str, str],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateReferenceStoreRequestRequestTypeDef(
-    _RequiredCreateReferenceStoreRequestRequestTypeDef,
-    _OptionalCreateReferenceStoreRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSequenceStoreRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSequenceStoreRequestRequestTypeDef",
-    {
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "tags": Mapping[str, str],
-        "clientToken": str,
-        "fallbackLocation": str,
-    },
-    total=False,
-)
-
-
-class CreateSequenceStoreRequestRequestTypeDef(
-    _RequiredCreateSequenceStoreRequestRequestTypeDef,
-    _OptionalCreateSequenceStoreRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVariantStoreRequestRequestTypeDef",
-    {
-        "reference": ReferenceItemTypeDef,
-    },
-)
-_OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVariantStoreRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateVariantStoreRequestRequestTypeDef(
-    _RequiredCreateVariantStoreRequestRequestTypeDef,
-    _OptionalCreateVariantStoreRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "requestId": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2339,14 +2249,38 @@
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
 
+GetWorkflowResponseTypeDef = TypedDict(
+    "GetWorkflowResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": WorkflowStatusType,
+        "type": WorkflowTypeType,
+        "name": str,
+        "description": str,
+        "engine": WorkflowEngineType,
+        "definition": str,
+        "main": str,
+        "digest": str,
+        "parameterTemplate": Dict[str, WorkflowParameterTypeDef],
+        "storageCapacity": int,
+        "creationTime": datetime,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+        "metadata": Dict[str, str],
+        "accelerators": Literal["GPU"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetReadSetExportJobResponseTypeDef = TypedDict(
     "GetReadSetExportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
@@ -2832,38 +2766,14 @@
         "items": List[VariantImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "annotationFields": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetWorkflowResponseTypeDef = TypedDict(
-    "GetWorkflowResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": WorkflowStatusType,
-        "type": WorkflowTypeType,
-        "name": str,
-        "description": str,
-        "engine": WorkflowEngineType,
-        "definition": str,
-        "main": str,
-        "digest": str,
-        "parameterTemplate": Dict[str, WorkflowParameterOutputTypeDef],
-        "storageCapacity": int,
-        "creationTime": datetime,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-        "metadata": Dict[str, str],
-        "accelerators": Literal["GPU"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReadSetImportJobsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
@@ -2892,15 +2802,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportReadSetSourceItemTypeDef = TypedDict(
     "_RequiredImportReadSetSourceItemTypeDef",
     {
-        "sourceFiles": SourceFilesOutputTypeDef,
+        "sourceFiles": SourceFilesTypeDef,
         "sourceFileType": FileTypeType,
         "status": ReadSetImportJobItemStatusType,
         "subjectId": str,
         "sampleId": str,
     },
 )
 _OptionalImportReadSetSourceItemTypeDef = TypedDict(
@@ -2919,14 +2829,42 @@
 
 class ImportReadSetSourceItemTypeDef(
     _RequiredImportReadSetSourceItemTypeDef, _OptionalImportReadSetSourceItemTypeDef
 ):
     pass
 
 
+_RequiredStartReadSetImportJobSourceItemTypeDef = TypedDict(
+    "_RequiredStartReadSetImportJobSourceItemTypeDef",
+    {
+        "sourceFiles": SourceFilesTypeDef,
+        "sourceFileType": FileTypeType,
+        "subjectId": str,
+        "sampleId": str,
+        "referenceArn": str,
+    },
+)
+_OptionalStartReadSetImportJobSourceItemTypeDef = TypedDict(
+    "_OptionalStartReadSetImportJobSourceItemTypeDef",
+    {
+        "generatedFrom": str,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class StartReadSetImportJobSourceItemTypeDef(
+    _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
+):
+    pass
+
+
 _RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReferenceImportJobsRequestRequestTypeDef",
     {
         "referenceStoreId": str,
     },
 )
 _OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
@@ -3456,58 +3394,22 @@
     {
         "items": List[WorkflowListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TsvOptionsOutputTypeDef = TypedDict(
-    "TsvOptionsOutputTypeDef",
-    {
-        "readOptions": ReadOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 TsvOptionsTypeDef = TypedDict(
     "TsvOptionsTypeDef",
     {
         "readOptions": ReadOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredStartReadSetImportJobSourceItemTypeDef = TypedDict(
-    "_RequiredStartReadSetImportJobSourceItemTypeDef",
-    {
-        "sourceFiles": SourceFilesTypeDef,
-        "sourceFileType": FileTypeType,
-        "subjectId": str,
-        "sampleId": str,
-        "referenceArn": str,
-    },
-)
-_OptionalStartReadSetImportJobSourceItemTypeDef = TypedDict(
-    "_OptionalStartReadSetImportJobSourceItemTypeDef",
-    {
-        "generatedFrom": str,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class StartReadSetImportJobSourceItemTypeDef(
-    _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
-):
-    pass
-
-
 _RequiredStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetActivationJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sources": Sequence[StartReadSetActivationJobSourceItemTypeDef],
     },
 )
@@ -3686,32 +3588,14 @@
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReadSetSourceItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FormatOptionsOutputTypeDef = TypedDict(
-    "FormatOptionsOutputTypeDef",
-    {
-        "tsvOptions": TsvOptionsOutputTypeDef,
-        "vcfOptions": VcfOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-FormatOptionsTypeDef = TypedDict(
-    "FormatOptionsTypeDef",
-    {
-        "tsvOptions": TsvOptionsTypeDef,
-        "vcfOptions": VcfOptionsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartReadSetImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetImportJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "roleArn": str,
         "sources": Sequence[StartReadSetImportJobSourceItemTypeDef],
     },
@@ -3728,38 +3612,47 @@
 class StartReadSetImportJobRequestRequestTypeDef(
     _RequiredStartReadSetImportJobRequestRequestTypeDef,
     _OptionalStartReadSetImportJobRequestRequestTypeDef,
 ):
     pass
 
 
+FormatOptionsTypeDef = TypedDict(
+    "FormatOptionsTypeDef",
+    {
+        "tsvOptions": TsvOptionsTypeDef,
+        "vcfOptions": VcfOptionsTypeDef,
+    },
+    total=False,
+)
+
 CreateAnnotationStoreResponseTypeDef = TypedDict(
     "CreateAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "storeFormat": StoreFormatType,
         "storeOptions": StoreOptionsOutputTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnnotationStoreResponseTypeDef = TypedDict(
     "GetAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
         "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
         "statusMessage": str,
         "storeSizeBytes": int,
@@ -3767,15 +3660,15 @@
     },
 )
 
 UpdateAnnotationStoreResponseTypeDef = TypedDict(
     "UpdateAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
@@ -3819,15 +3712,15 @@
         "status": JobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[AnnotationImportItemDetailTypeDef],
         "runLeftNormalization": bool,
-        "formatOptions": FormatOptionsOutputTypeDef,
+        "formatOptions": FormatOptionsTypeDef,
         "annotationFields": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartAnnotationImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartAnnotationImportRequestRequestTypeDef",
```

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/type_defs.pyi` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,25 +59,23 @@
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     "ActivateReadSetFilterTypeDef",
     "ActivateReadSetJobItemTypeDef",
     "ActivateReadSetSourceItemTypeDef",
     "AnnotationImportItemDetailTypeDef",
     "AnnotationImportItemSourceTypeDef",
     "AnnotationImportJobItemTypeDef",
-    "ReferenceItemOutputTypeDef",
-    "SseConfigOutputTypeDef",
+    "ReferenceItemTypeDef",
+    "SseConfigTypeDef",
     "BatchDeleteReadSetRequestRequestTypeDef",
     "ReadSetBatchErrorTypeDef",
     "ResponseMetadataTypeDef",
     "CancelAnnotationImportRequestRequestTypeDef",
     "CancelRunRequestRequestTypeDef",
     "CancelVariantImportRequestRequestTypeDef",
     "CompleteReadSetUploadPartListItemTypeDef",
-    "ReferenceItemTypeDef",
-    "SseConfigTypeDef",
     "CreateMultipartReadSetUploadRequestRequestTypeDef",
     "CreateRunGroupRequestRequestTypeDef",
     "WorkflowParameterTypeDef",
     "DeleteAnnotationStoreRequestRequestTypeDef",
     "DeleteReferenceRequestRequestTypeDef",
     "DeleteReferenceStoreRequestRequestTypeDef",
     "DeleteRunGroupRequestRequestTypeDef",
@@ -86,15 +84,14 @@
     "DeleteVariantStoreRequestRequestTypeDef",
     "DeleteWorkflowRequestRequestTypeDef",
     "ExportReadSetDetailTypeDef",
     "ExportReadSetFilterTypeDef",
     "ExportReadSetJobDetailTypeDef",
     "ExportReadSetTypeDef",
     "FileInformationTypeDef",
-    "VcfOptionsOutputTypeDef",
     "VcfOptionsTypeDef",
     "WaiterConfigTypeDef",
     "GetAnnotationImportRequestRequestTypeDef",
     "GetAnnotationStoreRequestRequestTypeDef",
     "GetReadSetActivationJobRequestRequestTypeDef",
     "GetReadSetExportJobRequestRequestTypeDef",
     "GetReadSetImportJobRequestRequestTypeDef",
@@ -110,18 +107,17 @@
     "GetRunRequestRequestTypeDef",
     "GetRunTaskRequestRequestTypeDef",
     "GetSequenceStoreRequestRequestTypeDef",
     "GetVariantImportRequestRequestTypeDef",
     "VariantImportItemDetailTypeDef",
     "GetVariantStoreRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
-    "WorkflowParameterOutputTypeDef",
     "ImportReadSetFilterTypeDef",
     "ImportReadSetJobItemTypeDef",
-    "SourceFilesOutputTypeDef",
+    "SourceFilesTypeDef",
     "ImportReferenceFilterTypeDef",
     "ImportReferenceJobItemTypeDef",
     "ListAnnotationImportJobsFilterTypeDef",
     "PaginatorConfigTypeDef",
     "ListAnnotationStoresFilterTypeDef",
     "ListMultipartReadSetUploadsRequestRequestTypeDef",
     "MultipartReadSetUploadListItemTypeDef",
@@ -140,17 +136,15 @@
     "SequenceStoreFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListVariantImportJobsFilterTypeDef",
     "VariantImportJobItemTypeDef",
     "ListVariantStoresFilterTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
-    "ReadOptionsOutputTypeDef",
     "ReadOptionsTypeDef",
-    "SourceFilesTypeDef",
     "StartReadSetActivationJobSourceItemTypeDef",
     "StartReferenceImportJobSourceItemTypeDef",
     "StartRunRequestRequestTypeDef",
     "VariantImportItemSourceTypeDef",
     "TsvStoreOptionsOutputTypeDef",
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
@@ -158,14 +152,17 @@
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
     "UploadReadSetPartRequestRequestTypeDef",
     "ListReadSetActivationJobsRequestRequestTypeDef",
     "AnnotationStoreItemTypeDef",
+    "CreateReferenceStoreRequestRequestTypeDef",
+    "CreateSequenceStoreRequestRequestTypeDef",
+    "CreateVariantStoreRequestRequestTypeDef",
     "ReferenceStoreDetailTypeDef",
     "SequenceStoreDetailTypeDef",
     "VariantStoreItemTypeDef",
     "BatchDeleteReadSetResponseTypeDef",
     "CompleteMultipartReadSetUploadResponseTypeDef",
     "CreateMultipartReadSetUploadResponseTypeDef",
     "CreateReferenceStoreResponseTypeDef",
@@ -194,18 +191,16 @@
     "StartReadSetImportJobResponseTypeDef",
     "StartReferenceImportJobResponseTypeDef",
     "StartRunResponseTypeDef",
     "StartVariantImportResponseTypeDef",
     "UpdateVariantStoreResponseTypeDef",
     "UploadReadSetPartResponseTypeDef",
     "CompleteMultipartReadSetUploadRequestRequestTypeDef",
-    "CreateReferenceStoreRequestRequestTypeDef",
-    "CreateSequenceStoreRequestRequestTypeDef",
-    "CreateVariantStoreRequestRequestTypeDef",
     "CreateWorkflowRequestRequestTypeDef",
+    "GetWorkflowResponseTypeDef",
     "GetReadSetExportJobResponseTypeDef",
     "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetExportJobsResponseTypeDef",
     "StartReadSetExportJobRequestRequestTypeDef",
     "ReadSetFilesTypeDef",
     "ReferenceFilesTypeDef",
     "GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef",
@@ -222,18 +217,18 @@
     "GetVariantImportRequestVariantImportJobCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreCreatedWaitTypeDef",
     "GetVariantStoreRequestVariantStoreDeletedWaitTypeDef",
     "GetWorkflowRequestWorkflowActiveWaitTypeDef",
     "ReadSetListItemTypeDef",
     "GetReferenceImportJobResponseTypeDef",
     "GetVariantImportResponseTypeDef",
-    "GetWorkflowResponseTypeDef",
     "ListReadSetImportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsResponseTypeDef",
     "ImportReadSetSourceItemTypeDef",
+    "StartReadSetImportJobSourceItemTypeDef",
     "ListReferenceImportJobsRequestRequestTypeDef",
     "ListReferenceImportJobsResponseTypeDef",
     "ListAnnotationImportJobsRequestRequestTypeDef",
     "ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef",
     "ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef",
     "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
     "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
@@ -263,33 +258,30 @@
     "ListSequenceStoresRequestRequestTypeDef",
     "ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef",
     "ListVariantImportJobsRequestRequestTypeDef",
     "ListVariantImportJobsResponseTypeDef",
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
-    "TsvOptionsOutputTypeDef",
     "TsvOptionsTypeDef",
-    "StartReadSetImportJobSourceItemTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
     "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
     "ListAnnotationStoresResponseTypeDef",
     "ListReferenceStoresResponseTypeDef",
     "ListSequenceStoresResponseTypeDef",
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
-    "FormatOptionsOutputTypeDef",
-    "FormatOptionsTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
+    "FormatOptionsTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
     "CreateAnnotationStoreRequestRequestTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
@@ -391,37 +383,37 @@
 )
 
 class AnnotationImportJobItemTypeDef(
     _RequiredAnnotationImportJobItemTypeDef, _OptionalAnnotationImportJobItemTypeDef
 ):
     pass
 
-ReferenceItemOutputTypeDef = TypedDict(
-    "ReferenceItemOutputTypeDef",
+ReferenceItemTypeDef = TypedDict(
+    "ReferenceItemTypeDef",
     {
         "referenceArn": str,
     },
     total=False,
 )
 
-_RequiredSseConfigOutputTypeDef = TypedDict(
-    "_RequiredSseConfigOutputTypeDef",
+_RequiredSseConfigTypeDef = TypedDict(
+    "_RequiredSseConfigTypeDef",
     {
         "type": Literal["KMS"],
     },
 )
-_OptionalSseConfigOutputTypeDef = TypedDict(
-    "_OptionalSseConfigOutputTypeDef",
+_OptionalSseConfigTypeDef = TypedDict(
+    "_OptionalSseConfigTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
-class SseConfigOutputTypeDef(_RequiredSseConfigOutputTypeDef, _OptionalSseConfigOutputTypeDef):
+class SseConfigTypeDef(_RequiredSseConfigTypeDef, _OptionalSseConfigTypeDef):
     pass
 
 BatchDeleteReadSetRequestRequestTypeDef = TypedDict(
     "BatchDeleteReadSetRequestRequestTypeDef",
     {
         "ids": Sequence[str],
         "sequenceStoreId": str,
@@ -474,39 +466,14 @@
     {
         "partNumber": int,
         "partSource": ReadSetPartSourceType,
         "checksum": str,
     },
 )
 
-ReferenceItemTypeDef = TypedDict(
-    "ReferenceItemTypeDef",
-    {
-        "referenceArn": str,
-    },
-    total=False,
-)
-
-_RequiredSseConfigTypeDef = TypedDict(
-    "_RequiredSseConfigTypeDef",
-    {
-        "type": Literal["KMS"],
-    },
-)
-_OptionalSseConfigTypeDef = TypedDict(
-    "_OptionalSseConfigTypeDef",
-    {
-        "keyArn": str,
-    },
-    total=False,
-)
-
-class SseConfigTypeDef(_RequiredSseConfigTypeDef, _OptionalSseConfigTypeDef):
-    pass
-
 _RequiredCreateMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMultipartReadSetUploadRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sourceFileType": FileTypeType,
         "subjectId": str,
         "sampleId": str,
@@ -713,23 +680,14 @@
         "totalParts": int,
         "partSize": int,
         "contentLength": int,
     },
     total=False,
 )
 
-VcfOptionsOutputTypeDef = TypedDict(
-    "VcfOptionsOutputTypeDef",
-    {
-        "ignoreQualField": bool,
-        "ignoreFilterField": bool,
-    },
-    total=False,
-)
-
 VcfOptionsTypeDef = TypedDict(
     "VcfOptionsTypeDef",
     {
         "ignoreQualField": bool,
         "ignoreFilterField": bool,
     },
     total=False,
@@ -981,23 +939,14 @@
 )
 
 class GetWorkflowRequestRequestTypeDef(
     _RequiredGetWorkflowRequestRequestTypeDef, _OptionalGetWorkflowRequestRequestTypeDef
 ):
     pass
 
-WorkflowParameterOutputTypeDef = TypedDict(
-    "WorkflowParameterOutputTypeDef",
-    {
-        "description": str,
-        "optional": bool,
-    },
-    total=False,
-)
-
 ImportReadSetFilterTypeDef = TypedDict(
     "ImportReadSetFilterTypeDef",
     {
         "status": ReadSetImportJobStatusType,
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
     },
@@ -1023,31 +972,29 @@
 )
 
 class ImportReadSetJobItemTypeDef(
     _RequiredImportReadSetJobItemTypeDef, _OptionalImportReadSetJobItemTypeDef
 ):
     pass
 
-_RequiredSourceFilesOutputTypeDef = TypedDict(
-    "_RequiredSourceFilesOutputTypeDef",
+_RequiredSourceFilesTypeDef = TypedDict(
+    "_RequiredSourceFilesTypeDef",
     {
         "source1": str,
     },
 )
-_OptionalSourceFilesOutputTypeDef = TypedDict(
-    "_OptionalSourceFilesOutputTypeDef",
+_OptionalSourceFilesTypeDef = TypedDict(
+    "_OptionalSourceFilesTypeDef",
     {
         "source2": str,
     },
     total=False,
 )
 
-class SourceFilesOutputTypeDef(
-    _RequiredSourceFilesOutputTypeDef, _OptionalSourceFilesOutputTypeDef
-):
+class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
     pass
 
 ImportReferenceFilterTypeDef = TypedDict(
     "ImportReferenceFilterTypeDef",
     {
         "status": ReferenceImportJobStatusType,
         "createdAfter": Union[datetime, str],
@@ -1422,30 +1369,14 @@
         "digest": str,
         "creationTime": datetime,
         "metadata": Dict[str, str],
     },
     total=False,
 )
 
-ReadOptionsOutputTypeDef = TypedDict(
-    "ReadOptionsOutputTypeDef",
-    {
-        "sep": str,
-        "encoding": str,
-        "quote": str,
-        "quoteAll": bool,
-        "escape": str,
-        "escapeQuotes": bool,
-        "comment": str,
-        "header": bool,
-        "lineSep": str,
-    },
-    total=False,
-)
-
 ReadOptionsTypeDef = TypedDict(
     "ReadOptionsTypeDef",
     {
         "sep": str,
         "encoding": str,
         "quote": str,
         "quoteAll": bool,
@@ -1454,31 +1385,14 @@
         "comment": str,
         "header": bool,
         "lineSep": str,
     },
     total=False,
 )
 
-_RequiredSourceFilesTypeDef = TypedDict(
-    "_RequiredSourceFilesTypeDef",
-    {
-        "source1": str,
-    },
-)
-_OptionalSourceFilesTypeDef = TypedDict(
-    "_OptionalSourceFilesTypeDef",
-    {
-        "source2": str,
-    },
-    total=False,
-)
-
-class SourceFilesTypeDef(_RequiredSourceFilesTypeDef, _OptionalSourceFilesTypeDef):
-    pass
-
 StartReadSetActivationJobSourceItemTypeDef = TypedDict(
     "StartReadSetActivationJobSourceItemTypeDef",
     {
         "readSetId": str,
     },
 )
 
@@ -1693,42 +1607,112 @@
 ):
     pass
 
 AnnotationStoreItemTypeDef = TypedDict(
     "AnnotationStoreItemTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "storeFormat": StoreFormatType,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "statusMessage": str,
         "storeSizeBytes": int,
     },
 )
 
+_RequiredCreateReferenceStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReferenceStoreRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateReferenceStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReferenceStoreRequestRequestTypeDef",
+    {
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "tags": Mapping[str, str],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateReferenceStoreRequestRequestTypeDef(
+    _RequiredCreateReferenceStoreRequestRequestTypeDef,
+    _OptionalCreateReferenceStoreRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSequenceStoreRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSequenceStoreRequestRequestTypeDef",
+    {
+        "description": str,
+        "sseConfig": SseConfigTypeDef,
+        "tags": Mapping[str, str],
+        "clientToken": str,
+        "fallbackLocation": str,
+    },
+    total=False,
+)
+
+class CreateSequenceStoreRequestRequestTypeDef(
+    _RequiredCreateSequenceStoreRequestRequestTypeDef,
+    _OptionalCreateSequenceStoreRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVariantStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+    },
+)
+_OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVariantStoreRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateVariantStoreRequestRequestTypeDef(
+    _RequiredCreateVariantStoreRequestRequestTypeDef,
+    _OptionalCreateVariantStoreRequestRequestTypeDef,
+):
+    pass
+
 _RequiredReferenceStoreDetailTypeDef = TypedDict(
     "_RequiredReferenceStoreDetailTypeDef",
     {
         "arn": str,
         "id": str,
         "creationTime": datetime,
     },
 )
 _OptionalReferenceStoreDetailTypeDef = TypedDict(
     "_OptionalReferenceStoreDetailTypeDef",
     {
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
     },
     total=False,
 )
 
 class ReferenceStoreDetailTypeDef(
     _RequiredReferenceStoreDetailTypeDef, _OptionalReferenceStoreDetailTypeDef
 ):
@@ -1743,35 +1727,35 @@
     },
 )
 _OptionalSequenceStoreDetailTypeDef = TypedDict(
     "_OptionalSequenceStoreDetailTypeDef",
     {
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "fallbackLocation": str,
     },
     total=False,
 )
 
 class SequenceStoreDetailTypeDef(
     _RequiredSequenceStoreDetailTypeDef, _OptionalSequenceStoreDetailTypeDef
 ):
     pass
 
 VariantStoreItemTypeDef = TypedDict(
     "VariantStoreItemTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "statusMessage": str,
         "storeSizeBytes": int,
     },
 )
 
@@ -1812,15 +1796,15 @@
 CreateReferenceStoreResponseTypeDef = TypedDict(
     "CreateReferenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRunGroupResponseTypeDef = TypedDict(
     "CreateRunGroupResponseTypeDef",
@@ -1835,26 +1819,26 @@
 CreateSequenceStoreResponseTypeDef = TypedDict(
     "CreateSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVariantStoreResponseTypeDef = TypedDict(
     "CreateVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1925,15 +1909,15 @@
 GetReferenceStoreResponseTypeDef = TypedDict(
     "GetReferenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRunGroupResponseTypeDef = TypedDict(
     "GetRunGroupResponseTypeDef",
@@ -2003,31 +1987,31 @@
 GetSequenceStoreResponseTypeDef = TypedDict(
     "GetSequenceStoreResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "fallbackLocation": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVariantStoreResponseTypeDef = TypedDict(
     "GetVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
         "statusMessage": str,
         "storeSizeBytes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2133,15 +2117,15 @@
     },
 )
 
 UpdateVariantStoreResponseTypeDef = TypedDict(
     "UpdateVariantStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2160,84 +2144,14 @@
     {
         "sequenceStoreId": str,
         "uploadId": str,
         "parts": Sequence[CompleteReadSetUploadPartListItemTypeDef],
     },
 )
 
-_RequiredCreateReferenceStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReferenceStoreRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateReferenceStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReferenceStoreRequestRequestTypeDef",
-    {
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "tags": Mapping[str, str],
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreateReferenceStoreRequestRequestTypeDef(
-    _RequiredCreateReferenceStoreRequestRequestTypeDef,
-    _OptionalCreateReferenceStoreRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateSequenceStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSequenceStoreRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSequenceStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSequenceStoreRequestRequestTypeDef",
-    {
-        "description": str,
-        "sseConfig": SseConfigTypeDef,
-        "tags": Mapping[str, str],
-        "clientToken": str,
-        "fallbackLocation": str,
-    },
-    total=False,
-)
-
-class CreateSequenceStoreRequestRequestTypeDef(
-    _RequiredCreateSequenceStoreRequestRequestTypeDef,
-    _OptionalCreateSequenceStoreRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateVariantStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVariantStoreRequestRequestTypeDef",
-    {
-        "reference": ReferenceItemTypeDef,
-    },
-)
-_OptionalCreateVariantStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVariantStoreRequestRequestTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
-    },
-    total=False,
-)
-
-class CreateVariantStoreRequestRequestTypeDef(
-    _RequiredCreateVariantStoreRequestRequestTypeDef,
-    _OptionalCreateVariantStoreRequestRequestTypeDef,
-):
-    pass
-
 _RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowRequestRequestTypeDef",
     {
         "requestId": str,
     },
 )
 _OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
@@ -2258,14 +2172,38 @@
 )
 
 class CreateWorkflowRequestRequestTypeDef(
     _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
 ):
     pass
 
+GetWorkflowResponseTypeDef = TypedDict(
+    "GetWorkflowResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "status": WorkflowStatusType,
+        "type": WorkflowTypeType,
+        "name": str,
+        "description": str,
+        "engine": WorkflowEngineType,
+        "definition": str,
+        "main": str,
+        "digest": str,
+        "parameterTemplate": Dict[str, WorkflowParameterTypeDef],
+        "storageCapacity": int,
+        "creationTime": datetime,
+        "statusMessage": str,
+        "tags": Dict[str, str],
+        "metadata": Dict[str, str],
+        "accelerators": Literal["GPU"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetReadSetExportJobResponseTypeDef = TypedDict(
     "GetReadSetExportJobResponseTypeDef",
     {
         "id": str,
         "sequenceStoreId": str,
         "destination": str,
         "status": ReadSetExportJobStatusType,
@@ -2715,38 +2653,14 @@
         "items": List[VariantImportItemDetailTypeDef],
         "runLeftNormalization": bool,
         "annotationFields": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetWorkflowResponseTypeDef = TypedDict(
-    "GetWorkflowResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": WorkflowStatusType,
-        "type": WorkflowTypeType,
-        "name": str,
-        "description": str,
-        "engine": WorkflowEngineType,
-        "definition": str,
-        "main": str,
-        "digest": str,
-        "parameterTemplate": Dict[str, WorkflowParameterOutputTypeDef],
-        "storageCapacity": int,
-        "creationTime": datetime,
-        "statusMessage": str,
-        "tags": Dict[str, str],
-        "metadata": Dict[str, str],
-        "accelerators": Literal["GPU"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredListReadSetImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReadSetImportJobsRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
     },
 )
 _OptionalListReadSetImportJobsRequestRequestTypeDef = TypedDict(
@@ -2773,15 +2687,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportReadSetSourceItemTypeDef = TypedDict(
     "_RequiredImportReadSetSourceItemTypeDef",
     {
-        "sourceFiles": SourceFilesOutputTypeDef,
+        "sourceFiles": SourceFilesTypeDef,
         "sourceFileType": FileTypeType,
         "status": ReadSetImportJobItemStatusType,
         "subjectId": str,
         "sampleId": str,
     },
 )
 _OptionalImportReadSetSourceItemTypeDef = TypedDict(
@@ -2798,14 +2712,40 @@
 )
 
 class ImportReadSetSourceItemTypeDef(
     _RequiredImportReadSetSourceItemTypeDef, _OptionalImportReadSetSourceItemTypeDef
 ):
     pass
 
+_RequiredStartReadSetImportJobSourceItemTypeDef = TypedDict(
+    "_RequiredStartReadSetImportJobSourceItemTypeDef",
+    {
+        "sourceFiles": SourceFilesTypeDef,
+        "sourceFileType": FileTypeType,
+        "subjectId": str,
+        "sampleId": str,
+        "referenceArn": str,
+    },
+)
+_OptionalStartReadSetImportJobSourceItemTypeDef = TypedDict(
+    "_OptionalStartReadSetImportJobSourceItemTypeDef",
+    {
+        "generatedFrom": str,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartReadSetImportJobSourceItemTypeDef(
+    _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
+):
+    pass
+
 _RequiredListReferenceImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListReferenceImportJobsRequestRequestTypeDef",
     {
         "referenceStoreId": str,
     },
 )
 _OptionalListReferenceImportJobsRequestRequestTypeDef = TypedDict(
@@ -3309,56 +3249,22 @@
     {
         "items": List[WorkflowListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TsvOptionsOutputTypeDef = TypedDict(
-    "TsvOptionsOutputTypeDef",
-    {
-        "readOptions": ReadOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 TsvOptionsTypeDef = TypedDict(
     "TsvOptionsTypeDef",
     {
         "readOptions": ReadOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredStartReadSetImportJobSourceItemTypeDef = TypedDict(
-    "_RequiredStartReadSetImportJobSourceItemTypeDef",
-    {
-        "sourceFiles": SourceFilesTypeDef,
-        "sourceFileType": FileTypeType,
-        "subjectId": str,
-        "sampleId": str,
-        "referenceArn": str,
-    },
-)
-_OptionalStartReadSetImportJobSourceItemTypeDef = TypedDict(
-    "_OptionalStartReadSetImportJobSourceItemTypeDef",
-    {
-        "generatedFrom": str,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class StartReadSetImportJobSourceItemTypeDef(
-    _RequiredStartReadSetImportJobSourceItemTypeDef, _OptionalStartReadSetImportJobSourceItemTypeDef
-):
-    pass
-
 _RequiredStartReadSetActivationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetActivationJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "sources": Sequence[StartReadSetActivationJobSourceItemTypeDef],
     },
 )
@@ -3531,32 +3437,14 @@
         "creationTime": datetime,
         "completionTime": datetime,
         "sources": List[ImportReadSetSourceItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FormatOptionsOutputTypeDef = TypedDict(
-    "FormatOptionsOutputTypeDef",
-    {
-        "tsvOptions": TsvOptionsOutputTypeDef,
-        "vcfOptions": VcfOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-FormatOptionsTypeDef = TypedDict(
-    "FormatOptionsTypeDef",
-    {
-        "tsvOptions": TsvOptionsTypeDef,
-        "vcfOptions": VcfOptionsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredStartReadSetImportJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartReadSetImportJobRequestRequestTypeDef",
     {
         "sequenceStoreId": str,
         "roleArn": str,
         "sources": Sequence[StartReadSetImportJobSourceItemTypeDef],
     },
@@ -3571,38 +3459,47 @@
 
 class StartReadSetImportJobRequestRequestTypeDef(
     _RequiredStartReadSetImportJobRequestRequestTypeDef,
     _OptionalStartReadSetImportJobRequestRequestTypeDef,
 ):
     pass
 
+FormatOptionsTypeDef = TypedDict(
+    "FormatOptionsTypeDef",
+    {
+        "tsvOptions": TsvOptionsTypeDef,
+        "vcfOptions": VcfOptionsTypeDef,
+    },
+    total=False,
+)
+
 CreateAnnotationStoreResponseTypeDef = TypedDict(
     "CreateAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "storeFormat": StoreFormatType,
         "storeOptions": StoreOptionsOutputTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAnnotationStoreResponseTypeDef = TypedDict(
     "GetAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "storeArn": str,
         "name": str,
         "description": str,
-        "sseConfig": SseConfigOutputTypeDef,
+        "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
         "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
         "statusMessage": str,
         "storeSizeBytes": int,
@@ -3610,15 +3507,15 @@
     },
 )
 
 UpdateAnnotationStoreResponseTypeDef = TypedDict(
     "UpdateAnnotationStoreResponseTypeDef",
     {
         "id": str,
-        "reference": ReferenceItemOutputTypeDef,
+        "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "storeOptions": StoreOptionsOutputTypeDef,
         "storeFormat": StoreFormatType,
@@ -3660,15 +3557,15 @@
         "status": JobStatusType,
         "statusMessage": str,
         "creationTime": datetime,
         "updateTime": datetime,
         "completionTime": datetime,
         "items": List[AnnotationImportItemDetailTypeDef],
         "runLeftNormalization": bool,
-        "formatOptions": FormatOptionsOutputTypeDef,
+        "formatOptions": FormatOptionsTypeDef,
         "annotationFields": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartAnnotationImportRequestRequestTypeDef = TypedDict(
     "_RequiredStartAnnotationImportRequestRequestTypeDef",
```

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/waiter.py` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics/waiter.pyi` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/PKG-INFO` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.12
-Summary: Type annotations for boto3.Omics 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
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
 [mypy-boto3-omics docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -514,25 +514,23 @@
     AbortMultipartReadSetUploadRequestRequestTypeDef,
     ActivateReadSetFilterTypeDef,
     ActivateReadSetJobItemTypeDef,
     ActivateReadSetSourceItemTypeDef,
     AnnotationImportItemDetailTypeDef,
     AnnotationImportItemSourceTypeDef,
     AnnotationImportJobItemTypeDef,
-    ReferenceItemOutputTypeDef,
-    SseConfigOutputTypeDef,
+    ReferenceItemTypeDef,
+    SseConfigTypeDef,
     BatchDeleteReadSetRequestRequestTypeDef,
     ReadSetBatchErrorTypeDef,
     ResponseMetadataTypeDef,
     CancelAnnotationImportRequestRequestTypeDef,
     CancelRunRequestRequestTypeDef,
     CancelVariantImportRequestRequestTypeDef,
     CompleteReadSetUploadPartListItemTypeDef,
-    ReferenceItemTypeDef,
-    SseConfigTypeDef,
     CreateMultipartReadSetUploadRequestRequestTypeDef,
     CreateRunGroupRequestRequestTypeDef,
     WorkflowParameterTypeDef,
     DeleteAnnotationStoreRequestRequestTypeDef,
     DeleteReferenceRequestRequestTypeDef,
     DeleteReferenceStoreRequestRequestTypeDef,
     DeleteRunGroupRequestRequestTypeDef,
@@ -541,15 +539,14 @@
     DeleteVariantStoreRequestRequestTypeDef,
     DeleteWorkflowRequestRequestTypeDef,
     ExportReadSetDetailTypeDef,
     ExportReadSetFilterTypeDef,
     ExportReadSetJobDetailTypeDef,
     ExportReadSetTypeDef,
     FileInformationTypeDef,
-    VcfOptionsOutputTypeDef,
     VcfOptionsTypeDef,
     WaiterConfigTypeDef,
     GetAnnotationImportRequestRequestTypeDef,
     GetAnnotationStoreRequestRequestTypeDef,
     GetReadSetActivationJobRequestRequestTypeDef,
     GetReadSetExportJobRequestRequestTypeDef,
     GetReadSetImportJobRequestRequestTypeDef,
@@ -565,18 +562,17 @@
     GetRunRequestRequestTypeDef,
     GetRunTaskRequestRequestTypeDef,
     GetSequenceStoreRequestRequestTypeDef,
     GetVariantImportRequestRequestTypeDef,
     VariantImportItemDetailTypeDef,
     GetVariantStoreRequestRequestTypeDef,
     GetWorkflowRequestRequestTypeDef,
-    WorkflowParameterOutputTypeDef,
     ImportReadSetFilterTypeDef,
     ImportReadSetJobItemTypeDef,
-    SourceFilesOutputTypeDef,
+    SourceFilesTypeDef,
     ImportReferenceFilterTypeDef,
     ImportReferenceJobItemTypeDef,
     ListAnnotationImportJobsFilterTypeDef,
     PaginatorConfigTypeDef,
     ListAnnotationStoresFilterTypeDef,
     ListMultipartReadSetUploadsRequestRequestTypeDef,
     MultipartReadSetUploadListItemTypeDef,
@@ -595,17 +591,15 @@
     SequenceStoreFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListVariantImportJobsFilterTypeDef,
     VariantImportJobItemTypeDef,
     ListVariantStoresFilterTypeDef,
     ListWorkflowsRequestRequestTypeDef,
     WorkflowListItemTypeDef,
-    ReadOptionsOutputTypeDef,
     ReadOptionsTypeDef,
-    SourceFilesTypeDef,
     StartReadSetActivationJobSourceItemTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunRequestRequestTypeDef,
     VariantImportItemSourceTypeDef,
     TsvStoreOptionsOutputTypeDef,
     TsvStoreOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
@@ -613,14 +607,17 @@
     UpdateAnnotationStoreRequestRequestTypeDef,
     UpdateRunGroupRequestRequestTypeDef,
     UpdateVariantStoreRequestRequestTypeDef,
     UpdateWorkflowRequestRequestTypeDef,
     UploadReadSetPartRequestRequestTypeDef,
     ListReadSetActivationJobsRequestRequestTypeDef,
     AnnotationStoreItemTypeDef,
+    CreateReferenceStoreRequestRequestTypeDef,
+    CreateSequenceStoreRequestRequestTypeDef,
+    CreateVariantStoreRequestRequestTypeDef,
     ReferenceStoreDetailTypeDef,
     SequenceStoreDetailTypeDef,
     VariantStoreItemTypeDef,
     BatchDeleteReadSetResponseTypeDef,
     CompleteMultipartReadSetUploadResponseTypeDef,
     CreateMultipartReadSetUploadResponseTypeDef,
     CreateReferenceStoreResponseTypeDef,
@@ -649,18 +646,16 @@
     StartReadSetImportJobResponseTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     CompleteMultipartReadSetUploadRequestRequestTypeDef,
-    CreateReferenceStoreRequestRequestTypeDef,
-    CreateSequenceStoreRequestRequestTypeDef,
-    CreateVariantStoreRequestRequestTypeDef,
     CreateWorkflowRequestRequestTypeDef,
+    GetWorkflowResponseTypeDef,
     GetReadSetExportJobResponseTypeDef,
     ListReadSetExportJobsRequestRequestTypeDef,
     ListReadSetExportJobsResponseTypeDef,
     StartReadSetExportJobRequestRequestTypeDef,
     ReadSetFilesTypeDef,
     ReferenceFilesTypeDef,
     GetAnnotationImportRequestAnnotationImportJobCreatedWaitTypeDef,
@@ -677,18 +672,18 @@
     GetVariantImportRequestVariantImportJobCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreCreatedWaitTypeDef,
     GetVariantStoreRequestVariantStoreDeletedWaitTypeDef,
     GetWorkflowRequestWorkflowActiveWaitTypeDef,
     ReadSetListItemTypeDef,
     GetReferenceImportJobResponseTypeDef,
     GetVariantImportResponseTypeDef,
-    GetWorkflowResponseTypeDef,
     ListReadSetImportJobsRequestRequestTypeDef,
     ListReadSetImportJobsResponseTypeDef,
     ImportReadSetSourceItemTypeDef,
+    StartReadSetImportJobSourceItemTypeDef,
     ListReferenceImportJobsRequestRequestTypeDef,
     ListReferenceImportJobsResponseTypeDef,
     ListAnnotationImportJobsRequestRequestTypeDef,
     ListAnnotationImportJobsRequestListAnnotationImportJobsPaginateTypeDef,
     ListMultipartReadSetUploadsRequestListMultipartReadSetUploadsPaginateTypeDef,
     ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef,
     ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef,
@@ -718,33 +713,30 @@
     ListSequenceStoresRequestRequestTypeDef,
     ListVariantImportJobsRequestListVariantImportJobsPaginateTypeDef,
     ListVariantImportJobsRequestRequestTypeDef,
     ListVariantImportJobsResponseTypeDef,
     ListVariantStoresRequestListVariantStoresPaginateTypeDef,
     ListVariantStoresRequestRequestTypeDef,
     ListWorkflowsResponseTypeDef,
-    TsvOptionsOutputTypeDef,
     TsvOptionsTypeDef,
-    StartReadSetImportJobSourceItemTypeDef,
     StartReadSetActivationJobRequestRequestTypeDef,
     StartReferenceImportJobRequestRequestTypeDef,
     StartVariantImportRequestRequestTypeDef,
     StoreOptionsOutputTypeDef,
     StoreOptionsTypeDef,
     ListAnnotationStoresResponseTypeDef,
     ListReferenceStoresResponseTypeDef,
     ListSequenceStoresResponseTypeDef,
     ListVariantStoresResponseTypeDef,
     GetReadSetMetadataResponseTypeDef,
     GetReferenceMetadataResponseTypeDef,
     ListReadSetsResponseTypeDef,
     GetReadSetImportJobResponseTypeDef,
-    FormatOptionsOutputTypeDef,
-    FormatOptionsTypeDef,
     StartReadSetImportJobRequestRequestTypeDef,
+    FormatOptionsTypeDef,
     CreateAnnotationStoreResponseTypeDef,
     GetAnnotationStoreResponseTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     CreateAnnotationStoreRequestRequestTypeDef,
     GetAnnotationImportResponseTypeDef,
     StartAnnotationImportRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-omics-1.28.12/mypy_boto3_omics.egg-info/SOURCES.txt` & `mypy-boto3-omics-1.28.15/mypy_boto3_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.12/setup.py` & `mypy-boto3-omics-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-omics",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Omics 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

