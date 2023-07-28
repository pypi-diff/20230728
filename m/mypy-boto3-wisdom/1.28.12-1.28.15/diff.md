# Comparing `tmp/mypy-boto3-wisdom-1.28.12.tar.gz` & `tmp/mypy-boto3-wisdom-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wisdom-1.28.12.tar", last modified: Thu Jul 27 11:49:49 2023, max compression
+gzip compressed data, was "mypy-boto3-wisdom-1.28.15.tar", last modified: Fri Jul 28 20:43:56 2023, max compression
```

## Comparing `mypy-boto3-wisdom-1.28.12.tar` & `mypy-boto3-wisdom-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37471 2023-07-27 11:48:48.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37408 2023-07-27 11:48:47.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17865 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 11:49:49.000000 mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:49.585492 mypy-boto3-wisdom-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:48:46.000000 mypy-boto3-wisdom-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.794043 mypy-boto3-wisdom-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-07-28 20:43:56.790043 mypy-boto3-wisdom-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.782043 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37013 2023-07-28 20:41:31.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-07-28 20:41:30.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:56.790043 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17772 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:56.000000 mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:56.794043 mypy-boto3-wisdom-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:41:29.000000 mypy-boto3-wisdom-1.28.15/setup.py
```

### Comparing `mypy-boto3-wisdom-1.28.12/LICENSE` & `mypy-boto3-wisdom-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/PKG-INFO` & `mypy-boto3-wisdom-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,20 +359,19 @@
 ```python
 from mypy_boto3_wisdom.type_defs import (
     AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     AssistantIntegrationConfigurationTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
     ResponseMetadataTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
     DeleteKnowledgeBaseRequestRequestTypeDef,
@@ -381,15 +380,14 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    RenderingConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
     ListAssistantsRequestRequestTypeDef,
     ListContentsRequestRequestTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
@@ -406,23 +404,23 @@
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
+    CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
-    CreateAssistantRequestRequestTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
     ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
     ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListContentsRequestListContentsPaginateTypeDef,
     ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     QueryAssistantRequestQueryAssistantPaginateTypeDef,
```

### Comparing `mypy-boto3-wisdom-1.28.12/README.md` & `mypy-boto3-wisdom-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,20 +327,19 @@
 ```python
 from mypy_boto3_wisdom.type_defs import (
     AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     AssistantIntegrationConfigurationTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
     ResponseMetadataTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
     DeleteKnowledgeBaseRequestRequestTypeDef,
@@ -349,15 +348,14 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    RenderingConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
     ListAssistantsRequestRequestTypeDef,
     ListContentsRequestRequestTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
@@ -374,23 +372,23 @@
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
+    CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
-    CreateAssistantRequestRequestTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
     ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
     ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListContentsRequestListContentsPaginateTypeDef,
     ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     QueryAssistantRequestQueryAssistantPaginateTypeDef,
```

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__init__.py` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__init__.pyi` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/__main__.py` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectWisdomService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ConnectWisdomService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/client.py` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/client.pyi` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/literals.py` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/literals.pyi` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/paginator.py` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/paginator.pyi` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/type_defs.py` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,19 @@
 
 __all__ = (
     "AppIntegrationsConfigurationOutputTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
     "AssistantIntegrationConfigurationTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
+    "ServerSideEncryptionConfigurationTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
     "ResponseMetadataTypeDef",
-    "ServerSideEncryptionConfigurationTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
     "DeleteKnowledgeBaseRequestRequestTypeDef",
@@ -58,15 +57,14 @@
     "GetAssistantAssociationRequestRequestTypeDef",
     "GetAssistantRequestRequestTypeDef",
     "GetContentRequestRequestTypeDef",
     "GetContentSummaryRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "RenderingConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListAssistantAssociationsRequestRequestTypeDef",
     "ListAssistantsRequestRequestTypeDef",
     "ListContentsRequestRequestTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
@@ -83,23 +81,23 @@
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
+    "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
     "StartContentUploadResponseTypeDef",
     "UpdateContentResponseTypeDef",
-    "CreateAssistantRequestRequestTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
     "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListContentsRequestListContentsPaginateTypeDef",
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "QueryAssistantRequestQueryAssistantPaginateTypeDef",
@@ -200,16 +198,16 @@
     "AssistantIntegrationConfigurationTypeDef",
     {
         "topicIntegrationArn": str,
     },
     total=False,
 )
 
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
+ServerSideEncryptionConfigurationTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
 _RequiredContentDataTypeDef = TypedDict(
@@ -289,22 +287,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ServerSideEncryptionConfigurationTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationTypeDef",
-    {
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
 _RequiredCreateContentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
         "uploadId": str,
     },
@@ -474,22 +464,14 @@
     "GetSessionRequestRequestTypeDef",
     {
         "assistantId": str,
         "sessionId": str,
     },
 )
 
-RenderingConfigurationOutputTypeDef = TypedDict(
-    "RenderingConfigurationOutputTypeDef",
-    {
-        "templateUri": str,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -759,15 +741,15 @@
     },
 )
 _OptionalAssistantDataTypeDef = TypedDict(
     "_OptionalAssistantDataTypeDef",
     {
         "description": str,
         "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class AssistantDataTypeDef(_RequiredAssistantDataTypeDef, _OptionalAssistantDataTypeDef):
@@ -785,25 +767,50 @@
     },
 )
 _OptionalAssistantSummaryTypeDef = TypedDict(
     "_OptionalAssistantSummaryTypeDef",
     {
         "description": str,
         "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class AssistantSummaryTypeDef(_RequiredAssistantSummaryTypeDef, _OptionalAssistantSummaryTypeDef):
     pass
 
 
+_RequiredCreateAssistantRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAssistantRequestRequestTypeDef",
+    {
+        "name": str,
+        "type": Literal["AGENT"],
+    },
+)
+_OptionalCreateAssistantRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAssistantRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "description": str,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateAssistantRequestRequestTypeDef(
+    _RequiredCreateAssistantRequestRequestTypeDef, _OptionalCreateAssistantRequestRequestTypeDef
+):
+    pass
+
+
 CreateContentResponseTypeDef = TypedDict(
     "CreateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -865,39 +872,14 @@
     "UpdateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAssistantRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAssistantRequestRequestTypeDef",
-    {
-        "name": str,
-        "type": Literal["AGENT"],
-    },
-)
-_OptionalCreateAssistantRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAssistantRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "description": str,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateAssistantRequestRequestTypeDef(
-    _RequiredCreateAssistantRequestRequestTypeDef, _OptionalCreateAssistantRequestRequestTypeDef
-):
-    pass
-
-
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
         "text": str,
     },
     total=False,
@@ -1053,16 +1035,16 @@
     },
 )
 _OptionalKnowledgeBaseDataTypeDef = TypedDict(
     "_OptionalKnowledgeBaseDataTypeDef",
     {
         "description": str,
         "lastContentModificationTime": datetime,
-        "renderingConfiguration": RenderingConfigurationOutputTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "renderingConfiguration": RenderingConfigurationTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
@@ -1082,16 +1064,16 @@
         "status": KnowledgeBaseStatusType,
     },
 )
 _OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
     "_OptionalKnowledgeBaseSummaryTypeDef",
     {
         "description": str,
-        "renderingConfiguration": RenderingConfigurationOutputTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "renderingConfiguration": RenderingConfigurationTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
```

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom/type_defs.pyi` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,19 @@
 
 __all__ = (
     "AppIntegrationsConfigurationOutputTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
     "AssistantIntegrationConfigurationTypeDef",
-    "ServerSideEncryptionConfigurationOutputTypeDef",
+    "ServerSideEncryptionConfigurationTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
     "ResponseMetadataTypeDef",
-    "ServerSideEncryptionConfigurationTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
     "DeleteKnowledgeBaseRequestRequestTypeDef",
@@ -57,15 +56,14 @@
     "GetAssistantAssociationRequestRequestTypeDef",
     "GetAssistantRequestRequestTypeDef",
     "GetContentRequestRequestTypeDef",
     "GetContentSummaryRequestRequestTypeDef",
     "GetKnowledgeBaseRequestRequestTypeDef",
     "GetRecommendationsRequestRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "RenderingConfigurationOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListAssistantAssociationsRequestRequestTypeDef",
     "ListAssistantsRequestRequestTypeDef",
     "ListContentsRequestRequestTypeDef",
     "ListKnowledgeBasesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
@@ -82,23 +80,23 @@
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
+    "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
     "StartContentUploadResponseTypeDef",
     "UpdateContentResponseTypeDef",
-    "CreateAssistantRequestRequestTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
     "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListContentsRequestListContentsPaginateTypeDef",
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "QueryAssistantRequestQueryAssistantPaginateTypeDef",
@@ -195,16 +193,16 @@
     "AssistantIntegrationConfigurationTypeDef",
     {
         "topicIntegrationArn": str,
     },
     total=False,
 )
 
-ServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationOutputTypeDef",
+ServerSideEncryptionConfigurationTypeDef = TypedDict(
+    "ServerSideEncryptionConfigurationTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
 
 _RequiredContentDataTypeDef = TypedDict(
@@ -280,22 +278,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ServerSideEncryptionConfigurationTypeDef = TypedDict(
-    "ServerSideEncryptionConfigurationTypeDef",
-    {
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
 _RequiredCreateContentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContentRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "name": str,
         "uploadId": str,
     },
@@ -459,22 +449,14 @@
     "GetSessionRequestRequestTypeDef",
     {
         "assistantId": str,
         "sessionId": str,
     },
 )
 
-RenderingConfigurationOutputTypeDef = TypedDict(
-    "RenderingConfigurationOutputTypeDef",
-    {
-        "templateUri": str,
-    },
-    total=False,
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -734,15 +716,15 @@
     },
 )
 _OptionalAssistantDataTypeDef = TypedDict(
     "_OptionalAssistantDataTypeDef",
     {
         "description": str,
         "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class AssistantDataTypeDef(_RequiredAssistantDataTypeDef, _OptionalAssistantDataTypeDef):
     pass
@@ -758,23 +740,46 @@
     },
 )
 _OptionalAssistantSummaryTypeDef = TypedDict(
     "_OptionalAssistantSummaryTypeDef",
     {
         "description": str,
         "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class AssistantSummaryTypeDef(_RequiredAssistantSummaryTypeDef, _OptionalAssistantSummaryTypeDef):
     pass
 
+_RequiredCreateAssistantRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAssistantRequestRequestTypeDef",
+    {
+        "name": str,
+        "type": Literal["AGENT"],
+    },
+)
+_OptionalCreateAssistantRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAssistantRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "description": str,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateAssistantRequestRequestTypeDef(
+    _RequiredCreateAssistantRequestRequestTypeDef, _OptionalCreateAssistantRequestRequestTypeDef
+):
+    pass
+
 CreateContentResponseTypeDef = TypedDict(
     "CreateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -836,37 +841,14 @@
     "UpdateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAssistantRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAssistantRequestRequestTypeDef",
-    {
-        "name": str,
-        "type": Literal["AGENT"],
-    },
-)
-_OptionalCreateAssistantRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAssistantRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "description": str,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateAssistantRequestRequestTypeDef(
-    _RequiredCreateAssistantRequestRequestTypeDef, _OptionalCreateAssistantRequestRequestTypeDef
-):
-    pass
-
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
         "text": str,
     },
     total=False,
@@ -1014,16 +996,16 @@
     },
 )
 _OptionalKnowledgeBaseDataTypeDef = TypedDict(
     "_OptionalKnowledgeBaseDataTypeDef",
     {
         "description": str,
         "lastContentModificationTime": datetime,
-        "renderingConfiguration": RenderingConfigurationOutputTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "renderingConfiguration": RenderingConfigurationTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class KnowledgeBaseDataTypeDef(
@@ -1041,16 +1023,16 @@
         "status": KnowledgeBaseStatusType,
     },
 )
 _OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
     "_OptionalKnowledgeBaseSummaryTypeDef",
     {
         "description": str,
-        "renderingConfiguration": RenderingConfigurationOutputTypeDef,
-        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationOutputTypeDef,
+        "renderingConfiguration": RenderingConfigurationTypeDef,
+        "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "sourceConfiguration": SourceConfigurationOutputTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class KnowledgeBaseSummaryTypeDef(
```

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/PKG-INFO` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wisdom
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectWisdomService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wisdom.svg?color=blue)](https://pypi.org/project/mypy-boto3-wisdom)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wisdom)](https://pepy.tech/project/mypy-boto3-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectWisdomService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[boto3.ConnectWisdomService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [mypy-boto3-wisdom docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wisdom/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,20 +359,19 @@
 ```python
 from mypy_boto3_wisdom.type_defs import (
     AppIntegrationsConfigurationOutputTypeDef,
     AppIntegrationsConfigurationTypeDef,
     AssistantAssociationInputDataTypeDef,
     KnowledgeBaseAssociationDataTypeDef,
     AssistantIntegrationConfigurationTypeDef,
-    ServerSideEncryptionConfigurationOutputTypeDef,
+    ServerSideEncryptionConfigurationTypeDef,
     ContentDataTypeDef,
     ContentReferenceTypeDef,
     ContentSummaryTypeDef,
     ResponseMetadataTypeDef,
-    ServerSideEncryptionConfigurationTypeDef,
     CreateContentRequestRequestTypeDef,
     RenderingConfigurationTypeDef,
     CreateSessionRequestRequestTypeDef,
     DeleteAssistantAssociationRequestRequestTypeDef,
     DeleteAssistantRequestRequestTypeDef,
     DeleteContentRequestRequestTypeDef,
     DeleteKnowledgeBaseRequestRequestTypeDef,
@@ -381,15 +380,14 @@
     GetAssistantAssociationRequestRequestTypeDef,
     GetAssistantRequestRequestTypeDef,
     GetContentRequestRequestTypeDef,
     GetContentSummaryRequestRequestTypeDef,
     GetKnowledgeBaseRequestRequestTypeDef,
     GetRecommendationsRequestRequestTypeDef,
     GetSessionRequestRequestTypeDef,
-    RenderingConfigurationOutputTypeDef,
     PaginatorConfigTypeDef,
     ListAssistantAssociationsRequestRequestTypeDef,
     ListAssistantsRequestRequestTypeDef,
     ListContentsRequestRequestTypeDef,
     ListKnowledgeBasesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NotifyRecommendationsReceivedErrorTypeDef,
@@ -406,23 +404,23 @@
     UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef,
     SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
     CreateAssistantAssociationRequestRequestTypeDef,
     AssistantAssociationOutputDataTypeDef,
     AssistantDataTypeDef,
     AssistantSummaryTypeDef,
+    CreateAssistantRequestRequestTypeDef,
     CreateContentResponseTypeDef,
     GetContentResponseTypeDef,
     GetContentSummaryResponseTypeDef,
     ListContentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     SearchContentResponseTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
-    CreateAssistantRequestRequestTypeDef,
     DocumentTextTypeDef,
     SearchExpressionTypeDef,
     ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef,
     ListAssistantsRequestListAssistantsPaginateTypeDef,
     ListContentsRequestListContentsPaginateTypeDef,
     ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef,
     QueryAssistantRequestQueryAssistantPaginateTypeDef,
```

### Comparing `mypy-boto3-wisdom-1.28.12/mypy_boto3_wisdom.egg-info/SOURCES.txt` & `mypy-boto3-wisdom-1.28.15/mypy_boto3_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wisdom-1.28.12/setup.py` & `mypy-boto3-wisdom-1.28.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wisdom",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectWisdomService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ConnectWisdomService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

