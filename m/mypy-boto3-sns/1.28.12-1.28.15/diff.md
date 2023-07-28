# Comparing `tmp/mypy-boto3-sns-1.28.12.tar.gz` & `tmp/mypy-boto3-sns-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sns-1.28.12.tar", last modified: Thu Jul 27 11:49:41 2023, max compression
+gzip compressed data, was "mypy-boto3-sns-1.28.15.tar", last modified: Fri Jul 28 20:43:47 2023, max compression
```

## Comparing `mypy-boto3-sns-1.28.12.tar` & `mypy-boto3-sns-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.477319 mypy-boto3-sns-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-07-27 11:49:41.473318 mypy-boto3-sns-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.469318 mypy-boto3-sns-1.28.12/mypy_boto3_sns/
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33161 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33864 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    33795 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34686 2023-07-27 11:47:11.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34639 2023-07-27 11:47:11.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:41.473318 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:41.000000 mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:41.477319 mypy-boto3-sns-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:10.000000 mypy-boto3-sns-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:47.425915 mypy-boto3-sns-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20732 2023-07-28 20:43:47.425915 mypy-boto3-sns-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:47.425915 mypy-boto3-sns-1.28.15/mypy_boto3_sns/
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-07-28 20:39:45.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33161 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-07-28 20:39:45.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-28 20:39:45.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-07-28 20:39:45.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-28 20:39:45.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33864 2023-07-28 20:39:45.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33795 2023-07-28 20:39:45.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34544 2023-07-28 20:39:46.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34497 2023-07-28 20:39:46.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:47.425915 mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20732 2023-07-28 20:43:47.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-28 20:43:47.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:47.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:47.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:47.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:47.000000 mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:47.425915 mypy-boto3-sns-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:39:44.000000 mypy-boto3-sns-1.28.15/setup.py
```

### Comparing `mypy-boto3-sns-1.28.12/LICENSE` & `mypy-boto3-sns-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/PKG-INFO` & `mypy-boto3-sns-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sns
-Version: 1.28.12
-Summary: Type annotations for boto3.SNS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SNS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -470,15 +470,14 @@
     PlatformApplicationTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
     PublishBatchResultEntryTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
@@ -511,14 +510,15 @@
     GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesResponseTypeDef,
     ListPhoneNumbersOptedOutResponseTypeDef,
     PublishResponseTypeDef,
     SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
     ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
     ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
@@ -526,15 +526,14 @@
     ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
     PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
```

### Comparing `mypy-boto3-sns-1.28.12/README.md` & `mypy-boto3-sns-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -438,15 +438,14 @@
     PlatformApplicationTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
     PublishBatchResultEntryTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
@@ -479,14 +478,15 @@
     GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesResponseTypeDef,
     ListPhoneNumbersOptedOutResponseTypeDef,
     PublishResponseTypeDef,
     SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
     ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
     ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
@@ -494,15 +494,14 @@
     ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
     PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
```

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/__init__.py` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/__init__.pyi` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/__main__.py` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SNS 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SNS 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS\nOther"
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

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/client.py` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/client.pyi` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/literals.py` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/literals.pyi` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/paginator.py` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/paginator.pyi` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/service_resource.py` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/service_resource.pyi` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/type_defs.py` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     "PlatformApplicationTypeDef",
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     "SMSSandboxPhoneNumberTypeDef",
     "ListSubscriptionsByTopicInputRequestTypeDef",
     "SubscriptionTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListTopicsInputRequestTypeDef",
     "TopicTypeDef",
     "MessageAttributeValueTypeDef",
     "OptInPhoneNumberInputRequestTypeDef",
     "PublishBatchResultEntryTypeDef",
     "PutDataProtectionPolicyInputRequestTypeDef",
     "RemovePermissionInputRequestTypeDef",
@@ -105,14 +104,15 @@
     "GetSubscriptionAttributesResponseTypeDef",
     "GetTopicAttributesResponseTypeDef",
     "ListPhoneNumbersOptedOutResponseTypeDef",
     "PublishResponseTypeDef",
     "SubscribeResponseTypeDef",
     "CreateTopicInputRequestTypeDef",
     "CreateTopicInputServiceResourceCreateTopicTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEndpointsByPlatformApplicationResponseTypeDef",
     "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
     "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
     "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
     "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
     "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
@@ -120,15 +120,14 @@
     "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "ListTopicsInputListTopicsPaginateTypeDef",
     "ListOriginationNumbersResultTypeDef",
     "ListPlatformApplicationsResponseTypeDef",
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     "ListSubscriptionsByTopicResponseTypeDef",
     "ListSubscriptionsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTopicsResponseTypeDef",
     "PublishBatchRequestEntryTypeDef",
     "PublishInputPlatformEndpointPublishTypeDef",
     "PublishInputRequestTypeDef",
     "PublishInputTopicPublishTypeDef",
     "PublishBatchResponseTypeDef",
     "PublishBatchInputRequestTypeDef",
@@ -555,22 +554,14 @@
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
 ListTopicsInputRequestTypeDef = TypedDict(
     "ListTopicsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -1013,14 +1004,22 @@
 class CreateTopicInputServiceResourceCreateTopicTypeDef(
     _RequiredCreateTopicInputServiceResourceCreateTopicTypeDef,
     _OptionalCreateTopicInputServiceResourceCreateTopicTypeDef,
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
@@ -1167,22 +1166,14 @@
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "NextToken": str,
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
 ListTopicsResponseTypeDef = TypedDict(
     "ListTopicsResponseTypeDef",
     {
         "Topics": List[TopicTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns/type_defs.pyi` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     "PlatformApplicationTypeDef",
     "ListSMSSandboxPhoneNumbersInputRequestTypeDef",
     "SMSSandboxPhoneNumberTypeDef",
     "ListSubscriptionsByTopicInputRequestTypeDef",
     "SubscriptionTypeDef",
     "ListSubscriptionsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListTopicsInputRequestTypeDef",
     "TopicTypeDef",
     "MessageAttributeValueTypeDef",
     "OptInPhoneNumberInputRequestTypeDef",
     "PublishBatchResultEntryTypeDef",
     "PutDataProtectionPolicyInputRequestTypeDef",
     "RemovePermissionInputRequestTypeDef",
@@ -104,14 +103,15 @@
     "GetSubscriptionAttributesResponseTypeDef",
     "GetTopicAttributesResponseTypeDef",
     "ListPhoneNumbersOptedOutResponseTypeDef",
     "PublishResponseTypeDef",
     "SubscribeResponseTypeDef",
     "CreateTopicInputRequestTypeDef",
     "CreateTopicInputServiceResourceCreateTopicTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEndpointsByPlatformApplicationResponseTypeDef",
     "ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef",
     "ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef",
     "ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef",
     "ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef",
     "ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef",
@@ -119,15 +119,14 @@
     "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "ListTopicsInputListTopicsPaginateTypeDef",
     "ListOriginationNumbersResultTypeDef",
     "ListPlatformApplicationsResponseTypeDef",
     "ListSMSSandboxPhoneNumbersResultTypeDef",
     "ListSubscriptionsByTopicResponseTypeDef",
     "ListSubscriptionsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTopicsResponseTypeDef",
     "PublishBatchRequestEntryTypeDef",
     "PublishInputPlatformEndpointPublishTypeDef",
     "PublishInputRequestTypeDef",
     "PublishInputTopicPublishTypeDef",
     "PublishBatchResponseTypeDef",
     "PublishBatchInputRequestTypeDef",
@@ -538,22 +537,14 @@
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
 ListTopicsInputRequestTypeDef = TypedDict(
     "ListTopicsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -978,14 +969,22 @@
 
 class CreateTopicInputServiceResourceCreateTopicTypeDef(
     _RequiredCreateTopicInputServiceResourceCreateTopicTypeDef,
     _OptionalCreateTopicInputServiceResourceCreateTopicTypeDef,
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
@@ -1128,22 +1127,14 @@
     {
         "Subscriptions": List[SubscriptionTypeDef],
         "NextToken": str,
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
 ListTopicsResponseTypeDef = TypedDict(
     "ListTopicsResponseTypeDef",
     {
         "Topics": List[TopicTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/PKG-INFO` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sns
-Version: 1.28.12
-Summary: Type annotations for boto3.SNS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SNS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sns.svg?color=blue)](https://pypi.org/project/mypy-boto3-sns)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-sns)](https://pepy.tech/project/mypy-boto3-sns)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SNS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
+[boto3.SNS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
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
 [mypy-boto3-sns docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sns/).
 
 See how it helps to find and fix potential bugs:
 
@@ -470,15 +470,14 @@
     PlatformApplicationTypeDef,
     ListSMSSandboxPhoneNumbersInputRequestTypeDef,
     SMSSandboxPhoneNumberTypeDef,
     ListSubscriptionsByTopicInputRequestTypeDef,
     SubscriptionTypeDef,
     ListSubscriptionsInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListTopicsInputRequestTypeDef,
     TopicTypeDef,
     MessageAttributeValueTypeDef,
     OptInPhoneNumberInputRequestTypeDef,
     PublishBatchResultEntryTypeDef,
     PutDataProtectionPolicyInputRequestTypeDef,
     RemovePermissionInputRequestTypeDef,
@@ -511,14 +510,15 @@
     GetSubscriptionAttributesResponseTypeDef,
     GetTopicAttributesResponseTypeDef,
     ListPhoneNumbersOptedOutResponseTypeDef,
     PublishResponseTypeDef,
     SubscribeResponseTypeDef,
     CreateTopicInputRequestTypeDef,
     CreateTopicInputServiceResourceCreateTopicTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEndpointsByPlatformApplicationResponseTypeDef,
     ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef,
     ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef,
     ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef,
     ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef,
     ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef,
@@ -526,15 +526,14 @@
     ListSubscriptionsInputListSubscriptionsPaginateTypeDef,
     ListTopicsInputListTopicsPaginateTypeDef,
     ListOriginationNumbersResultTypeDef,
     ListPlatformApplicationsResponseTypeDef,
     ListSMSSandboxPhoneNumbersResultTypeDef,
     ListSubscriptionsByTopicResponseTypeDef,
     ListSubscriptionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTopicsResponseTypeDef,
     PublishBatchRequestEntryTypeDef,
     PublishInputPlatformEndpointPublishTypeDef,
     PublishInputRequestTypeDef,
     PublishInputTopicPublishTypeDef,
     PublishBatchResponseTypeDef,
     PublishBatchInputRequestTypeDef,
```

### Comparing `mypy-boto3-sns-1.28.12/mypy_boto3_sns.egg-info/SOURCES.txt` & `mypy-boto3-sns-1.28.15/mypy_boto3_sns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sns-1.28.12/setup.py` & `mypy-boto3-sns-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sns",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_sns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SNS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SNS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

