# Comparing `tmp/mypy-boto3-accessanalyzer-1.28.12.tar.gz` & `tmp/mypy-boto3-accessanalyzer-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-accessanalyzer-1.28.12.tar", last modified: Thu Jul 27 05:34:13 2023, max compression
+gzip compressed data, was "mypy-boto3-accessanalyzer-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
```

## Comparing `mypy-boto3-accessanalyzer-1.28.12.tar` & `mypy-boto3-accessanalyzer-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.852594 mypy-boto3-accessanalyzer-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-07-27 05:34:13.832594 mypy-boto3-accessanalyzer-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18281 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.832594 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49396 2023-07-27 05:16:52.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49315 2023-07-27 05:16:51.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:13.832594 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:13.000000 mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:13.852594 mypy-boto3-accessanalyzer-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:16:50.000000 mypy-boto3-accessanalyzer-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24748 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24705 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-07-28 20:18:36.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12124 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47242 2023-07-28 20:18:37.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47161 2023-07-28 20:18:36.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19372 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:12.000000 mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.660609 mypy-boto3-accessanalyzer-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:18:35.000000 mypy-boto3-accessanalyzer-1.28.15/setup.py
```

### Comparing `mypy-boto3-accessanalyzer-1.28.12/LICENSE` & `mypy-boto3-accessanalyzer-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/PKG-INFO` & `mypy-boto3-accessanalyzer-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.28.12
-Summary: Type annotations for boto3.AccessAnalyzer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,38 +371,31 @@
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
-    AclGranteeOutputTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
     CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
     EbsSnapshotConfigurationOutputTypeDef,
-    EcrRepositoryConfigurationOutputTypeDef,
-    EfsFileSystemConfigurationOutputTypeDef,
-    IamRoleConfigurationOutputTypeDef,
-    SecretsManagerSecretConfigurationOutputTypeDef,
-    SnsTopicConfigurationOutputTypeDef,
-    SqsQueueConfigurationOutputTypeDef,
-    EbsSnapshotConfigurationTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
     SnsTopicConfigurationTypeDef,
     SqsQueueConfigurationTypeDef,
+    EbsSnapshotConfigurationTypeDef,
     ResponseMetadataTypeDef,
     CriterionTypeDef,
     DeleteAnalyzerRequestRequestTypeDef,
     DeleteArchiveRuleRequestRequestTypeDef,
     FindingSourceDetailTypeDef,
     GeneratedPolicyTypeDef,
     GetAccessPreviewRequestRequestTypeDef,
@@ -419,32 +412,29 @@
     ListAnalyzedResourcesRequestRequestTypeDef,
     ListAnalyzersRequestRequestTypeDef,
     ListArchiveRulesRequestRequestTypeDef,
     SortCriteriaTypeDef,
     ListPolicyGenerationsRequestRequestTypeDef,
     PolicyGenerationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     SubstringTypeDef,
     PolicyGenerationDetailsTypeDef,
     PositionTypeDef,
     RdsDbClusterSnapshotAttributeValueOutputTypeDef,
     RdsDbClusterSnapshotAttributeValueTypeDef,
     RdsDbSnapshotAttributeValueOutputTypeDef,
     RdsDbSnapshotAttributeValueTypeDef,
-    S3PublicAccessBlockConfigurationOutputTypeDef,
     S3PublicAccessBlockConfigurationTypeDef,
     StartResourceScanRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     ValidatePolicyRequestRequestTypeDef,
     AccessPreviewSummaryTypeDef,
-    S3BucketAclGrantConfigurationOutputTypeDef,
     S3BucketAclGrantConfigurationTypeDef,
     AnalyzerSummaryTypeDef,
     ArchiveRuleSummaryTypeDef,
     CloudTrailDetailsTypeDef,
     CloudTrailPropertiesTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
```

### Comparing `mypy-boto3-accessanalyzer-1.28.12/README.md` & `mypy-boto3-accessanalyzer-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,38 +339,31 @@
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
-    AclGranteeOutputTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
     CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
     EbsSnapshotConfigurationOutputTypeDef,
-    EcrRepositoryConfigurationOutputTypeDef,
-    EfsFileSystemConfigurationOutputTypeDef,
-    IamRoleConfigurationOutputTypeDef,
-    SecretsManagerSecretConfigurationOutputTypeDef,
-    SnsTopicConfigurationOutputTypeDef,
-    SqsQueueConfigurationOutputTypeDef,
-    EbsSnapshotConfigurationTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
     SnsTopicConfigurationTypeDef,
     SqsQueueConfigurationTypeDef,
+    EbsSnapshotConfigurationTypeDef,
     ResponseMetadataTypeDef,
     CriterionTypeDef,
     DeleteAnalyzerRequestRequestTypeDef,
     DeleteArchiveRuleRequestRequestTypeDef,
     FindingSourceDetailTypeDef,
     GeneratedPolicyTypeDef,
     GetAccessPreviewRequestRequestTypeDef,
@@ -387,32 +380,29 @@
     ListAnalyzedResourcesRequestRequestTypeDef,
     ListAnalyzersRequestRequestTypeDef,
     ListArchiveRulesRequestRequestTypeDef,
     SortCriteriaTypeDef,
     ListPolicyGenerationsRequestRequestTypeDef,
     PolicyGenerationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     SubstringTypeDef,
     PolicyGenerationDetailsTypeDef,
     PositionTypeDef,
     RdsDbClusterSnapshotAttributeValueOutputTypeDef,
     RdsDbClusterSnapshotAttributeValueTypeDef,
     RdsDbSnapshotAttributeValueOutputTypeDef,
     RdsDbSnapshotAttributeValueTypeDef,
-    S3PublicAccessBlockConfigurationOutputTypeDef,
     S3PublicAccessBlockConfigurationTypeDef,
     StartResourceScanRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     ValidatePolicyRequestRequestTypeDef,
     AccessPreviewSummaryTypeDef,
-    S3BucketAclGrantConfigurationOutputTypeDef,
     S3BucketAclGrantConfigurationTypeDef,
     AnalyzerSummaryTypeDef,
     ArchiveRuleSummaryTypeDef,
     CloudTrailDetailsTypeDef,
     CloudTrailPropertiesTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
```

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__init__.py` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__init__.pyi` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/__main__.py` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AccessAnalyzer 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.AccessAnalyzer 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer\nOther"
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

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/client.py` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/client.pyi` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/literals.py` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/literals.pyi` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/paginator.py` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/paginator.pyi` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/type_defs.py` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,38 +41,31 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessPreviewStatusReasonTypeDef",
-    "AclGranteeOutputTypeDef",
     "AclGranteeTypeDef",
     "AnalyzedResourceSummaryTypeDef",
     "AnalyzedResourceTypeDef",
     "StatusReasonTypeDef",
     "ApplyArchiveRuleRequestRequestTypeDef",
     "CriterionOutputTypeDef",
     "CancelPolicyGenerationRequestRequestTypeDef",
     "TrailTypeDef",
     "TrailPropertiesTypeDef",
     "EbsSnapshotConfigurationOutputTypeDef",
-    "EcrRepositoryConfigurationOutputTypeDef",
-    "EfsFileSystemConfigurationOutputTypeDef",
-    "IamRoleConfigurationOutputTypeDef",
-    "SecretsManagerSecretConfigurationOutputTypeDef",
-    "SnsTopicConfigurationOutputTypeDef",
-    "SqsQueueConfigurationOutputTypeDef",
-    "EbsSnapshotConfigurationTypeDef",
     "EcrRepositoryConfigurationTypeDef",
     "EfsFileSystemConfigurationTypeDef",
     "IamRoleConfigurationTypeDef",
     "SecretsManagerSecretConfigurationTypeDef",
     "SnsTopicConfigurationTypeDef",
     "SqsQueueConfigurationTypeDef",
+    "EbsSnapshotConfigurationTypeDef",
     "ResponseMetadataTypeDef",
     "CriterionTypeDef",
     "DeleteAnalyzerRequestRequestTypeDef",
     "DeleteArchiveRuleRequestRequestTypeDef",
     "FindingSourceDetailTypeDef",
     "GeneratedPolicyTypeDef",
     "GetAccessPreviewRequestRequestTypeDef",
@@ -89,32 +82,29 @@
     "ListAnalyzedResourcesRequestRequestTypeDef",
     "ListAnalyzersRequestRequestTypeDef",
     "ListArchiveRulesRequestRequestTypeDef",
     "SortCriteriaTypeDef",
     "ListPolicyGenerationsRequestRequestTypeDef",
     "PolicyGenerationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
     "SubstringTypeDef",
     "PolicyGenerationDetailsTypeDef",
     "PositionTypeDef",
     "RdsDbClusterSnapshotAttributeValueOutputTypeDef",
     "RdsDbClusterSnapshotAttributeValueTypeDef",
     "RdsDbSnapshotAttributeValueOutputTypeDef",
     "RdsDbSnapshotAttributeValueTypeDef",
-    "S3PublicAccessBlockConfigurationOutputTypeDef",
     "S3PublicAccessBlockConfigurationTypeDef",
     "StartResourceScanRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "ValidatePolicyRequestRequestTypeDef",
     "AccessPreviewSummaryTypeDef",
-    "S3BucketAclGrantConfigurationOutputTypeDef",
     "S3BucketAclGrantConfigurationTypeDef",
     "AnalyzerSummaryTypeDef",
     "ArchiveRuleSummaryTypeDef",
     "CloudTrailDetailsTypeDef",
     "CloudTrailPropertiesTypeDef",
     "CreateAccessPreviewResponseTypeDef",
     "CreateAnalyzerResponseTypeDef",
@@ -184,23 +174,14 @@
 AccessPreviewStatusReasonTypeDef = TypedDict(
     "AccessPreviewStatusReasonTypeDef",
     {
         "code": AccessPreviewStatusReasonCodeType,
     },
 )
 
-AclGranteeOutputTypeDef = TypedDict(
-    "AclGranteeOutputTypeDef",
-    {
-        "id": str,
-        "uri": str,
-    },
-    total=False,
-)
-
 AclGranteeTypeDef = TypedDict(
     "AclGranteeTypeDef",
     {
         "id": str,
         "uri": str,
     },
     total=False,
@@ -336,73 +317,14 @@
         "userIds": List[str],
         "groups": List[str],
         "kmsKeyId": str,
     },
     total=False,
 )
 
-EcrRepositoryConfigurationOutputTypeDef = TypedDict(
-    "EcrRepositoryConfigurationOutputTypeDef",
-    {
-        "repositoryPolicy": str,
-    },
-    total=False,
-)
-
-EfsFileSystemConfigurationOutputTypeDef = TypedDict(
-    "EfsFileSystemConfigurationOutputTypeDef",
-    {
-        "fileSystemPolicy": str,
-    },
-    total=False,
-)
-
-IamRoleConfigurationOutputTypeDef = TypedDict(
-    "IamRoleConfigurationOutputTypeDef",
-    {
-        "trustPolicy": str,
-    },
-    total=False,
-)
-
-SecretsManagerSecretConfigurationOutputTypeDef = TypedDict(
-    "SecretsManagerSecretConfigurationOutputTypeDef",
-    {
-        "kmsKeyId": str,
-        "secretPolicy": str,
-    },
-    total=False,
-)
-
-SnsTopicConfigurationOutputTypeDef = TypedDict(
-    "SnsTopicConfigurationOutputTypeDef",
-    {
-        "topicPolicy": str,
-    },
-    total=False,
-)
-
-SqsQueueConfigurationOutputTypeDef = TypedDict(
-    "SqsQueueConfigurationOutputTypeDef",
-    {
-        "queuePolicy": str,
-    },
-    total=False,
-)
-
-EbsSnapshotConfigurationTypeDef = TypedDict(
-    "EbsSnapshotConfigurationTypeDef",
-    {
-        "userIds": Sequence[str],
-        "groups": Sequence[str],
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
 EcrRepositoryConfigurationTypeDef = TypedDict(
     "EcrRepositoryConfigurationTypeDef",
     {
         "repositoryPolicy": str,
     },
     total=False,
 )
@@ -444,14 +366,24 @@
     "SqsQueueConfigurationTypeDef",
     {
         "queuePolicy": str,
     },
     total=False,
 )
 
+EbsSnapshotConfigurationTypeDef = TypedDict(
+    "EbsSnapshotConfigurationTypeDef",
+    {
+        "userIds": Sequence[str],
+        "groups": Sequence[str],
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -750,21 +682,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "vpcId": str,
-    },
-)
-
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "vpcId": str,
     },
 )
 
@@ -820,22 +745,14 @@
     "RdsDbSnapshotAttributeValueTypeDef",
     {
         "accountIds": Sequence[str],
     },
     total=False,
 )
 
-S3PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
-    "S3PublicAccessBlockConfigurationOutputTypeDef",
-    {
-        "ignorePublicAcls": bool,
-        "restrictPublicBuckets": bool,
-    },
-)
-
 S3PublicAccessBlockConfigurationTypeDef = TypedDict(
     "S3PublicAccessBlockConfigurationTypeDef",
     {
         "ignorePublicAcls": bool,
         "restrictPublicBuckets": bool,
     },
 )
@@ -947,22 +864,14 @@
 
 class AccessPreviewSummaryTypeDef(
     _RequiredAccessPreviewSummaryTypeDef, _OptionalAccessPreviewSummaryTypeDef
 ):
     pass
 
 
-S3BucketAclGrantConfigurationOutputTypeDef = TypedDict(
-    "S3BucketAclGrantConfigurationOutputTypeDef",
-    {
-        "permission": AclPermissionType,
-        "grantee": AclGranteeOutputTypeDef,
-    },
-)
-
 S3BucketAclGrantConfigurationTypeDef = TypedDict(
     "S3BucketAclGrantConfigurationTypeDef",
     {
         "permission": AclPermissionType,
         "grantee": AclGranteeTypeDef,
     },
 )
@@ -1449,15 +1358,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkOriginConfigurationOutputTypeDef = TypedDict(
     "NetworkOriginConfigurationOutputTypeDef",
     {
-        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "vpcConfiguration": VpcConfigurationTypeDef,
         "internetConfiguration": Dict[str, Any],
     },
     total=False,
 )
 
 NetworkOriginConfigurationTypeDef = TypedDict(
     "NetworkOriginConfigurationTypeDef",
@@ -1749,15 +1658,15 @@
     total=False,
 )
 
 S3AccessPointConfigurationOutputTypeDef = TypedDict(
     "S3AccessPointConfigurationOutputTypeDef",
     {
         "accessPointPolicy": str,
-        "publicAccessBlock": S3PublicAccessBlockConfigurationOutputTypeDef,
+        "publicAccessBlock": S3PublicAccessBlockConfigurationTypeDef,
         "networkOrigin": NetworkOriginConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 S3AccessPointConfigurationTypeDef = TypedDict(
     "S3AccessPointConfigurationTypeDef",
@@ -1824,16 +1733,16 @@
     },
 )
 
 S3BucketConfigurationOutputTypeDef = TypedDict(
     "S3BucketConfigurationOutputTypeDef",
     {
         "bucketPolicy": str,
-        "bucketAclGrants": List[S3BucketAclGrantConfigurationOutputTypeDef],
-        "bucketPublicAccessBlock": S3PublicAccessBlockConfigurationOutputTypeDef,
+        "bucketAclGrants": List[S3BucketAclGrantConfigurationTypeDef],
+        "bucketPublicAccessBlock": S3PublicAccessBlockConfigurationTypeDef,
         "accessPoints": Dict[str, S3AccessPointConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 S3BucketConfigurationTypeDef = TypedDict(
     "S3BucketConfigurationTypeDef",
@@ -1866,24 +1775,24 @@
     },
 )
 
 ConfigurationOutputTypeDef = TypedDict(
     "ConfigurationOutputTypeDef",
     {
         "ebsSnapshot": EbsSnapshotConfigurationOutputTypeDef,
-        "ecrRepository": EcrRepositoryConfigurationOutputTypeDef,
-        "iamRole": IamRoleConfigurationOutputTypeDef,
-        "efsFileSystem": EfsFileSystemConfigurationOutputTypeDef,
+        "ecrRepository": EcrRepositoryConfigurationTypeDef,
+        "iamRole": IamRoleConfigurationTypeDef,
+        "efsFileSystem": EfsFileSystemConfigurationTypeDef,
         "kmsKey": KmsKeyConfigurationOutputTypeDef,
         "rdsDbClusterSnapshot": RdsDbClusterSnapshotConfigurationOutputTypeDef,
         "rdsDbSnapshot": RdsDbSnapshotConfigurationOutputTypeDef,
-        "secretsManagerSecret": SecretsManagerSecretConfigurationOutputTypeDef,
+        "secretsManagerSecret": SecretsManagerSecretConfigurationTypeDef,
         "s3Bucket": S3BucketConfigurationOutputTypeDef,
-        "snsTopic": SnsTopicConfigurationOutputTypeDef,
-        "sqsQueue": SqsQueueConfigurationOutputTypeDef,
+        "snsTopic": SnsTopicConfigurationTypeDef,
+        "sqsQueue": SqsQueueConfigurationTypeDef,
     },
     total=False,
 )
 
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
```

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer/type_defs.pyi` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -40,38 +40,31 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessPreviewStatusReasonTypeDef",
-    "AclGranteeOutputTypeDef",
     "AclGranteeTypeDef",
     "AnalyzedResourceSummaryTypeDef",
     "AnalyzedResourceTypeDef",
     "StatusReasonTypeDef",
     "ApplyArchiveRuleRequestRequestTypeDef",
     "CriterionOutputTypeDef",
     "CancelPolicyGenerationRequestRequestTypeDef",
     "TrailTypeDef",
     "TrailPropertiesTypeDef",
     "EbsSnapshotConfigurationOutputTypeDef",
-    "EcrRepositoryConfigurationOutputTypeDef",
-    "EfsFileSystemConfigurationOutputTypeDef",
-    "IamRoleConfigurationOutputTypeDef",
-    "SecretsManagerSecretConfigurationOutputTypeDef",
-    "SnsTopicConfigurationOutputTypeDef",
-    "SqsQueueConfigurationOutputTypeDef",
-    "EbsSnapshotConfigurationTypeDef",
     "EcrRepositoryConfigurationTypeDef",
     "EfsFileSystemConfigurationTypeDef",
     "IamRoleConfigurationTypeDef",
     "SecretsManagerSecretConfigurationTypeDef",
     "SnsTopicConfigurationTypeDef",
     "SqsQueueConfigurationTypeDef",
+    "EbsSnapshotConfigurationTypeDef",
     "ResponseMetadataTypeDef",
     "CriterionTypeDef",
     "DeleteAnalyzerRequestRequestTypeDef",
     "DeleteArchiveRuleRequestRequestTypeDef",
     "FindingSourceDetailTypeDef",
     "GeneratedPolicyTypeDef",
     "GetAccessPreviewRequestRequestTypeDef",
@@ -88,32 +81,29 @@
     "ListAnalyzedResourcesRequestRequestTypeDef",
     "ListAnalyzersRequestRequestTypeDef",
     "ListArchiveRulesRequestRequestTypeDef",
     "SortCriteriaTypeDef",
     "ListPolicyGenerationsRequestRequestTypeDef",
     "PolicyGenerationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
     "SubstringTypeDef",
     "PolicyGenerationDetailsTypeDef",
     "PositionTypeDef",
     "RdsDbClusterSnapshotAttributeValueOutputTypeDef",
     "RdsDbClusterSnapshotAttributeValueTypeDef",
     "RdsDbSnapshotAttributeValueOutputTypeDef",
     "RdsDbSnapshotAttributeValueTypeDef",
-    "S3PublicAccessBlockConfigurationOutputTypeDef",
     "S3PublicAccessBlockConfigurationTypeDef",
     "StartResourceScanRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "ValidatePolicyRequestRequestTypeDef",
     "AccessPreviewSummaryTypeDef",
-    "S3BucketAclGrantConfigurationOutputTypeDef",
     "S3BucketAclGrantConfigurationTypeDef",
     "AnalyzerSummaryTypeDef",
     "ArchiveRuleSummaryTypeDef",
     "CloudTrailDetailsTypeDef",
     "CloudTrailPropertiesTypeDef",
     "CreateAccessPreviewResponseTypeDef",
     "CreateAnalyzerResponseTypeDef",
@@ -183,23 +173,14 @@
 AccessPreviewStatusReasonTypeDef = TypedDict(
     "AccessPreviewStatusReasonTypeDef",
     {
         "code": AccessPreviewStatusReasonCodeType,
     },
 )
 
-AclGranteeOutputTypeDef = TypedDict(
-    "AclGranteeOutputTypeDef",
-    {
-        "id": str,
-        "uri": str,
-    },
-    total=False,
-)
-
 AclGranteeTypeDef = TypedDict(
     "AclGranteeTypeDef",
     {
         "id": str,
         "uri": str,
     },
     total=False,
@@ -327,73 +308,14 @@
         "userIds": List[str],
         "groups": List[str],
         "kmsKeyId": str,
     },
     total=False,
 )
 
-EcrRepositoryConfigurationOutputTypeDef = TypedDict(
-    "EcrRepositoryConfigurationOutputTypeDef",
-    {
-        "repositoryPolicy": str,
-    },
-    total=False,
-)
-
-EfsFileSystemConfigurationOutputTypeDef = TypedDict(
-    "EfsFileSystemConfigurationOutputTypeDef",
-    {
-        "fileSystemPolicy": str,
-    },
-    total=False,
-)
-
-IamRoleConfigurationOutputTypeDef = TypedDict(
-    "IamRoleConfigurationOutputTypeDef",
-    {
-        "trustPolicy": str,
-    },
-    total=False,
-)
-
-SecretsManagerSecretConfigurationOutputTypeDef = TypedDict(
-    "SecretsManagerSecretConfigurationOutputTypeDef",
-    {
-        "kmsKeyId": str,
-        "secretPolicy": str,
-    },
-    total=False,
-)
-
-SnsTopicConfigurationOutputTypeDef = TypedDict(
-    "SnsTopicConfigurationOutputTypeDef",
-    {
-        "topicPolicy": str,
-    },
-    total=False,
-)
-
-SqsQueueConfigurationOutputTypeDef = TypedDict(
-    "SqsQueueConfigurationOutputTypeDef",
-    {
-        "queuePolicy": str,
-    },
-    total=False,
-)
-
-EbsSnapshotConfigurationTypeDef = TypedDict(
-    "EbsSnapshotConfigurationTypeDef",
-    {
-        "userIds": Sequence[str],
-        "groups": Sequence[str],
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
 EcrRepositoryConfigurationTypeDef = TypedDict(
     "EcrRepositoryConfigurationTypeDef",
     {
         "repositoryPolicy": str,
     },
     total=False,
 )
@@ -435,14 +357,24 @@
     "SqsQueueConfigurationTypeDef",
     {
         "queuePolicy": str,
     },
     total=False,
 )
 
+EbsSnapshotConfigurationTypeDef = TypedDict(
+    "EbsSnapshotConfigurationTypeDef",
+    {
+        "userIds": Sequence[str],
+        "groups": Sequence[str],
+        "kmsKeyId": str,
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -727,21 +659,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-VpcConfigurationOutputTypeDef = TypedDict(
-    "VpcConfigurationOutputTypeDef",
-    {
-        "vpcId": str,
-    },
-)
-
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "vpcId": str,
     },
 )
 
@@ -797,22 +722,14 @@
     "RdsDbSnapshotAttributeValueTypeDef",
     {
         "accountIds": Sequence[str],
     },
     total=False,
 )
 
-S3PublicAccessBlockConfigurationOutputTypeDef = TypedDict(
-    "S3PublicAccessBlockConfigurationOutputTypeDef",
-    {
-        "ignorePublicAcls": bool,
-        "restrictPublicBuckets": bool,
-    },
-)
-
 S3PublicAccessBlockConfigurationTypeDef = TypedDict(
     "S3PublicAccessBlockConfigurationTypeDef",
     {
         "ignorePublicAcls": bool,
         "restrictPublicBuckets": bool,
     },
 )
@@ -916,22 +833,14 @@
 )
 
 class AccessPreviewSummaryTypeDef(
     _RequiredAccessPreviewSummaryTypeDef, _OptionalAccessPreviewSummaryTypeDef
 ):
     pass
 
-S3BucketAclGrantConfigurationOutputTypeDef = TypedDict(
-    "S3BucketAclGrantConfigurationOutputTypeDef",
-    {
-        "permission": AclPermissionType,
-        "grantee": AclGranteeOutputTypeDef,
-    },
-)
-
 S3BucketAclGrantConfigurationTypeDef = TypedDict(
     "S3BucketAclGrantConfigurationTypeDef",
     {
         "permission": AclPermissionType,
         "grantee": AclGranteeTypeDef,
     },
 )
@@ -1386,15 +1295,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkOriginConfigurationOutputTypeDef = TypedDict(
     "NetworkOriginConfigurationOutputTypeDef",
     {
-        "vpcConfiguration": VpcConfigurationOutputTypeDef,
+        "vpcConfiguration": VpcConfigurationTypeDef,
         "internetConfiguration": Dict[str, Any],
     },
     total=False,
 )
 
 NetworkOriginConfigurationTypeDef = TypedDict(
     "NetworkOriginConfigurationTypeDef",
@@ -1674,15 +1583,15 @@
     total=False,
 )
 
 S3AccessPointConfigurationOutputTypeDef = TypedDict(
     "S3AccessPointConfigurationOutputTypeDef",
     {
         "accessPointPolicy": str,
-        "publicAccessBlock": S3PublicAccessBlockConfigurationOutputTypeDef,
+        "publicAccessBlock": S3PublicAccessBlockConfigurationTypeDef,
         "networkOrigin": NetworkOriginConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 S3AccessPointConfigurationTypeDef = TypedDict(
     "S3AccessPointConfigurationTypeDef",
@@ -1747,16 +1656,16 @@
     },
 )
 
 S3BucketConfigurationOutputTypeDef = TypedDict(
     "S3BucketConfigurationOutputTypeDef",
     {
         "bucketPolicy": str,
-        "bucketAclGrants": List[S3BucketAclGrantConfigurationOutputTypeDef],
-        "bucketPublicAccessBlock": S3PublicAccessBlockConfigurationOutputTypeDef,
+        "bucketAclGrants": List[S3BucketAclGrantConfigurationTypeDef],
+        "bucketPublicAccessBlock": S3PublicAccessBlockConfigurationTypeDef,
         "accessPoints": Dict[str, S3AccessPointConfigurationOutputTypeDef],
     },
     total=False,
 )
 
 S3BucketConfigurationTypeDef = TypedDict(
     "S3BucketConfigurationTypeDef",
@@ -1789,24 +1698,24 @@
     },
 )
 
 ConfigurationOutputTypeDef = TypedDict(
     "ConfigurationOutputTypeDef",
     {
         "ebsSnapshot": EbsSnapshotConfigurationOutputTypeDef,
-        "ecrRepository": EcrRepositoryConfigurationOutputTypeDef,
-        "iamRole": IamRoleConfigurationOutputTypeDef,
-        "efsFileSystem": EfsFileSystemConfigurationOutputTypeDef,
+        "ecrRepository": EcrRepositoryConfigurationTypeDef,
+        "iamRole": IamRoleConfigurationTypeDef,
+        "efsFileSystem": EfsFileSystemConfigurationTypeDef,
         "kmsKey": KmsKeyConfigurationOutputTypeDef,
         "rdsDbClusterSnapshot": RdsDbClusterSnapshotConfigurationOutputTypeDef,
         "rdsDbSnapshot": RdsDbSnapshotConfigurationOutputTypeDef,
-        "secretsManagerSecret": SecretsManagerSecretConfigurationOutputTypeDef,
+        "secretsManagerSecret": SecretsManagerSecretConfigurationTypeDef,
         "s3Bucket": S3BucketConfigurationOutputTypeDef,
-        "snsTopic": SnsTopicConfigurationOutputTypeDef,
-        "sqsQueue": SqsQueueConfigurationOutputTypeDef,
+        "snsTopic": SnsTopicConfigurationTypeDef,
+        "sqsQueue": SqsQueueConfigurationTypeDef,
     },
     total=False,
 )
 
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
```

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/PKG-INFO` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-accessanalyzer
-Version: 1.28.12
-Summary: Type annotations for boto3.AccessAnalyzer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-accessanalyzer.svg?color=blue)](https://pypi.org/project/mypy-boto3-accessanalyzer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-accessanalyzer)](https://pepy.tech/project/mypy-boto3-accessanalyzer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AccessAnalyzer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
+[boto3.AccessAnalyzer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
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
 [mypy-boto3-accessanalyzer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_accessanalyzer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,38 +371,31 @@
 
 `mypy_boto3_accessanalyzer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_accessanalyzer.type_defs import (
     AccessPreviewStatusReasonTypeDef,
-    AclGranteeOutputTypeDef,
     AclGranteeTypeDef,
     AnalyzedResourceSummaryTypeDef,
     AnalyzedResourceTypeDef,
     StatusReasonTypeDef,
     ApplyArchiveRuleRequestRequestTypeDef,
     CriterionOutputTypeDef,
     CancelPolicyGenerationRequestRequestTypeDef,
     TrailTypeDef,
     TrailPropertiesTypeDef,
     EbsSnapshotConfigurationOutputTypeDef,
-    EcrRepositoryConfigurationOutputTypeDef,
-    EfsFileSystemConfigurationOutputTypeDef,
-    IamRoleConfigurationOutputTypeDef,
-    SecretsManagerSecretConfigurationOutputTypeDef,
-    SnsTopicConfigurationOutputTypeDef,
-    SqsQueueConfigurationOutputTypeDef,
-    EbsSnapshotConfigurationTypeDef,
     EcrRepositoryConfigurationTypeDef,
     EfsFileSystemConfigurationTypeDef,
     IamRoleConfigurationTypeDef,
     SecretsManagerSecretConfigurationTypeDef,
     SnsTopicConfigurationTypeDef,
     SqsQueueConfigurationTypeDef,
+    EbsSnapshotConfigurationTypeDef,
     ResponseMetadataTypeDef,
     CriterionTypeDef,
     DeleteAnalyzerRequestRequestTypeDef,
     DeleteArchiveRuleRequestRequestTypeDef,
     FindingSourceDetailTypeDef,
     GeneratedPolicyTypeDef,
     GetAccessPreviewRequestRequestTypeDef,
@@ -419,32 +412,29 @@
     ListAnalyzedResourcesRequestRequestTypeDef,
     ListAnalyzersRequestRequestTypeDef,
     ListArchiveRulesRequestRequestTypeDef,
     SortCriteriaTypeDef,
     ListPolicyGenerationsRequestRequestTypeDef,
     PolicyGenerationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
     SubstringTypeDef,
     PolicyGenerationDetailsTypeDef,
     PositionTypeDef,
     RdsDbClusterSnapshotAttributeValueOutputTypeDef,
     RdsDbClusterSnapshotAttributeValueTypeDef,
     RdsDbSnapshotAttributeValueOutputTypeDef,
     RdsDbSnapshotAttributeValueTypeDef,
-    S3PublicAccessBlockConfigurationOutputTypeDef,
     S3PublicAccessBlockConfigurationTypeDef,
     StartResourceScanRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     ValidatePolicyRequestRequestTypeDef,
     AccessPreviewSummaryTypeDef,
-    S3BucketAclGrantConfigurationOutputTypeDef,
     S3BucketAclGrantConfigurationTypeDef,
     AnalyzerSummaryTypeDef,
     ArchiveRuleSummaryTypeDef,
     CloudTrailDetailsTypeDef,
     CloudTrailPropertiesTypeDef,
     CreateAccessPreviewResponseTypeDef,
     CreateAnalyzerResponseTypeDef,
```

### Comparing `mypy-boto3-accessanalyzer-1.28.12/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt` & `mypy-boto3-accessanalyzer-1.28.15/mypy_boto3_accessanalyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-accessanalyzer-1.28.12/setup.py` & `mypy-boto3-accessanalyzer-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-accessanalyzer",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_accessanalyzer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AccessAnalyzer 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.AccessAnalyzer 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

