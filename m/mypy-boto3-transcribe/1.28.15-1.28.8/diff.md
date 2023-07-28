# Comparing `tmp/mypy-boto3-transcribe-1.28.15.tar.gz` & `tmp/mypy-boto3-transcribe-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-transcribe-1.28.15.tar", last modified: Fri Jul 28 20:43:53 2023, max compression
+gzip compressed data, was "mypy-boto3-transcribe-1.28.8.tar", last modified: Thu Jul 20 19:47:57 2023, max compression
```

## Comparing `mypy-boto3-transcribe-1.28.15.tar` & `mypy-boto3-transcribe-1.28.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.622000 mypy-boto3-transcribe-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-07-28 20:43:53.617999 mypy-boto3-transcribe-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.610000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29784 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42544 2023-07-28 20:40:47.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42507 2023-07-28 20:40:47.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:46.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:53.617999 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-07-28 20:43:53.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 20:43:53.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:53.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:53.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:53.000000 mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:53.622000 mypy-boto3-transcribe-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:40:45.000000 mypy-boto3-transcribe-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29784 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10538 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44839 2023-07-20 19:47:45.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44808 2023-07-20 19:47:44.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:47:57.000000 mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:57.856787 mypy-boto3-transcribe-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-20 19:47:43.000000 mypy-boto3-transcribe-1.28.8/setup.py
```

### Comparing `mypy-boto3-transcribe-1.28.15/LICENSE` & `mypy-boto3-transcribe-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.15/PKG-INFO` & `mypy-boto3-transcribe-1.28.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.28.15
-Summary: Type annotations for boto3.TranscribeService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.8
+Summary: Type annotations for boto3.TranscribeService 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,25 +318,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
     ContentRedactionOutputTypeDef,
-    LanguageIdSettingsTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
+    LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
     ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
@@ -345,32 +349,39 @@
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
     ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
@@ -385,31 +396,33 @@
     GetMedicalVocabularyResponseTypeDef,
     GetVocabularyFilterResponseTypeDef,
     GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
-    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
-    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
@@ -431,15 +444,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.15/README.md` & `mypy-boto3-transcribe-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -286,25 +286,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
     ContentRedactionOutputTypeDef,
-    LanguageIdSettingsTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
+    LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
     ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
@@ -313,32 +317,39 @@
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
     ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
@@ -353,31 +364,33 @@
     GetMedicalVocabularyResponseTypeDef,
     GetVocabularyFilterResponseTypeDef,
     GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
-    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
-    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
@@ -399,15 +412,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/__main__.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TranscribeService 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.TranscribeService 1.28.8\nVersion:         1.28.8\nBuilder"
+        " version: 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.8")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/client.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/client.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/literals.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -327,15 +326,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/literals.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,14 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
-    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -325,15 +324,14 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
-    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
```

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/type_defs.py` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for transcribe service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeTypeDef
+    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeOutputTypeDef
 
-    data: AbsoluteTimeRangeTypeDef = {...}
+    data: AbsoluteTimeRangeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -42,25 +42,29 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AbsoluteTimeRangeOutputTypeDef",
     "AbsoluteTimeRangeTypeDef",
     "ContentRedactionOutputTypeDef",
-    "LanguageIdSettingsTypeDef",
+    "LanguageIdSettingsOutputTypeDef",
     "ContentRedactionTypeDef",
+    "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
-    "ChannelDefinitionTypeDef",
-    "MediaTypeDef",
+    "ChannelDefinitionOutputTypeDef",
+    "MediaOutputTypeDef",
     "TranscriptTypeDef",
+    "ChannelDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
+    "InputDataConfigOutputTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
@@ -69,32 +73,39 @@
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
     "GetVocabularyRequestRequestTypeDef",
+    "RelativeTimeRangeOutputTypeDef",
     "RelativeTimeRangeTypeDef",
+    "JobExecutionSettingsOutputTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
     "MedicalTranscriptionJobSummaryTypeDef",
     "ListMedicalVocabulariesRequestRequestTypeDef",
     "VocabularyInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
+    "MediaTypeDef",
     "MedicalTranscriptTypeDef",
+    "MedicalTranscriptionSettingOutputTypeDef",
     "MedicalTranscriptionSettingTypeDef",
+    "ModelSettingsOutputTypeDef",
     "ModelSettingsTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
     "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
     "ToxicityDetectionSettingsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
@@ -109,31 +120,33 @@
     "GetMedicalVocabularyResponseTypeDef",
     "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
     "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyResponseTypeDef",
-    "CreateLanguageModelResponseTypeDef",
-    "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateLanguageModelResponseTypeDef",
+    "LanguageModelTypeDef",
+    "InterruptionFilterOutputTypeDef",
+    "NonTalkTimeFilterOutputTypeDef",
+    "SentimentFilterOutputTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
-    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
-    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
     "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
@@ -154,55 +167,51 @@
     "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
 )
 
+AbsoluteTimeRangeOutputTypeDef = TypedDict(
+    "AbsoluteTimeRangeOutputTypeDef",
+    {
+        "StartTime": int,
+        "EndTime": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionOutputTypeDef = TypedDict(
-    "_RequiredContentRedactionOutputTypeDef",
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
-    },
-)
-_OptionalContentRedactionOutputTypeDef = TypedDict(
-    "_OptionalContentRedactionOutputTypeDef",
-    {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
-    total=False,
 )
 
-
-class ContentRedactionOutputTypeDef(
-    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
-):
-    pass
-
-
-LanguageIdSettingsTypeDef = TypedDict(
-    "LanguageIdSettingsTypeDef",
+LanguageIdSettingsOutputTypeDef = TypedDict(
+    "LanguageIdSettingsOutputTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
-    total=False,
 )
 
 _RequiredContentRedactionTypeDef = TypedDict(
     "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
@@ -217,52 +226,67 @@
 )
 
 
 class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
     pass
 
 
+LanguageIdSettingsTypeDef = TypedDict(
+    "LanguageIdSettingsTypeDef",
+    {
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "LanguageModelName": str,
+    },
+    total=False,
+)
+
 CallAnalyticsJobSummaryTypeDef = TypedDict(
     "CallAnalyticsJobSummaryTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-ChannelDefinitionTypeDef = TypedDict(
-    "ChannelDefinitionTypeDef",
+ChannelDefinitionOutputTypeDef = TypedDict(
+    "ChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
     },
-    total=False,
 )
 
-MediaTypeDef = TypedDict(
-    "MediaTypeDef",
+MediaOutputTypeDef = TypedDict(
+    "MediaOutputTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
     },
-    total=False,
 )
 
 TranscriptTypeDef = TypedDict(
     "TranscriptTypeDef",
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
+)
+
+ChannelDefinitionTypeDef = TypedDict(
+    "ChannelDefinitionTypeDef",
+    {
+        "ChannelId": int,
+        "ParticipantRole": ParticipantRoleType,
+    },
     total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -297,14 +321,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "TuningDataS3Uri": str,
+        "DataAccessRoleArn": str,
+    },
+)
+
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -409,25 +442,43 @@
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
+RelativeTimeRangeOutputTypeDef = TypedDict(
+    "RelativeTimeRangeOutputTypeDef",
+    {
+        "StartPercentage": int,
+        "EndPercentage": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
+JobExecutionSettingsOutputTypeDef = TypedDict(
+    "JobExecutionSettingsOutputTypeDef",
+    {
+        "AllowDeferredExecution": bool,
+        "DataAccessRoleArn": str,
+    },
+)
+
 JobExecutionSettingsTypeDef = TypedDict(
     "JobExecutionSettingsTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
     },
     total=False,
@@ -435,15 +486,14 @@
 
 LanguageCodeItemTypeDef = TypedDict(
     "LanguageCodeItemTypeDef",
     {
         "LanguageCode": LanguageCodeType,
         "DurationInSeconds": float,
     },
-    total=False,
 )
 
 ListCallAnalyticsCategoriesRequestRequestTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -495,15 +545,14 @@
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "Specialty": Literal["PRIMARYCARE"],
         "ContentIdentificationType": Literal["PHI"],
         "Type": TypeType,
     },
-    total=False,
 )
 
 ListMedicalVocabulariesRequestRequestTypeDef = TypedDict(
     "ListMedicalVocabulariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -517,24 +566,31 @@
     "VocabularyInfoTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ListTranscriptionJobsRequestRequestTypeDef = TypedDict(
     "ListTranscriptionJobsRequestRequestTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "JobNameContains": str,
         "NextToken": str,
         "MaxResults": int,
@@ -566,23 +622,42 @@
 VocabularyFilterInfoTypeDef = TypedDict(
     "VocabularyFilterInfoTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
     },
+)
+
+MediaTypeDef = TypedDict(
+    "MediaTypeDef",
+    {
+        "MediaFileUri": str,
+        "RedactedMediaFileUri": str,
+    },
     total=False,
 )
 
 MedicalTranscriptTypeDef = TypedDict(
     "MedicalTranscriptTypeDef",
     {
         "TranscriptFileUri": str,
     },
-    total=False,
+)
+
+MedicalTranscriptionSettingOutputTypeDef = TypedDict(
+    "MedicalTranscriptionSettingOutputTypeDef",
+    {
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyName": str,
+    },
 )
 
 MedicalTranscriptionSettingTypeDef = TypedDict(
     "MedicalTranscriptionSettingTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
@@ -590,22 +665,43 @@
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyName": str,
     },
     total=False,
 )
 
+ModelSettingsOutputTypeDef = TypedDict(
+    "ModelSettingsOutputTypeDef",
+    {
+        "LanguageModelName": str,
+    },
+)
+
 ModelSettingsTypeDef = TypedDict(
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
     },
     total=False,
 )
 
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
+    {
+        "VocabularyName": str,
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+    },
+)
+
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
@@ -636,15 +732,14 @@
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
-    total=False,
 )
 
 ToxicityDetectionSettingsOutputTypeDef = TypedDict(
     "ToxicityDetectionSettingsOutputTypeDef",
     {
         "ToxicityCategories": List[Literal["ALL"]],
     },
@@ -720,17 +815,16 @@
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
@@ -859,42 +953,14 @@
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLanguageModelResponseTypeDef = TypedDict(
-    "CreateLanguageModelResponseTypeDef",
-    {
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelName": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "ModelStatus": ModelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LanguageModelTypeDef = TypedDict(
-    "LanguageModelTypeDef",
-    {
-        "ModelName": str,
-        "CreateTime": datetime,
-        "LastModifiedTime": datetime,
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelStatus": ModelStatusType,
-        "UpgradeAvailability": bool,
-        "FailureReason": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateLanguageModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLanguageModelRequestRequestTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelName": str,
         "InputDataConfig": InputDataConfigTypeDef,
@@ -987,122 +1053,135 @@
 
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateLanguageModelResponseTypeDef = TypedDict(
+    "CreateLanguageModelResponseTypeDef",
+    {
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelName": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "ModelStatus": ModelStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+LanguageModelTypeDef = TypedDict(
+    "LanguageModelTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ModelName": str,
+        "CreateTime": datetime,
+        "LastModifiedTime": datetime,
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelStatus": ModelStatusType,
+        "UpgradeAvailability": bool,
+        "FailureReason": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
     },
 )
 
-InterruptionFilterTypeDef = TypedDict(
-    "InterruptionFilterTypeDef",
+InterruptionFilterOutputTypeDef = TypedDict(
+    "InterruptionFilterOutputTypeDef",
     {
         "Threshold": int,
         "ParticipantRole": ParticipantRoleType,
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-NonTalkTimeFilterTypeDef = TypedDict(
-    "NonTalkTimeFilterTypeDef",
+NonTalkTimeFilterOutputTypeDef = TypedDict(
+    "NonTalkTimeFilterOutputTypeDef",
     {
         "Threshold": int,
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-_RequiredSentimentFilterOutputTypeDef = TypedDict(
-    "_RequiredSentimentFilterOutputTypeDef",
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
     {
         "Sentiments": List[SentimentValueType],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
     },
 )
-_OptionalSentimentFilterOutputTypeDef = TypedDict(
-    "_OptionalSentimentFilterOutputTypeDef",
+
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
     {
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "TranscriptFilterType": Literal["EXACT"],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
+        "Targets": List[str],
     },
-    total=False,
 )
 
-
-class SentimentFilterOutputTypeDef(
-    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
-):
-    pass
-
-
-_RequiredSentimentFilterTypeDef = TypedDict(
-    "_RequiredSentimentFilterTypeDef",
+InterruptionFilterTypeDef = TypedDict(
+    "InterruptionFilterTypeDef",
     {
-        "Sentiments": Sequence[SentimentValueType],
+        "Threshold": int,
+        "ParticipantRole": ParticipantRoleType,
+        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "Negate": bool,
     },
+    total=False,
 )
-_OptionalSentimentFilterTypeDef = TypedDict(
-    "_OptionalSentimentFilterTypeDef",
+
+NonTalkTimeFilterTypeDef = TypedDict(
+    "NonTalkTimeFilterTypeDef",
     {
+        "Threshold": int,
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
-        "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
-
-class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
-    pass
-
-
-_RequiredTranscriptFilterOutputTypeDef = TypedDict(
-    "_RequiredTranscriptFilterOutputTypeDef",
+_RequiredSentimentFilterTypeDef = TypedDict(
+    "_RequiredSentimentFilterTypeDef",
     {
-        "TranscriptFilterType": Literal["EXACT"],
-        "Targets": List[str],
+        "Sentiments": Sequence[SentimentValueType],
     },
 )
-_OptionalTranscriptFilterOutputTypeDef = TypedDict(
-    "_OptionalTranscriptFilterOutputTypeDef",
+_OptionalSentimentFilterTypeDef = TypedDict(
+    "_OptionalSentimentFilterTypeDef",
     {
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
 
-class TranscriptFilterOutputTypeDef(
-    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
-):
+class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
     pass
 
 
 _RequiredTranscriptFilterTypeDef = TypedDict(
     "_RequiredTranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
@@ -1151,14 +1230,23 @@
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1168,27 +1256,26 @@
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": MedicalTranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": MedicalTranscriptionSettingTypeDef,
+        "Settings": MedicalTranscriptionSettingOutputTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Specialty": Literal["PRIMARYCARE"],
         "Type": TypeType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMedicalTranscriptionJobRequestRequestTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "LanguageCode": LanguageCodeType,
@@ -1269,75 +1356,72 @@
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "ContentRedaction": ContentRedactionOutputTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": SettingsTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "JobExecutionSettings": JobExecutionSettingsTypeDef,
+        "Settings": SettingsOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "JobExecutionSettings": JobExecutionSettingsOutputTypeDef,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
         "Settings": CallAnalyticsJobSettingsOutputTypeDef,
-        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
+        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
@@ -1379,20 +1463,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleOutputTypeDef = TypedDict(
     "RuleOutputTypeDef",
     {
-        "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
-        "InterruptionFilter": InterruptionFilterTypeDef,
+        "NonTalkTimeFilter": NonTalkTimeFilterOutputTypeDef,
+        "InterruptionFilter": InterruptionFilterOutputTypeDef,
         "TranscriptFilter": TranscriptFilterOutputTypeDef,
         "SentimentFilter": SentimentFilterOutputTypeDef,
     },
-    total=False,
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
@@ -1465,15 +1548,14 @@
     {
         "CategoryName": str,
         "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
         "Rules": Sequence[RuleTypeDef],
```

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe/type_defs.pyi` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for transcribe service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeTypeDef
+    from mypy_boto3_transcribe.type_defs import AbsoluteTimeRangeOutputTypeDef
 
-    data: AbsoluteTimeRangeTypeDef = {...}
+    data: AbsoluteTimeRangeOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -41,25 +41,29 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AbsoluteTimeRangeOutputTypeDef",
     "AbsoluteTimeRangeTypeDef",
     "ContentRedactionOutputTypeDef",
-    "LanguageIdSettingsTypeDef",
+    "LanguageIdSettingsOutputTypeDef",
     "ContentRedactionTypeDef",
+    "LanguageIdSettingsTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
-    "ChannelDefinitionTypeDef",
-    "MediaTypeDef",
+    "ChannelDefinitionOutputTypeDef",
+    "MediaOutputTypeDef",
     "TranscriptTypeDef",
+    "ChannelDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
+    "InputDataConfigOutputTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
@@ -68,32 +72,39 @@
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
     "GetVocabularyRequestRequestTypeDef",
+    "RelativeTimeRangeOutputTypeDef",
     "RelativeTimeRangeTypeDef",
+    "JobExecutionSettingsOutputTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
     "MedicalTranscriptionJobSummaryTypeDef",
     "ListMedicalVocabulariesRequestRequestTypeDef",
     "VocabularyInfoTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
+    "MediaTypeDef",
     "MedicalTranscriptTypeDef",
+    "MedicalTranscriptionSettingOutputTypeDef",
     "MedicalTranscriptionSettingTypeDef",
+    "ModelSettingsOutputTypeDef",
     "ModelSettingsTypeDef",
+    "SettingsOutputTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
     "ToxicityDetectionSettingsTypeDef",
     "SubtitlesOutputTypeDef",
     "ToxicityDetectionSettingsOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
@@ -108,31 +119,33 @@
     "GetMedicalVocabularyResponseTypeDef",
     "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
     "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyResponseTypeDef",
-    "CreateLanguageModelResponseTypeDef",
-    "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateLanguageModelResponseTypeDef",
+    "LanguageModelTypeDef",
+    "InterruptionFilterOutputTypeDef",
+    "NonTalkTimeFilterOutputTypeDef",
+    "SentimentFilterOutputTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
-    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
-    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
     "TranscriptionJobSummaryTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
@@ -153,53 +166,51 @@
     "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
 )
 
+AbsoluteTimeRangeOutputTypeDef = TypedDict(
+    "AbsoluteTimeRangeOutputTypeDef",
+    {
+        "StartTime": int,
+        "EndTime": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionOutputTypeDef = TypedDict(
-    "_RequiredContentRedactionOutputTypeDef",
+ContentRedactionOutputTypeDef = TypedDict(
+    "ContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
-    },
-)
-_OptionalContentRedactionOutputTypeDef = TypedDict(
-    "_OptionalContentRedactionOutputTypeDef",
-    {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
-    total=False,
 )
 
-class ContentRedactionOutputTypeDef(
-    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
-):
-    pass
-
-LanguageIdSettingsTypeDef = TypedDict(
-    "LanguageIdSettingsTypeDef",
+LanguageIdSettingsOutputTypeDef = TypedDict(
+    "LanguageIdSettingsOutputTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
-    total=False,
 )
 
 _RequiredContentRedactionTypeDef = TypedDict(
     "_RequiredContentRedactionTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
@@ -212,52 +223,67 @@
     },
     total=False,
 )
 
 class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
     pass
 
+LanguageIdSettingsTypeDef = TypedDict(
+    "LanguageIdSettingsTypeDef",
+    {
+        "VocabularyName": str,
+        "VocabularyFilterName": str,
+        "LanguageModelName": str,
+    },
+    total=False,
+)
+
 CallAnalyticsJobSummaryTypeDef = TypedDict(
     "CallAnalyticsJobSummaryTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "FailureReason": str,
     },
-    total=False,
 )
 
-ChannelDefinitionTypeDef = TypedDict(
-    "ChannelDefinitionTypeDef",
+ChannelDefinitionOutputTypeDef = TypedDict(
+    "ChannelDefinitionOutputTypeDef",
     {
         "ChannelId": int,
         "ParticipantRole": ParticipantRoleType,
     },
-    total=False,
 )
 
-MediaTypeDef = TypedDict(
-    "MediaTypeDef",
+MediaOutputTypeDef = TypedDict(
+    "MediaOutputTypeDef",
     {
         "MediaFileUri": str,
         "RedactedMediaFileUri": str,
     },
-    total=False,
 )
 
 TranscriptTypeDef = TypedDict(
     "TranscriptTypeDef",
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
     },
+)
+
+ChannelDefinitionTypeDef = TypedDict(
+    "ChannelDefinitionTypeDef",
+    {
+        "ChannelId": int,
+        "ParticipantRole": ParticipantRoleType,
+    },
     total=False,
 )
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
@@ -290,14 +316,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+InputDataConfigOutputTypeDef = TypedDict(
+    "InputDataConfigOutputTypeDef",
+    {
+        "S3Uri": str,
+        "TuningDataS3Uri": str,
+        "DataAccessRoleArn": str,
+    },
+)
+
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -402,25 +437,43 @@
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
+RelativeTimeRangeOutputTypeDef = TypedDict(
+    "RelativeTimeRangeOutputTypeDef",
+    {
+        "StartPercentage": int,
+        "EndPercentage": int,
+        "First": int,
+        "Last": int,
+    },
+)
+
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
+JobExecutionSettingsOutputTypeDef = TypedDict(
+    "JobExecutionSettingsOutputTypeDef",
+    {
+        "AllowDeferredExecution": bool,
+        "DataAccessRoleArn": str,
+    },
+)
+
 JobExecutionSettingsTypeDef = TypedDict(
     "JobExecutionSettingsTypeDef",
     {
         "AllowDeferredExecution": bool,
         "DataAccessRoleArn": str,
     },
     total=False,
@@ -428,15 +481,14 @@
 
 LanguageCodeItemTypeDef = TypedDict(
     "LanguageCodeItemTypeDef",
     {
         "LanguageCode": LanguageCodeType,
         "DurationInSeconds": float,
     },
-    total=False,
 )
 
 ListCallAnalyticsCategoriesRequestRequestTypeDef = TypedDict(
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -488,15 +540,14 @@
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "Specialty": Literal["PRIMARYCARE"],
         "ContentIdentificationType": Literal["PHI"],
         "Type": TypeType,
     },
-    total=False,
 )
 
 ListMedicalVocabulariesRequestRequestTypeDef = TypedDict(
     "ListMedicalVocabulariesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
@@ -510,24 +561,31 @@
     "VocabularyInfoTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
     },
-    total=False,
 )
 
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 ListTranscriptionJobsRequestRequestTypeDef = TypedDict(
     "ListTranscriptionJobsRequestRequestTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "JobNameContains": str,
         "NextToken": str,
         "MaxResults": int,
@@ -559,23 +617,42 @@
 VocabularyFilterInfoTypeDef = TypedDict(
     "VocabularyFilterInfoTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
     },
+)
+
+MediaTypeDef = TypedDict(
+    "MediaTypeDef",
+    {
+        "MediaFileUri": str,
+        "RedactedMediaFileUri": str,
+    },
     total=False,
 )
 
 MedicalTranscriptTypeDef = TypedDict(
     "MedicalTranscriptTypeDef",
     {
         "TranscriptFileUri": str,
     },
-    total=False,
+)
+
+MedicalTranscriptionSettingOutputTypeDef = TypedDict(
+    "MedicalTranscriptionSettingOutputTypeDef",
+    {
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyName": str,
+    },
 )
 
 MedicalTranscriptionSettingTypeDef = TypedDict(
     "MedicalTranscriptionSettingTypeDef",
     {
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
@@ -583,22 +660,43 @@
         "ShowAlternatives": bool,
         "MaxAlternatives": int,
         "VocabularyName": str,
     },
     total=False,
 )
 
+ModelSettingsOutputTypeDef = TypedDict(
+    "ModelSettingsOutputTypeDef",
+    {
+        "LanguageModelName": str,
+    },
+)
+
 ModelSettingsTypeDef = TypedDict(
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
     },
     total=False,
 )
 
+SettingsOutputTypeDef = TypedDict(
+    "SettingsOutputTypeDef",
+    {
+        "VocabularyName": str,
+        "ShowSpeakerLabels": bool,
+        "MaxSpeakerLabels": int,
+        "ChannelIdentification": bool,
+        "ShowAlternatives": bool,
+        "MaxAlternatives": int,
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+    },
+)
+
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
@@ -629,15 +727,14 @@
 SubtitlesOutputTypeDef = TypedDict(
     "SubtitlesOutputTypeDef",
     {
         "Formats": List[SubtitleFormatType],
         "SubtitleFileUris": List[str],
         "OutputStartIndex": int,
     },
-    total=False,
 )
 
 ToxicityDetectionSettingsOutputTypeDef = TypedDict(
     "ToxicityDetectionSettingsOutputTypeDef",
     {
         "ToxicityCategories": List[Literal["ALL"]],
     },
@@ -709,17 +806,16 @@
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
@@ -848,42 +944,14 @@
         "LanguageCode": LanguageCodeType,
         "LastModifiedTime": datetime,
         "VocabularyState": VocabularyStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateLanguageModelResponseTypeDef = TypedDict(
-    "CreateLanguageModelResponseTypeDef",
-    {
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelName": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "ModelStatus": ModelStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-LanguageModelTypeDef = TypedDict(
-    "LanguageModelTypeDef",
-    {
-        "ModelName": str,
-        "CreateTime": datetime,
-        "LastModifiedTime": datetime,
-        "LanguageCode": CLMLanguageCodeType,
-        "BaseModelName": BaseModelNameType,
-        "ModelStatus": ModelStatusType,
-        "UpgradeAvailability": bool,
-        "FailureReason": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateLanguageModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLanguageModelRequestRequestTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelName": str,
         "InputDataConfig": InputDataConfigTypeDef,
@@ -968,117 +1036,134 @@
 )
 
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateLanguageModelResponseTypeDef = TypedDict(
+    "CreateLanguageModelResponseTypeDef",
+    {
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelName": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "ModelStatus": ModelStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+LanguageModelTypeDef = TypedDict(
+    "LanguageModelTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Sequence[TagTypeDef],
+        "ModelName": str,
+        "CreateTime": datetime,
+        "LastModifiedTime": datetime,
+        "LanguageCode": CLMLanguageCodeType,
+        "BaseModelName": BaseModelNameType,
+        "ModelStatus": ModelStatusType,
+        "UpgradeAvailability": bool,
+        "FailureReason": str,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
     },
 )
 
-InterruptionFilterTypeDef = TypedDict(
-    "InterruptionFilterTypeDef",
+InterruptionFilterOutputTypeDef = TypedDict(
+    "InterruptionFilterOutputTypeDef",
     {
         "Threshold": int,
         "ParticipantRole": ParticipantRoleType,
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-NonTalkTimeFilterTypeDef = TypedDict(
-    "NonTalkTimeFilterTypeDef",
+NonTalkTimeFilterOutputTypeDef = TypedDict(
+    "NonTalkTimeFilterOutputTypeDef",
     {
         "Threshold": int,
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "Negate": bool,
     },
-    total=False,
 )
 
-_RequiredSentimentFilterOutputTypeDef = TypedDict(
-    "_RequiredSentimentFilterOutputTypeDef",
+SentimentFilterOutputTypeDef = TypedDict(
+    "SentimentFilterOutputTypeDef",
     {
         "Sentiments": List[SentimentValueType],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
     },
 )
-_OptionalSentimentFilterOutputTypeDef = TypedDict(
-    "_OptionalSentimentFilterOutputTypeDef",
+
+TranscriptFilterOutputTypeDef = TypedDict(
+    "TranscriptFilterOutputTypeDef",
     {
-        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
-        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "TranscriptFilterType": Literal["EXACT"],
+        "AbsoluteTimeRange": AbsoluteTimeRangeOutputTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeOutputTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
+        "Targets": List[str],
     },
-    total=False,
 )
 
-class SentimentFilterOutputTypeDef(
-    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
-):
-    pass
-
-_RequiredSentimentFilterTypeDef = TypedDict(
-    "_RequiredSentimentFilterTypeDef",
+InterruptionFilterTypeDef = TypedDict(
+    "InterruptionFilterTypeDef",
     {
-        "Sentiments": Sequence[SentimentValueType],
+        "Threshold": int,
+        "ParticipantRole": ParticipantRoleType,
+        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "Negate": bool,
     },
+    total=False,
 )
-_OptionalSentimentFilterTypeDef = TypedDict(
-    "_OptionalSentimentFilterTypeDef",
+
+NonTalkTimeFilterTypeDef = TypedDict(
+    "NonTalkTimeFilterTypeDef",
     {
+        "Threshold": int,
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
-        "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
-class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
-    pass
-
-_RequiredTranscriptFilterOutputTypeDef = TypedDict(
-    "_RequiredTranscriptFilterOutputTypeDef",
+_RequiredSentimentFilterTypeDef = TypedDict(
+    "_RequiredSentimentFilterTypeDef",
     {
-        "TranscriptFilterType": Literal["EXACT"],
-        "Targets": List[str],
+        "Sentiments": Sequence[SentimentValueType],
     },
 )
-_OptionalTranscriptFilterOutputTypeDef = TypedDict(
-    "_OptionalTranscriptFilterOutputTypeDef",
+_OptionalSentimentFilterTypeDef = TypedDict(
+    "_OptionalSentimentFilterTypeDef",
     {
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
-class TranscriptFilterOutputTypeDef(
-    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
-):
+class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
     pass
 
 _RequiredTranscriptFilterTypeDef = TypedDict(
     "_RequiredTranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
         "Targets": Sequence[str],
@@ -1124,14 +1209,23 @@
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1141,27 +1235,26 @@
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": MedicalTranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": MedicalTranscriptionSettingTypeDef,
+        "Settings": MedicalTranscriptionSettingOutputTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Specialty": Literal["PRIMARYCARE"],
         "Type": TypeType,
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartMedicalTranscriptionJobRequestRequestTypeDef",
     {
         "MedicalTranscriptionJobName": str,
         "LanguageCode": LanguageCodeType,
@@ -1238,75 +1331,72 @@
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
         "ContentRedaction": ContentRedactionOutputTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
-        "Settings": SettingsTypeDef,
-        "ModelSettings": ModelSettingsTypeDef,
-        "JobExecutionSettings": JobExecutionSettingsTypeDef,
+        "Settings": SettingsOutputTypeDef,
+        "ModelSettings": ModelSettingsOutputTypeDef,
+        "JobExecutionSettings": JobExecutionSettingsOutputTypeDef,
         "ContentRedaction": ContentRedactionOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
-        "Tags": List[TagTypeDef],
+        "Tags": List[TagOutputTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsOutputTypeDef],
         "ToxicityDetection": List[ToxicityDetectionSettingsOutputTypeDef],
     },
-    total=False,
 )
 
 CallAnalyticsJobTypeDef = TypedDict(
     "CallAnalyticsJobTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CallAnalyticsJobStatus": CallAnalyticsJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
         "MediaFormat": MediaFormatType,
-        "Media": MediaTypeDef,
+        "Media": MediaOutputTypeDef,
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
         "Settings": CallAnalyticsJobSettingsOutputTypeDef,
-        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
+        "ChannelDefinitions": List[ChannelDefinitionOutputTypeDef],
     },
-    total=False,
 )
 
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
@@ -1346,20 +1436,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleOutputTypeDef = TypedDict(
     "RuleOutputTypeDef",
     {
-        "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
-        "InterruptionFilter": InterruptionFilterTypeDef,
+        "NonTalkTimeFilter": NonTalkTimeFilterOutputTypeDef,
+        "InterruptionFilter": InterruptionFilterOutputTypeDef,
         "TranscriptFilter": TranscriptFilterOutputTypeDef,
         "SentimentFilter": SentimentFilterOutputTypeDef,
     },
-    total=False,
 )
 
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
@@ -1432,15 +1521,14 @@
     {
         "CategoryName": str,
         "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
-    total=False,
 )
 
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
         "Rules": Sequence[RuleTypeDef],
```

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/PKG-INFO` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transcribe
-Version: 1.28.15
-Summary: Type annotations for boto3.TranscribeService 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.8
+Summary: Type annotations for boto3.TranscribeService 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-transcribe"></a>
 
 # mypy-boto3-transcribe
 
 [![PyPI - mypy-boto3-transcribe](https://img.shields.io/pypi/v/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transcribe.svg?color=blue)](https://pypi.org/project/mypy-boto3-transcribe)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transcribe)](https://pepy.tech/project/mypy-boto3-transcribe)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-transcribe?color=blue)](https://pypistats.org/packages/mypy-boto3-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TranscribeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[boto3.TranscribeService 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-transcribe docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transcribe/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,25 +318,29 @@
 ### Typed dictionaries
 
 `mypy_boto3_transcribe.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_transcribe.type_defs import (
+    AbsoluteTimeRangeOutputTypeDef,
     AbsoluteTimeRangeTypeDef,
     ContentRedactionOutputTypeDef,
-    LanguageIdSettingsTypeDef,
+    LanguageIdSettingsOutputTypeDef,
     ContentRedactionTypeDef,
+    LanguageIdSettingsTypeDef,
     CallAnalyticsJobSummaryTypeDef,
-    ChannelDefinitionTypeDef,
-    MediaTypeDef,
+    ChannelDefinitionOutputTypeDef,
+    MediaOutputTypeDef,
     TranscriptTypeDef,
+    ChannelDefinitionTypeDef,
     ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
+    InputDataConfigOutputTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
@@ -345,32 +349,39 @@
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
     GetVocabularyRequestRequestTypeDef,
+    RelativeTimeRangeOutputTypeDef,
     RelativeTimeRangeTypeDef,
+    JobExecutionSettingsOutputTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
     MedicalTranscriptionJobSummaryTypeDef,
     ListMedicalVocabulariesRequestRequestTypeDef,
     VocabularyInfoTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
+    MediaTypeDef,
     MedicalTranscriptTypeDef,
+    MedicalTranscriptionSettingOutputTypeDef,
     MedicalTranscriptionSettingTypeDef,
+    ModelSettingsOutputTypeDef,
     ModelSettingsTypeDef,
+    SettingsOutputTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     ToxicityDetectionSettingsTypeDef,
     SubtitlesOutputTypeDef,
     ToxicityDetectionSettingsOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
@@ -385,31 +396,33 @@
     GetMedicalVocabularyResponseTypeDef,
     GetVocabularyFilterResponseTypeDef,
     GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
     UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyResponseTypeDef,
-    CreateLanguageModelResponseTypeDef,
-    LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateLanguageModelResponseTypeDef,
+    LanguageModelTypeDef,
+    InterruptionFilterOutputTypeDef,
+    NonTalkTimeFilterOutputTypeDef,
+    SentimentFilterOutputTypeDef,
+    TranscriptFilterOutputTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
-    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
-    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobSummaryTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
@@ -431,15 +444,15 @@
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_structure() -> AbsoluteTimeRangeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-transcribe-1.28.15/mypy_boto3_transcribe.egg-info/SOURCES.txt` & `mypy-boto3-transcribe-1.28.8/mypy_boto3_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-transcribe-1.28.15/setup.py` & `mypy-boto3-transcribe-1.28.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transcribe",
-    version="1.28.15",
+    version="1.28.8",
     packages=["mypy_boto3_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TranscribeService 1.28.15 service generated with"
-        " mypy-boto3-builder 7.16.1"
+        "Type annotations for boto3.TranscribeService 1.28.8 service generated with"
+        " mypy-boto3-builder 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

