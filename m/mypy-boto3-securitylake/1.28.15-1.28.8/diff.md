# Comparing `tmp/mypy-boto3-securitylake-1.28.15.tar.gz` & `tmp/mypy-boto3-securitylake-1.28.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securitylake-1.28.15.tar", last modified: Fri Jul 28 20:43:43 2023, max compression
+gzip compressed data, was "mypy-boto3-securitylake-1.28.8.tar", last modified: Thu Jul 20 19:47:57 2023, max compression
```

## Comparing `mypy-boto3-securitylake-1.28.15.tar` & `mypy-boto3-securitylake-1.28.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:43.001854 mypy-boto3-securitylake-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-07-28 20:43:42.997854 mypy-boto3-securitylake-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15394 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:42.993854 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-07-28 20:39:04.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-07-28 20:39:04.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-28 20:39:04.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-28 20:39:04.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-28 20:39:04.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26354 2023-07-28 20:39:05.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26329 2023-07-28 20:39:04.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:42.997854 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-07-28 20:43:42.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:43:42.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:42.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:42.000000 mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:43.001854 mypy-boto3-securitylake-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:39:03.000000 mypy-boto3-securitylake-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26036 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-20 19:47:42.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27940 2023-07-20 19:47:43.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27919 2023-07-20 19:47:43.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17317 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 19:47:57.000000 mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:47:57.872787 mypy-boto3-securitylake-1.28.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-20 19:47:41.000000 mypy-boto3-securitylake-1.28.8/setup.py
```

### Comparing `mypy-boto3-securitylake-1.28.15/LICENSE` & `mypy-boto3-securitylake-1.28.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.15/PKG-INFO` & `mypy-boto3-securitylake-1.28.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securitylake
-Version: 1.28.15
-Summary: Type annotations for boto3.SecurityLake 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.8
+Summary: Type annotations for boto3.SecurityLake 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-securitylake"></a>
 
 # mypy-boto3-securitylake
 
 [![PyPI - mypy-boto3-securitylake](https://img.shields.io/pypi/v/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securitylake)](https://pepy.tech/project/mypy-boto3-securitylake)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,26 +340,33 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
+    AwsIdentityOutputTypeDef,
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceOutputTypeDef,
     AwsLogSourceResourceTypeDef,
     ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     TagTypeDef,
+    CustomLogSourceAttributesOutputTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderOutputTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
+    DataLakeEncryptionConfigurationOutputTypeDef,
     DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationOutputTypeDef,
+    DataLakeLifecycleTransitionOutputTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
     DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
@@ -369,70 +376,73 @@
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
     ListSubscribersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
     DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateSubscriberNotificationResponseTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
     GetDataLakeExceptionSubscriptionResponseTypeDef,
     UpdateSubscriberNotificationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceOutputTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
     DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
     GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
     ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
     DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
+    LogSourceResourceOutputTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    LogSourceTypeDef,
+    SubscriberResourceTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
-    LogSourceTypeDef,
-    SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
     UpdateDataLakeRequestRequestTypeDef,
     CreateDataLakeResponseTypeDef,
     ListDataLakesResponseTypeDef,
     UpdateDataLakeResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_structure() -> AwsIdentityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securitylake-1.28.15/README.md` & `mypy-boto3-securitylake-1.28.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-securitylake"></a>
 
 # mypy-boto3-securitylake
 
 [![PyPI - mypy-boto3-securitylake](https://img.shields.io/pypi/v/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securitylake)](https://pepy.tech/project/mypy-boto3-securitylake)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -308,26 +308,33 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
+    AwsIdentityOutputTypeDef,
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceOutputTypeDef,
     AwsLogSourceResourceTypeDef,
     ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     TagTypeDef,
+    CustomLogSourceAttributesOutputTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderOutputTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
+    DataLakeEncryptionConfigurationOutputTypeDef,
     DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationOutputTypeDef,
+    DataLakeLifecycleTransitionOutputTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
     DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
@@ -337,70 +344,73 @@
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
     ListSubscribersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
     DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateSubscriberNotificationResponseTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
     GetDataLakeExceptionSubscriptionResponseTypeDef,
     UpdateSubscriberNotificationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceOutputTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
     DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
     GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
     ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
     DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
+    LogSourceResourceOutputTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    LogSourceTypeDef,
+    SubscriberResourceTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
-    LogSourceTypeDef,
-    SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
     UpdateDataLakeRequestRequestTypeDef,
     CreateDataLakeResponseTypeDef,
     ListDataLakesResponseTypeDef,
     UpdateDataLakeResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_structure() -> AwsIdentityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/__init__.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/__init__.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/__main__.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityLake 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.SecurityLake 1.28.8\nVersion:         1.28.8\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake\nOther"
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

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/client.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/client.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/literals.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,14 @@
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
@@ -253,15 +252,14 @@
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

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/literals.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,14 @@
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
@@ -251,15 +250,14 @@
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

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/paginator.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/paginator.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/type_defs.py` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for securitylake service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_securitylake.type_defs import AwsIdentityTypeDef
+    from mypy_boto3_securitylake.type_defs import AwsIdentityOutputTypeDef
 
-    data: AwsIdentityTypeDef = {...}
+    data: AwsIdentityOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -27,26 +27,33 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AwsIdentityOutputTypeDef",
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
+    "AwsLogSourceResourceOutputTypeDef",
     "AwsLogSourceResourceTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     "TagTypeDef",
+    "CustomLogSourceAttributesOutputTypeDef",
     "CustomLogSourceAttributesTypeDef",
     "CustomLogSourceCrawlerConfigurationTypeDef",
+    "CustomLogSourceProviderOutputTypeDef",
     "CustomLogSourceProviderTypeDef",
     "DataLakeEncryptionConfigurationTypeDef",
     "DataLakeReplicationConfigurationTypeDef",
+    "DataLakeEncryptionConfigurationOutputTypeDef",
     "DataLakeExceptionTypeDef",
+    "DataLakeLifecycleExpirationOutputTypeDef",
+    "DataLakeLifecycleTransitionOutputTypeDef",
     "DataLakeLifecycleExpirationTypeDef",
     "DataLakeLifecycleTransitionTypeDef",
     "DataLakeReplicationConfigurationOutputTypeDef",
     "DataLakeSourceStatusTypeDef",
     "DataLakeUpdateExceptionTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
     "DeleteDataLakeRequestRequestTypeDef",
@@ -56,68 +63,79 @@
     "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
     "HttpsNotificationConfigurationTypeDef",
     "ListDataLakeExceptionsRequestRequestTypeDef",
     "ListDataLakesRequestRequestTypeDef",
     "ListSubscribersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     "CreateAwsLogSourceRequestRequestTypeDef",
     "DeleteAwsLogSourceRequestRequestTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     "CreateAwsLogSourceResponseTypeDef",
     "CreateSubscriberNotificationResponseTypeDef",
     "DeleteAwsLogSourceResponseTypeDef",
     "GetDataLakeExceptionSubscriptionResponseTypeDef",
     "UpdateSubscriberNotificationResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomLogSourceConfigurationTypeDef",
+    "CustomLogSourceResourceOutputTypeDef",
     "CustomLogSourceResourceTypeDef",
     "ListDataLakeExceptionsResponseTypeDef",
     "DataLakeLifecycleConfigurationOutputTypeDef",
     "DataLakeLifecycleConfigurationTypeDef",
     "DataLakeSourceTypeDef",
     "DataLakeUpdateStatusTypeDef",
     "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "NotificationConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
     "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
+    "LogSourceResourceOutputTypeDef",
     "LogSourceResourceTypeDef",
     "DataLakeConfigurationTypeDef",
     "GetDataLakeSourcesResponseTypeDef",
     "DataLakeResourceTypeDef",
     "CreateSubscriberNotificationRequestRequestTypeDef",
     "UpdateSubscriberNotificationRequestRequestTypeDef",
+    "LogSourceTypeDef",
+    "SubscriberResourceTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     "ListLogSourcesRequestRequestTypeDef",
-    "LogSourceTypeDef",
-    "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CreateDataLakeRequestRequestTypeDef",
     "UpdateDataLakeRequestRequestTypeDef",
     "CreateDataLakeResponseTypeDef",
     "ListDataLakesResponseTypeDef",
     "UpdateDataLakeResponseTypeDef",
     "ListLogSourcesResponseTypeDef",
     "CreateSubscriberResponseTypeDef",
     "GetSubscriberResponseTypeDef",
     "ListSubscribersResponseTypeDef",
     "UpdateSubscriberResponseTypeDef",
 )
 
+AwsIdentityOutputTypeDef = TypedDict(
+    "AwsIdentityOutputTypeDef",
+    {
+        "externalId": str,
+        "principal": str,
+    },
+)
+
 AwsIdentityTypeDef = TypedDict(
     "AwsIdentityTypeDef",
     {
         "externalId": str,
         "principal": str,
     },
 )
@@ -141,14 +159,22 @@
 
 class AwsLogSourceConfigurationTypeDef(
     _RequiredAwsLogSourceConfigurationTypeDef, _OptionalAwsLogSourceConfigurationTypeDef
 ):
     pass
 
 
+AwsLogSourceResourceOutputTypeDef = TypedDict(
+    "AwsLogSourceResourceOutputTypeDef",
+    {
+        "sourceName": AwsLogSourceNameType,
+        "sourceVersion": str,
+    },
+)
+
 AwsLogSourceResourceTypeDef = TypedDict(
     "AwsLogSourceResourceTypeDef",
     {
         "sourceName": AwsLogSourceNameType,
         "sourceVersion": str,
     },
     total=False,
@@ -192,14 +218,23 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+CustomLogSourceAttributesOutputTypeDef = TypedDict(
+    "CustomLogSourceAttributesOutputTypeDef",
+    {
+        "crawlerArn": str,
+        "databaseArn": str,
+        "tableArn": str,
+    },
+)
+
 CustomLogSourceAttributesTypeDef = TypedDict(
     "CustomLogSourceAttributesTypeDef",
     {
         "crawlerArn": str,
         "databaseArn": str,
         "tableArn": str,
     },
@@ -209,14 +244,22 @@
 CustomLogSourceCrawlerConfigurationTypeDef = TypedDict(
     "CustomLogSourceCrawlerConfigurationTypeDef",
     {
         "roleArn": str,
     },
 )
 
+CustomLogSourceProviderOutputTypeDef = TypedDict(
+    "CustomLogSourceProviderOutputTypeDef",
+    {
+        "location": str,
+        "roleArn": str,
+    },
+)
+
 CustomLogSourceProviderTypeDef = TypedDict(
     "CustomLogSourceProviderTypeDef",
     {
         "location": str,
         "roleArn": str,
     },
     total=False,
@@ -235,23 +278,44 @@
     {
         "regions": Sequence[str],
         "roleArn": str,
     },
     total=False,
 )
 
+DataLakeEncryptionConfigurationOutputTypeDef = TypedDict(
+    "DataLakeEncryptionConfigurationOutputTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+)
+
 DataLakeExceptionTypeDef = TypedDict(
     "DataLakeExceptionTypeDef",
     {
         "exception": str,
         "region": str,
         "remediation": str,
         "timestamp": datetime,
     },
-    total=False,
+)
+
+DataLakeLifecycleExpirationOutputTypeDef = TypedDict(
+    "DataLakeLifecycleExpirationOutputTypeDef",
+    {
+        "days": int,
+    },
+)
+
+DataLakeLifecycleTransitionOutputTypeDef = TypedDict(
+    "DataLakeLifecycleTransitionOutputTypeDef",
+    {
+        "days": int,
+        "storageClass": str,
+    },
 )
 
 DataLakeLifecycleExpirationTypeDef = TypedDict(
     "DataLakeLifecycleExpirationTypeDef",
     {
         "days": int,
     },
@@ -269,33 +333,30 @@
 
 DataLakeReplicationConfigurationOutputTypeDef = TypedDict(
     "DataLakeReplicationConfigurationOutputTypeDef",
     {
         "regions": List[str],
         "roleArn": str,
     },
-    total=False,
 )
 
 DataLakeSourceStatusTypeDef = TypedDict(
     "DataLakeSourceStatusTypeDef",
     {
         "resource": str,
         "status": SourceCollectionStatusType,
     },
-    total=False,
 )
 
 DataLakeUpdateExceptionTypeDef = TypedDict(
     "DataLakeUpdateExceptionTypeDef",
     {
         "code": str,
         "reason": str,
     },
-    total=False,
 )
 
 _RequiredDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
@@ -418,14 +479,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
@@ -474,15 +543,15 @@
     },
 )
 
 DataLakeAutoEnableNewAccountConfigurationOutputTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     {
         "region": str,
-        "sources": List[AwsLogSourceResourceTypeDef],
+        "sources": List[AwsLogSourceResourceOutputTypeDef],
     },
 )
 
 DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     {
         "region": str,
@@ -528,22 +597,14 @@
     "UpdateSubscriberNotificationResponseTypeDef",
     {
         "subscriberEndpoint": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -552,14 +613,24 @@
     "CustomLogSourceConfigurationTypeDef",
     {
         "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
         "providerIdentity": AwsIdentityTypeDef,
     },
 )
 
+CustomLogSourceResourceOutputTypeDef = TypedDict(
+    "CustomLogSourceResourceOutputTypeDef",
+    {
+        "attributes": CustomLogSourceAttributesOutputTypeDef,
+        "provider": CustomLogSourceProviderOutputTypeDef,
+        "sourceName": str,
+        "sourceVersion": str,
+    },
+)
+
 CustomLogSourceResourceTypeDef = TypedDict(
     "CustomLogSourceResourceTypeDef",
     {
         "attributes": CustomLogSourceAttributesTypeDef,
         "provider": CustomLogSourceProviderTypeDef,
         "sourceName": str,
         "sourceVersion": str,
@@ -575,18 +646,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataLakeLifecycleConfigurationOutputTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationOutputTypeDef",
     {
-        "expiration": DataLakeLifecycleExpirationTypeDef,
-        "transitions": List[DataLakeLifecycleTransitionTypeDef],
+        "expiration": DataLakeLifecycleExpirationOutputTypeDef,
+        "transitions": List[DataLakeLifecycleTransitionOutputTypeDef],
     },
-    total=False,
 )
 
 DataLakeLifecycleConfigurationTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationTypeDef",
     {
         "expiration": DataLakeLifecycleExpirationTypeDef,
         "transitions": Sequence[DataLakeLifecycleTransitionTypeDef],
@@ -598,25 +668,23 @@
     "DataLakeSourceTypeDef",
     {
         "account": str,
         "eventClasses": List[str],
         "sourceName": str,
         "sourceStatuses": List[DataLakeSourceStatusTypeDef],
     },
-    total=False,
 )
 
 DataLakeUpdateStatusTypeDef = TypedDict(
     "DataLakeUpdateStatusTypeDef",
     {
         "exception": DataLakeUpdateExceptionTypeDef,
         "requestId": str,
         "status": DataLakeStatusType,
     },
-    total=False,
 )
 
 GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
     "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     {
         "accounts": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -646,14 +714,22 @@
     {
         "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
         "sqsNotificationConfiguration": Mapping[str, Any],
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
     {
         "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -695,19 +771,27 @@
 ):
     pass
 
 
 CreateCustomLogSourceResponseTypeDef = TypedDict(
     "CreateCustomLogSourceResponseTypeDef",
     {
-        "source": CustomLogSourceResourceTypeDef,
+        "source": CustomLogSourceResourceOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LogSourceResourceOutputTypeDef = TypedDict(
+    "LogSourceResourceOutputTypeDef",
+    {
+        "awsLogSource": AwsLogSourceResourceOutputTypeDef,
+        "customLogSource": CustomLogSourceResourceOutputTypeDef,
+    },
+)
+
 LogSourceResourceTypeDef = TypedDict(
     "LogSourceResourceTypeDef",
     {
         "awsLogSource": AwsLogSourceResourceTypeDef,
         "customLogSource": CustomLogSourceResourceTypeDef,
     },
     total=False,
@@ -742,39 +826,28 @@
         "dataLakeArn": str,
         "dataLakeSources": List[DataLakeSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDataLakeResourceTypeDef = TypedDict(
-    "_RequiredDataLakeResourceTypeDef",
-    {
-        "dataLakeArn": str,
-        "region": str,
-    },
-)
-_OptionalDataLakeResourceTypeDef = TypedDict(
-    "_OptionalDataLakeResourceTypeDef",
+DataLakeResourceTypeDef = TypedDict(
+    "DataLakeResourceTypeDef",
     {
         "createStatus": DataLakeStatusType,
-        "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
+        "dataLakeArn": str,
+        "encryptionConfiguration": DataLakeEncryptionConfigurationOutputTypeDef,
         "lifecycleConfiguration": DataLakeLifecycleConfigurationOutputTypeDef,
+        "region": str,
         "replicationConfiguration": DataLakeReplicationConfigurationOutputTypeDef,
         "s3BucketArn": str,
         "updateStatus": DataLakeUpdateStatusTypeDef,
     },
-    total=False,
 )
 
-
-class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
-    pass
-
-
 CreateSubscriberNotificationRequestRequestTypeDef = TypedDict(
     "CreateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
@@ -783,14 +856,44 @@
     "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
 
+LogSourceTypeDef = TypedDict(
+    "LogSourceTypeDef",
+    {
+        "account": str,
+        "region": str,
+        "sources": List[LogSourceResourceOutputTypeDef],
+    },
+)
+
+SubscriberResourceTypeDef = TypedDict(
+    "SubscriberResourceTypeDef",
+    {
+        "accessTypes": List[AccessTypeType],
+        "createdAt": datetime,
+        "resourceShareArn": str,
+        "resourceShareName": str,
+        "roleArn": str,
+        "s3BucketArn": str,
+        "sources": List[LogSourceResourceOutputTypeDef],
+        "subscriberArn": str,
+        "subscriberDescription": str,
+        "subscriberEndpoint": str,
+        "subscriberId": str,
+        "subscriberIdentity": AwsIdentityOutputTypeDef,
+        "subscriberName": str,
+        "subscriberStatus": SubscriberStatusType,
+        "updatedAt": datetime,
+    },
+)
+
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
         "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
@@ -831,58 +934,14 @@
         "nextToken": str,
         "regions": Sequence[str],
         "sources": Sequence[LogSourceResourceTypeDef],
     },
     total=False,
 )
 
-LogSourceTypeDef = TypedDict(
-    "LogSourceTypeDef",
-    {
-        "account": str,
-        "region": str,
-        "sources": List[LogSourceResourceTypeDef],
-    },
-    total=False,
-)
-
-_RequiredSubscriberResourceTypeDef = TypedDict(
-    "_RequiredSubscriberResourceTypeDef",
-    {
-        "sources": List[LogSourceResourceTypeDef],
-        "subscriberArn": str,
-        "subscriberId": str,
-        "subscriberIdentity": AwsIdentityTypeDef,
-        "subscriberName": str,
-    },
-)
-_OptionalSubscriberResourceTypeDef = TypedDict(
-    "_OptionalSubscriberResourceTypeDef",
-    {
-        "accessTypes": List[AccessTypeType],
-        "createdAt": datetime,
-        "resourceShareArn": str,
-        "resourceShareName": str,
-        "roleArn": str,
-        "s3BucketArn": str,
-        "subscriberDescription": str,
-        "subscriberEndpoint": str,
-        "subscriberStatus": SubscriberStatusType,
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-
-class SubscriberResourceTypeDef(
-    _RequiredSubscriberResourceTypeDef, _OptionalSubscriberResourceTypeDef
-):
-    pass
-
-
 _RequiredUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 _OptionalUpdateSubscriberRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake/type_defs.pyi` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for securitylake service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_securitylake.type_defs import AwsIdentityTypeDef
+    from mypy_boto3_securitylake.type_defs import AwsIdentityOutputTypeDef
 
-    data: AwsIdentityTypeDef = {...}
+    data: AwsIdentityOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -26,26 +26,33 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AwsIdentityOutputTypeDef",
     "AwsIdentityTypeDef",
     "AwsLogSourceConfigurationTypeDef",
+    "AwsLogSourceResourceOutputTypeDef",
     "AwsLogSourceResourceTypeDef",
     "ResponseMetadataTypeDef",
     "CreateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     "TagTypeDef",
+    "CustomLogSourceAttributesOutputTypeDef",
     "CustomLogSourceAttributesTypeDef",
     "CustomLogSourceCrawlerConfigurationTypeDef",
+    "CustomLogSourceProviderOutputTypeDef",
     "CustomLogSourceProviderTypeDef",
     "DataLakeEncryptionConfigurationTypeDef",
     "DataLakeReplicationConfigurationTypeDef",
+    "DataLakeEncryptionConfigurationOutputTypeDef",
     "DataLakeExceptionTypeDef",
+    "DataLakeLifecycleExpirationOutputTypeDef",
+    "DataLakeLifecycleTransitionOutputTypeDef",
     "DataLakeLifecycleExpirationTypeDef",
     "DataLakeLifecycleTransitionTypeDef",
     "DataLakeReplicationConfigurationOutputTypeDef",
     "DataLakeSourceStatusTypeDef",
     "DataLakeUpdateExceptionTypeDef",
     "DeleteCustomLogSourceRequestRequestTypeDef",
     "DeleteDataLakeRequestRequestTypeDef",
@@ -55,68 +62,79 @@
     "GetDataLakeSourcesRequestRequestTypeDef",
     "GetSubscriberRequestRequestTypeDef",
     "HttpsNotificationConfigurationTypeDef",
     "ListDataLakeExceptionsRequestRequestTypeDef",
     "ListDataLakesRequestRequestTypeDef",
     "ListSubscribersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "TagOutputTypeDef",
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef",
     "CreateAwsLogSourceRequestRequestTypeDef",
     "DeleteAwsLogSourceRequestRequestTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     "CreateAwsLogSourceResponseTypeDef",
     "CreateSubscriberNotificationResponseTypeDef",
     "DeleteAwsLogSourceResponseTypeDef",
     "GetDataLakeExceptionSubscriptionResponseTypeDef",
     "UpdateSubscriberNotificationResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomLogSourceConfigurationTypeDef",
+    "CustomLogSourceResourceOutputTypeDef",
     "CustomLogSourceResourceTypeDef",
     "ListDataLakeExceptionsResponseTypeDef",
     "DataLakeLifecycleConfigurationOutputTypeDef",
     "DataLakeLifecycleConfigurationTypeDef",
     "DataLakeSourceTypeDef",
     "DataLakeUpdateStatusTypeDef",
     "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     "ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef",
     "ListSubscribersRequestListSubscribersPaginateTypeDef",
     "NotificationConfigurationTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
     "CreateDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef",
     "CreateCustomLogSourceRequestRequestTypeDef",
     "CreateCustomLogSourceResponseTypeDef",
+    "LogSourceResourceOutputTypeDef",
     "LogSourceResourceTypeDef",
     "DataLakeConfigurationTypeDef",
     "GetDataLakeSourcesResponseTypeDef",
     "DataLakeResourceTypeDef",
     "CreateSubscriberNotificationRequestRequestTypeDef",
     "UpdateSubscriberNotificationRequestRequestTypeDef",
+    "LogSourceTypeDef",
+    "SubscriberResourceTypeDef",
     "CreateSubscriberRequestRequestTypeDef",
     "ListLogSourcesRequestListLogSourcesPaginateTypeDef",
     "ListLogSourcesRequestRequestTypeDef",
-    "LogSourceTypeDef",
-    "SubscriberResourceTypeDef",
     "UpdateSubscriberRequestRequestTypeDef",
     "CreateDataLakeRequestRequestTypeDef",
     "UpdateDataLakeRequestRequestTypeDef",
     "CreateDataLakeResponseTypeDef",
     "ListDataLakesResponseTypeDef",
     "UpdateDataLakeResponseTypeDef",
     "ListLogSourcesResponseTypeDef",
     "CreateSubscriberResponseTypeDef",
     "GetSubscriberResponseTypeDef",
     "ListSubscribersResponseTypeDef",
     "UpdateSubscriberResponseTypeDef",
 )
 
+AwsIdentityOutputTypeDef = TypedDict(
+    "AwsIdentityOutputTypeDef",
+    {
+        "externalId": str,
+        "principal": str,
+    },
+)
+
 AwsIdentityTypeDef = TypedDict(
     "AwsIdentityTypeDef",
     {
         "externalId": str,
         "principal": str,
     },
 )
@@ -138,14 +156,22 @@
 )
 
 class AwsLogSourceConfigurationTypeDef(
     _RequiredAwsLogSourceConfigurationTypeDef, _OptionalAwsLogSourceConfigurationTypeDef
 ):
     pass
 
+AwsLogSourceResourceOutputTypeDef = TypedDict(
+    "AwsLogSourceResourceOutputTypeDef",
+    {
+        "sourceName": AwsLogSourceNameType,
+        "sourceVersion": str,
+    },
+)
+
 AwsLogSourceResourceTypeDef = TypedDict(
     "AwsLogSourceResourceTypeDef",
     {
         "sourceName": AwsLogSourceNameType,
         "sourceVersion": str,
     },
     total=False,
@@ -187,14 +213,23 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+CustomLogSourceAttributesOutputTypeDef = TypedDict(
+    "CustomLogSourceAttributesOutputTypeDef",
+    {
+        "crawlerArn": str,
+        "databaseArn": str,
+        "tableArn": str,
+    },
+)
+
 CustomLogSourceAttributesTypeDef = TypedDict(
     "CustomLogSourceAttributesTypeDef",
     {
         "crawlerArn": str,
         "databaseArn": str,
         "tableArn": str,
     },
@@ -204,14 +239,22 @@
 CustomLogSourceCrawlerConfigurationTypeDef = TypedDict(
     "CustomLogSourceCrawlerConfigurationTypeDef",
     {
         "roleArn": str,
     },
 )
 
+CustomLogSourceProviderOutputTypeDef = TypedDict(
+    "CustomLogSourceProviderOutputTypeDef",
+    {
+        "location": str,
+        "roleArn": str,
+    },
+)
+
 CustomLogSourceProviderTypeDef = TypedDict(
     "CustomLogSourceProviderTypeDef",
     {
         "location": str,
         "roleArn": str,
     },
     total=False,
@@ -230,23 +273,44 @@
     {
         "regions": Sequence[str],
         "roleArn": str,
     },
     total=False,
 )
 
+DataLakeEncryptionConfigurationOutputTypeDef = TypedDict(
+    "DataLakeEncryptionConfigurationOutputTypeDef",
+    {
+        "kmsKeyId": str,
+    },
+)
+
 DataLakeExceptionTypeDef = TypedDict(
     "DataLakeExceptionTypeDef",
     {
         "exception": str,
         "region": str,
         "remediation": str,
         "timestamp": datetime,
     },
-    total=False,
+)
+
+DataLakeLifecycleExpirationOutputTypeDef = TypedDict(
+    "DataLakeLifecycleExpirationOutputTypeDef",
+    {
+        "days": int,
+    },
+)
+
+DataLakeLifecycleTransitionOutputTypeDef = TypedDict(
+    "DataLakeLifecycleTransitionOutputTypeDef",
+    {
+        "days": int,
+        "storageClass": str,
+    },
 )
 
 DataLakeLifecycleExpirationTypeDef = TypedDict(
     "DataLakeLifecycleExpirationTypeDef",
     {
         "days": int,
     },
@@ -264,33 +328,30 @@
 
 DataLakeReplicationConfigurationOutputTypeDef = TypedDict(
     "DataLakeReplicationConfigurationOutputTypeDef",
     {
         "regions": List[str],
         "roleArn": str,
     },
-    total=False,
 )
 
 DataLakeSourceStatusTypeDef = TypedDict(
     "DataLakeSourceStatusTypeDef",
     {
         "resource": str,
         "status": SourceCollectionStatusType,
     },
-    total=False,
 )
 
 DataLakeUpdateExceptionTypeDef = TypedDict(
     "DataLakeUpdateExceptionTypeDef",
     {
         "code": str,
         "reason": str,
     },
-    total=False,
 )
 
 _RequiredDeleteCustomLogSourceRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteCustomLogSourceRequestRequestTypeDef",
     {
         "sourceName": str,
     },
@@ -409,14 +470,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+TagOutputTypeDef = TypedDict(
+    "TagOutputTypeDef",
+    {
+        "key": str,
+        "value": str,
+    },
+)
+
 RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef = TypedDict(
     "RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
@@ -463,15 +532,15 @@
     },
 )
 
 DataLakeAutoEnableNewAccountConfigurationOutputTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationOutputTypeDef",
     {
         "region": str,
-        "sources": List[AwsLogSourceResourceTypeDef],
+        "sources": List[AwsLogSourceResourceOutputTypeDef],
     },
 )
 
 DataLakeAutoEnableNewAccountConfigurationTypeDef = TypedDict(
     "DataLakeAutoEnableNewAccountConfigurationTypeDef",
     {
         "region": str,
@@ -517,22 +586,14 @@
     "UpdateSubscriberNotificationResponseTypeDef",
     {
         "subscriberEndpoint": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -541,14 +602,24 @@
     "CustomLogSourceConfigurationTypeDef",
     {
         "crawlerConfiguration": CustomLogSourceCrawlerConfigurationTypeDef,
         "providerIdentity": AwsIdentityTypeDef,
     },
 )
 
+CustomLogSourceResourceOutputTypeDef = TypedDict(
+    "CustomLogSourceResourceOutputTypeDef",
+    {
+        "attributes": CustomLogSourceAttributesOutputTypeDef,
+        "provider": CustomLogSourceProviderOutputTypeDef,
+        "sourceName": str,
+        "sourceVersion": str,
+    },
+)
+
 CustomLogSourceResourceTypeDef = TypedDict(
     "CustomLogSourceResourceTypeDef",
     {
         "attributes": CustomLogSourceAttributesTypeDef,
         "provider": CustomLogSourceProviderTypeDef,
         "sourceName": str,
         "sourceVersion": str,
@@ -564,18 +635,17 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataLakeLifecycleConfigurationOutputTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationOutputTypeDef",
     {
-        "expiration": DataLakeLifecycleExpirationTypeDef,
-        "transitions": List[DataLakeLifecycleTransitionTypeDef],
+        "expiration": DataLakeLifecycleExpirationOutputTypeDef,
+        "transitions": List[DataLakeLifecycleTransitionOutputTypeDef],
     },
-    total=False,
 )
 
 DataLakeLifecycleConfigurationTypeDef = TypedDict(
     "DataLakeLifecycleConfigurationTypeDef",
     {
         "expiration": DataLakeLifecycleExpirationTypeDef,
         "transitions": Sequence[DataLakeLifecycleTransitionTypeDef],
@@ -587,25 +657,23 @@
     "DataLakeSourceTypeDef",
     {
         "account": str,
         "eventClasses": List[str],
         "sourceName": str,
         "sourceStatuses": List[DataLakeSourceStatusTypeDef],
     },
-    total=False,
 )
 
 DataLakeUpdateStatusTypeDef = TypedDict(
     "DataLakeUpdateStatusTypeDef",
     {
         "exception": DataLakeUpdateExceptionTypeDef,
         "requestId": str,
         "status": DataLakeStatusType,
     },
-    total=False,
 )
 
 GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef = TypedDict(
     "GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef",
     {
         "accounts": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -635,14 +703,22 @@
     {
         "httpsNotificationConfiguration": HttpsNotificationConfigurationTypeDef,
         "sqsNotificationConfiguration": Mapping[str, Any],
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetDataLakeOrganizationConfigurationResponseTypeDef = TypedDict(
     "GetDataLakeOrganizationConfigurationResponseTypeDef",
     {
         "autoEnableNewAccount": List[DataLakeAutoEnableNewAccountConfigurationOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -682,19 +758,27 @@
     _OptionalCreateCustomLogSourceRequestRequestTypeDef,
 ):
     pass
 
 CreateCustomLogSourceResponseTypeDef = TypedDict(
     "CreateCustomLogSourceResponseTypeDef",
     {
-        "source": CustomLogSourceResourceTypeDef,
+        "source": CustomLogSourceResourceOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LogSourceResourceOutputTypeDef = TypedDict(
+    "LogSourceResourceOutputTypeDef",
+    {
+        "awsLogSource": AwsLogSourceResourceOutputTypeDef,
+        "customLogSource": CustomLogSourceResourceOutputTypeDef,
+    },
+)
+
 LogSourceResourceTypeDef = TypedDict(
     "LogSourceResourceTypeDef",
     {
         "awsLogSource": AwsLogSourceResourceTypeDef,
         "customLogSource": CustomLogSourceResourceTypeDef,
     },
     total=False,
@@ -727,37 +811,28 @@
         "dataLakeArn": str,
         "dataLakeSources": List[DataLakeSourceTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDataLakeResourceTypeDef = TypedDict(
-    "_RequiredDataLakeResourceTypeDef",
-    {
-        "dataLakeArn": str,
-        "region": str,
-    },
-)
-_OptionalDataLakeResourceTypeDef = TypedDict(
-    "_OptionalDataLakeResourceTypeDef",
+DataLakeResourceTypeDef = TypedDict(
+    "DataLakeResourceTypeDef",
     {
         "createStatus": DataLakeStatusType,
-        "encryptionConfiguration": DataLakeEncryptionConfigurationTypeDef,
+        "dataLakeArn": str,
+        "encryptionConfiguration": DataLakeEncryptionConfigurationOutputTypeDef,
         "lifecycleConfiguration": DataLakeLifecycleConfigurationOutputTypeDef,
+        "region": str,
         "replicationConfiguration": DataLakeReplicationConfigurationOutputTypeDef,
         "s3BucketArn": str,
         "updateStatus": DataLakeUpdateStatusTypeDef,
     },
-    total=False,
 )
 
-class DataLakeResourceTypeDef(_RequiredDataLakeResourceTypeDef, _OptionalDataLakeResourceTypeDef):
-    pass
-
 CreateSubscriberNotificationRequestRequestTypeDef = TypedDict(
     "CreateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
@@ -766,14 +841,44 @@
     "UpdateSubscriberNotificationRequestRequestTypeDef",
     {
         "configuration": NotificationConfigurationTypeDef,
         "subscriberId": str,
     },
 )
 
+LogSourceTypeDef = TypedDict(
+    "LogSourceTypeDef",
+    {
+        "account": str,
+        "region": str,
+        "sources": List[LogSourceResourceOutputTypeDef],
+    },
+)
+
+SubscriberResourceTypeDef = TypedDict(
+    "SubscriberResourceTypeDef",
+    {
+        "accessTypes": List[AccessTypeType],
+        "createdAt": datetime,
+        "resourceShareArn": str,
+        "resourceShareName": str,
+        "roleArn": str,
+        "s3BucketArn": str,
+        "sources": List[LogSourceResourceOutputTypeDef],
+        "subscriberArn": str,
+        "subscriberDescription": str,
+        "subscriberEndpoint": str,
+        "subscriberId": str,
+        "subscriberIdentity": AwsIdentityOutputTypeDef,
+        "subscriberName": str,
+        "subscriberStatus": SubscriberStatusType,
+        "updatedAt": datetime,
+    },
+)
+
 _RequiredCreateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSubscriberRequestRequestTypeDef",
     {
         "sources": Sequence[LogSourceResourceTypeDef],
         "subscriberIdentity": AwsIdentityTypeDef,
         "subscriberName": str,
     },
@@ -812,56 +917,14 @@
         "nextToken": str,
         "regions": Sequence[str],
         "sources": Sequence[LogSourceResourceTypeDef],
     },
     total=False,
 )
 
-LogSourceTypeDef = TypedDict(
-    "LogSourceTypeDef",
-    {
-        "account": str,
-        "region": str,
-        "sources": List[LogSourceResourceTypeDef],
-    },
-    total=False,
-)
-
-_RequiredSubscriberResourceTypeDef = TypedDict(
-    "_RequiredSubscriberResourceTypeDef",
-    {
-        "sources": List[LogSourceResourceTypeDef],
-        "subscriberArn": str,
-        "subscriberId": str,
-        "subscriberIdentity": AwsIdentityTypeDef,
-        "subscriberName": str,
-    },
-)
-_OptionalSubscriberResourceTypeDef = TypedDict(
-    "_OptionalSubscriberResourceTypeDef",
-    {
-        "accessTypes": List[AccessTypeType],
-        "createdAt": datetime,
-        "resourceShareArn": str,
-        "resourceShareName": str,
-        "roleArn": str,
-        "s3BucketArn": str,
-        "subscriberDescription": str,
-        "subscriberEndpoint": str,
-        "subscriberStatus": SubscriberStatusType,
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-class SubscriberResourceTypeDef(
-    _RequiredSubscriberResourceTypeDef, _OptionalSubscriberResourceTypeDef
-):
-    pass
-
 _RequiredUpdateSubscriberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubscriberRequestRequestTypeDef",
     {
         "subscriberId": str,
     },
 )
 _OptionalUpdateSubscriberRequestRequestTypeDef = TypedDict(
```

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/PKG-INFO` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securitylake
-Version: 1.28.15
-Summary: Type annotations for boto3.SecurityLake 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.8
+Summary: Type annotations for boto3.SecurityLake 1.28.8 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-securitylake"></a>
 
 # mypy-boto3-securitylake
 
 [![PyPI - mypy-boto3-securitylake](https://img.shields.io/pypi/v/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securitylake.svg?color=blue)](https://pypi.org/project/mypy-boto3-securitylake)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securitylake)](https://pepy.tech/project/mypy-boto3-securitylake)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-securitylake?color=blue)](https://pypistats.org/packages/mypy-boto3-securitylake)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityLake 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
+[boto3.SecurityLake 1.28.8](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#SecurityLake)
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
 [mypy-boto3-securitylake docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securitylake/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,26 +340,33 @@
 ### Typed dictionaries
 
 `mypy_boto3_securitylake.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securitylake.type_defs import (
+    AwsIdentityOutputTypeDef,
     AwsIdentityTypeDef,
     AwsLogSourceConfigurationTypeDef,
+    AwsLogSourceResourceOutputTypeDef,
     AwsLogSourceResourceTypeDef,
     ResponseMetadataTypeDef,
     CreateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     TagTypeDef,
+    CustomLogSourceAttributesOutputTypeDef,
     CustomLogSourceAttributesTypeDef,
     CustomLogSourceCrawlerConfigurationTypeDef,
+    CustomLogSourceProviderOutputTypeDef,
     CustomLogSourceProviderTypeDef,
     DataLakeEncryptionConfigurationTypeDef,
     DataLakeReplicationConfigurationTypeDef,
+    DataLakeEncryptionConfigurationOutputTypeDef,
     DataLakeExceptionTypeDef,
+    DataLakeLifecycleExpirationOutputTypeDef,
+    DataLakeLifecycleTransitionOutputTypeDef,
     DataLakeLifecycleExpirationTypeDef,
     DataLakeLifecycleTransitionTypeDef,
     DataLakeReplicationConfigurationOutputTypeDef,
     DataLakeSourceStatusTypeDef,
     DataLakeUpdateExceptionTypeDef,
     DeleteCustomLogSourceRequestRequestTypeDef,
     DeleteDataLakeRequestRequestTypeDef,
@@ -369,70 +376,73 @@
     GetDataLakeSourcesRequestRequestTypeDef,
     GetSubscriberRequestRequestTypeDef,
     HttpsNotificationConfigurationTypeDef,
     ListDataLakeExceptionsRequestRequestTypeDef,
     ListDataLakesRequestRequestTypeDef,
     ListSubscribersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    TagOutputTypeDef,
     RegisterDataLakeDelegatedAdministratorRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataLakeExceptionSubscriptionRequestRequestTypeDef,
     CreateAwsLogSourceRequestRequestTypeDef,
     DeleteAwsLogSourceRequestRequestTypeDef,
     DataLakeAutoEnableNewAccountConfigurationOutputTypeDef,
     DataLakeAutoEnableNewAccountConfigurationTypeDef,
     CreateAwsLogSourceResponseTypeDef,
     CreateSubscriberNotificationResponseTypeDef,
     DeleteAwsLogSourceResponseTypeDef,
     GetDataLakeExceptionSubscriptionResponseTypeDef,
     UpdateSubscriberNotificationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomLogSourceConfigurationTypeDef,
+    CustomLogSourceResourceOutputTypeDef,
     CustomLogSourceResourceTypeDef,
     ListDataLakeExceptionsResponseTypeDef,
     DataLakeLifecycleConfigurationOutputTypeDef,
     DataLakeLifecycleConfigurationTypeDef,
     DataLakeSourceTypeDef,
     DataLakeUpdateStatusTypeDef,
     GetDataLakeSourcesRequestGetDataLakeSourcesPaginateTypeDef,
     ListDataLakeExceptionsRequestListDataLakeExceptionsPaginateTypeDef,
     ListSubscribersRequestListSubscribersPaginateTypeDef,
     NotificationConfigurationTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetDataLakeOrganizationConfigurationResponseTypeDef,
     CreateDataLakeOrganizationConfigurationRequestRequestTypeDef,
     DeleteDataLakeOrganizationConfigurationRequestRequestTypeDef,
     CreateCustomLogSourceRequestRequestTypeDef,
     CreateCustomLogSourceResponseTypeDef,
+    LogSourceResourceOutputTypeDef,
     LogSourceResourceTypeDef,
     DataLakeConfigurationTypeDef,
     GetDataLakeSourcesResponseTypeDef,
     DataLakeResourceTypeDef,
     CreateSubscriberNotificationRequestRequestTypeDef,
     UpdateSubscriberNotificationRequestRequestTypeDef,
+    LogSourceTypeDef,
+    SubscriberResourceTypeDef,
     CreateSubscriberRequestRequestTypeDef,
     ListLogSourcesRequestListLogSourcesPaginateTypeDef,
     ListLogSourcesRequestRequestTypeDef,
-    LogSourceTypeDef,
-    SubscriberResourceTypeDef,
     UpdateSubscriberRequestRequestTypeDef,
     CreateDataLakeRequestRequestTypeDef,
     UpdateDataLakeRequestRequestTypeDef,
     CreateDataLakeResponseTypeDef,
     ListDataLakesResponseTypeDef,
     UpdateDataLakeResponseTypeDef,
     ListLogSourcesResponseTypeDef,
     CreateSubscriberResponseTypeDef,
     GetSubscriberResponseTypeDef,
     ListSubscribersResponseTypeDef,
     UpdateSubscriberResponseTypeDef,
 )
 
 
-def get_structure() -> AwsIdentityTypeDef:
+def get_structure() -> AwsIdentityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-securitylake-1.28.15/mypy_boto3_securitylake.egg-info/SOURCES.txt` & `mypy-boto3-securitylake-1.28.8/mypy_boto3_securitylake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securitylake-1.28.15/setup.py` & `mypy-boto3-securitylake-1.28.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securitylake",
-    version="1.28.15",
+    version="1.28.8",
     packages=["mypy_boto3_securitylake"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityLake 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        "Type annotations for boto3.SecurityLake 1.28.8 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

