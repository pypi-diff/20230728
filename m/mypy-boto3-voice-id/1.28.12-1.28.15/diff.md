# Comparing `tmp/mypy-boto3-voice-id-1.28.12.tar.gz` & `tmp/mypy-boto3-voice-id-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-voice-id-1.28.12.tar", last modified: Thu Jul 27 11:49:48 2023, max compression
+gzip compressed data, was "mypy-boto3-voice-id-1.28.15.tar", last modified: Fri Jul 28 20:43:55 2023, max compression
```

## Comparing `mypy-boto3-voice-id-1.28.12.tar` & `mypy-boto3-voice-id-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16181 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-27 11:48:18.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-07-27 11:48:18.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34377 2023-07-27 11:48:18.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34338 2023-07-27 11:48:18.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17671 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:48.000000 mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:48.593483 mypy-boto3-voice-id-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-27 11:48:17.000000 mypy-boto3-voice-id-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.214021 mypy-boto3-voice-id-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-07-28 20:43:55.214021 mypy-boto3-voice-id-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.210021 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23148 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23106 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7565 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33375 2023-07-28 20:40:56.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33338 2023-07-28 20:40:56.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:55.214021 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:43:55.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:54.000000 mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:55.214021 mypy-boto3-voice-id-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-28 20:40:55.000000 mypy-boto3-voice-id-1.28.15/setup.py
```

### Comparing `mypy-boto3-voice-id-1.28.12/LICENSE` & `mypy-boto3-voice-id-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/PKG-INFO` & `mypy-boto3-voice-id-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.28.12
-Summary: Type annotations for boto3.VoiceID 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,53 +371,50 @@
     DescribeFraudsterRegistrationJobRequestRequestTypeDef,
     DescribeFraudsterRequestRequestTypeDef,
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
     EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
-    InputDataConfigOutputTypeDef,
-    OutputDataConfigOutputTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    InputDataConfigTypeDef,
     PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
     ListFraudstersRequestRequestTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    OutputDataConfigTypeDef,
     RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
@@ -432,15 +429,14 @@
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.28.12/README.md` & `mypy-boto3-voice-id-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,53 +339,50 @@
     DescribeFraudsterRegistrationJobRequestRequestTypeDef,
     DescribeFraudsterRequestRequestTypeDef,
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
     EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
-    InputDataConfigOutputTypeDef,
-    OutputDataConfigOutputTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    InputDataConfigTypeDef,
     PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
     ListFraudstersRequestRequestTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    OutputDataConfigTypeDef,
     RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
@@ -400,15 +397,14 @@
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__init__.py` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__init__.pyi` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/__main__.py` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.VoiceID 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.VoiceID 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/client.py` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/client.pyi` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/literals.py` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/literals.pyi` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/paginator.py` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/paginator.pyi` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/type_defs.py` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,53 +53,50 @@
     "DescribeFraudsterRegistrationJobRequestRequestTypeDef",
     "DescribeFraudsterRequestRequestTypeDef",
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
     "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
-    "InputDataConfigOutputTypeDef",
-    "OutputDataConfigOutputTypeDef",
+    "InputDataConfigTypeDef",
+    "OutputDataConfigTypeDef",
     "RegistrationConfigOutputTypeDef",
     "FraudsterSummaryTypeDef",
-    "InputDataConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
     "ListFraudstersRequestRequestTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
-    "OutputDataConfigTypeDef",
     "RegistrationConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
     "UpdateWatchlistResponseTypeDef",
     "DescribeSpeakerResponseTypeDef",
     "OptOutSpeakerResponseTypeDef",
     "DomainSummaryTypeDef",
@@ -114,15 +111,14 @@
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
     "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
@@ -324,21 +320,14 @@
     {
         "DomainId": str,
         "FraudsterId": str,
         "WatchlistId": str,
     },
 )
 
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-)
-
 ServerSideEncryptionUpdateDetailsTypeDef = TypedDict(
     "ServerSideEncryptionUpdateDetailsTypeDef",
     {
         "Message": str,
         "OldKmsKeyId": str,
         "UpdateStatus": ServerSideEncryptionUpdateStatusType,
     },
@@ -430,39 +419,37 @@
     "JobProgressTypeDef",
     {
         "PercentComplete": int,
     },
     total=False,
 )
 
-InputDataConfigOutputTypeDef = TypedDict(
-    "InputDataConfigOutputTypeDef",
+InputDataConfigTypeDef = TypedDict(
+    "InputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 
-_RequiredOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredOutputDataConfigOutputTypeDef",
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
-_OptionalOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalOutputDataConfigOutputTypeDef",
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
 
-class OutputDataConfigOutputTypeDef(
-    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
-):
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
 
 RegistrationConfigOutputTypeDef = TypedDict(
     "RegistrationConfigOutputTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
@@ -479,21 +466,14 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
     },
     total=False,
 )
 
-InputDataConfigTypeDef = TypedDict(
-    "InputDataConfigTypeDef",
-    {
-        "S3Uri": str,
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
@@ -619,22 +599,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredListWatchlistsRequestRequestTypeDef = TypedDict(
     "_RequiredListWatchlistsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListWatchlistsRequestRequestTypeDef = TypedDict(
@@ -671,33 +643,14 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
 )
 
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
-    pass
-
-
 RegistrationConfigTypeDef = TypedDict(
     "RegistrationConfigTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
         "WatchlistIds": Sequence[str],
     },
@@ -824,14 +777,22 @@
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -881,15 +842,15 @@
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "DomainId": str,
         "DomainStatus": DomainStatusType,
         "Name": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
@@ -898,15 +859,15 @@
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "DomainId": str,
         "DomainStatus": DomainStatusType,
         "Name": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
@@ -970,20 +931,20 @@
     "FraudsterRegistrationJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
         "FailureDetails": FailureDetailsTypeDef,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": FraudsterRegistrationJobStatusType,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "RegistrationConfig": RegistrationConfigOutputTypeDef,
     },
     total=False,
 )
 
 ListFraudstersResponseTypeDef = TypedDict(
     "ListFraudstersResponseTypeDef",
@@ -1124,22 +1085,14 @@
     {
         "NextToken": str,
         "SpeakerSummaries": List[SpeakerSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListWatchlistsResponseTypeDef = TypedDict(
     "ListWatchlistsResponseTypeDef",
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1210,20 +1163,20 @@
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
         "EnrollmentConfig": EnrollmentConfigOutputTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id/type_defs.pyi` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -52,53 +52,50 @@
     "DescribeFraudsterRegistrationJobRequestRequestTypeDef",
     "DescribeFraudsterRequestRequestTypeDef",
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
     "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
-    "InputDataConfigOutputTypeDef",
-    "OutputDataConfigOutputTypeDef",
+    "InputDataConfigTypeDef",
+    "OutputDataConfigTypeDef",
     "RegistrationConfigOutputTypeDef",
     "FraudsterSummaryTypeDef",
-    "InputDataConfigTypeDef",
     "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
     "ListFraudstersRequestRequestTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
-    "OutputDataConfigTypeDef",
     "RegistrationConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
     "UpdateWatchlistResponseTypeDef",
     "DescribeSpeakerResponseTypeDef",
     "OptOutSpeakerResponseTypeDef",
     "DomainSummaryTypeDef",
@@ -113,15 +110,14 @@
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
     "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
@@ -321,21 +317,14 @@
     {
         "DomainId": str,
         "FraudsterId": str,
         "WatchlistId": str,
     },
 )
 
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-)
-
 ServerSideEncryptionUpdateDetailsTypeDef = TypedDict(
     "ServerSideEncryptionUpdateDetailsTypeDef",
     {
         "Message": str,
         "OldKmsKeyId": str,
         "UpdateStatus": ServerSideEncryptionUpdateStatusType,
     },
@@ -425,38 +414,36 @@
     "JobProgressTypeDef",
     {
         "PercentComplete": int,
     },
     total=False,
 )
 
-InputDataConfigOutputTypeDef = TypedDict(
-    "InputDataConfigOutputTypeDef",
+InputDataConfigTypeDef = TypedDict(
+    "InputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 
-_RequiredOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredOutputDataConfigOutputTypeDef",
+_RequiredOutputDataConfigTypeDef = TypedDict(
+    "_RequiredOutputDataConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
-_OptionalOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalOutputDataConfigOutputTypeDef",
+_OptionalOutputDataConfigTypeDef = TypedDict(
+    "_OptionalOutputDataConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
-class OutputDataConfigOutputTypeDef(
-    _RequiredOutputDataConfigOutputTypeDef, _OptionalOutputDataConfigOutputTypeDef
-):
+class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
 RegistrationConfigOutputTypeDef = TypedDict(
     "RegistrationConfigOutputTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
@@ -472,21 +459,14 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
     },
     total=False,
 )
 
-InputDataConfigTypeDef = TypedDict(
-    "InputDataConfigTypeDef",
-    {
-        "S3Uri": str,
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
@@ -604,22 +584,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredListWatchlistsRequestRequestTypeDef = TypedDict(
     "_RequiredListWatchlistsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListWatchlistsRequestRequestTypeDef = TypedDict(
@@ -654,31 +626,14 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
 )
 
-_RequiredOutputDataConfigTypeDef = TypedDict(
-    "_RequiredOutputDataConfigTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalOutputDataConfigTypeDef = TypedDict(
-    "_OptionalOutputDataConfigTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
-    pass
-
 RegistrationConfigTypeDef = TypedDict(
     "RegistrationConfigTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
         "WatchlistIds": Sequence[str],
     },
@@ -799,14 +754,22 @@
 )
 
 class CreateDomainRequestRequestTypeDef(
     _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -856,15 +819,15 @@
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "DomainId": str,
         "DomainStatus": DomainStatusType,
         "Name": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
@@ -873,15 +836,15 @@
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "DomainId": str,
         "DomainStatus": DomainStatusType,
         "Name": str,
-        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "ServerSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
@@ -945,20 +908,20 @@
     "FraudsterRegistrationJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
         "FailureDetails": FailureDetailsTypeDef,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": FraudsterRegistrationJobStatusType,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
         "RegistrationConfig": RegistrationConfigOutputTypeDef,
     },
     total=False,
 )
 
 ListFraudstersResponseTypeDef = TypedDict(
     "ListFraudstersResponseTypeDef",
@@ -1089,22 +1052,14 @@
     {
         "NextToken": str,
         "SpeakerSummaries": List[SpeakerSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListWatchlistsResponseTypeDef = TypedDict(
     "ListWatchlistsResponseTypeDef",
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1173,20 +1128,20 @@
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
         "EnrollmentConfig": EnrollmentConfigOutputTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
-        "OutputDataConfig": OutputDataConfigOutputTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
```

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/PKG-INFO` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-voice-id
-Version: 1.28.12
-Summary: Type annotations for boto3.VoiceID 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-voice-id.svg?color=blue)](https://pypi.org/project/mypy-boto3-voice-id)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-voice-id)](https://pepy.tech/project/mypy-boto3-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.VoiceID 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
+[boto3.VoiceID 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [mypy-boto3-voice-id docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_voice_id/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,53 +371,50 @@
     DescribeFraudsterRegistrationJobRequestRequestTypeDef,
     DescribeFraudsterRequestRequestTypeDef,
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
     EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
-    InputDataConfigOutputTypeDef,
-    OutputDataConfigOutputTypeDef,
+    InputDataConfigTypeDef,
+    OutputDataConfigTypeDef,
     RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    InputDataConfigTypeDef,
     PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
     ListFraudstersRequestRequestTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    OutputDataConfigTypeDef,
     RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
@@ -432,15 +429,14 @@
     ListDomainsRequestListDomainsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
```

### Comparing `mypy-boto3-voice-id-1.28.12/mypy_boto3_voice_id.egg-info/SOURCES.txt` & `mypy-boto3-voice-id-1.28.15/mypy_boto3_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-voice-id-1.28.12/setup.py` & `mypy-boto3-voice-id-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-voice-id",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.VoiceID 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.VoiceID 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

