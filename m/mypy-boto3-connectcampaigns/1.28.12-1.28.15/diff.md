# Comparing `tmp/mypy-boto3-connectcampaigns-1.28.12.tar.gz` & `tmp/mypy-boto3-connectcampaigns-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectcampaigns-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
+gzip compressed data, was "mypy-boto3-connectcampaigns-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
```

## Comparing `mypy-boto3-connectcampaigns-1.28.12.tar` & `mypy-boto3-connectcampaigns-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.520542 mypy-boto3-connectcampaigns-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-27 05:34:31.516543 mypy-boto3-connectcampaigns-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14070 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.516543 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.516543 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 05:34:31.000000 mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.520542 mypy-boto3-connectcampaigns-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:47.000000 mypy-boto3-connectcampaigns-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.660912 mypy-boto3-connectcampaigns-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:16.000000 mypy-boto3-connectcampaigns-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-07-28 20:42:34.656912 mypy-boto3-connectcampaigns-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-07-28 20:22:16.000000 mypy-boto3-connectcampaigns-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.648912 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-28 20:22:16.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-28 20:22:16.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 20:22:16.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16759 2023-07-28 20:22:17.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16729 2023-07-28 20:22:17.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-28 20:22:17.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-07-28 20:22:17.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:22:17.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-28 20:22:17.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:16.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-28 20:22:18.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-07-28 20:22:18.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:16.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.656912 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-07-28 20:42:34.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:42:34.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:42:34.000000 mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.660912 mypy-boto3-connectcampaigns-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:22:16.000000 mypy-boto3-connectcampaigns-1.28.15/setup.py
```

### Comparing `mypy-boto3-connectcampaigns-1.28.12/LICENSE` & `mypy-boto3-connectcampaigns-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.12/PKG-INFO` & `mypy-boto3-connectcampaigns-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectCampaignService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConnectCampaignService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,59 +327,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
-    AnswerMachineDetectionConfigOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    CreateCampaignResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
-    PredictiveDialerConfigOutputTypeDef,
-    ProgressiveDialerConfigOutputTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
-    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
-    OutboundCallConfigOutputTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
+    CreateCampaignResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
-    DialerConfigOutputTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
@@ -389,15 +383,15 @@
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigOutputTypeDef:
+def get_structure() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.12/README.md` & `mypy-boto3-connectcampaigns-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,59 +295,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
-    AnswerMachineDetectionConfigOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    CreateCampaignResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
-    PredictiveDialerConfigOutputTypeDef,
-    ProgressiveDialerConfigOutputTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
-    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
-    OutboundCallConfigOutputTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
+    CreateCampaignResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
-    DialerConfigOutputTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
@@ -357,15 +351,15 @@
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigOutputTypeDef:
+def get_structure() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__init__.py` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__init__.pyi` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/__main__.py` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectCampaignService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ConnectCampaignService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService\nOther"
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

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/client.py` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/client.pyi` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/literals.py` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/literals.pyi` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/paginator.py` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,13 +44,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: CampaignFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/paginators/#listcampaignspaginator)
         """
```

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/paginator.pyi` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -41,13 +41,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/paginators/#listcampaignspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: CampaignFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/paginators/#listcampaignspaginator)
         """
```

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/type_defs.py` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for connectcampaigns service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigOutputTypeDef
+    from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
-    data: AnswerMachineDetectionConfigOutputTypeDef = {...}
+    data: AnswerMachineDetectionConfigTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,59 +30,53 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AnswerMachineDetectionConfigOutputTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
-    "CreateCampaignResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DialRequestTypeDef",
-    "PredictiveDialerConfigOutputTypeDef",
-    "ProgressiveDialerConfigOutputTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
     "GetCampaignStateRequestRequestTypeDef",
-    "GetCampaignStateResponseTypeDef",
     "GetConnectInstanceConfigRequestRequestTypeDef",
     "GetInstanceOnboardingJobStatusRequestRequestTypeDef",
     "InstanceOnboardingJobStatusTypeDef",
-    "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "PauseCampaignRequestRequestTypeDef",
     "SuccessfulRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeCampaignRequestRequestTypeDef",
     "StartCampaignRequestRequestTypeDef",
     "StopCampaignRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignNameRequestRequestTypeDef",
-    "OutboundCallConfigOutputTypeDef",
     "OutboundCallConfigTypeDef",
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCampaignStateResponseTypeDef",
     "ListCampaignsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutDialRequestBatchRequestRequestTypeDef",
-    "DialerConfigOutputTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
     "PutDialRequestBatchResponseTypeDef",
@@ -91,21 +85,14 @@
     "CampaignTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     "GetConnectInstanceConfigResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
 )
 
-AnswerMachineDetectionConfigOutputTypeDef = TypedDict(
-    "AnswerMachineDetectionConfigOutputTypeDef",
-    {
-        "enableAnswerMachineDetection": bool,
-    },
-)
-
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "enableAnswerMachineDetection": bool,
     },
 )
 
@@ -123,21 +110,22 @@
         "arn": str,
         "connectInstanceId": str,
         "id": str,
         "name": str,
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "id": str,
@@ -171,71 +159,28 @@
         "attributes": Mapping[str, str],
         "clientToken": str,
         "expirationTime": Union[datetime, str],
         "phoneNumber": str,
     },
 )
 
-PredictiveDialerConfigOutputTypeDef = TypedDict(
-    "PredictiveDialerConfigOutputTypeDef",
-    {
-        "bandwidthAllocation": float,
-    },
-)
-
-ProgressiveDialerConfigOutputTypeDef = TypedDict(
-    "ProgressiveDialerConfigOutputTypeDef",
-    {
-        "bandwidthAllocation": float,
-    },
-)
-
 PredictiveDialerConfigTypeDef = TypedDict(
     "PredictiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
 ProgressiveDialerConfigTypeDef = TypedDict(
     "ProgressiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredEncryptionConfigOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalEncryptionConfigOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigOutputTypeDef",
-    {
-        "encryptionType": Literal["KMS"],
-        "keyArn": str,
-    },
-    total=False,
-)
-
-
-class EncryptionConfigOutputTypeDef(
-    _RequiredEncryptionConfigOutputTypeDef, _OptionalEncryptionConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredEncryptionConfigTypeDef = TypedDict(
     "_RequiredEncryptionConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEncryptionConfigTypeDef = TypedDict(
@@ -290,22 +235,14 @@
 GetCampaignStateRequestRequestTypeDef = TypedDict(
     "GetCampaignStateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetCampaignStateResponseTypeDef = TypedDict(
-    "GetCampaignStateResponseTypeDef",
-    {
-        "state": CampaignStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConnectInstanceConfigRequestRequestTypeDef = TypedDict(
     "GetConnectInstanceConfigRequestRequestTypeDef",
     {
         "connectInstanceId": str,
     },
 )
 
@@ -334,39 +271,31 @@
 
 class InstanceOnboardingJobStatusTypeDef(
     _RequiredInstanceOnboardingJobStatusTypeDef, _OptionalInstanceOnboardingJobStatusTypeDef
 ):
     pass
 
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 PauseCampaignRequestRequestTypeDef = TypedDict(
     "PauseCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -375,25 +304,14 @@
     {
         "clientToken": str,
         "id": str,
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
 ResumeCampaignRequestRequestTypeDef = TypedDict(
     "ResumeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -431,37 +349,14 @@
     "UpdateCampaignNameRequestRequestTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
 
-_RequiredOutboundCallConfigOutputTypeDef = TypedDict(
-    "_RequiredOutboundCallConfigOutputTypeDef",
-    {
-        "connectContactFlowId": str,
-        "connectQueueId": str,
-    },
-)
-_OptionalOutboundCallConfigOutputTypeDef = TypedDict(
-    "_OptionalOutboundCallConfigOutputTypeDef",
-    {
-        "answerMachineDetectionConfig": AnswerMachineDetectionConfigOutputTypeDef,
-        "connectSourcePhoneNumber": str,
-    },
-    total=False,
-)
-
-
-class OutboundCallConfigOutputTypeDef(
-    _RequiredOutboundCallConfigOutputTypeDef, _OptionalOutboundCallConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredOutboundCallConfigTypeDef = TypedDict(
     "_RequiredOutboundCallConfigTypeDef",
     {
         "connectContactFlowId": str,
         "connectQueueId": str,
     },
 )
@@ -509,38 +404,62 @@
     "CampaignFiltersTypeDef",
     {
         "instanceIdFilter": InstanceIdFilterTypeDef,
     },
     total=False,
 )
 
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCampaignStateResponseTypeDef = TypedDict(
+    "GetCampaignStateResponseTypeDef",
+    {
+        "state": CampaignStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaryList": List[CampaignSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutDialRequestBatchRequestRequestTypeDef = TypedDict(
-    "PutDialRequestBatchRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "dialRequests": Sequence[DialRequestTypeDef],
-        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DialerConfigOutputTypeDef = TypedDict(
-    "DialerConfigOutputTypeDef",
+PutDialRequestBatchRequestRequestTypeDef = TypedDict(
+    "PutDialRequestBatchRequestRequestTypeDef",
     {
-        "predictiveDialerConfig": PredictiveDialerConfigOutputTypeDef,
-        "progressiveDialerConfig": ProgressiveDialerConfigOutputTypeDef,
+        "dialRequests": Sequence[DialRequestTypeDef],
+        "id": str,
     },
-    total=False,
 )
 
 DialerConfigTypeDef = TypedDict(
     "DialerConfigTypeDef",
     {
         "predictiveDialerConfig": PredictiveDialerConfigTypeDef,
         "progressiveDialerConfig": ProgressiveDialerConfigTypeDef,
@@ -548,15 +467,15 @@
     total=False,
 )
 
 InstanceConfigTypeDef = TypedDict(
     "InstanceConfigTypeDef",
     {
         "connectInstanceId": str,
-        "encryptionConfig": EncryptionConfigOutputTypeDef,
+        "encryptionConfig": EncryptionConfigTypeDef,
         "serviceLinkedRoleArn": str,
     },
 )
 
 StartInstanceOnboardingJobRequestRequestTypeDef = TypedDict(
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     {
@@ -566,48 +485,48 @@
 )
 
 GetCampaignStateBatchResponseTypeDef = TypedDict(
     "GetCampaignStateBatchResponseTypeDef",
     {
         "failedRequests": List[FailedCampaignStateResponseTypeDef],
         "successfulRequests": List[SuccessfulCampaignStateResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceOnboardingJobStatusResponseTypeDef = TypedDict(
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartInstanceOnboardingJobResponseTypeDef = TypedDict(
     "StartInstanceOnboardingJobResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDialRequestBatchResponseTypeDef = TypedDict(
     "PutDialRequestBatchResponseTypeDef",
     {
         "failedRequests": List[FailedRequestTypeDef],
         "successfulRequests": List[SuccessfulRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     {
         "filters": CampaignFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
@@ -619,18 +538,18 @@
 )
 
 _RequiredCampaignTypeDef = TypedDict(
     "_RequiredCampaignTypeDef",
     {
         "arn": str,
         "connectInstanceId": str,
-        "dialerConfig": DialerConfigOutputTypeDef,
+        "dialerConfig": DialerConfigTypeDef,
         "id": str,
         "name": str,
-        "outboundCallConfig": OutboundCallConfigOutputTypeDef,
+        "outboundCallConfig": OutboundCallConfigTypeDef,
     },
 )
 _OptionalCampaignTypeDef = TypedDict(
     "_OptionalCampaignTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -674,18 +593,18 @@
     },
 )
 
 GetConnectInstanceConfigResponseTypeDef = TypedDict(
     "GetConnectInstanceConfigResponseTypeDef",
     {
         "connectInstanceConfig": InstanceConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCampaignResponseTypeDef = TypedDict(
     "DescribeCampaignResponseTypeDef",
     {
         "campaign": CampaignTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns/type_defs.pyi` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for connectcampaigns service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigOutputTypeDef
+    from mypy_boto3_connectcampaigns.type_defs import AnswerMachineDetectionConfigTypeDef
 
-    data: AnswerMachineDetectionConfigOutputTypeDef = {...}
+    data: AnswerMachineDetectionConfigTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -29,59 +29,53 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AnswerMachineDetectionConfigOutputTypeDef",
     "AnswerMachineDetectionConfigTypeDef",
     "InstanceIdFilterTypeDef",
     "CampaignSummaryTypeDef",
-    "CreateCampaignResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
     "DeleteConnectInstanceConfigRequestRequestTypeDef",
     "DeleteInstanceOnboardingJobRequestRequestTypeDef",
     "DescribeCampaignRequestRequestTypeDef",
     "DialRequestTypeDef",
-    "PredictiveDialerConfigOutputTypeDef",
-    "ProgressiveDialerConfigOutputTypeDef",
     "PredictiveDialerConfigTypeDef",
     "ProgressiveDialerConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
     "FailedCampaignStateResponseTypeDef",
     "FailedRequestTypeDef",
     "GetCampaignStateBatchRequestRequestTypeDef",
     "SuccessfulCampaignStateResponseTypeDef",
     "GetCampaignStateRequestRequestTypeDef",
-    "GetCampaignStateResponseTypeDef",
     "GetConnectInstanceConfigRequestRequestTypeDef",
     "GetInstanceOnboardingJobStatusRequestRequestTypeDef",
     "InstanceOnboardingJobStatusTypeDef",
-    "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
+    "ListTagsForResourceRequestRequestTypeDef",
     "PauseCampaignRequestRequestTypeDef",
     "SuccessfulRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeCampaignRequestRequestTypeDef",
     "StartCampaignRequestRequestTypeDef",
     "StopCampaignRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignNameRequestRequestTypeDef",
-    "OutboundCallConfigOutputTypeDef",
     "OutboundCallConfigTypeDef",
     "UpdateCampaignOutboundCallConfigRequestRequestTypeDef",
     "CampaignFiltersTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCampaignStateResponseTypeDef",
     "ListCampaignsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutDialRequestBatchRequestRequestTypeDef",
-    "DialerConfigOutputTypeDef",
     "DialerConfigTypeDef",
     "InstanceConfigTypeDef",
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     "GetCampaignStateBatchResponseTypeDef",
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     "StartInstanceOnboardingJobResponseTypeDef",
     "PutDialRequestBatchResponseTypeDef",
@@ -90,21 +84,14 @@
     "CampaignTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "UpdateCampaignDialerConfigRequestRequestTypeDef",
     "GetConnectInstanceConfigResponseTypeDef",
     "DescribeCampaignResponseTypeDef",
 )
 
-AnswerMachineDetectionConfigOutputTypeDef = TypedDict(
-    "AnswerMachineDetectionConfigOutputTypeDef",
-    {
-        "enableAnswerMachineDetection": bool,
-    },
-)
-
 AnswerMachineDetectionConfigTypeDef = TypedDict(
     "AnswerMachineDetectionConfigTypeDef",
     {
         "enableAnswerMachineDetection": bool,
     },
 )
 
@@ -122,21 +109,22 @@
         "arn": str,
         "connectInstanceId": str,
         "id": str,
         "name": str,
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "id": str,
@@ -170,69 +158,28 @@
         "attributes": Mapping[str, str],
         "clientToken": str,
         "expirationTime": Union[datetime, str],
         "phoneNumber": str,
     },
 )
 
-PredictiveDialerConfigOutputTypeDef = TypedDict(
-    "PredictiveDialerConfigOutputTypeDef",
-    {
-        "bandwidthAllocation": float,
-    },
-)
-
-ProgressiveDialerConfigOutputTypeDef = TypedDict(
-    "ProgressiveDialerConfigOutputTypeDef",
-    {
-        "bandwidthAllocation": float,
-    },
-)
-
 PredictiveDialerConfigTypeDef = TypedDict(
     "PredictiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
 ProgressiveDialerConfigTypeDef = TypedDict(
     "ProgressiveDialerConfigTypeDef",
     {
         "bandwidthAllocation": float,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredEncryptionConfigOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalEncryptionConfigOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigOutputTypeDef",
-    {
-        "encryptionType": Literal["KMS"],
-        "keyArn": str,
-    },
-    total=False,
-)
-
-class EncryptionConfigOutputTypeDef(
-    _RequiredEncryptionConfigOutputTypeDef, _OptionalEncryptionConfigOutputTypeDef
-):
-    pass
-
 _RequiredEncryptionConfigTypeDef = TypedDict(
     "_RequiredEncryptionConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEncryptionConfigTypeDef = TypedDict(
@@ -285,22 +232,14 @@
 GetCampaignStateRequestRequestTypeDef = TypedDict(
     "GetCampaignStateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetCampaignStateResponseTypeDef = TypedDict(
-    "GetCampaignStateResponseTypeDef",
-    {
-        "state": CampaignStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConnectInstanceConfigRequestRequestTypeDef = TypedDict(
     "GetConnectInstanceConfigRequestRequestTypeDef",
     {
         "connectInstanceId": str,
     },
 )
 
@@ -327,39 +266,31 @@
 )
 
 class InstanceOnboardingJobStatusTypeDef(
     _RequiredInstanceOnboardingJobStatusTypeDef, _OptionalInstanceOnboardingJobStatusTypeDef
 ):
     pass
 
-ListTagsForResourceRequestRequestTypeDef = TypedDict(
-    "ListTagsForResourceRequestRequestTypeDef",
-    {
-        "arn": str,
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
+ListTagsForResourceRequestRequestTypeDef = TypedDict(
+    "ListTagsForResourceRequestRequestTypeDef",
+    {
+        "arn": str,
+    },
+)
+
 PauseCampaignRequestRequestTypeDef = TypedDict(
     "PauseCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -368,25 +299,14 @@
     {
         "clientToken": str,
         "id": str,
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
 ResumeCampaignRequestRequestTypeDef = TypedDict(
     "ResumeCampaignRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -424,35 +344,14 @@
     "UpdateCampaignNameRequestRequestTypeDef",
     {
         "id": str,
         "name": str,
     },
 )
 
-_RequiredOutboundCallConfigOutputTypeDef = TypedDict(
-    "_RequiredOutboundCallConfigOutputTypeDef",
-    {
-        "connectContactFlowId": str,
-        "connectQueueId": str,
-    },
-)
-_OptionalOutboundCallConfigOutputTypeDef = TypedDict(
-    "_OptionalOutboundCallConfigOutputTypeDef",
-    {
-        "answerMachineDetectionConfig": AnswerMachineDetectionConfigOutputTypeDef,
-        "connectSourcePhoneNumber": str,
-    },
-    total=False,
-)
-
-class OutboundCallConfigOutputTypeDef(
-    _RequiredOutboundCallConfigOutputTypeDef, _OptionalOutboundCallConfigOutputTypeDef
-):
-    pass
-
 _RequiredOutboundCallConfigTypeDef = TypedDict(
     "_RequiredOutboundCallConfigTypeDef",
     {
         "connectContactFlowId": str,
         "connectQueueId": str,
     },
 )
@@ -496,38 +395,62 @@
     "CampaignFiltersTypeDef",
     {
         "instanceIdFilter": InstanceIdFilterTypeDef,
     },
     total=False,
 )
 
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCampaignStateResponseTypeDef = TypedDict(
+    "GetCampaignStateResponseTypeDef",
+    {
+        "state": CampaignStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCampaignsResponseTypeDef = TypedDict(
     "ListCampaignsResponseTypeDef",
     {
         "campaignSummaryList": List[CampaignSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutDialRequestBatchRequestRequestTypeDef = TypedDict(
-    "PutDialRequestBatchRequestRequestTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "dialRequests": Sequence[DialRequestTypeDef],
-        "id": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DialerConfigOutputTypeDef = TypedDict(
-    "DialerConfigOutputTypeDef",
+PutDialRequestBatchRequestRequestTypeDef = TypedDict(
+    "PutDialRequestBatchRequestRequestTypeDef",
     {
-        "predictiveDialerConfig": PredictiveDialerConfigOutputTypeDef,
-        "progressiveDialerConfig": ProgressiveDialerConfigOutputTypeDef,
+        "dialRequests": Sequence[DialRequestTypeDef],
+        "id": str,
     },
-    total=False,
 )
 
 DialerConfigTypeDef = TypedDict(
     "DialerConfigTypeDef",
     {
         "predictiveDialerConfig": PredictiveDialerConfigTypeDef,
         "progressiveDialerConfig": ProgressiveDialerConfigTypeDef,
@@ -535,15 +458,15 @@
     total=False,
 )
 
 InstanceConfigTypeDef = TypedDict(
     "InstanceConfigTypeDef",
     {
         "connectInstanceId": str,
-        "encryptionConfig": EncryptionConfigOutputTypeDef,
+        "encryptionConfig": EncryptionConfigTypeDef,
         "serviceLinkedRoleArn": str,
     },
 )
 
 StartInstanceOnboardingJobRequestRequestTypeDef = TypedDict(
     "StartInstanceOnboardingJobRequestRequestTypeDef",
     {
@@ -553,48 +476,48 @@
 )
 
 GetCampaignStateBatchResponseTypeDef = TypedDict(
     "GetCampaignStateBatchResponseTypeDef",
     {
         "failedRequests": List[FailedCampaignStateResponseTypeDef],
         "successfulRequests": List[SuccessfulCampaignStateResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceOnboardingJobStatusResponseTypeDef = TypedDict(
     "GetInstanceOnboardingJobStatusResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartInstanceOnboardingJobResponseTypeDef = TypedDict(
     "StartInstanceOnboardingJobResponseTypeDef",
     {
         "connectInstanceOnboardingJobStatus": InstanceOnboardingJobStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDialRequestBatchResponseTypeDef = TypedDict(
     "PutDialRequestBatchResponseTypeDef",
     {
         "failedRequests": List[FailedRequestTypeDef],
         "successfulRequests": List[SuccessfulRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
     "ListCampaignsRequestListCampaignsPaginateTypeDef",
     {
         "filters": CampaignFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
@@ -606,18 +529,18 @@
 )
 
 _RequiredCampaignTypeDef = TypedDict(
     "_RequiredCampaignTypeDef",
     {
         "arn": str,
         "connectInstanceId": str,
-        "dialerConfig": DialerConfigOutputTypeDef,
+        "dialerConfig": DialerConfigTypeDef,
         "id": str,
         "name": str,
-        "outboundCallConfig": OutboundCallConfigOutputTypeDef,
+        "outboundCallConfig": OutboundCallConfigTypeDef,
     },
 )
 _OptionalCampaignTypeDef = TypedDict(
     "_OptionalCampaignTypeDef",
     {
         "tags": Dict[str, str],
     },
@@ -657,18 +580,18 @@
     },
 )
 
 GetConnectInstanceConfigResponseTypeDef = TypedDict(
     "GetConnectInstanceConfigResponseTypeDef",
     {
         "connectInstanceConfig": InstanceConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCampaignResponseTypeDef = TypedDict(
     "DescribeCampaignResponseTypeDef",
     {
         "campaign": CampaignTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/PKG-INFO` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectcampaigns
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectCampaignService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConnectCampaignService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectcampaigns.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectcampaigns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectcampaigns)](https://pepy.tech/project/mypy-boto3-connectcampaigns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectCampaignService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
+[boto3.ConnectCampaignService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
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
 [mypy-boto3-connectcampaigns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectcampaigns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,59 +327,53 @@
 ### Typed dictionaries
 
 `mypy_boto3_connectcampaigns.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_connectcampaigns.type_defs import (
-    AnswerMachineDetectionConfigOutputTypeDef,
     AnswerMachineDetectionConfigTypeDef,
     InstanceIdFilterTypeDef,
     CampaignSummaryTypeDef,
-    CreateCampaignResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteCampaignRequestRequestTypeDef,
     DeleteConnectInstanceConfigRequestRequestTypeDef,
     DeleteInstanceOnboardingJobRequestRequestTypeDef,
     DescribeCampaignRequestRequestTypeDef,
     DialRequestTypeDef,
-    PredictiveDialerConfigOutputTypeDef,
-    ProgressiveDialerConfigOutputTypeDef,
     PredictiveDialerConfigTypeDef,
     ProgressiveDialerConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EncryptionConfigOutputTypeDef,
     EncryptionConfigTypeDef,
     FailedCampaignStateResponseTypeDef,
     FailedRequestTypeDef,
     GetCampaignStateBatchRequestRequestTypeDef,
     SuccessfulCampaignStateResponseTypeDef,
     GetCampaignStateRequestRequestTypeDef,
-    GetCampaignStateResponseTypeDef,
     GetConnectInstanceConfigRequestRequestTypeDef,
     GetInstanceOnboardingJobStatusRequestRequestTypeDef,
     InstanceOnboardingJobStatusTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
+    ListTagsForResourceRequestRequestTypeDef,
     PauseCampaignRequestRequestTypeDef,
     SuccessfulRequestTypeDef,
-    ResponseMetadataTypeDef,
     ResumeCampaignRequestRequestTypeDef,
     StartCampaignRequestRequestTypeDef,
     StopCampaignRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignNameRequestRequestTypeDef,
-    OutboundCallConfigOutputTypeDef,
     OutboundCallConfigTypeDef,
     UpdateCampaignOutboundCallConfigRequestRequestTypeDef,
     CampaignFiltersTypeDef,
+    CreateCampaignResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCampaignStateResponseTypeDef,
     ListCampaignsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutDialRequestBatchRequestRequestTypeDef,
-    DialerConfigOutputTypeDef,
     DialerConfigTypeDef,
     InstanceConfigTypeDef,
     StartInstanceOnboardingJobRequestRequestTypeDef,
     GetCampaignStateBatchResponseTypeDef,
     GetInstanceOnboardingJobStatusResponseTypeDef,
     StartInstanceOnboardingJobResponseTypeDef,
     PutDialRequestBatchResponseTypeDef,
@@ -389,15 +383,15 @@
     CreateCampaignRequestRequestTypeDef,
     UpdateCampaignDialerConfigRequestRequestTypeDef,
     GetConnectInstanceConfigResponseTypeDef,
     DescribeCampaignResponseTypeDef,
 )
 
 
-def get_structure() -> AnswerMachineDetectionConfigOutputTypeDef:
+def get_structure() -> AnswerMachineDetectionConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-connectcampaigns-1.28.12/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt` & `mypy-boto3-connectcampaigns-1.28.15/mypy_boto3_connectcampaigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectcampaigns-1.28.12/setup.py` & `mypy-boto3-connectcampaigns-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectcampaigns",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_connectcampaigns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectCampaignService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ConnectCampaignService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

