# Comparing `tmp/mypy-boto3-mturk-1.28.12.tar.gz` & `tmp/mypy-boto3-mturk-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mturk-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
+gzip compressed data, was "mypy-boto3-mturk-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
```

## Comparing `mypy-boto3-mturk-1.28.12.tar` & `mypy-boto3-mturk-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.496428 mypy-boto3-mturk-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18357 2023-07-27 05:35:04.492428 mypy-boto3-mturk-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.488428 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33295 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33240 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39632 2023-07-27 05:26:49.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39572 2023-07-27 05:26:48.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.488428 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18357 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 05:35:04.000000 mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.496428 mypy-boto3-mturk-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-27 05:26:47.000000 mypy-boto3-mturk-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.389558 mypy-boto3-mturk-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-07-28 20:43:21.385558 mypy-boto3-mturk-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.381558 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33295 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33240 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-07-28 20:32:13.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39176 2023-07-28 20:32:14.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39118 2023-07-28 20:32:14.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.385558 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18332 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-28 20:43:21.000000 mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.389558 mypy-boto3-mturk-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-28 20:32:12.000000 mypy-boto3-mturk-1.28.15/setup.py
```

### Comparing `mypy-boto3-mturk-1.28.12/LICENSE` & `mypy-boto3-mturk-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.12/PKG-INFO` & `mypy-boto3-mturk-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.28.12
-Summary: Type annotations for boto3.MTurk 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -378,89 +378,88 @@
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    CreateHITTypeResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
-    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
-    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
-    LocaleOutputTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
     UpdateExpirationForHITRequestRequestTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
+    CreateHITTypeResponseTypeDef,
+    GetAccountBalanceResponseTypeDef,
+    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     QualificationRequirementOutputTypeDef,
-    QualificationTypeDef,
     QualificationRequirementTypeDef,
+    QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
     PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
     HITTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
     ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
```

### Comparing `mypy-boto3-mturk-1.28.12/README.md` & `mypy-boto3-mturk-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -346,89 +346,88 @@
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    CreateHITTypeResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
-    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
-    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
-    LocaleOutputTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
     UpdateExpirationForHITRequestRequestTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
+    CreateHITTypeResponseTypeDef,
+    GetAccountBalanceResponseTypeDef,
+    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     QualificationRequirementOutputTypeDef,
-    QualificationTypeDef,
     QualificationRequirementTypeDef,
+    QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
     PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
     HITTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
     ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
```

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__init__.py` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__init__.pyi` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/__main__.py` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MTurk 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.MTurk 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk\nOther"
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

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/client.py` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/client.pyi` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/literals.py` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/literals.pyi` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/paginator.py` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/paginator.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -61,172 +61,161 @@
     "ListQualificationRequestsPaginator",
     "ListQualificationTypesPaginator",
     "ListReviewableHITsPaginator",
     "ListWorkerBlocksPaginator",
     "ListWorkersWithQualificationTypePaginator",
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
 class ListAssignmentsForHITPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listassignmentsforhitpaginator)
     """
 
     def paginate(
         self,
         *,
         HITId: str,
         AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssignmentsForHITResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listassignmentsforhitpaginator)
         """
 
-
 class ListBonusPaymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listbonuspaymentspaginator)
     """
 
     def paginate(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBonusPaymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listbonuspaymentspaginator)
         """
 
-
 class ListHITsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitspaginator)
         """
 
-
 class ListHITsForQualificationTypePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitsforqualificationtypepaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QualificationTypeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHITsForQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitsforqualificationtypepaginator)
         """
 
-
 class ListQualificationRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationrequestspaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QualificationTypeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQualificationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationrequestspaginator)
         """
 
-
 class ListQualificationTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationtypespaginator)
     """
 
     def paginate(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQualificationTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationtypespaginator)
         """
 
-
 class ListReviewableHITsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listreviewablehitspaginator)
     """
 
     def paginate(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReviewableHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listreviewablehitspaginator)
         """
 
-
 class ListWorkerBlocksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerblockspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkerBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerblockspaginator)
         """
 
-
 class ListWorkersWithQualificationTypePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerswithqualificationtypepaginator)
     """
 
     def paginate(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkersWithQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerswithqualificationtypepaginator)
         """
```

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/paginator.pyi` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,161 +61,172 @@
     "ListQualificationRequestsPaginator",
     "ListQualificationTypesPaginator",
     "ListReviewableHITsPaginator",
     "ListWorkerBlocksPaginator",
     "ListWorkersWithQualificationTypePaginator",
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
 class ListAssignmentsForHITPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listassignmentsforhitpaginator)
     """
 
     def paginate(
         self,
         *,
         HITId: str,
         AssignmentStatuses: Sequence[AssignmentStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAssignmentsForHITResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListAssignmentsForHIT.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listassignmentsforhitpaginator)
         """
 
+
 class ListBonusPaymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listbonuspaymentspaginator)
     """
 
     def paginate(
         self,
         *,
         HITId: str = ...,
         AssignmentId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBonusPaymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListBonusPayments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listbonuspaymentspaginator)
         """
 
+
 class ListHITsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitspaginator)
         """
 
+
 class ListHITsForQualificationTypePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitsforqualificationtypepaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QualificationTypeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListHITsForQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListHITsForQualificationType.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listhitsforqualificationtypepaginator)
         """
 
+
 class ListQualificationRequestsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationrequestspaginator)
     """
 
     def paginate(
-        self, *, QualificationTypeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QualificationTypeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQualificationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationrequestspaginator)
         """
 
+
 class ListQualificationTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationtypespaginator)
     """
 
     def paginate(
         self,
         *,
         MustBeRequestable: bool,
         Query: str = ...,
         MustBeOwnedByCaller: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQualificationTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListQualificationTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listqualificationtypespaginator)
         """
 
+
 class ListReviewableHITsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listreviewablehitspaginator)
     """
 
     def paginate(
         self,
         *,
         HITTypeId: str = ...,
         Status: ReviewableHITStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReviewableHITsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListReviewableHITs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listreviewablehitspaginator)
         """
 
+
 class ListWorkerBlocksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerblockspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkerBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkerBlocks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerblockspaginator)
         """
 
+
 class ListWorkersWithQualificationTypePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerswithqualificationtypepaginator)
     """
 
     def paginate(
         self,
         *,
         QualificationTypeId: str,
         Status: QualificationStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListWorkersWithQualificationTypeResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Paginator.ListWorkersWithQualificationType.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/paginators/#listworkerswithqualificationtypepaginator)
         """
```

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/type_defs.py` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,89 +41,88 @@
     "AcceptQualificationRequestRequestRequestTypeDef",
     "ApproveAssignmentRequestRequestTypeDef",
     "AssignmentTypeDef",
     "AssociateQualificationWithWorkerRequestRequestTypeDef",
     "BonusPaymentTypeDef",
     "CreateAdditionalAssignmentsForHITRequestRequestTypeDef",
     "HITLayoutParameterTypeDef",
-    "CreateHITTypeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateQualificationTypeRequestRequestTypeDef",
     "QualificationTypeTypeDef",
     "CreateWorkerBlockRequestRequestTypeDef",
     "DeleteHITRequestRequestTypeDef",
     "DeleteQualificationTypeRequestRequestTypeDef",
     "DeleteWorkerBlockRequestRequestTypeDef",
     "DisassociateQualificationFromWorkerRequestRequestTypeDef",
-    "GetAccountBalanceResponseTypeDef",
     "GetAssignmentRequestRequestTypeDef",
     "GetFileUploadURLRequestRequestTypeDef",
-    "GetFileUploadURLResponseTypeDef",
     "GetHITRequestRequestTypeDef",
     "GetQualificationScoreRequestRequestTypeDef",
     "GetQualificationTypeRequestRequestTypeDef",
-    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssignmentsForHITRequestRequestTypeDef",
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
     "ListBonusPaymentsRequestRequestTypeDef",
-    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
     "ListHITsForQualificationTypeRequestRequestTypeDef",
-    "ListHITsRequestListHITsPaginateTypeDef",
     "ListHITsRequestRequestTypeDef",
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
     "ListQualificationRequestsRequestRequestTypeDef",
     "QualificationRequestTypeDef",
-    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
     "ListQualificationTypesRequestRequestTypeDef",
     "ListReviewPolicyResultsForHITRequestRequestTypeDef",
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListReviewableHITsRequestRequestTypeDef",
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
-    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
-    "LocaleOutputTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
     "UpdateExpirationForHITRequestRequestTypeDef",
     "UpdateHITReviewStatusRequestRequestTypeDef",
     "UpdateHITTypeOfHITRequestRequestTypeDef",
     "UpdateQualificationTypeRequestRequestTypeDef",
+    "CreateHITTypeResponseTypeDef",
+    "GetAccountBalanceResponseTypeDef",
+    "GetFileUploadURLResponseTypeDef",
     "ListAssignmentsForHITResponseTypeDef",
     "ListBonusPaymentsResponseTypeDef",
     "CreateQualificationTypeResponseTypeDef",
     "GetQualificationTypeResponseTypeDef",
     "ListQualificationTypesResponseTypeDef",
     "UpdateQualificationTypeResponseTypeDef",
+    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    "ListHITsRequestListHITsPaginateTypeDef",
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
     "QualificationRequirementOutputTypeDef",
-    "QualificationTypeDef",
     "QualificationRequirementTypeDef",
+    "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
     "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
     "HITTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
     "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
@@ -260,19 +259,22 @@
     "HITLayoutParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-CreateHITTypeResponseTypeDef = TypedDict(
-    "CreateHITTypeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "HITTypeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQualificationTypeRequestRequestTypeDef",
     {
         "Name": str,
@@ -384,23 +386,14 @@
 class DisassociateQualificationFromWorkerRequestRequestTypeDef(
     _RequiredDisassociateQualificationFromWorkerRequestRequestTypeDef,
     _OptionalDisassociateQualificationFromWorkerRequestRequestTypeDef,
 ):
     pass
 
 
-GetAccountBalanceResponseTypeDef = TypedDict(
-    "GetAccountBalanceResponseTypeDef",
-    {
-        "AvailableBalance": str,
-        "OnHoldBalance": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAssignmentRequestRequestTypeDef = TypedDict(
     "GetAssignmentRequestRequestTypeDef",
     {
         "AssignmentId": str,
     },
 )
 
@@ -408,22 +401,14 @@
     "GetFileUploadURLRequestRequestTypeDef",
     {
         "AssignmentId": str,
         "QuestionIdentifier": str,
     },
 )
 
-GetFileUploadURLResponseTypeDef = TypedDict(
-    "GetFileUploadURLResponseTypeDef",
-    {
-        "FileUploadURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHITRequestRequestTypeDef = TypedDict(
     "GetHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 
@@ -438,37 +423,24 @@
 GetQualificationTypeRequestRequestTypeDef = TypedDict(
     "GetQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 
-_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    {
-        "HITId": str,
-    },
-)
-_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AssignmentStatuses": Sequence[AssignmentStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
-    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAssignmentsForHITRequestRequestTypeDef = TypedDict(
     "_RequiredListAssignmentsForHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalListAssignmentsForHITRequestRequestTypeDef = TypedDict(
@@ -485,57 +457,25 @@
 class ListAssignmentsForHITRequestRequestTypeDef(
     _RequiredListAssignmentsForHITRequestRequestTypeDef,
     _OptionalListAssignmentsForHITRequestRequestTypeDef,
 ):
     pass
 
 
-ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
-    {
-        "HITId": str,
-        "AssignmentId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBonusPaymentsRequestRequestTypeDef = TypedDict(
     "ListBonusPaymentsRequestRequestTypeDef",
     {
         "HITId": str,
         "AssignmentId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
-    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListHITsForQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -551,40 +491,23 @@
 class ListHITsForQualificationTypeRequestRequestTypeDef(
     _RequiredListHITsForQualificationTypeRequestRequestTypeDef,
     _OptionalListHITsForQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
 
-ListHITsRequestListHITsPaginateTypeDef = TypedDict(
-    "ListHITsRequestListHITsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHITsRequestRequestTypeDef = TypedDict(
     "ListHITsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQualificationRequestsRequestRequestTypeDef = TypedDict(
     "ListQualificationRequestsRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -600,38 +523,14 @@
         "Test": str,
         "Answer": str,
         "SubmitTime": datetime,
     },
     total=False,
 )
 
-_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "MustBeRequestable": bool,
-    },
-)
-_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "Query": str,
-        "MustBeOwnedByCaller": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
-    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListQualificationTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListQualificationTypesRequestRequestTypeDef",
     {
         "MustBeRequestable": bool,
     },
 )
 _OptionalListQualificationTypesRequestRequestTypeDef = TypedDict(
@@ -675,43 +574,25 @@
 class ListReviewPolicyResultsForHITRequestRequestTypeDef(
     _RequiredListReviewPolicyResultsForHITRequestRequestTypeDef,
     _OptionalListReviewPolicyResultsForHITRequestRequestTypeDef,
 ):
     pass
 
 
-ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
-    {
-        "HITTypeId": str,
-        "Status": ReviewableHITStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReviewableHITsRequestRequestTypeDef = TypedDict(
     "ListReviewableHITsRequestRequestTypeDef",
     {
         "HITTypeId": str,
         "Status": ReviewableHITStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkerBlocksRequestRequestTypeDef = TypedDict(
     "ListWorkerBlocksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -722,37 +603,14 @@
     {
         "WorkerId": str,
         "Reason": str,
     },
     total=False,
 )
 
-_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "Status": QualificationStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
-    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersWithQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -769,33 +627,14 @@
 class ListWorkersWithQualificationTypeRequestRequestTypeDef(
     _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef,
     _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredLocaleOutputTypeDef = TypedDict(
-    "_RequiredLocaleOutputTypeDef",
-    {
-        "Country": str,
-    },
-)
-_OptionalLocaleOutputTypeDef = TypedDict(
-    "_OptionalLocaleOutputTypeDef",
-    {
-        "Subdivision": str,
-    },
-    total=False,
-)
-
-
-class LocaleOutputTypeDef(_RequiredLocaleOutputTypeDef, _OptionalLocaleOutputTypeDef):
-    pass
-
-
 _RequiredLocaleTypeDef = TypedDict(
     "_RequiredLocaleTypeDef",
     {
         "Country": str,
     },
 )
 _OptionalLocaleTypeDef = TypedDict(
@@ -836,24 +675,14 @@
     {
         "Subject": str,
         "MessageText": str,
         "WorkerIds": Sequence[str],
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
 ParameterMapEntryOutputTypeDef = TypedDict(
     "ParameterMapEntryOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
     },
     total=False,
@@ -894,25 +723,14 @@
 class RejectQualificationRequestRequestRequestTypeDef(
     _RequiredRejectQualificationRequestRequestRequestTypeDef,
     _OptionalRejectQualificationRequestRequestRequestTypeDef,
 ):
     pass
 
 
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
 ReviewActionDetailTypeDef = TypedDict(
     "ReviewActionDetailTypeDef",
     {
         "ActionId": str,
         "ActionName": str,
         "TargetId": str,
         "TargetType": str,
@@ -1024,126 +842,275 @@
 class UpdateQualificationTypeRequestRequestTypeDef(
     _RequiredUpdateQualificationTypeRequestRequestTypeDef,
     _OptionalUpdateQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
 
+CreateHITTypeResponseTypeDef = TypedDict(
+    "CreateHITTypeResponseTypeDef",
+    {
+        "HITTypeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountBalanceResponseTypeDef = TypedDict(
+    "GetAccountBalanceResponseTypeDef",
+    {
+        "AvailableBalance": str,
+        "OnHoldBalance": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFileUploadURLResponseTypeDef = TypedDict(
+    "GetFileUploadURLResponseTypeDef",
+    {
+        "FileUploadURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAssignmentsForHITResponseTypeDef = TypedDict(
     "ListAssignmentsForHITResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Assignments": List[AssignmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBonusPaymentsResponseTypeDef = TypedDict(
     "ListBonusPaymentsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "BonusPayments": List[BonusPaymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateQualificationTypeResponseTypeDef = TypedDict(
     "CreateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQualificationTypeResponseTypeDef = TypedDict(
     "GetQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQualificationTypesResponseTypeDef = TypedDict(
     "ListQualificationTypesResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationTypes": List[QualificationTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQualificationTypeResponseTypeDef = TypedDict(
     "UpdateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "HITId": str,
+    },
+)
+_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "AssignmentStatuses": Sequence[AssignmentStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
+    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+):
+    pass
+
+
+ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    {
+        "HITId": str,
+        "AssignmentId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
+    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+):
+    pass
+
+
+ListHITsRequestListHITsPaginateTypeDef = TypedDict(
+    "ListHITsRequestListHITsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "MustBeRequestable": bool,
+    },
+)
+_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "Query": str,
+        "MustBeOwnedByCaller": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
+    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+):
+    pass
+
+
+ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    {
+        "HITTypeId": str,
+        "Status": ReviewableHITStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "Status": QualificationStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
+    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+):
+    pass
+
+
 ListQualificationRequestsResponseTypeDef = TypedDict(
     "ListQualificationRequestsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationRequests": List[QualificationRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkerBlocksResponseTypeDef = TypedDict(
     "ListWorkerBlocksResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredQualificationRequirementOutputTypeDef = TypedDict(
     "_RequiredQualificationRequirementOutputTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
 _OptionalQualificationRequirementOutputTypeDef = TypedDict(
     "_OptionalQualificationRequirementOutputTypeDef",
     {
         "IntegerValues": List[int],
-        "LocaleValues": List[LocaleOutputTypeDef],
+        "LocaleValues": List[LocaleTypeDef],
         "RequiredToPreview": bool,
         "ActionsGuarded": HITAccessActionsType,
     },
     total=False,
 )
 
 
 class QualificationRequirementOutputTypeDef(
     _RequiredQualificationRequirementOutputTypeDef, _OptionalQualificationRequirementOutputTypeDef
 ):
     pass
 
 
-QualificationTypeDef = TypedDict(
-    "QualificationTypeDef",
-    {
-        "QualificationTypeId": str,
-        "WorkerId": str,
-        "GrantTime": datetime,
-        "IntegerValue": int,
-        "LocaleValue": LocaleOutputTypeDef,
-        "Status": QualificationStatusType,
-    },
-    total=False,
-)
-
 _RequiredQualificationRequirementTypeDef = TypedDict(
     "_RequiredQualificationRequirementTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
@@ -1161,14 +1128,27 @@
 
 class QualificationRequirementTypeDef(
     _RequiredQualificationRequirementTypeDef, _OptionalQualificationRequirementTypeDef
 ):
     pass
 
 
+QualificationTypeDef = TypedDict(
+    "QualificationTypeDef",
+    {
+        "QualificationTypeId": str,
+        "WorkerId": str,
+        "GrantTime": datetime,
+        "IntegerValue": int,
+        "LocaleValue": LocaleTypeDef,
+        "Status": QualificationStatusType,
+    },
+    total=False,
+)
+
 SendTestEventNotificationRequestRequestTypeDef = TypedDict(
     "SendTestEventNotificationRequestRequestTypeDef",
     {
         "Notification": NotificationSpecificationTypeDef,
         "TestEventType": EventTypeType,
     },
 )
@@ -1196,15 +1176,15 @@
     pass
 
 
 NotifyWorkersResponseTypeDef = TypedDict(
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyParameterOutputTypeDef = TypedDict(
     "PolicyParameterOutputTypeDef",
     {
         "Key": str,
@@ -1257,32 +1237,14 @@
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
 
-GetQualificationScoreResponseTypeDef = TypedDict(
-    "GetQualificationScoreResponseTypeDef",
-    {
-        "Qualification": QualificationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWorkersWithQualificationTypeResponseTypeDef = TypedDict(
-    "ListWorkersWithQualificationTypeResponseTypeDef",
-    {
-        "NextToken": str,
-        "NumResults": int,
-        "Qualifications": List[QualificationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITTypeRequestRequestTypeDef",
     {
         "AssignmentDurationInSeconds": int,
         "Reward": str,
         "Title": str,
         "Description": str,
@@ -1301,14 +1263,32 @@
 
 class CreateHITTypeRequestRequestTypeDef(
     _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
 ):
     pass
 
 
+GetQualificationScoreResponseTypeDef = TypedDict(
+    "GetQualificationScoreResponseTypeDef",
+    {
+        "Qualification": QualificationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListWorkersWithQualificationTypeResponseTypeDef = TypedDict(
+    "ListWorkersWithQualificationTypeResponseTypeDef",
+    {
+        "NextToken": str,
+        "NumResults": int,
+        "Qualifications": List[QualificationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredReviewPolicyOutputTypeDef = TypedDict(
     "_RequiredReviewPolicyOutputTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalReviewPolicyOutputTypeDef = TypedDict(
@@ -1345,83 +1325,83 @@
     pass
 
 
 CreateHITResponseTypeDef = TypedDict(
     "CreateHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHITWithHITTypeResponseTypeDef = TypedDict(
     "CreateHITWithHITTypeResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssignmentResponseTypeDef = TypedDict(
     "GetAssignmentResponseTypeDef",
     {
         "Assignment": AssignmentTypeDef,
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHITResponseTypeDef = TypedDict(
     "GetHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHITsForQualificationTypeResponseTypeDef = TypedDict(
     "ListHITsForQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHITsResponseTypeDef = TypedDict(
     "ListHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReviewableHITsResponseTypeDef = TypedDict(
     "ListReviewableHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
     "ListReviewPolicyResultsForHITResponseTypeDef",
     {
         "HITId": str,
         "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
         "HITReviewPolicy": ReviewPolicyOutputTypeDef,
         "AssignmentReviewReport": ReviewReportTypeDef,
         "HITReviewReport": ReviewReportTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
```

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk/type_defs.pyi` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -40,89 +40,88 @@
     "AcceptQualificationRequestRequestRequestTypeDef",
     "ApproveAssignmentRequestRequestTypeDef",
     "AssignmentTypeDef",
     "AssociateQualificationWithWorkerRequestRequestTypeDef",
     "BonusPaymentTypeDef",
     "CreateAdditionalAssignmentsForHITRequestRequestTypeDef",
     "HITLayoutParameterTypeDef",
-    "CreateHITTypeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateQualificationTypeRequestRequestTypeDef",
     "QualificationTypeTypeDef",
     "CreateWorkerBlockRequestRequestTypeDef",
     "DeleteHITRequestRequestTypeDef",
     "DeleteQualificationTypeRequestRequestTypeDef",
     "DeleteWorkerBlockRequestRequestTypeDef",
     "DisassociateQualificationFromWorkerRequestRequestTypeDef",
-    "GetAccountBalanceResponseTypeDef",
     "GetAssignmentRequestRequestTypeDef",
     "GetFileUploadURLRequestRequestTypeDef",
-    "GetFileUploadURLResponseTypeDef",
     "GetHITRequestRequestTypeDef",
     "GetQualificationScoreRequestRequestTypeDef",
     "GetQualificationTypeRequestRequestTypeDef",
-    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAssignmentsForHITRequestRequestTypeDef",
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
     "ListBonusPaymentsRequestRequestTypeDef",
-    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
     "ListHITsForQualificationTypeRequestRequestTypeDef",
-    "ListHITsRequestListHITsPaginateTypeDef",
     "ListHITsRequestRequestTypeDef",
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
     "ListQualificationRequestsRequestRequestTypeDef",
     "QualificationRequestTypeDef",
-    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
     "ListQualificationTypesRequestRequestTypeDef",
     "ListReviewPolicyResultsForHITRequestRequestTypeDef",
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListReviewableHITsRequestRequestTypeDef",
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
-    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
-    "LocaleOutputTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
     "UpdateExpirationForHITRequestRequestTypeDef",
     "UpdateHITReviewStatusRequestRequestTypeDef",
     "UpdateHITTypeOfHITRequestRequestTypeDef",
     "UpdateQualificationTypeRequestRequestTypeDef",
+    "CreateHITTypeResponseTypeDef",
+    "GetAccountBalanceResponseTypeDef",
+    "GetFileUploadURLResponseTypeDef",
     "ListAssignmentsForHITResponseTypeDef",
     "ListBonusPaymentsResponseTypeDef",
     "CreateQualificationTypeResponseTypeDef",
     "GetQualificationTypeResponseTypeDef",
     "ListQualificationTypesResponseTypeDef",
     "UpdateQualificationTypeResponseTypeDef",
+    "ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    "ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    "ListHITsRequestListHITsPaginateTypeDef",
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
     "QualificationRequirementOutputTypeDef",
-    "QualificationTypeDef",
     "QualificationRequirementTypeDef",
+    "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
     "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
     "HITTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
     "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
@@ -251,19 +250,22 @@
     "HITLayoutParameterTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
-CreateHITTypeResponseTypeDef = TypedDict(
-    "CreateHITTypeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "HITTypeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQualificationTypeRequestRequestTypeDef",
     {
         "Name": str,
@@ -369,23 +371,14 @@
 
 class DisassociateQualificationFromWorkerRequestRequestTypeDef(
     _RequiredDisassociateQualificationFromWorkerRequestRequestTypeDef,
     _OptionalDisassociateQualificationFromWorkerRequestRequestTypeDef,
 ):
     pass
 
-GetAccountBalanceResponseTypeDef = TypedDict(
-    "GetAccountBalanceResponseTypeDef",
-    {
-        "AvailableBalance": str,
-        "OnHoldBalance": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAssignmentRequestRequestTypeDef = TypedDict(
     "GetAssignmentRequestRequestTypeDef",
     {
         "AssignmentId": str,
     },
 )
 
@@ -393,22 +386,14 @@
     "GetFileUploadURLRequestRequestTypeDef",
     {
         "AssignmentId": str,
         "QuestionIdentifier": str,
     },
 )
 
-GetFileUploadURLResponseTypeDef = TypedDict(
-    "GetFileUploadURLResponseTypeDef",
-    {
-        "FileUploadURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHITRequestRequestTypeDef = TypedDict(
     "GetHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 
@@ -423,35 +408,24 @@
 GetQualificationTypeRequestRequestTypeDef = TypedDict(
     "GetQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 
-_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
-    {
-        "HITId": str,
-    },
-)
-_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
-    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AssignmentStatuses": Sequence[AssignmentStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
-    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
-):
-    pass
-
 _RequiredListAssignmentsForHITRequestRequestTypeDef = TypedDict(
     "_RequiredListAssignmentsForHITRequestRequestTypeDef",
     {
         "HITId": str,
     },
 )
 _OptionalListAssignmentsForHITRequestRequestTypeDef = TypedDict(
@@ -466,55 +440,25 @@
 
 class ListAssignmentsForHITRequestRequestTypeDef(
     _RequiredListAssignmentsForHITRequestRequestTypeDef,
     _OptionalListAssignmentsForHITRequestRequestTypeDef,
 ):
     pass
 
-ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
-    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
-    {
-        "HITId": str,
-        "AssignmentId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBonusPaymentsRequestRequestTypeDef = TypedDict(
     "ListBonusPaymentsRequestRequestTypeDef",
     {
         "HITId": str,
         "AssignmentId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
-    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
-):
-    pass
-
 _RequiredListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListHITsForQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListHITsForQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -528,40 +472,23 @@
 
 class ListHITsForQualificationTypeRequestRequestTypeDef(
     _RequiredListHITsForQualificationTypeRequestRequestTypeDef,
     _OptionalListHITsForQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
-ListHITsRequestListHITsPaginateTypeDef = TypedDict(
-    "ListHITsRequestListHITsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHITsRequestRequestTypeDef = TypedDict(
     "ListHITsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
-    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQualificationRequestsRequestRequestTypeDef = TypedDict(
     "ListQualificationRequestsRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -577,36 +504,14 @@
         "Test": str,
         "Answer": str,
         "SubmitTime": datetime,
     },
     total=False,
 )
 
-_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "MustBeRequestable": bool,
-    },
-)
-_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
-    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
-    {
-        "Query": str,
-        "MustBeOwnedByCaller": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
-    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredListQualificationTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListQualificationTypesRequestRequestTypeDef",
     {
         "MustBeRequestable": bool,
     },
 )
 _OptionalListQualificationTypesRequestRequestTypeDef = TypedDict(
@@ -646,43 +551,25 @@
 
 class ListReviewPolicyResultsForHITRequestRequestTypeDef(
     _RequiredListReviewPolicyResultsForHITRequestRequestTypeDef,
     _OptionalListReviewPolicyResultsForHITRequestRequestTypeDef,
 ):
     pass
 
-ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
-    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
-    {
-        "HITTypeId": str,
-        "Status": ReviewableHITStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListReviewableHITsRequestRequestTypeDef = TypedDict(
     "ListReviewableHITsRequestRequestTypeDef",
     {
         "HITTypeId": str,
         "Status": ReviewableHITStatusType,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
-    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorkerBlocksRequestRequestTypeDef = TypedDict(
     "ListWorkerBlocksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -693,35 +580,14 @@
     {
         "WorkerId": str,
         "Reason": str,
     },
     total=False,
 )
 
-_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "QualificationTypeId": str,
-    },
-)
-_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
-    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
-    {
-        "Status": QualificationStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
-    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersWithQualificationTypeRequestRequestTypeDef",
     {
         "QualificationTypeId": str,
     },
 )
 _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef = TypedDict(
@@ -736,31 +602,14 @@
 
 class ListWorkersWithQualificationTypeRequestRequestTypeDef(
     _RequiredListWorkersWithQualificationTypeRequestRequestTypeDef,
     _OptionalListWorkersWithQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
-_RequiredLocaleOutputTypeDef = TypedDict(
-    "_RequiredLocaleOutputTypeDef",
-    {
-        "Country": str,
-    },
-)
-_OptionalLocaleOutputTypeDef = TypedDict(
-    "_OptionalLocaleOutputTypeDef",
-    {
-        "Subdivision": str,
-    },
-    total=False,
-)
-
-class LocaleOutputTypeDef(_RequiredLocaleOutputTypeDef, _OptionalLocaleOutputTypeDef):
-    pass
-
 _RequiredLocaleTypeDef = TypedDict(
     "_RequiredLocaleTypeDef",
     {
         "Country": str,
     },
 )
 _OptionalLocaleTypeDef = TypedDict(
@@ -799,24 +648,14 @@
     {
         "Subject": str,
         "MessageText": str,
         "WorkerIds": Sequence[str],
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
 ParameterMapEntryOutputTypeDef = TypedDict(
     "ParameterMapEntryOutputTypeDef",
     {
         "Key": str,
         "Values": List[str],
     },
     total=False,
@@ -855,25 +694,14 @@
 
 class RejectQualificationRequestRequestRequestTypeDef(
     _RequiredRejectQualificationRequestRequestRequestTypeDef,
     _OptionalRejectQualificationRequestRequestRequestTypeDef,
 ):
     pass
 
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
 ReviewActionDetailTypeDef = TypedDict(
     "ReviewActionDetailTypeDef",
     {
         "ActionId": str,
         "ActionName": str,
         "TargetId": str,
         "TargetType": str,
@@ -979,124 +807,265 @@
 
 class UpdateQualificationTypeRequestRequestTypeDef(
     _RequiredUpdateQualificationTypeRequestRequestTypeDef,
     _OptionalUpdateQualificationTypeRequestRequestTypeDef,
 ):
     pass
 
+CreateHITTypeResponseTypeDef = TypedDict(
+    "CreateHITTypeResponseTypeDef",
+    {
+        "HITTypeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountBalanceResponseTypeDef = TypedDict(
+    "GetAccountBalanceResponseTypeDef",
+    {
+        "AvailableBalance": str,
+        "OnHoldBalance": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFileUploadURLResponseTypeDef = TypedDict(
+    "GetFileUploadURLResponseTypeDef",
+    {
+        "FileUploadURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAssignmentsForHITResponseTypeDef = TypedDict(
     "ListAssignmentsForHITResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "Assignments": List[AssignmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBonusPaymentsResponseTypeDef = TypedDict(
     "ListBonusPaymentsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "BonusPayments": List[BonusPaymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateQualificationTypeResponseTypeDef = TypedDict(
     "CreateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQualificationTypeResponseTypeDef = TypedDict(
     "GetQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQualificationTypesResponseTypeDef = TypedDict(
     "ListQualificationTypesResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationTypes": List[QualificationTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQualificationTypeResponseTypeDef = TypedDict(
     "UpdateQualificationTypeResponseTypeDef",
     {
         "QualificationType": QualificationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "HITId": str,
+    },
+)
+_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef = TypedDict(
+    "_OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef",
+    {
+        "AssignmentStatuses": Sequence[AssignmentStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef(
+    _RequiredListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    _OptionalListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+):
+    pass
+
+ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef = TypedDict(
+    "ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef",
+    {
+        "HITId": str,
+        "AssignmentId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef(
+    _RequiredListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    _OptionalListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+):
+    pass
+
+ListHITsRequestListHITsPaginateTypeDef = TypedDict(
+    "ListHITsRequestListHITsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef = TypedDict(
+    "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "MustBeRequestable": bool,
+    },
+)
+_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef = TypedDict(
+    "_OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
+    {
+        "Query": str,
+        "MustBeOwnedByCaller": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListQualificationTypesRequestListQualificationTypesPaginateTypeDef(
+    _RequiredListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    _OptionalListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+):
+    pass
+
+ListReviewableHITsRequestListReviewableHITsPaginateTypeDef = TypedDict(
+    "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
+    {
+        "HITTypeId": str,
+        "Status": ReviewableHITStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef = TypedDict(
+    "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
+_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "QualificationTypeId": str,
+    },
+)
+_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef = TypedDict(
+    "_OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
+    {
+        "Status": QualificationStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef(
+    _RequiredListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+    _OptionalListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
+):
+    pass
+
 ListQualificationRequestsResponseTypeDef = TypedDict(
     "ListQualificationRequestsResponseTypeDef",
     {
         "NumResults": int,
         "NextToken": str,
         "QualificationRequests": List[QualificationRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkerBlocksResponseTypeDef = TypedDict(
     "ListWorkerBlocksResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredQualificationRequirementOutputTypeDef = TypedDict(
     "_RequiredQualificationRequirementOutputTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
 _OptionalQualificationRequirementOutputTypeDef = TypedDict(
     "_OptionalQualificationRequirementOutputTypeDef",
     {
         "IntegerValues": List[int],
-        "LocaleValues": List[LocaleOutputTypeDef],
+        "LocaleValues": List[LocaleTypeDef],
         "RequiredToPreview": bool,
         "ActionsGuarded": HITAccessActionsType,
     },
     total=False,
 )
 
 class QualificationRequirementOutputTypeDef(
     _RequiredQualificationRequirementOutputTypeDef, _OptionalQualificationRequirementOutputTypeDef
 ):
     pass
 
-QualificationTypeDef = TypedDict(
-    "QualificationTypeDef",
-    {
-        "QualificationTypeId": str,
-        "WorkerId": str,
-        "GrantTime": datetime,
-        "IntegerValue": int,
-        "LocaleValue": LocaleOutputTypeDef,
-        "Status": QualificationStatusType,
-    },
-    total=False,
-)
-
 _RequiredQualificationRequirementTypeDef = TypedDict(
     "_RequiredQualificationRequirementTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
@@ -1112,14 +1081,27 @@
 )
 
 class QualificationRequirementTypeDef(
     _RequiredQualificationRequirementTypeDef, _OptionalQualificationRequirementTypeDef
 ):
     pass
 
+QualificationTypeDef = TypedDict(
+    "QualificationTypeDef",
+    {
+        "QualificationTypeId": str,
+        "WorkerId": str,
+        "GrantTime": datetime,
+        "IntegerValue": int,
+        "LocaleValue": LocaleTypeDef,
+        "Status": QualificationStatusType,
+    },
+    total=False,
+)
+
 SendTestEventNotificationRequestRequestTypeDef = TypedDict(
     "SendTestEventNotificationRequestRequestTypeDef",
     {
         "Notification": NotificationSpecificationTypeDef,
         "TestEventType": EventTypeType,
     },
 )
@@ -1145,15 +1127,15 @@
 ):
     pass
 
 NotifyWorkersResponseTypeDef = TypedDict(
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyParameterOutputTypeDef = TypedDict(
     "PolicyParameterOutputTypeDef",
     {
         "Key": str,
@@ -1206,32 +1188,14 @@
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
 
-GetQualificationScoreResponseTypeDef = TypedDict(
-    "GetQualificationScoreResponseTypeDef",
-    {
-        "Qualification": QualificationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListWorkersWithQualificationTypeResponseTypeDef = TypedDict(
-    "ListWorkersWithQualificationTypeResponseTypeDef",
-    {
-        "NextToken": str,
-        "NumResults": int,
-        "Qualifications": List[QualificationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITTypeRequestRequestTypeDef",
     {
         "AssignmentDurationInSeconds": int,
         "Reward": str,
         "Title": str,
         "Description": str,
@@ -1248,14 +1212,32 @@
 )
 
 class CreateHITTypeRequestRequestTypeDef(
     _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
 ):
     pass
 
+GetQualificationScoreResponseTypeDef = TypedDict(
+    "GetQualificationScoreResponseTypeDef",
+    {
+        "Qualification": QualificationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListWorkersWithQualificationTypeResponseTypeDef = TypedDict(
+    "ListWorkersWithQualificationTypeResponseTypeDef",
+    {
+        "NextToken": str,
+        "NumResults": int,
+        "Qualifications": List[QualificationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredReviewPolicyOutputTypeDef = TypedDict(
     "_RequiredReviewPolicyOutputTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalReviewPolicyOutputTypeDef = TypedDict(
@@ -1288,83 +1270,83 @@
 class ReviewPolicyTypeDef(_RequiredReviewPolicyTypeDef, _OptionalReviewPolicyTypeDef):
     pass
 
 CreateHITResponseTypeDef = TypedDict(
     "CreateHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHITWithHITTypeResponseTypeDef = TypedDict(
     "CreateHITWithHITTypeResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssignmentResponseTypeDef = TypedDict(
     "GetAssignmentResponseTypeDef",
     {
         "Assignment": AssignmentTypeDef,
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHITResponseTypeDef = TypedDict(
     "GetHITResponseTypeDef",
     {
         "HIT": HITTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHITsForQualificationTypeResponseTypeDef = TypedDict(
     "ListHITsForQualificationTypeResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHITsResponseTypeDef = TypedDict(
     "ListHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReviewableHITsResponseTypeDef = TypedDict(
     "ListReviewableHITsResponseTypeDef",
     {
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
     "ListReviewPolicyResultsForHITResponseTypeDef",
     {
         "HITId": str,
         "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
         "HITReviewPolicy": ReviewPolicyOutputTypeDef,
         "AssignmentReviewReport": ReviewReportTypeDef,
         "HITReviewReport": ReviewReportTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
```

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/PKG-INFO` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mturk
-Version: 1.28.12
-Summary: Type annotations for boto3.MTurk 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mturk.svg?color=blue)](https://pypi.org/project/mypy-boto3-mturk)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mturk)](https://pepy.tech/project/mypy-boto3-mturk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MTurk 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
+[boto3.MTurk 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk)
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
 [mypy-boto3-mturk docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mturk/).
 
 See how it helps to find and fix potential bugs:
 
@@ -378,89 +378,88 @@
     AcceptQualificationRequestRequestRequestTypeDef,
     ApproveAssignmentRequestRequestTypeDef,
     AssignmentTypeDef,
     AssociateQualificationWithWorkerRequestRequestTypeDef,
     BonusPaymentTypeDef,
     CreateAdditionalAssignmentsForHITRequestRequestTypeDef,
     HITLayoutParameterTypeDef,
-    CreateHITTypeResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateQualificationTypeRequestRequestTypeDef,
     QualificationTypeTypeDef,
     CreateWorkerBlockRequestRequestTypeDef,
     DeleteHITRequestRequestTypeDef,
     DeleteQualificationTypeRequestRequestTypeDef,
     DeleteWorkerBlockRequestRequestTypeDef,
     DisassociateQualificationFromWorkerRequestRequestTypeDef,
-    GetAccountBalanceResponseTypeDef,
     GetAssignmentRequestRequestTypeDef,
     GetFileUploadURLRequestRequestTypeDef,
-    GetFileUploadURLResponseTypeDef,
     GetHITRequestRequestTypeDef,
     GetQualificationScoreRequestRequestTypeDef,
     GetQualificationTypeRequestRequestTypeDef,
-    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAssignmentsForHITRequestRequestTypeDef,
-    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
     ListBonusPaymentsRequestRequestTypeDef,
-    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
     ListHITsForQualificationTypeRequestRequestTypeDef,
-    ListHITsRequestListHITsPaginateTypeDef,
     ListHITsRequestRequestTypeDef,
-    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
     ListQualificationRequestsRequestRequestTypeDef,
     QualificationRequestTypeDef,
-    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
     ListQualificationTypesRequestRequestTypeDef,
     ListReviewPolicyResultsForHITRequestRequestTypeDef,
-    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
     ListReviewableHITsRequestRequestTypeDef,
-    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
     ListWorkerBlocksRequestRequestTypeDef,
     WorkerBlockTypeDef,
-    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListWorkersWithQualificationTypeRequestRequestTypeDef,
-    LocaleOutputTypeDef,
     LocaleTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersFailureStatusTypeDef,
     NotifyWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMapEntryOutputTypeDef,
     ParameterMapEntryTypeDef,
     RejectAssignmentRequestRequestTypeDef,
     RejectQualificationRequestRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     ReviewActionDetailTypeDef,
     ReviewResultDetailTypeDef,
     SendBonusRequestRequestTypeDef,
     UpdateExpirationForHITRequestRequestTypeDef,
     UpdateHITReviewStatusRequestRequestTypeDef,
     UpdateHITTypeOfHITRequestRequestTypeDef,
     UpdateQualificationTypeRequestRequestTypeDef,
+    CreateHITTypeResponseTypeDef,
+    GetAccountBalanceResponseTypeDef,
+    GetFileUploadURLResponseTypeDef,
     ListAssignmentsForHITResponseTypeDef,
     ListBonusPaymentsResponseTypeDef,
     CreateQualificationTypeResponseTypeDef,
     GetQualificationTypeResponseTypeDef,
     ListQualificationTypesResponseTypeDef,
     UpdateQualificationTypeResponseTypeDef,
+    ListAssignmentsForHITRequestListAssignmentsForHITPaginateTypeDef,
+    ListBonusPaymentsRequestListBonusPaymentsPaginateTypeDef,
+    ListHITsForQualificationTypeRequestListHITsForQualificationTypePaginateTypeDef,
+    ListHITsRequestListHITsPaginateTypeDef,
+    ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef,
+    ListQualificationTypesRequestListQualificationTypesPaginateTypeDef,
+    ListReviewableHITsRequestListReviewableHITsPaginateTypeDef,
+    ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef,
+    ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef,
     ListQualificationRequestsResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     QualificationRequirementOutputTypeDef,
-    QualificationTypeDef,
     QualificationRequirementTypeDef,
+    QualificationTypeDef,
     SendTestEventNotificationRequestRequestTypeDef,
     UpdateNotificationSettingsRequestRequestTypeDef,
     NotifyWorkersResponseTypeDef,
     PolicyParameterOutputTypeDef,
     PolicyParameterTypeDef,
     ReviewReportTypeDef,
     HITTypeDef,
+    CreateHITTypeRequestRequestTypeDef,
     GetQualificationScoreResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
-    CreateHITTypeRequestRequestTypeDef,
     ReviewPolicyOutputTypeDef,
     ReviewPolicyTypeDef,
     CreateHITResponseTypeDef,
     CreateHITWithHITTypeResponseTypeDef,
     GetAssignmentResponseTypeDef,
     GetHITResponseTypeDef,
     ListHITsForQualificationTypeResponseTypeDef,
```

### Comparing `mypy-boto3-mturk-1.28.12/mypy_boto3_mturk.egg-info/SOURCES.txt` & `mypy-boto3-mturk-1.28.15/mypy_boto3_mturk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mturk-1.28.12/setup.py` & `mypy-boto3-mturk-1.28.15/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mturk",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mturk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MTurk 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MTurk 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

