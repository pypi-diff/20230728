# Comparing `tmp/mypy-boto3-auditmanager-1.28.12.tar.gz` & `tmp/mypy-boto3-auditmanager-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-auditmanager-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
+gzip compressed data, was "mypy-boto3-auditmanager-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
```

## Comparing `mypy-boto3-auditmanager-1.28.12.tar` & `mypy-boto3-auditmanager-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18492 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43294 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43226 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60586 2023-07-27 05:17:46.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60541 2023-07-27 05:17:45.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:20.000000 mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.604572 mypy-boto3-auditmanager-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:17:44.000000 mypy-boto3-auditmanager-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.200695 mypy-boto3-auditmanager-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-28 20:42:19.200695 mypy-boto3-auditmanager-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18130 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.196694 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43294 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43226 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57940 2023-07-28 20:19:53.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57895 2023-07-28 20:19:53.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:51.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.200695 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:18.000000 mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.200695 mypy-boto3-auditmanager-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:19:50.000000 mypy-boto3-auditmanager-1.28.15/setup.py
```

### Comparing `mypy-boto3-auditmanager-1.28.12/LICENSE` & `mypy-boto3-auditmanager-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.12/PKG-INFO` & `mypy-boto3-auditmanager-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.28.12
-Summary: Type annotations for boto3.AuditManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,137 +321,127 @@
 ### Typed dictionaries
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
-    AWSAccountOutputTypeDef,
     AWSAccountTypeDef,
-    AWSServiceOutputTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
-    RoleOutputTypeDef,
+    RoleTypeDef,
     ControlCommentTypeDef,
     AssessmentEvidenceFolderTypeDef,
     AssessmentFrameworkMetadataTypeDef,
     AssessmentFrameworkShareRequestTypeDef,
     FrameworkMetadataTypeDef,
-    AssessmentReportsDestinationOutputTypeDef,
+    AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
-    AssessmentReportsDestinationTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
-    CreateDelegationRequestOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
-    ManualEvidenceOutputTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
-    SourceKeywordOutputTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
-    RoleTypeDef,
-    DefaultExportDestinationOutputTypeDef,
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
-    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
-    DeregistrationPolicyOutputTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFileUploadUrlRequestRequestTypeDef,
-    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
-    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
     ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
+    DeregisterAccountResponseTypeDef,
+    GetAccountStatusResponseTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    ListAssessmentFrameworksResponseTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ListAssessmentFrameworkShareRequestsResponseTypeDef,
+    ListAssessmentFrameworksResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterAccountResponseTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
     ControlInsightsMetadataByAssessmentItemTypeDef,
     ControlInsightsMetadataItemTypeDef,
-    ControlMappingSourceOutputTypeDef,
     ControlMappingSourceTypeDef,
     CreateControlMappingSourceTypeDef,
     ListControlsResponseTypeDef,
     CreateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     GetDelegationsResponseTypeDef,
     UpdateSettingsRequestRequestTypeDef,
@@ -497,15 +487,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountOutputTypeDef:
+def get_structure() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.12/README.md` & `mypy-boto3-auditmanager-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,137 +289,127 @@
 ### Typed dictionaries
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
-    AWSAccountOutputTypeDef,
     AWSAccountTypeDef,
-    AWSServiceOutputTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
-    RoleOutputTypeDef,
+    RoleTypeDef,
     ControlCommentTypeDef,
     AssessmentEvidenceFolderTypeDef,
     AssessmentFrameworkMetadataTypeDef,
     AssessmentFrameworkShareRequestTypeDef,
     FrameworkMetadataTypeDef,
-    AssessmentReportsDestinationOutputTypeDef,
+    AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
-    AssessmentReportsDestinationTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
-    CreateDelegationRequestOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
-    ManualEvidenceOutputTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
-    SourceKeywordOutputTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
-    RoleTypeDef,
-    DefaultExportDestinationOutputTypeDef,
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
-    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
-    DeregistrationPolicyOutputTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFileUploadUrlRequestRequestTypeDef,
-    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
-    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
     ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
+    DeregisterAccountResponseTypeDef,
+    GetAccountStatusResponseTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    ListAssessmentFrameworksResponseTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ListAssessmentFrameworkShareRequestsResponseTypeDef,
+    ListAssessmentFrameworksResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterAccountResponseTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
     ControlInsightsMetadataByAssessmentItemTypeDef,
     ControlInsightsMetadataItemTypeDef,
-    ControlMappingSourceOutputTypeDef,
     ControlMappingSourceTypeDef,
     CreateControlMappingSourceTypeDef,
     ListControlsResponseTypeDef,
     CreateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     GetDelegationsResponseTypeDef,
     UpdateSettingsRequestRequestTypeDef,
@@ -465,15 +455,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountOutputTypeDef:
+def get_structure() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/__main__.py` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AuditManager 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.AuditManager 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
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

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/client.py` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/client.pyi` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/literals.py` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/literals.pyi` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/type_defs.py` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for auditmanager service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_auditmanager.type_defs import AWSAccountOutputTypeDef
+    from mypy_boto3_auditmanager.type_defs import AWSAccountTypeDef
 
-    data: AWSAccountOutputTypeDef = {...}
+    data: AWSAccountTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -48,137 +48,127 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AWSAccountOutputTypeDef",
     "AWSAccountTypeDef",
-    "AWSServiceOutputTypeDef",
     "AWSServiceTypeDef",
     "DelegationTypeDef",
-    "RoleOutputTypeDef",
+    "RoleTypeDef",
     "ControlCommentTypeDef",
     "AssessmentEvidenceFolderTypeDef",
     "AssessmentFrameworkMetadataTypeDef",
     "AssessmentFrameworkShareRequestTypeDef",
     "FrameworkMetadataTypeDef",
-    "AssessmentReportsDestinationOutputTypeDef",
+    "AssessmentReportsDestinationTypeDef",
     "AssessmentReportEvidenceErrorTypeDef",
     "AssessmentReportMetadataTypeDef",
     "AssessmentReportTypeDef",
-    "AssessmentReportsDestinationTypeDef",
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef",
-    "CreateDelegationRequestOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDelegationRequestTypeDef",
     "BatchDeleteDelegationByAssessmentErrorTypeDef",
     "BatchDeleteDelegationByAssessmentRequestRequestTypeDef",
     "BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef",
-    "ManualEvidenceOutputTypeDef",
     "ManualEvidenceTypeDef",
     "ChangeLogTypeDef",
     "EvidenceInsightsTypeDef",
-    "SourceKeywordOutputTypeDef",
     "SourceKeywordTypeDef",
     "ControlMetadataTypeDef",
     "CreateAssessmentFrameworkControlTypeDef",
     "CreateAssessmentReportRequestRequestTypeDef",
-    "RoleTypeDef",
-    "DefaultExportDestinationOutputTypeDef",
     "DefaultExportDestinationTypeDef",
     "DelegationMetadataTypeDef",
     "DeleteAssessmentFrameworkRequestRequestTypeDef",
     "DeleteAssessmentFrameworkShareRequestRequestTypeDef",
     "DeleteAssessmentReportRequestRequestTypeDef",
     "DeleteAssessmentRequestRequestTypeDef",
     "DeleteControlRequestRequestTypeDef",
-    "DeregisterAccountResponseTypeDef",
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
-    "DeregistrationPolicyOutputTypeDef",
     "DeregistrationPolicyTypeDef",
     "DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "EvidenceFinderEnablementTypeDef",
     "ResourceTypeDef",
-    "GetAccountStatusResponseTypeDef",
     "GetAssessmentFrameworkRequestRequestTypeDef",
     "GetAssessmentReportUrlRequestRequestTypeDef",
     "URLTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetChangeLogsRequestRequestTypeDef",
     "GetControlRequestRequestTypeDef",
     "GetDelegationsRequestRequestTypeDef",
     "GetEvidenceByEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
-    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentRequestRequestTypeDef",
     "GetEvidenceRequestRequestTypeDef",
     "GetInsightsByAssessmentRequestRequestTypeDef",
     "InsightsByAssessmentTypeDef",
     "InsightsTypeDef",
-    "GetOrganizationAdminAccountResponseTypeDef",
     "ServiceMetadataTypeDef",
     "GetSettingsRequestRequestTypeDef",
     "ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef",
     "ListAssessmentFrameworkShareRequestsRequestRequestTypeDef",
     "ListAssessmentFrameworksRequestRequestTypeDef",
     "ListAssessmentReportsRequestRequestTypeDef",
     "ListAssessmentsRequestRequestTypeDef",
     "ListControlDomainInsightsByAssessmentRequestRequestTypeDef",
     "ListControlDomainInsightsRequestRequestTypeDef",
     "ListControlInsightsByControlDomainRequestRequestTypeDef",
     "ListControlsRequestRequestTypeDef",
     "ListKeywordsForDataSourceRequestRequestTypeDef",
-    "ListKeywordsForDataSourceResponseTypeDef",
     "ListNotificationsRequestRequestTypeDef",
     "NotificationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RegisterAccountRequestRequestTypeDef",
-    "RegisterAccountResponseTypeDef",
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
-    "RegisterOrganizationAdminAccountResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAssessmentFrameworkShareRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
     "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    "CreateAssessmentReportResponseTypeDef",
+    "DeregisterAccountResponseTypeDef",
+    "GetAccountStatusResponseTypeDef",
+    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderResponseTypeDef",
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
-    "ListAssessmentFrameworksResponseTypeDef",
+    "GetOrganizationAdminAccountResponseTypeDef",
     "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+    "ListAssessmentFrameworksResponseTypeDef",
+    "ListAssessmentReportsResponseTypeDef",
+    "ListKeywordsForDataSourceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterAccountResponseTypeDef",
+    "RegisterOrganizationAdminAccountResponseTypeDef",
     "StartAssessmentFrameworkShareResponseTypeDef",
     "UpdateAssessmentFrameworkShareResponseTypeDef",
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
-    "ListAssessmentReportsResponseTypeDef",
-    "CreateAssessmentReportResponseTypeDef",
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     "BatchCreateDelegationByAssessmentRequestRequestTypeDef",
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     "BatchImportEvidenceToAssessmentControlRequestRequestTypeDef",
     "GetChangeLogsResponseTypeDef",
     "ControlDomainInsightsTypeDef",
     "ControlInsightsMetadataByAssessmentItemTypeDef",
     "ControlInsightsMetadataItemTypeDef",
-    "ControlMappingSourceOutputTypeDef",
     "ControlMappingSourceTypeDef",
     "CreateControlMappingSourceTypeDef",
     "ListControlsResponseTypeDef",
     "CreateAssessmentFrameworkControlSetTypeDef",
     "UpdateAssessmentFrameworkControlSetTypeDef",
     "GetDelegationsResponseTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
@@ -223,42 +213,24 @@
     "UpdateAssessmentResponseTypeDef",
     "UpdateAssessmentStatusResponseTypeDef",
     "CreateAssessmentFrameworkResponseTypeDef",
     "GetAssessmentFrameworkResponseTypeDef",
     "UpdateAssessmentFrameworkResponseTypeDef",
 )
 
-AWSAccountOutputTypeDef = TypedDict(
-    "AWSAccountOutputTypeDef",
-    {
-        "id": str,
-        "emailAddress": str,
-        "name": str,
-    },
-    total=False,
-)
-
 AWSAccountTypeDef = TypedDict(
     "AWSAccountTypeDef",
     {
         "id": str,
         "emailAddress": str,
         "name": str,
     },
     total=False,
 )
 
-AWSServiceOutputTypeDef = TypedDict(
-    "AWSServiceOutputTypeDef",
-    {
-        "serviceName": str,
-    },
-    total=False,
-)
-
 AWSServiceTypeDef = TypedDict(
     "AWSServiceTypeDef",
     {
         "serviceName": str,
     },
     total=False,
 )
@@ -277,16 +249,16 @@
         "controlSetId": str,
         "comment": str,
         "createdBy": str,
     },
     total=False,
 )
 
-RoleOutputTypeDef = TypedDict(
-    "RoleOutputTypeDef",
+RoleTypeDef = TypedDict(
+    "RoleTypeDef",
     {
         "roleType": RoleTypeType,
         "roleArn": str,
     },
 )
 
 ControlCommentTypeDef = TypedDict(
@@ -371,16 +343,16 @@
         "description": str,
         "logo": str,
         "complianceType": str,
     },
     total=False,
 )
 
-AssessmentReportsDestinationOutputTypeDef = TypedDict(
-    "AssessmentReportsDestinationOutputTypeDef",
+AssessmentReportsDestinationTypeDef = TypedDict(
+    "AssessmentReportsDestinationTypeDef",
     {
         "destinationType": Literal["S3"],
         "destination": str,
     },
     total=False,
 )
 
@@ -421,23 +393,14 @@
         "author": str,
         "status": AssessmentReportStatusType,
         "creationTime": datetime,
     },
     total=False,
 )
 
-AssessmentReportsDestinationTypeDef = TypedDict(
-    "AssessmentReportsDestinationTypeDef",
-    {
-        "destinationType": Literal["S3"],
-        "destination": str,
-    },
-    total=False,
-)
-
 AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef = TypedDict(
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "evidenceFolderId": str,
     },
 )
@@ -447,23 +410,23 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
 )
 
-CreateDelegationRequestOutputTypeDef = TypedDict(
-    "CreateDelegationRequestOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "comment": str,
-        "controlSetId": str,
-        "roleArn": str,
-        "roleType": RoleTypeType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 CreateDelegationRequestTypeDef = TypedDict(
     "CreateDelegationRequestTypeDef",
     {
         "comment": str,
         "controlSetId": str,
@@ -496,24 +459,14 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
 )
 
-ManualEvidenceOutputTypeDef = TypedDict(
-    "ManualEvidenceOutputTypeDef",
-    {
-        "s3ResourcePath": str,
-        "textResponse": str,
-        "evidenceFileName": str,
-    },
-    total=False,
-)
-
 ManualEvidenceTypeDef = TypedDict(
     "ManualEvidenceTypeDef",
     {
         "s3ResourcePath": str,
         "textResponse": str,
         "evidenceFileName": str,
     },
@@ -538,23 +491,14 @@
         "noncompliantEvidenceCount": int,
         "compliantEvidenceCount": int,
         "inconclusiveEvidenceCount": int,
     },
     total=False,
 )
 
-SourceKeywordOutputTypeDef = TypedDict(
-    "SourceKeywordOutputTypeDef",
-    {
-        "keywordInputType": KeywordInputTypeType,
-        "keywordValue": str,
-    },
-    total=False,
-)
-
 SourceKeywordTypeDef = TypedDict(
     "SourceKeywordTypeDef",
     {
         "keywordInputType": KeywordInputTypeType,
         "keywordValue": str,
     },
     total=False,
@@ -600,31 +544,14 @@
 class CreateAssessmentReportRequestRequestTypeDef(
     _RequiredCreateAssessmentReportRequestRequestTypeDef,
     _OptionalCreateAssessmentReportRequestRequestTypeDef,
 ):
     pass
 
 
-RoleTypeDef = TypedDict(
-    "RoleTypeDef",
-    {
-        "roleType": RoleTypeType,
-        "roleArn": str,
-    },
-)
-
-DefaultExportDestinationOutputTypeDef = TypedDict(
-    "DefaultExportDestinationOutputTypeDef",
-    {
-        "destinationType": Literal["S3"],
-        "destination": str,
-    },
-    total=False,
-)
-
 DefaultExportDestinationTypeDef = TypedDict(
     "DefaultExportDestinationTypeDef",
     {
         "destinationType": Literal["S3"],
         "destination": str,
     },
     total=False,
@@ -677,38 +604,22 @@
 DeleteControlRequestRequestTypeDef = TypedDict(
     "DeleteControlRequestRequestTypeDef",
     {
         "controlId": str,
     },
 )
 
-DeregisterAccountResponseTypeDef = TypedDict(
-    "DeregisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
     total=False,
 )
 
-DeregistrationPolicyOutputTypeDef = TypedDict(
-    "DeregistrationPolicyOutputTypeDef",
-    {
-        "deleteResources": DeleteResourcesType,
-    },
-    total=False,
-)
-
 DeregistrationPolicyTypeDef = TypedDict(
     "DeregistrationPolicyTypeDef",
     {
         "deleteResources": DeleteResourcesType,
     },
     total=False,
 )
@@ -738,22 +649,14 @@
         "arn": str,
         "value": str,
         "complianceCheck": str,
     },
     total=False,
 )
 
-GetAccountStatusResponseTypeDef = TypedDict(
-    "GetAccountStatusResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "GetAssessmentFrameworkRequestRequestTypeDef",
     {
         "frameworkId": str,
     },
 )
 
@@ -849,23 +752,14 @@
 GetEvidenceFileUploadUrlRequestRequestTypeDef = TypedDict(
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
     {
         "fileName": str,
     },
 )
 
-GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
-    "GetEvidenceFileUploadUrlResponseTypeDef",
-    {
-        "evidenceFileName": str,
-        "uploadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEvidenceFolderRequestRequestTypeDef = TypedDict(
     "GetEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "evidenceFolderId": str,
     },
@@ -959,23 +853,14 @@
         "assessmentControlsCountByNoncompliantEvidence": int,
         "totalAssessmentControlsCount": int,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
-GetOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "GetOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "name": str,
         "displayName": str,
         "description": str,
         "category": str,
@@ -1175,23 +1060,14 @@
 class ListKeywordsForDataSourceRequestRequestTypeDef(
     _RequiredListKeywordsForDataSourceRequestRequestTypeDef,
     _OptionalListKeywordsForDataSourceRequestRequestTypeDef,
 ):
     pass
 
 
-ListKeywordsForDataSourceResponseTypeDef = TypedDict(
-    "ListKeywordsForDataSourceResponseTypeDef",
-    {
-        "keywords": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListNotificationsRequestRequestTypeDef = TypedDict(
     "ListNotificationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1215,66 +1091,30 @@
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
 RegisterAccountRequestRequestTypeDef = TypedDict(
     "RegisterAccountRequestRequestTypeDef",
     {
         "kmsKey": str,
         "delegatedAdminAccount": str,
     },
     total=False,
 )
 
-RegisterAccountResponseTypeDef = TypedDict(
-    "RegisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
 )
 
-RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "RegisterOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
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
 _RequiredStartAssessmentFrameworkShareRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentFrameworkShareRequestRequestTypeDef",
     {
         "frameworkId": str,
         "destinationAccount": str,
         "destinationRegion": str,
     },
@@ -1366,31 +1206,19 @@
 ValidateAssessmentReportIntegrityRequestRequestTypeDef = TypedDict(
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     {
         "s3RelativePath": str,
     },
 )
 
-ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
-    {
-        "signatureValid": bool,
-        "signatureAlgorithm": str,
-        "signatureDateTime": str,
-        "signatureKeyId": str,
-        "validationErrors": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScopeOutputTypeDef = TypedDict(
     "ScopeOutputTypeDef",
     {
-        "awsAccounts": List[AWSAccountOutputTypeDef],
-        "awsServices": List[AWSServiceOutputTypeDef],
+        "awsAccounts": List[AWSAccountTypeDef],
+        "awsServices": List[AWSServiceTypeDef],
     },
     total=False,
 )
 
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
@@ -1403,15 +1231,15 @@
 AssessmentMetadataItemTypeDef = TypedDict(
     "AssessmentMetadataItemTypeDef",
     {
         "name": str,
         "id": str,
         "complianceType": str,
         "status": AssessmentStatusType,
-        "roles": List[RoleOutputTypeDef],
+        "roles": List[RoleTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
@@ -1427,113 +1255,193 @@
         "evidenceSources": List[str],
         "evidenceCount": int,
         "assessmentReportEvidenceCount": int,
     },
     total=False,
 )
 
+BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    {
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    {
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssessmentReportResponseTypeDef = TypedDict(
+    "CreateAssessmentReportResponseTypeDef",
+    {
+        "assessmentReport": AssessmentReportTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterAccountResponseTypeDef = TypedDict(
+    "DeregisterAccountResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountStatusResponseTypeDef = TypedDict(
+    "GetAccountStatusResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
+    "GetEvidenceFileUploadUrlResponseTypeDef",
+    {
+        "evidenceFileName": str,
+        "uploadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceFolderResponseTypeDef",
     {
         "evidenceFolder": AssessmentEvidenceFolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceFoldersByAssessmentControlResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceFoldersByAssessmentResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "GetOrganizationAdminAccountResponseTypeDef",
+    {
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
+    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+    {
+        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentFrameworksResponseTypeDef = TypedDict(
     "ListAssessmentFrameworksResponseTypeDef",
     {
         "frameworkMetadataList": List[AssessmentFrameworkMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
-    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+ListAssessmentReportsResponseTypeDef = TypedDict(
+    "ListAssessmentReportsResponseTypeDef",
     {
-        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
+        "assessmentReports": List[AssessmentReportMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "StartAssessmentFrameworkShareResponseTypeDef",
+ListKeywordsForDataSourceResponseTypeDef = TypedDict(
+    "ListKeywordsForDataSourceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "keywords": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "UpdateAssessmentFrameworkShareResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+RegisterAccountResponseTypeDef = TypedDict(
+    "RegisterAccountResponseTypeDef",
     {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "RegisterOrganizationAdminAccountResponseTypeDef",
     {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAssessmentReportsResponseTypeDef = TypedDict(
-    "ListAssessmentReportsResponseTypeDef",
+StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "StartAssessmentFrameworkShareResponseTypeDef",
     {
-        "assessmentReports": List[AssessmentReportMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssessmentReportResponseTypeDef = TypedDict(
-    "CreateAssessmentReportResponseTypeDef",
+UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "UpdateAssessmentFrameworkShareResponseTypeDef",
     {
-        "assessmentReport": AssessmentReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    {
+        "signatureValid": bool,
+        "signatureAlgorithm": str,
+        "signatureDateTime": str,
+        "signatureKeyId": str,
+        "validationErrors": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateDelegationByAssessmentErrorTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     {
-        "createDelegationRequest": CreateDelegationRequestOutputTypeDef,
+        "createDelegationRequest": CreateDelegationRequestTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 BatchCreateDelegationByAssessmentRequestRequestTypeDef = TypedDict(
@@ -1544,22 +1452,22 @@
     },
 )
 
 BatchDeleteDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     {
         "errors": List[BatchDeleteDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportEvidenceToAssessmentControlErrorTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     {
-        "manualEvidence": ManualEvidenceOutputTypeDef,
+        "manualEvidence": ManualEvidenceTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 BatchImportEvidenceToAssessmentControlRequestRequestTypeDef = TypedDict(
@@ -1573,15 +1481,15 @@
 )
 
 GetChangeLogsResponseTypeDef = TypedDict(
     "GetChangeLogsResponseTypeDef",
     {
         "changeLogs": List[ChangeLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlDomainInsightsTypeDef = TypedDict(
     "ControlDomainInsightsTypeDef",
     {
         "name": str,
@@ -1613,29 +1521,14 @@
         "id": str,
         "evidenceInsights": EvidenceInsightsTypeDef,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
-ControlMappingSourceOutputTypeDef = TypedDict(
-    "ControlMappingSourceOutputTypeDef",
-    {
-        "sourceId": str,
-        "sourceName": str,
-        "sourceDescription": str,
-        "sourceSetUpOption": SourceSetUpOptionType,
-        "sourceType": SourceTypeType,
-        "sourceKeyword": SourceKeywordOutputTypeDef,
-        "sourceFrequency": SourceFrequencyType,
-        "troubleshootingText": str,
-    },
-    total=False,
-)
-
 ControlMappingSourceTypeDef = TypedDict(
     "ControlMappingSourceTypeDef",
     {
         "sourceId": str,
         "sourceName": str,
         "sourceDescription": str,
         "sourceSetUpOption": SourceSetUpOptionType,
@@ -1662,15 +1555,15 @@
 )
 
 ListControlsResponseTypeDef = TypedDict(
     "ListControlsResponseTypeDef",
     {
         "controlMetadataList": List[ControlMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAssessmentFrameworkControlSetTypeDef = TypedDict(
     "_RequiredCreateAssessmentFrameworkControlSetTypeDef",
     {
         "name": str,
@@ -1716,15 +1609,15 @@
 
 
 GetDelegationsResponseTypeDef = TypedDict(
     "GetDelegationsResponseTypeDef",
     {
         "delegations": List[DelegationMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "snsTopic": str,
@@ -1739,20 +1632,20 @@
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "isAwsOrgEnabled": bool,
         "snsTopic": str,
-        "defaultAssessmentReportsDestination": AssessmentReportsDestinationOutputTypeDef,
-        "defaultProcessOwners": List[RoleOutputTypeDef],
+        "defaultAssessmentReportsDestination": AssessmentReportsDestinationTypeDef,
+        "defaultProcessOwners": List[RoleTypeDef],
         "kmsKey": str,
         "evidenceFinderEnablement": EvidenceFinderEnablementTypeDef,
-        "deregistrationPolicy": DeregistrationPolicyOutputTypeDef,
-        "defaultExportDestination": DefaultExportDestinationOutputTypeDef,
+        "deregistrationPolicy": DeregistrationPolicyTypeDef,
+        "defaultExportDestination": DefaultExportDestinationTypeDef,
     },
     total=False,
 )
 
 EvidenceTypeDef = TypedDict(
     "EvidenceTypeDef",
     {
@@ -1775,62 +1668,62 @@
     total=False,
 )
 
 GetAssessmentReportUrlResponseTypeDef = TypedDict(
     "GetAssessmentReportUrlResponseTypeDef",
     {
         "preSignedUrl": URLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightsByAssessmentResponseTypeDef = TypedDict(
     "GetInsightsByAssessmentResponseTypeDef",
     {
         "insights": InsightsByAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "insights": InsightsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServicesInScopeResponseTypeDef = TypedDict(
     "GetServicesInScopeResponseTypeDef",
     {
         "serviceMetadata": List[ServiceMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationsResponseTypeDef = TypedDict(
     "ListNotificationsResponseTypeDef",
     {
         "notifications": List[NotificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentMetadataTypeDef = TypedDict(
     "AssessmentMetadataTypeDef",
     {
         "name": str,
         "id": str,
         "description": str,
         "complianceType": str,
         "status": AssessmentStatusType,
-        "assessmentReportsDestination": AssessmentReportsDestinationOutputTypeDef,
+        "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
         "scope": ScopeOutputTypeDef,
-        "roles": List[RoleOutputTypeDef],
+        "roles": List[RoleTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
@@ -1886,91 +1779,91 @@
 
 
 ListAssessmentsResponseTypeDef = TypedDict(
     "ListAssessmentsResponseTypeDef",
     {
         "assessmentMetadata": List[AssessmentMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentControlSetTypeDef = TypedDict(
     "AssessmentControlSetTypeDef",
     {
         "id": str,
         "description": str,
         "status": ControlSetStatusType,
-        "roles": List[RoleOutputTypeDef],
+        "roles": List[RoleTypeDef],
         "controls": List[AssessmentControlTypeDef],
         "delegations": List[DelegationTypeDef],
         "systemEvidenceCount": int,
         "manualEvidenceCount": int,
     },
     total=False,
 )
 
 UpdateAssessmentControlResponseTypeDef = TypedDict(
     "UpdateAssessmentControlResponseTypeDef",
     {
         "control": AssessmentControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     {
         "delegations": List[DelegationTypeDef],
         "errors": List[BatchCreateDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportEvidenceToAssessmentControlResponseTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     {
         "errors": List[BatchImportEvidenceToAssessmentControlErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlDomainInsightsByAssessmentResponseTypeDef = TypedDict(
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlDomainInsightsResponseTypeDef = TypedDict(
     "ListControlDomainInsightsResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListAssessmentControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsByAssessment": List[ControlInsightsMetadataByAssessmentItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsMetadata": List[ControlInsightsMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlTypeDef = TypedDict(
     "ControlTypeDef",
     {
         "arn": str,
@@ -1978,15 +1871,15 @@
         "type": ControlTypeType,
         "name": str,
         "description": str,
         "testingInformation": str,
         "actionPlanTitle": str,
         "actionPlanInstructions": str,
         "controlSources": str,
-        "controlMappingSources": List[ControlMappingSourceOutputTypeDef],
+        "controlMappingSources": List[ControlMappingSourceTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "createdBy": str,
         "lastUpdatedBy": str,
         "tags": Dict[str, str],
     },
     total=False,
@@ -2094,40 +1987,40 @@
     pass
 
 
 GetSettingsResponseTypeDef = TypedDict(
     "GetSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSettingsResponseTypeDef = TypedDict(
     "UpdateSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceByEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceByEvidenceFolderResponseTypeDef",
     {
         "evidence": List[EvidenceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceResponseTypeDef = TypedDict(
     "GetEvidenceResponseTypeDef",
     {
         "evidence": EvidenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentFrameworkTypeDef = TypedDict(
     "AssessmentFrameworkTypeDef",
     {
         "id": str,
@@ -2138,15 +2031,15 @@
     total=False,
 )
 
 UpdateAssessmentControlSetStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentControlSetStatusResponseTypeDef",
     {
         "controlSet": AssessmentControlSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlSetTypeDef = TypedDict(
     "ControlSetTypeDef",
     {
         "id": str,
@@ -2156,39 +2049,39 @@
     total=False,
 )
 
 CreateControlResponseTypeDef = TypedDict(
     "CreateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetControlResponseTypeDef = TypedDict(
     "GetControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateControlResponseTypeDef = TypedDict(
     "UpdateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentTypeDef = TypedDict(
     "AssessmentTypeDef",
     {
         "arn": str,
-        "awsAccount": AWSAccountOutputTypeDef,
+        "awsAccount": AWSAccountTypeDef,
         "metadata": AssessmentMetadataTypeDef,
         "framework": AssessmentFrameworkTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
@@ -2213,59 +2106,59 @@
     total=False,
 )
 
 CreateAssessmentResponseTypeDef = TypedDict(
     "CreateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "userRole": RoleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "userRole": RoleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentResponseTypeDef = TypedDict(
     "UpdateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentStatusResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssessmentFrameworkResponseTypeDef = TypedDict(
     "CreateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssessmentFrameworkResponseTypeDef = TypedDict(
     "GetAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentFrameworkResponseTypeDef = TypedDict(
     "UpdateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager/type_defs.pyi` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for auditmanager service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_auditmanager.type_defs import AWSAccountOutputTypeDef
+    from mypy_boto3_auditmanager.type_defs import AWSAccountTypeDef
 
-    data: AWSAccountOutputTypeDef = {...}
+    data: AWSAccountTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -47,137 +47,127 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AWSAccountOutputTypeDef",
     "AWSAccountTypeDef",
-    "AWSServiceOutputTypeDef",
     "AWSServiceTypeDef",
     "DelegationTypeDef",
-    "RoleOutputTypeDef",
+    "RoleTypeDef",
     "ControlCommentTypeDef",
     "AssessmentEvidenceFolderTypeDef",
     "AssessmentFrameworkMetadataTypeDef",
     "AssessmentFrameworkShareRequestTypeDef",
     "FrameworkMetadataTypeDef",
-    "AssessmentReportsDestinationOutputTypeDef",
+    "AssessmentReportsDestinationTypeDef",
     "AssessmentReportEvidenceErrorTypeDef",
     "AssessmentReportMetadataTypeDef",
     "AssessmentReportTypeDef",
-    "AssessmentReportsDestinationTypeDef",
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef",
-    "CreateDelegationRequestOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDelegationRequestTypeDef",
     "BatchDeleteDelegationByAssessmentErrorTypeDef",
     "BatchDeleteDelegationByAssessmentRequestRequestTypeDef",
     "BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef",
-    "ManualEvidenceOutputTypeDef",
     "ManualEvidenceTypeDef",
     "ChangeLogTypeDef",
     "EvidenceInsightsTypeDef",
-    "SourceKeywordOutputTypeDef",
     "SourceKeywordTypeDef",
     "ControlMetadataTypeDef",
     "CreateAssessmentFrameworkControlTypeDef",
     "CreateAssessmentReportRequestRequestTypeDef",
-    "RoleTypeDef",
-    "DefaultExportDestinationOutputTypeDef",
     "DefaultExportDestinationTypeDef",
     "DelegationMetadataTypeDef",
     "DeleteAssessmentFrameworkRequestRequestTypeDef",
     "DeleteAssessmentFrameworkShareRequestRequestTypeDef",
     "DeleteAssessmentReportRequestRequestTypeDef",
     "DeleteAssessmentRequestRequestTypeDef",
     "DeleteControlRequestRequestTypeDef",
-    "DeregisterAccountResponseTypeDef",
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
-    "DeregistrationPolicyOutputTypeDef",
     "DeregistrationPolicyTypeDef",
     "DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     "EvidenceFinderEnablementTypeDef",
     "ResourceTypeDef",
-    "GetAccountStatusResponseTypeDef",
     "GetAssessmentFrameworkRequestRequestTypeDef",
     "GetAssessmentReportUrlRequestRequestTypeDef",
     "URLTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetChangeLogsRequestRequestTypeDef",
     "GetControlRequestRequestTypeDef",
     "GetDelegationsRequestRequestTypeDef",
     "GetEvidenceByEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
-    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef",
     "GetEvidenceFoldersByAssessmentRequestRequestTypeDef",
     "GetEvidenceRequestRequestTypeDef",
     "GetInsightsByAssessmentRequestRequestTypeDef",
     "InsightsByAssessmentTypeDef",
     "InsightsTypeDef",
-    "GetOrganizationAdminAccountResponseTypeDef",
     "ServiceMetadataTypeDef",
     "GetSettingsRequestRequestTypeDef",
     "ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef",
     "ListAssessmentFrameworkShareRequestsRequestRequestTypeDef",
     "ListAssessmentFrameworksRequestRequestTypeDef",
     "ListAssessmentReportsRequestRequestTypeDef",
     "ListAssessmentsRequestRequestTypeDef",
     "ListControlDomainInsightsByAssessmentRequestRequestTypeDef",
     "ListControlDomainInsightsRequestRequestTypeDef",
     "ListControlInsightsByControlDomainRequestRequestTypeDef",
     "ListControlsRequestRequestTypeDef",
     "ListKeywordsForDataSourceRequestRequestTypeDef",
-    "ListKeywordsForDataSourceResponseTypeDef",
     "ListNotificationsRequestRequestTypeDef",
     "NotificationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RegisterAccountRequestRequestTypeDef",
-    "RegisterAccountResponseTypeDef",
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
-    "RegisterOrganizationAdminAccountResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAssessmentFrameworkShareRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
     "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    "CreateAssessmentReportResponseTypeDef",
+    "DeregisterAccountResponseTypeDef",
+    "GetAccountStatusResponseTypeDef",
+    "GetEvidenceFileUploadUrlResponseTypeDef",
     "GetEvidenceFolderResponseTypeDef",
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
-    "ListAssessmentFrameworksResponseTypeDef",
+    "GetOrganizationAdminAccountResponseTypeDef",
     "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+    "ListAssessmentFrameworksResponseTypeDef",
+    "ListAssessmentReportsResponseTypeDef",
+    "ListKeywordsForDataSourceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterAccountResponseTypeDef",
+    "RegisterOrganizationAdminAccountResponseTypeDef",
     "StartAssessmentFrameworkShareResponseTypeDef",
     "UpdateAssessmentFrameworkShareResponseTypeDef",
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
-    "ListAssessmentReportsResponseTypeDef",
-    "CreateAssessmentReportResponseTypeDef",
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     "BatchCreateDelegationByAssessmentRequestRequestTypeDef",
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     "BatchImportEvidenceToAssessmentControlRequestRequestTypeDef",
     "GetChangeLogsResponseTypeDef",
     "ControlDomainInsightsTypeDef",
     "ControlInsightsMetadataByAssessmentItemTypeDef",
     "ControlInsightsMetadataItemTypeDef",
-    "ControlMappingSourceOutputTypeDef",
     "ControlMappingSourceTypeDef",
     "CreateControlMappingSourceTypeDef",
     "ListControlsResponseTypeDef",
     "CreateAssessmentFrameworkControlSetTypeDef",
     "UpdateAssessmentFrameworkControlSetTypeDef",
     "GetDelegationsResponseTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
@@ -222,42 +212,24 @@
     "UpdateAssessmentResponseTypeDef",
     "UpdateAssessmentStatusResponseTypeDef",
     "CreateAssessmentFrameworkResponseTypeDef",
     "GetAssessmentFrameworkResponseTypeDef",
     "UpdateAssessmentFrameworkResponseTypeDef",
 )
 
-AWSAccountOutputTypeDef = TypedDict(
-    "AWSAccountOutputTypeDef",
-    {
-        "id": str,
-        "emailAddress": str,
-        "name": str,
-    },
-    total=False,
-)
-
 AWSAccountTypeDef = TypedDict(
     "AWSAccountTypeDef",
     {
         "id": str,
         "emailAddress": str,
         "name": str,
     },
     total=False,
 )
 
-AWSServiceOutputTypeDef = TypedDict(
-    "AWSServiceOutputTypeDef",
-    {
-        "serviceName": str,
-    },
-    total=False,
-)
-
 AWSServiceTypeDef = TypedDict(
     "AWSServiceTypeDef",
     {
         "serviceName": str,
     },
     total=False,
 )
@@ -276,16 +248,16 @@
         "controlSetId": str,
         "comment": str,
         "createdBy": str,
     },
     total=False,
 )
 
-RoleOutputTypeDef = TypedDict(
-    "RoleOutputTypeDef",
+RoleTypeDef = TypedDict(
+    "RoleTypeDef",
     {
         "roleType": RoleTypeType,
         "roleArn": str,
     },
 )
 
 ControlCommentTypeDef = TypedDict(
@@ -370,16 +342,16 @@
         "description": str,
         "logo": str,
         "complianceType": str,
     },
     total=False,
 )
 
-AssessmentReportsDestinationOutputTypeDef = TypedDict(
-    "AssessmentReportsDestinationOutputTypeDef",
+AssessmentReportsDestinationTypeDef = TypedDict(
+    "AssessmentReportsDestinationTypeDef",
     {
         "destinationType": Literal["S3"],
         "destination": str,
     },
     total=False,
 )
 
@@ -420,23 +392,14 @@
         "author": str,
         "status": AssessmentReportStatusType,
         "creationTime": datetime,
     },
     total=False,
 )
 
-AssessmentReportsDestinationTypeDef = TypedDict(
-    "AssessmentReportsDestinationTypeDef",
-    {
-        "destinationType": Literal["S3"],
-        "destination": str,
-    },
-    total=False,
-)
-
 AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef = TypedDict(
     "AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "evidenceFolderId": str,
     },
 )
@@ -446,23 +409,23 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
 )
 
-CreateDelegationRequestOutputTypeDef = TypedDict(
-    "CreateDelegationRequestOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "comment": str,
-        "controlSetId": str,
-        "roleArn": str,
-        "roleType": RoleTypeType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
 CreateDelegationRequestTypeDef = TypedDict(
     "CreateDelegationRequestTypeDef",
     {
         "comment": str,
         "controlSetId": str,
@@ -495,24 +458,14 @@
     {
         "assessmentId": str,
         "evidenceFolderId": str,
         "evidenceIds": Sequence[str],
     },
 )
 
-ManualEvidenceOutputTypeDef = TypedDict(
-    "ManualEvidenceOutputTypeDef",
-    {
-        "s3ResourcePath": str,
-        "textResponse": str,
-        "evidenceFileName": str,
-    },
-    total=False,
-)
-
 ManualEvidenceTypeDef = TypedDict(
     "ManualEvidenceTypeDef",
     {
         "s3ResourcePath": str,
         "textResponse": str,
         "evidenceFileName": str,
     },
@@ -537,23 +490,14 @@
         "noncompliantEvidenceCount": int,
         "compliantEvidenceCount": int,
         "inconclusiveEvidenceCount": int,
     },
     total=False,
 )
 
-SourceKeywordOutputTypeDef = TypedDict(
-    "SourceKeywordOutputTypeDef",
-    {
-        "keywordInputType": KeywordInputTypeType,
-        "keywordValue": str,
-    },
-    total=False,
-)
-
 SourceKeywordTypeDef = TypedDict(
     "SourceKeywordTypeDef",
     {
         "keywordInputType": KeywordInputTypeType,
         "keywordValue": str,
     },
     total=False,
@@ -597,31 +541,14 @@
 
 class CreateAssessmentReportRequestRequestTypeDef(
     _RequiredCreateAssessmentReportRequestRequestTypeDef,
     _OptionalCreateAssessmentReportRequestRequestTypeDef,
 ):
     pass
 
-RoleTypeDef = TypedDict(
-    "RoleTypeDef",
-    {
-        "roleType": RoleTypeType,
-        "roleArn": str,
-    },
-)
-
-DefaultExportDestinationOutputTypeDef = TypedDict(
-    "DefaultExportDestinationOutputTypeDef",
-    {
-        "destinationType": Literal["S3"],
-        "destination": str,
-    },
-    total=False,
-)
-
 DefaultExportDestinationTypeDef = TypedDict(
     "DefaultExportDestinationTypeDef",
     {
         "destinationType": Literal["S3"],
         "destination": str,
     },
     total=False,
@@ -674,38 +601,22 @@
 DeleteControlRequestRequestTypeDef = TypedDict(
     "DeleteControlRequestRequestTypeDef",
     {
         "controlId": str,
     },
 )
 
-DeregisterAccountResponseTypeDef = TypedDict(
-    "DeregisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "DeregisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
     total=False,
 )
 
-DeregistrationPolicyOutputTypeDef = TypedDict(
-    "DeregistrationPolicyOutputTypeDef",
-    {
-        "deleteResources": DeleteResourcesType,
-    },
-    total=False,
-)
-
 DeregistrationPolicyTypeDef = TypedDict(
     "DeregistrationPolicyTypeDef",
     {
         "deleteResources": DeleteResourcesType,
     },
     total=False,
 )
@@ -735,22 +646,14 @@
         "arn": str,
         "value": str,
         "complianceCheck": str,
     },
     total=False,
 )
 
-GetAccountStatusResponseTypeDef = TypedDict(
-    "GetAccountStatusResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAssessmentFrameworkRequestRequestTypeDef = TypedDict(
     "GetAssessmentFrameworkRequestRequestTypeDef",
     {
         "frameworkId": str,
     },
 )
 
@@ -842,23 +745,14 @@
 GetEvidenceFileUploadUrlRequestRequestTypeDef = TypedDict(
     "GetEvidenceFileUploadUrlRequestRequestTypeDef",
     {
         "fileName": str,
     },
 )
 
-GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
-    "GetEvidenceFileUploadUrlResponseTypeDef",
-    {
-        "evidenceFileName": str,
-        "uploadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEvidenceFolderRequestRequestTypeDef = TypedDict(
     "GetEvidenceFolderRequestRequestTypeDef",
     {
         "assessmentId": str,
         "controlSetId": str,
         "evidenceFolderId": str,
     },
@@ -948,23 +842,14 @@
         "assessmentControlsCountByNoncompliantEvidence": int,
         "totalAssessmentControlsCount": int,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
-GetOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "GetOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "name": str,
         "displayName": str,
         "description": str,
         "category": str,
@@ -1150,23 +1035,14 @@
 
 class ListKeywordsForDataSourceRequestRequestTypeDef(
     _RequiredListKeywordsForDataSourceRequestRequestTypeDef,
     _OptionalListKeywordsForDataSourceRequestRequestTypeDef,
 ):
     pass
 
-ListKeywordsForDataSourceResponseTypeDef = TypedDict(
-    "ListKeywordsForDataSourceResponseTypeDef",
-    {
-        "keywords": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListNotificationsRequestRequestTypeDef = TypedDict(
     "ListNotificationsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1190,66 +1066,30 @@
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
 RegisterAccountRequestRequestTypeDef = TypedDict(
     "RegisterAccountRequestRequestTypeDef",
     {
         "kmsKey": str,
         "delegatedAdminAccount": str,
     },
     total=False,
 )
 
-RegisterAccountResponseTypeDef = TypedDict(
-    "RegisterAccountResponseTypeDef",
-    {
-        "status": AccountStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterOrganizationAdminAccountRequestRequestTypeDef = TypedDict(
     "RegisterOrganizationAdminAccountRequestRequestTypeDef",
     {
         "adminAccountId": str,
     },
 )
 
-RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
-    "RegisterOrganizationAdminAccountResponseTypeDef",
-    {
-        "adminAccountId": str,
-        "organizationId": str,
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
 _RequiredStartAssessmentFrameworkShareRequestRequestTypeDef = TypedDict(
     "_RequiredStartAssessmentFrameworkShareRequestRequestTypeDef",
     {
         "frameworkId": str,
         "destinationAccount": str,
         "destinationRegion": str,
     },
@@ -1337,31 +1177,19 @@
 ValidateAssessmentReportIntegrityRequestRequestTypeDef = TypedDict(
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     {
         "s3RelativePath": str,
     },
 )
 
-ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
-    "ValidateAssessmentReportIntegrityResponseTypeDef",
-    {
-        "signatureValid": bool,
-        "signatureAlgorithm": str,
-        "signatureDateTime": str,
-        "signatureKeyId": str,
-        "validationErrors": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ScopeOutputTypeDef = TypedDict(
     "ScopeOutputTypeDef",
     {
-        "awsAccounts": List[AWSAccountOutputTypeDef],
-        "awsServices": List[AWSServiceOutputTypeDef],
+        "awsAccounts": List[AWSAccountTypeDef],
+        "awsServices": List[AWSServiceTypeDef],
     },
     total=False,
 )
 
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
@@ -1374,15 +1202,15 @@
 AssessmentMetadataItemTypeDef = TypedDict(
     "AssessmentMetadataItemTypeDef",
     {
         "name": str,
         "id": str,
         "complianceType": str,
         "status": AssessmentStatusType,
-        "roles": List[RoleOutputTypeDef],
+        "roles": List[RoleTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
@@ -1398,113 +1226,193 @@
         "evidenceSources": List[str],
         "evidenceCount": int,
         "assessmentReportEvidenceCount": int,
     },
     total=False,
 )
 
+BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+    {
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
+    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+    {
+        "evidenceIds": List[str],
+        "errors": List[AssessmentReportEvidenceErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAssessmentReportResponseTypeDef = TypedDict(
+    "CreateAssessmentReportResponseTypeDef",
+    {
+        "assessmentReport": AssessmentReportTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterAccountResponseTypeDef = TypedDict(
+    "DeregisterAccountResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountStatusResponseTypeDef = TypedDict(
+    "GetAccountStatusResponseTypeDef",
+    {
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEvidenceFileUploadUrlResponseTypeDef = TypedDict(
+    "GetEvidenceFileUploadUrlResponseTypeDef",
+    {
+        "evidenceFileName": str,
+        "uploadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceFolderResponseTypeDef",
     {
         "evidenceFolder": AssessmentEvidenceFolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceFoldersByAssessmentControlResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentControlResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceFoldersByAssessmentResponseTypeDef = TypedDict(
     "GetEvidenceFoldersByAssessmentResponseTypeDef",
     {
         "evidenceFolders": List[AssessmentEvidenceFolderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "GetOrganizationAdminAccountResponseTypeDef",
+    {
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
+    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+    {
+        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentFrameworksResponseTypeDef = TypedDict(
     "ListAssessmentFrameworksResponseTypeDef",
     {
         "frameworkMetadataList": List[AssessmentFrameworkMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAssessmentFrameworkShareRequestsResponseTypeDef = TypedDict(
-    "ListAssessmentFrameworkShareRequestsResponseTypeDef",
+ListAssessmentReportsResponseTypeDef = TypedDict(
+    "ListAssessmentReportsResponseTypeDef",
     {
-        "assessmentFrameworkShareRequests": List[AssessmentFrameworkShareRequestTypeDef],
+        "assessmentReports": List[AssessmentReportMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "StartAssessmentFrameworkShareResponseTypeDef",
+ListKeywordsForDataSourceResponseTypeDef = TypedDict(
+    "ListKeywordsForDataSourceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "keywords": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
-    "UpdateAssessmentFrameworkShareResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchAssociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
+RegisterAccountResponseTypeDef = TypedDict(
+    "RegisterAccountResponseTypeDef",
     {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": AccountStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDisassociateAssessmentReportEvidenceResponseTypeDef = TypedDict(
-    "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
+RegisterOrganizationAdminAccountResponseTypeDef = TypedDict(
+    "RegisterOrganizationAdminAccountResponseTypeDef",
     {
-        "evidenceIds": List[str],
-        "errors": List[AssessmentReportEvidenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "adminAccountId": str,
+        "organizationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAssessmentReportsResponseTypeDef = TypedDict(
-    "ListAssessmentReportsResponseTypeDef",
+StartAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "StartAssessmentFrameworkShareResponseTypeDef",
     {
-        "assessmentReports": List[AssessmentReportMetadataTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateAssessmentReportResponseTypeDef = TypedDict(
-    "CreateAssessmentReportResponseTypeDef",
+UpdateAssessmentFrameworkShareResponseTypeDef = TypedDict(
+    "UpdateAssessmentFrameworkShareResponseTypeDef",
     {
-        "assessmentReport": AssessmentReportTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "assessmentFrameworkShareRequest": AssessmentFrameworkShareRequestTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ValidateAssessmentReportIntegrityResponseTypeDef = TypedDict(
+    "ValidateAssessmentReportIntegrityResponseTypeDef",
+    {
+        "signatureValid": bool,
+        "signatureAlgorithm": str,
+        "signatureDateTime": str,
+        "signatureKeyId": str,
+        "validationErrors": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateDelegationByAssessmentErrorTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentErrorTypeDef",
     {
-        "createDelegationRequest": CreateDelegationRequestOutputTypeDef,
+        "createDelegationRequest": CreateDelegationRequestTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 BatchCreateDelegationByAssessmentRequestRequestTypeDef = TypedDict(
@@ -1515,22 +1423,22 @@
     },
 )
 
 BatchDeleteDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchDeleteDelegationByAssessmentResponseTypeDef",
     {
         "errors": List[BatchDeleteDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportEvidenceToAssessmentControlErrorTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlErrorTypeDef",
     {
-        "manualEvidence": ManualEvidenceOutputTypeDef,
+        "manualEvidence": ManualEvidenceTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
 BatchImportEvidenceToAssessmentControlRequestRequestTypeDef = TypedDict(
@@ -1544,15 +1452,15 @@
 )
 
 GetChangeLogsResponseTypeDef = TypedDict(
     "GetChangeLogsResponseTypeDef",
     {
         "changeLogs": List[ChangeLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlDomainInsightsTypeDef = TypedDict(
     "ControlDomainInsightsTypeDef",
     {
         "name": str,
@@ -1584,29 +1492,14 @@
         "id": str,
         "evidenceInsights": EvidenceInsightsTypeDef,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
-ControlMappingSourceOutputTypeDef = TypedDict(
-    "ControlMappingSourceOutputTypeDef",
-    {
-        "sourceId": str,
-        "sourceName": str,
-        "sourceDescription": str,
-        "sourceSetUpOption": SourceSetUpOptionType,
-        "sourceType": SourceTypeType,
-        "sourceKeyword": SourceKeywordOutputTypeDef,
-        "sourceFrequency": SourceFrequencyType,
-        "troubleshootingText": str,
-    },
-    total=False,
-)
-
 ControlMappingSourceTypeDef = TypedDict(
     "ControlMappingSourceTypeDef",
     {
         "sourceId": str,
         "sourceName": str,
         "sourceDescription": str,
         "sourceSetUpOption": SourceSetUpOptionType,
@@ -1633,15 +1526,15 @@
 )
 
 ListControlsResponseTypeDef = TypedDict(
     "ListControlsResponseTypeDef",
     {
         "controlMetadataList": List[ControlMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAssessmentFrameworkControlSetTypeDef = TypedDict(
     "_RequiredCreateAssessmentFrameworkControlSetTypeDef",
     {
         "name": str,
@@ -1683,15 +1576,15 @@
     pass
 
 GetDelegationsResponseTypeDef = TypedDict(
     "GetDelegationsResponseTypeDef",
     {
         "delegations": List[DelegationMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSettingsRequestRequestTypeDef = TypedDict(
     "UpdateSettingsRequestRequestTypeDef",
     {
         "snsTopic": str,
@@ -1706,20 +1599,20 @@
 )
 
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "isAwsOrgEnabled": bool,
         "snsTopic": str,
-        "defaultAssessmentReportsDestination": AssessmentReportsDestinationOutputTypeDef,
-        "defaultProcessOwners": List[RoleOutputTypeDef],
+        "defaultAssessmentReportsDestination": AssessmentReportsDestinationTypeDef,
+        "defaultProcessOwners": List[RoleTypeDef],
         "kmsKey": str,
         "evidenceFinderEnablement": EvidenceFinderEnablementTypeDef,
-        "deregistrationPolicy": DeregistrationPolicyOutputTypeDef,
-        "defaultExportDestination": DefaultExportDestinationOutputTypeDef,
+        "deregistrationPolicy": DeregistrationPolicyTypeDef,
+        "defaultExportDestination": DefaultExportDestinationTypeDef,
     },
     total=False,
 )
 
 EvidenceTypeDef = TypedDict(
     "EvidenceTypeDef",
     {
@@ -1742,62 +1635,62 @@
     total=False,
 )
 
 GetAssessmentReportUrlResponseTypeDef = TypedDict(
     "GetAssessmentReportUrlResponseTypeDef",
     {
         "preSignedUrl": URLTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightsByAssessmentResponseTypeDef = TypedDict(
     "GetInsightsByAssessmentResponseTypeDef",
     {
         "insights": InsightsByAssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "insights": InsightsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServicesInScopeResponseTypeDef = TypedDict(
     "GetServicesInScopeResponseTypeDef",
     {
         "serviceMetadata": List[ServiceMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationsResponseTypeDef = TypedDict(
     "ListNotificationsResponseTypeDef",
     {
         "notifications": List[NotificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentMetadataTypeDef = TypedDict(
     "AssessmentMetadataTypeDef",
     {
         "name": str,
         "id": str,
         "description": str,
         "complianceType": str,
         "status": AssessmentStatusType,
-        "assessmentReportsDestination": AssessmentReportsDestinationOutputTypeDef,
+        "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
         "scope": ScopeOutputTypeDef,
-        "roles": List[RoleOutputTypeDef],
+        "roles": List[RoleTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
 
@@ -1849,91 +1742,91 @@
     pass
 
 ListAssessmentsResponseTypeDef = TypedDict(
     "ListAssessmentsResponseTypeDef",
     {
         "assessmentMetadata": List[AssessmentMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentControlSetTypeDef = TypedDict(
     "AssessmentControlSetTypeDef",
     {
         "id": str,
         "description": str,
         "status": ControlSetStatusType,
-        "roles": List[RoleOutputTypeDef],
+        "roles": List[RoleTypeDef],
         "controls": List[AssessmentControlTypeDef],
         "delegations": List[DelegationTypeDef],
         "systemEvidenceCount": int,
         "manualEvidenceCount": int,
     },
     total=False,
 )
 
 UpdateAssessmentControlResponseTypeDef = TypedDict(
     "UpdateAssessmentControlResponseTypeDef",
     {
         "control": AssessmentControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateDelegationByAssessmentResponseTypeDef = TypedDict(
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     {
         "delegations": List[DelegationTypeDef],
         "errors": List[BatchCreateDelegationByAssessmentErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchImportEvidenceToAssessmentControlResponseTypeDef = TypedDict(
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     {
         "errors": List[BatchImportEvidenceToAssessmentControlErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlDomainInsightsByAssessmentResponseTypeDef = TypedDict(
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlDomainInsightsResponseTypeDef = TypedDict(
     "ListControlDomainInsightsResponseTypeDef",
     {
         "controlDomainInsights": List[ControlDomainInsightsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAssessmentControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListAssessmentControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsByAssessment": List[ControlInsightsMetadataByAssessmentItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListControlInsightsByControlDomainResponseTypeDef = TypedDict(
     "ListControlInsightsByControlDomainResponseTypeDef",
     {
         "controlInsightsMetadata": List[ControlInsightsMetadataItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlTypeDef = TypedDict(
     "ControlTypeDef",
     {
         "arn": str,
@@ -1941,15 +1834,15 @@
         "type": ControlTypeType,
         "name": str,
         "description": str,
         "testingInformation": str,
         "actionPlanTitle": str,
         "actionPlanInstructions": str,
         "controlSources": str,
-        "controlMappingSources": List[ControlMappingSourceOutputTypeDef],
+        "controlMappingSources": List[ControlMappingSourceTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "createdBy": str,
         "lastUpdatedBy": str,
         "tags": Dict[str, str],
     },
     total=False,
@@ -2049,40 +1942,40 @@
 ):
     pass
 
 GetSettingsResponseTypeDef = TypedDict(
     "GetSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSettingsResponseTypeDef = TypedDict(
     "UpdateSettingsResponseTypeDef",
     {
         "settings": SettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceByEvidenceFolderResponseTypeDef = TypedDict(
     "GetEvidenceByEvidenceFolderResponseTypeDef",
     {
         "evidence": List[EvidenceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEvidenceResponseTypeDef = TypedDict(
     "GetEvidenceResponseTypeDef",
     {
         "evidence": EvidenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentFrameworkTypeDef = TypedDict(
     "AssessmentFrameworkTypeDef",
     {
         "id": str,
@@ -2093,15 +1986,15 @@
     total=False,
 )
 
 UpdateAssessmentControlSetStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentControlSetStatusResponseTypeDef",
     {
         "controlSet": AssessmentControlSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ControlSetTypeDef = TypedDict(
     "ControlSetTypeDef",
     {
         "id": str,
@@ -2111,39 +2004,39 @@
     total=False,
 )
 
 CreateControlResponseTypeDef = TypedDict(
     "CreateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetControlResponseTypeDef = TypedDict(
     "GetControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateControlResponseTypeDef = TypedDict(
     "UpdateControlResponseTypeDef",
     {
         "control": ControlTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssessmentTypeDef = TypedDict(
     "AssessmentTypeDef",
     {
         "arn": str,
-        "awsAccount": AWSAccountOutputTypeDef,
+        "awsAccount": AWSAccountTypeDef,
         "metadata": AssessmentMetadataTypeDef,
         "framework": AssessmentFrameworkTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
@@ -2168,59 +2061,59 @@
     total=False,
 )
 
 CreateAssessmentResponseTypeDef = TypedDict(
     "CreateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssessmentResponseTypeDef = TypedDict(
     "GetAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "userRole": RoleOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "userRole": RoleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentResponseTypeDef = TypedDict(
     "UpdateAssessmentResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentStatusResponseTypeDef = TypedDict(
     "UpdateAssessmentStatusResponseTypeDef",
     {
         "assessment": AssessmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAssessmentFrameworkResponseTypeDef = TypedDict(
     "CreateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAssessmentFrameworkResponseTypeDef = TypedDict(
     "GetAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAssessmentFrameworkResponseTypeDef = TypedDict(
     "UpdateAssessmentFrameworkResponseTypeDef",
     {
         "framework": FrameworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/PKG-INFO` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-auditmanager
-Version: 1.28.12
-Summary: Type annotations for boto3.AuditManager 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-auditmanager.svg?color=blue)](https://pypi.org/project/mypy-boto3-auditmanager)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-auditmanager)](https://pepy.tech/project/mypy-boto3-auditmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AuditManager 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
+[boto3.AuditManager 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager)
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
 [mypy-boto3-auditmanager docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_auditmanager/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,137 +321,127 @@
 ### Typed dictionaries
 
 `mypy_boto3_auditmanager.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_auditmanager.type_defs import (
-    AWSAccountOutputTypeDef,
     AWSAccountTypeDef,
-    AWSServiceOutputTypeDef,
     AWSServiceTypeDef,
     DelegationTypeDef,
-    RoleOutputTypeDef,
+    RoleTypeDef,
     ControlCommentTypeDef,
     AssessmentEvidenceFolderTypeDef,
     AssessmentFrameworkMetadataTypeDef,
     AssessmentFrameworkShareRequestTypeDef,
     FrameworkMetadataTypeDef,
-    AssessmentReportsDestinationOutputTypeDef,
+    AssessmentReportsDestinationTypeDef,
     AssessmentReportEvidenceErrorTypeDef,
     AssessmentReportMetadataTypeDef,
     AssessmentReportTypeDef,
-    AssessmentReportsDestinationTypeDef,
     AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef,
-    CreateDelegationRequestOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateDelegationRequestTypeDef,
     BatchDeleteDelegationByAssessmentErrorTypeDef,
     BatchDeleteDelegationByAssessmentRequestRequestTypeDef,
     BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef,
-    ManualEvidenceOutputTypeDef,
     ManualEvidenceTypeDef,
     ChangeLogTypeDef,
     EvidenceInsightsTypeDef,
-    SourceKeywordOutputTypeDef,
     SourceKeywordTypeDef,
     ControlMetadataTypeDef,
     CreateAssessmentFrameworkControlTypeDef,
     CreateAssessmentReportRequestRequestTypeDef,
-    RoleTypeDef,
-    DefaultExportDestinationOutputTypeDef,
     DefaultExportDestinationTypeDef,
     DelegationMetadataTypeDef,
     DeleteAssessmentFrameworkRequestRequestTypeDef,
     DeleteAssessmentFrameworkShareRequestRequestTypeDef,
     DeleteAssessmentReportRequestRequestTypeDef,
     DeleteAssessmentRequestRequestTypeDef,
     DeleteControlRequestRequestTypeDef,
-    DeregisterAccountResponseTypeDef,
     DeregisterOrganizationAdminAccountRequestRequestTypeDef,
-    DeregistrationPolicyOutputTypeDef,
     DeregistrationPolicyTypeDef,
     DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef,
     EvidenceFinderEnablementTypeDef,
     ResourceTypeDef,
-    GetAccountStatusResponseTypeDef,
     GetAssessmentFrameworkRequestRequestTypeDef,
     GetAssessmentReportUrlRequestRequestTypeDef,
     URLTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetChangeLogsRequestRequestTypeDef,
     GetControlRequestRequestTypeDef,
     GetDelegationsRequestRequestTypeDef,
     GetEvidenceByEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFileUploadUrlRequestRequestTypeDef,
-    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef,
     GetEvidenceFoldersByAssessmentRequestRequestTypeDef,
     GetEvidenceRequestRequestTypeDef,
     GetInsightsByAssessmentRequestRequestTypeDef,
     InsightsByAssessmentTypeDef,
     InsightsTypeDef,
-    GetOrganizationAdminAccountResponseTypeDef,
     ServiceMetadataTypeDef,
     GetSettingsRequestRequestTypeDef,
     ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef,
     ListAssessmentFrameworkShareRequestsRequestRequestTypeDef,
     ListAssessmentFrameworksRequestRequestTypeDef,
     ListAssessmentReportsRequestRequestTypeDef,
     ListAssessmentsRequestRequestTypeDef,
     ListControlDomainInsightsByAssessmentRequestRequestTypeDef,
     ListControlDomainInsightsRequestRequestTypeDef,
     ListControlInsightsByControlDomainRequestRequestTypeDef,
     ListControlsRequestRequestTypeDef,
     ListKeywordsForDataSourceRequestRequestTypeDef,
-    ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsRequestRequestTypeDef,
     NotificationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RegisterAccountRequestRequestTypeDef,
-    RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountRequestRequestTypeDef,
-    RegisterOrganizationAdminAccountResponseTypeDef,
-    ResponseMetadataTypeDef,
     StartAssessmentFrameworkShareRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAssessmentControlRequestRequestTypeDef,
     UpdateAssessmentControlSetStatusRequestRequestTypeDef,
     UpdateAssessmentFrameworkShareRequestRequestTypeDef,
     UpdateAssessmentStatusRequestRequestTypeDef,
     ValidateAssessmentReportIntegrityRequestRequestTypeDef,
-    ValidateAssessmentReportIntegrityResponseTypeDef,
     ScopeOutputTypeDef,
     ScopeTypeDef,
     AssessmentMetadataItemTypeDef,
     AssessmentControlTypeDef,
+    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
+    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
+    CreateAssessmentReportResponseTypeDef,
+    DeregisterAccountResponseTypeDef,
+    GetAccountStatusResponseTypeDef,
+    GetEvidenceFileUploadUrlResponseTypeDef,
     GetEvidenceFolderResponseTypeDef,
     GetEvidenceFoldersByAssessmentControlResponseTypeDef,
     GetEvidenceFoldersByAssessmentResponseTypeDef,
-    ListAssessmentFrameworksResponseTypeDef,
+    GetOrganizationAdminAccountResponseTypeDef,
     ListAssessmentFrameworkShareRequestsResponseTypeDef,
+    ListAssessmentFrameworksResponseTypeDef,
+    ListAssessmentReportsResponseTypeDef,
+    ListKeywordsForDataSourceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterAccountResponseTypeDef,
+    RegisterOrganizationAdminAccountResponseTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
-    BatchAssociateAssessmentReportEvidenceResponseTypeDef,
-    BatchDisassociateAssessmentReportEvidenceResponseTypeDef,
-    ListAssessmentReportsResponseTypeDef,
-    CreateAssessmentReportResponseTypeDef,
+    ValidateAssessmentReportIntegrityResponseTypeDef,
     BatchCreateDelegationByAssessmentErrorTypeDef,
     BatchCreateDelegationByAssessmentRequestRequestTypeDef,
     BatchDeleteDelegationByAssessmentResponseTypeDef,
     BatchImportEvidenceToAssessmentControlErrorTypeDef,
     BatchImportEvidenceToAssessmentControlRequestRequestTypeDef,
     GetChangeLogsResponseTypeDef,
     ControlDomainInsightsTypeDef,
     ControlInsightsMetadataByAssessmentItemTypeDef,
     ControlInsightsMetadataItemTypeDef,
-    ControlMappingSourceOutputTypeDef,
     ControlMappingSourceTypeDef,
     CreateControlMappingSourceTypeDef,
     ListControlsResponseTypeDef,
     CreateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     GetDelegationsResponseTypeDef,
     UpdateSettingsRequestRequestTypeDef,
@@ -497,15 +487,15 @@
     UpdateAssessmentStatusResponseTypeDef,
     CreateAssessmentFrameworkResponseTypeDef,
     GetAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
 )
 
 
-def get_structure() -> AWSAccountOutputTypeDef:
+def get_structure() -> AWSAccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-auditmanager-1.28.12/mypy_boto3_auditmanager.egg-info/SOURCES.txt` & `mypy-boto3-auditmanager-1.28.15/mypy_boto3_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-auditmanager-1.28.12/setup.py` & `mypy-boto3-auditmanager-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-auditmanager",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AuditManager 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AuditManager 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

