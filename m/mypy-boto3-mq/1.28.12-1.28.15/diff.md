# Comparing `tmp/mypy-boto3-mq-1.28.12.tar.gz` & `tmp/mypy-boto3-mq-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mq-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
+gzip compressed data, was "mypy-boto3-mq-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
```

## Comparing `mypy-boto3-mq-1.28.12.tar` & `mypy-boto3-mq-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/mypy_boto3_mq/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29695 2023-07-27 05:26:47.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-07-27 05:26:47.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 05:35:04.000000 mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.224429 mypy-boto3-mq-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-27 05:26:46.000000 mypy-boto3-mq-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.097554 mypy-boto3-mq-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-07-28 20:43:21.093554 mypy-boto3-mq-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.089554 mypy-boto3-mq-1.28.15/mypy_boto3_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17207 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9392 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-07-28 20:32:12.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27972 2023-07-28 20:32:11.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.093554 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 20:43:20.000000 mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.101554 mypy-boto3-mq-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-28 20:32:10.000000 mypy-boto3-mq-1.28.15/setup.py
```

### Comparing `mypy-boto3-mq-1.28.12/LICENSE` & `mypy-boto3-mq-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.12/PKG-INFO` & `mypy-boto3-mq-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.28.12
-Summary: Type annotations for boto3.MQ 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mq)](https://pepy.tech/project/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,74 +332,70 @@
 ```python
 from mypy_boto3_mq.type_defs import (
     ActionRequiredTypeDef,
     AvailabilityZoneTypeDef,
     EngineVersionTypeDef,
     BrokerInstanceTypeDef,
     BrokerSummaryTypeDef,
-    ConfigurationIdOutputTypeDef,
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
-    CreateBrokerResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
-    DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
-    EncryptionOptionsOutputTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
-    WeeklyStartTimeOutputTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBrokersRequestListBrokersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
-    LogsOutputTypeDef,
     PendingLogsTypeDef,
-    PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
-    PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
-    ListBrokersResponseTypeDef,
     ConfigurationsTypeDef,
     ConfigurationTypeDef,
+    CreateBrokerRequestRequestTypeDef,
+    UpdateBrokerRequestRequestTypeDef,
+    CreateBrokerResponseTypeDef,
     CreateConfigurationResponseTypeDef,
+    DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
-    CreateBrokerRequestRequestTypeDef,
-    UpdateBrokerRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    PromoteResponseTypeDef,
     DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
+    ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
```

### Comparing `mypy-boto3-mq-1.28.12/README.md` & `mypy-boto3-mq-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mq)](https://pepy.tech/project/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,74 +300,70 @@
 ```python
 from mypy_boto3_mq.type_defs import (
     ActionRequiredTypeDef,
     AvailabilityZoneTypeDef,
     EngineVersionTypeDef,
     BrokerInstanceTypeDef,
     BrokerSummaryTypeDef,
-    ConfigurationIdOutputTypeDef,
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
-    CreateBrokerResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
-    DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
-    EncryptionOptionsOutputTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
-    WeeklyStartTimeOutputTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBrokersRequestListBrokersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
-    LogsOutputTypeDef,
     PendingLogsTypeDef,
-    PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
-    PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
-    ListBrokersResponseTypeDef,
     ConfigurationsTypeDef,
     ConfigurationTypeDef,
+    CreateBrokerRequestRequestTypeDef,
+    UpdateBrokerRequestRequestTypeDef,
+    CreateBrokerResponseTypeDef,
     CreateConfigurationResponseTypeDef,
+    DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
-    CreateBrokerRequestRequestTypeDef,
-    UpdateBrokerRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    PromoteResponseTypeDef,
     DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
+    ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
```

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/__init__.py` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/__init__.pyi` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/__main__.py` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MQ 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.MQ 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ\nOther"
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

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/client.py` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/client.pyi` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/literals.py` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/literals.pyi` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/paginator.py` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListBrokersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/paginators/#listbrokerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBrokersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/paginators/#listbrokerspaginator)
         """
```

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/paginator.pyi` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListBrokersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/paginators/#listbrokerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBrokersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ.Paginator.ListBrokers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/paginators/#listbrokerspaginator)
         """
```

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/type_defs.py` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,74 +36,70 @@
 
 __all__ = (
     "ActionRequiredTypeDef",
     "AvailabilityZoneTypeDef",
     "EngineVersionTypeDef",
     "BrokerInstanceTypeDef",
     "BrokerSummaryTypeDef",
-    "ConfigurationIdOutputTypeDef",
     "ConfigurationIdTypeDef",
     "ConfigurationRevisionTypeDef",
     "EncryptionOptionsTypeDef",
     "LdapServerMetadataInputTypeDef",
     "LogsTypeDef",
     "UserTypeDef",
     "WeeklyStartTimeTypeDef",
-    "CreateBrokerResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DataReplicationCounterpartTypeDef",
     "DeleteBrokerRequestRequestTypeDef",
-    "DeleteBrokerResponseTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeBrokerEngineTypesRequestRequestTypeDef",
     "DescribeBrokerInstanceOptionsRequestRequestTypeDef",
     "DescribeBrokerRequestRequestTypeDef",
-    "EncryptionOptionsOutputTypeDef",
     "LdapServerMetadataOutputTypeDef",
     "UserSummaryTypeDef",
-    "WeeklyStartTimeOutputTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
-    "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserPendingChangesTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListBrokersRequestListBrokersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBrokersRequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "LogsOutputTypeDef",
     "PendingLogsTypeDef",
-    "PaginatorConfigTypeDef",
     "PromoteRequestRequestTypeDef",
-    "PromoteResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SanitizationWarningTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "BrokerInstanceOptionTypeDef",
     "BrokerEngineTypeTypeDef",
-    "ListBrokersResponseTypeDef",
     "ConfigurationsTypeDef",
     "ConfigurationTypeDef",
+    "CreateBrokerRequestRequestTypeDef",
+    "UpdateBrokerRequestRequestTypeDef",
+    "CreateBrokerResponseTypeDef",
     "CreateConfigurationResponseTypeDef",
+    "DeleteBrokerResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
+    "DescribeConfigurationRevisionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListBrokersResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
-    "CreateBrokerRequestRequestTypeDef",
-    "UpdateBrokerRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
+    "PromoteResponseTypeDef",
     "DataReplicationMetadataOutputTypeDef",
     "ListUsersResponseTypeDef",
     "DescribeUserResponseTypeDef",
+    "ListBrokersRequestListBrokersPaginateTypeDef",
     "LogsSummaryTypeDef",
     "UpdateConfigurationResponseTypeDef",
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     "DescribeBrokerEngineTypesResponseTypeDef",
     "ListConfigurationsResponseTypeDef",
     "UpdateBrokerResponseTypeDef",
     "DescribeBrokerResponseTypeDef",
@@ -165,35 +161,14 @@
 )
 
 
 class BrokerSummaryTypeDef(_RequiredBrokerSummaryTypeDef, _OptionalBrokerSummaryTypeDef):
     pass
 
 
-_RequiredConfigurationIdOutputTypeDef = TypedDict(
-    "_RequiredConfigurationIdOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalConfigurationIdOutputTypeDef = TypedDict(
-    "_OptionalConfigurationIdOutputTypeDef",
-    {
-        "Revision": int,
-    },
-    total=False,
-)
-
-
-class ConfigurationIdOutputTypeDef(
-    _RequiredConfigurationIdOutputTypeDef, _OptionalConfigurationIdOutputTypeDef
-):
-    pass
-
-
 _RequiredConfigurationIdTypeDef = TypedDict(
     "_RequiredConfigurationIdTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigurationIdTypeDef = TypedDict(
@@ -329,20 +304,22 @@
 )
 
 
 class WeeklyStartTimeTypeDef(_RequiredWeeklyStartTimeTypeDef, _OptionalWeeklyStartTimeTypeDef):
     pass
 
 
-CreateBrokerResponseTypeDef = TypedDict(
-    "CreateBrokerResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "BrokerArn": str,
-        "BrokerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationRequestRequestTypeDef",
     {
         "EngineType": EngineTypeType,
@@ -424,22 +401,14 @@
 DeleteBrokerRequestRequestTypeDef = TypedDict(
     "DeleteBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
-DeleteBrokerResponseTypeDef = TypedDict(
-    "DeleteBrokerResponseTypeDef",
-    {
-        "BrokerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTagsRequestRequestTypeDef = TypedDict(
     "DeleteTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -477,35 +446,14 @@
 DescribeBrokerRequestRequestTypeDef = TypedDict(
     "DescribeBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
-_RequiredEncryptionOptionsOutputTypeDef = TypedDict(
-    "_RequiredEncryptionOptionsOutputTypeDef",
-    {
-        "UseAwsOwnedKey": bool,
-    },
-)
-_OptionalEncryptionOptionsOutputTypeDef = TypedDict(
-    "_OptionalEncryptionOptionsOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class EncryptionOptionsOutputTypeDef(
-    _RequiredEncryptionOptionsOutputTypeDef, _OptionalEncryptionOptionsOutputTypeDef
-):
-    pass
-
-
 _RequiredLdapServerMetadataOutputTypeDef = TypedDict(
     "_RequiredLdapServerMetadataOutputTypeDef",
     {
         "Hosts": List[str],
         "RoleBase": str,
         "RoleSearchMatching": str,
         "ServiceAccountUsername": str,
@@ -546,36 +494,14 @@
 )
 
 
 class UserSummaryTypeDef(_RequiredUserSummaryTypeDef, _OptionalUserSummaryTypeDef):
     pass
 
 
-_RequiredWeeklyStartTimeOutputTypeDef = TypedDict(
-    "_RequiredWeeklyStartTimeOutputTypeDef",
-    {
-        "DayOfWeek": DayOfWeekType,
-        "TimeOfDay": str,
-    },
-)
-_OptionalWeeklyStartTimeOutputTypeDef = TypedDict(
-    "_OptionalWeeklyStartTimeOutputTypeDef",
-    {
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-
-class WeeklyStartTimeOutputTypeDef(
-    _RequiredWeeklyStartTimeOutputTypeDef, _OptionalWeeklyStartTimeOutputTypeDef
-):
-    pass
-
-
 DescribeConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationRequestRequestTypeDef",
     {
         "ConfigurationId": str,
     },
 )
 
@@ -583,25 +509,14 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "ConfigurationId": str,
         "ConfigurationRevision": str,
     },
 )
 
-DescribeConfigurationRevisionResponseTypeDef = TypedDict(
-    "DescribeConfigurationRevisionResponseTypeDef",
-    {
-        "ConfigurationId": str,
-        "Created": datetime,
-        "Data": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "BrokerId": str,
         "Username": str,
     },
 )
@@ -624,25 +539,20 @@
 
 class UserPendingChangesTypeDef(
     _RequiredUserPendingChangesTypeDef, _OptionalUserPendingChangesTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
-    "ListBrokersRequestListBrokersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBrokersRequestRequestTypeDef = TypedDict(
     "ListBrokersRequestRequestTypeDef",
     {
@@ -687,22 +597,14 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -717,76 +619,38 @@
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
 
-LogsOutputTypeDef = TypedDict(
-    "LogsOutputTypeDef",
-    {
-        "Audit": bool,
-        "General": bool,
-    },
-    total=False,
-)
-
 PendingLogsTypeDef = TypedDict(
     "PendingLogsTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
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
 PromoteRequestRequestTypeDef = TypedDict(
     "PromoteRequestRequestTypeDef",
     {
         "BrokerId": str,
         "Mode": PromoteModeType,
     },
 )
 
-PromoteResponseTypeDef = TypedDict(
-    "PromoteResponseTypeDef",
-    {
-        "BrokerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
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
 _RequiredSanitizationWarningTypeDef = TypedDict(
     "_RequiredSanitizationWarningTypeDef",
     {
         "Reason": SanitizationWarningReasonType,
     },
 )
 _OptionalSanitizationWarningTypeDef = TypedDict(
@@ -871,29 +735,20 @@
     {
         "EngineType": EngineTypeType,
         "EngineVersions": List[EngineVersionTypeDef],
     },
     total=False,
 )
 
-ListBrokersResponseTypeDef = TypedDict(
-    "ListBrokersResponseTypeDef",
-    {
-        "BrokerSummaries": List[BrokerSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfigurationsTypeDef = TypedDict(
     "ConfigurationsTypeDef",
     {
-        "Current": ConfigurationIdOutputTypeDef,
-        "History": List[ConfigurationIdOutputTypeDef],
-        "Pending": ConfigurationIdOutputTypeDef,
+        "Current": ConfigurationIdTypeDef,
+        "History": List[ConfigurationIdTypeDef],
+        "Pending": ConfigurationIdTypeDef,
     },
     total=False,
 )
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
@@ -917,55 +772,14 @@
 )
 
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
 
-CreateConfigurationResponseTypeDef = TypedDict(
-    "CreateConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "Created": datetime,
-        "Id": str,
-        "LatestRevision": ConfigurationRevisionTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeConfigurationResponseTypeDef = TypedDict(
-    "DescribeConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "Created": datetime,
-        "Description": str,
-        "EngineType": EngineTypeType,
-        "EngineVersion": str,
-        "Id": str,
-        "LatestRevision": ConfigurationRevisionTypeDef,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListConfigurationRevisionsResponseTypeDef = TypedDict(
-    "ListConfigurationRevisionsResponseTypeDef",
-    {
-        "ConfigurationId": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "Revisions": List[ConfigurationRevisionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBrokerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrokerRequestRequestTypeDef",
     {
         "AutoMinorVersionUpgrade": bool,
         "BrokerName": str,
         "DeploymentMode": DeploymentModeType,
         "EngineType": EngineTypeType,
@@ -1028,14 +842,115 @@
 
 class UpdateBrokerRequestRequestTypeDef(
     _RequiredUpdateBrokerRequestRequestTypeDef, _OptionalUpdateBrokerRequestRequestTypeDef
 ):
     pass
 
 
+CreateBrokerResponseTypeDef = TypedDict(
+    "CreateBrokerResponseTypeDef",
+    {
+        "BrokerArn": str,
+        "BrokerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConfigurationResponseTypeDef = TypedDict(
+    "CreateConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "Created": datetime,
+        "Id": str,
+        "LatestRevision": ConfigurationRevisionTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBrokerResponseTypeDef = TypedDict(
+    "DeleteBrokerResponseTypeDef",
+    {
+        "BrokerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationResponseTypeDef = TypedDict(
+    "DescribeConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "Created": datetime,
+        "Description": str,
+        "EngineType": EngineTypeType,
+        "EngineVersion": str,
+        "Id": str,
+        "LatestRevision": ConfigurationRevisionTypeDef,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationRevisionResponseTypeDef = TypedDict(
+    "DescribeConfigurationRevisionResponseTypeDef",
+    {
+        "ConfigurationId": str,
+        "Created": datetime,
+        "Data": str,
+        "Description": str,
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
+ListBrokersResponseTypeDef = TypedDict(
+    "ListBrokersResponseTypeDef",
+    {
+        "BrokerSummaries": List[BrokerSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationRevisionsResponseTypeDef = TypedDict(
+    "ListConfigurationRevisionsResponseTypeDef",
+    {
+        "ConfigurationId": str,
+        "MaxResults": int,
+        "NextToken": str,
+        "Revisions": List[ConfigurationRevisionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PromoteResponseTypeDef = TypedDict(
+    "PromoteResponseTypeDef",
+    {
+        "BrokerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDataReplicationMetadataOutputTypeDef = TypedDict(
     "_RequiredDataReplicationMetadataOutputTypeDef",
     {
         "DataReplicationRole": str,
     },
 )
 _OptionalDataReplicationMetadataOutputTypeDef = TypedDict(
@@ -1056,29 +971,37 @@
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "BrokerId": str,
         "MaxResults": int,
         "NextToken": str,
         "Users": List[UserSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "BrokerId": str,
         "ConsoleAccess": bool,
         "Groups": List[str],
         "Pending": UserPendingChangesTypeDef,
         "Username": str,
         "ReplicationUser": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
+    "ListBrokersRequestListBrokersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 _RequiredLogsSummaryTypeDef = TypedDict(
     "_RequiredLogsSummaryTypeDef",
     {
         "General": bool,
         "GeneralLogGroup": str,
@@ -1104,66 +1027,66 @@
     {
         "Arn": str,
         "Created": datetime,
         "Id": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "Warnings": List[SanitizationWarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBrokerInstanceOptionsResponseTypeDef = TypedDict(
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     {
         "BrokerInstanceOptions": List[BrokerInstanceOptionTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBrokerEngineTypesResponseTypeDef = TypedDict(
     "DescribeBrokerEngineTypesResponseTypeDef",
     {
         "BrokerEngineTypes": List[BrokerEngineTypeTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBrokerResponseTypeDef = TypedDict(
     "UpdateBrokerResponseTypeDef",
     {
         "AuthenticationStrategy": AuthenticationStrategyType,
         "AutoMinorVersionUpgrade": bool,
         "BrokerId": str,
-        "Configuration": ConfigurationIdOutputTypeDef,
+        "Configuration": ConfigurationIdTypeDef,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
-        "Logs": LogsOutputTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeOutputTypeDef,
+        "Logs": LogsTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "SecurityGroups": List[str],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBrokerResponseTypeDef = TypedDict(
     "DescribeBrokerResponseTypeDef",
     {
         "ActionsRequired": List[ActionRequiredTypeDef],
@@ -1173,21 +1096,21 @@
         "BrokerId": str,
         "BrokerInstances": List[BrokerInstanceTypeDef],
         "BrokerName": str,
         "BrokerState": BrokerStateType,
         "Configurations": ConfigurationsTypeDef,
         "Created": datetime,
         "DeploymentMode": DeploymentModeType,
-        "EncryptionOptions": EncryptionOptionsOutputTypeDef,
+        "EncryptionOptions": EncryptionOptionsTypeDef,
         "EngineType": EngineTypeType,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
         "Logs": LogsSummaryTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeOutputTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "PendingAuthenticationStrategy": AuthenticationStrategyType,
         "PendingEngineVersion": str,
         "PendingHostInstanceType": str,
         "PendingLdapServerMetadata": LdapServerMetadataOutputTypeDef,
         "PendingSecurityGroups": List[str],
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
@@ -1195,10 +1118,10 @@
         "SubnetIds": List[str],
         "Tags": Dict[str, str],
         "Users": List[UserSummaryTypeDef],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq/type_defs.pyi` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -35,74 +35,70 @@
 
 __all__ = (
     "ActionRequiredTypeDef",
     "AvailabilityZoneTypeDef",
     "EngineVersionTypeDef",
     "BrokerInstanceTypeDef",
     "BrokerSummaryTypeDef",
-    "ConfigurationIdOutputTypeDef",
     "ConfigurationIdTypeDef",
     "ConfigurationRevisionTypeDef",
     "EncryptionOptionsTypeDef",
     "LdapServerMetadataInputTypeDef",
     "LogsTypeDef",
     "UserTypeDef",
     "WeeklyStartTimeTypeDef",
-    "CreateBrokerResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateConfigurationRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DataReplicationCounterpartTypeDef",
     "DeleteBrokerRequestRequestTypeDef",
-    "DeleteBrokerResponseTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DescribeBrokerEngineTypesRequestRequestTypeDef",
     "DescribeBrokerInstanceOptionsRequestRequestTypeDef",
     "DescribeBrokerRequestRequestTypeDef",
-    "EncryptionOptionsOutputTypeDef",
     "LdapServerMetadataOutputTypeDef",
     "UserSummaryTypeDef",
-    "WeeklyStartTimeOutputTypeDef",
     "DescribeConfigurationRequestRequestTypeDef",
     "DescribeConfigurationRevisionRequestRequestTypeDef",
-    "DescribeConfigurationRevisionResponseTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserPendingChangesTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListBrokersRequestListBrokersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBrokersRequestRequestTypeDef",
     "ListConfigurationRevisionsRequestRequestTypeDef",
     "ListConfigurationsRequestRequestTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "ListUsersRequestRequestTypeDef",
-    "LogsOutputTypeDef",
     "PendingLogsTypeDef",
-    "PaginatorConfigTypeDef",
     "PromoteRequestRequestTypeDef",
-    "PromoteResponseTypeDef",
     "RebootBrokerRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SanitizationWarningTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "BrokerInstanceOptionTypeDef",
     "BrokerEngineTypeTypeDef",
-    "ListBrokersResponseTypeDef",
     "ConfigurationsTypeDef",
     "ConfigurationTypeDef",
+    "CreateBrokerRequestRequestTypeDef",
+    "UpdateBrokerRequestRequestTypeDef",
+    "CreateBrokerResponseTypeDef",
     "CreateConfigurationResponseTypeDef",
+    "DeleteBrokerResponseTypeDef",
     "DescribeConfigurationResponseTypeDef",
+    "DescribeConfigurationRevisionResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListBrokersResponseTypeDef",
     "ListConfigurationRevisionsResponseTypeDef",
-    "CreateBrokerRequestRequestTypeDef",
-    "UpdateBrokerRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
+    "PromoteResponseTypeDef",
     "DataReplicationMetadataOutputTypeDef",
     "ListUsersResponseTypeDef",
     "DescribeUserResponseTypeDef",
+    "ListBrokersRequestListBrokersPaginateTypeDef",
     "LogsSummaryTypeDef",
     "UpdateConfigurationResponseTypeDef",
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     "DescribeBrokerEngineTypesResponseTypeDef",
     "ListConfigurationsResponseTypeDef",
     "UpdateBrokerResponseTypeDef",
     "DescribeBrokerResponseTypeDef",
@@ -162,33 +158,14 @@
     },
     total=False,
 )
 
 class BrokerSummaryTypeDef(_RequiredBrokerSummaryTypeDef, _OptionalBrokerSummaryTypeDef):
     pass
 
-_RequiredConfigurationIdOutputTypeDef = TypedDict(
-    "_RequiredConfigurationIdOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalConfigurationIdOutputTypeDef = TypedDict(
-    "_OptionalConfigurationIdOutputTypeDef",
-    {
-        "Revision": int,
-    },
-    total=False,
-)
-
-class ConfigurationIdOutputTypeDef(
-    _RequiredConfigurationIdOutputTypeDef, _OptionalConfigurationIdOutputTypeDef
-):
-    pass
-
 _RequiredConfigurationIdTypeDef = TypedDict(
     "_RequiredConfigurationIdTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalConfigurationIdTypeDef = TypedDict(
@@ -312,20 +289,22 @@
     },
     total=False,
 )
 
 class WeeklyStartTimeTypeDef(_RequiredWeeklyStartTimeTypeDef, _OptionalWeeklyStartTimeTypeDef):
     pass
 
-CreateBrokerResponseTypeDef = TypedDict(
-    "CreateBrokerResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "BrokerArn": str,
-        "BrokerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationRequestRequestTypeDef",
     {
         "EngineType": EngineTypeType,
@@ -401,22 +380,14 @@
 DeleteBrokerRequestRequestTypeDef = TypedDict(
     "DeleteBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
-DeleteBrokerResponseTypeDef = TypedDict(
-    "DeleteBrokerResponseTypeDef",
-    {
-        "BrokerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTagsRequestRequestTypeDef = TypedDict(
     "DeleteTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -454,33 +425,14 @@
 DescribeBrokerRequestRequestTypeDef = TypedDict(
     "DescribeBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 
-_RequiredEncryptionOptionsOutputTypeDef = TypedDict(
-    "_RequiredEncryptionOptionsOutputTypeDef",
-    {
-        "UseAwsOwnedKey": bool,
-    },
-)
-_OptionalEncryptionOptionsOutputTypeDef = TypedDict(
-    "_OptionalEncryptionOptionsOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class EncryptionOptionsOutputTypeDef(
-    _RequiredEncryptionOptionsOutputTypeDef, _OptionalEncryptionOptionsOutputTypeDef
-):
-    pass
-
 _RequiredLdapServerMetadataOutputTypeDef = TypedDict(
     "_RequiredLdapServerMetadataOutputTypeDef",
     {
         "Hosts": List[str],
         "RoleBase": str,
         "RoleSearchMatching": str,
         "ServiceAccountUsername": str,
@@ -517,34 +469,14 @@
     },
     total=False,
 )
 
 class UserSummaryTypeDef(_RequiredUserSummaryTypeDef, _OptionalUserSummaryTypeDef):
     pass
 
-_RequiredWeeklyStartTimeOutputTypeDef = TypedDict(
-    "_RequiredWeeklyStartTimeOutputTypeDef",
-    {
-        "DayOfWeek": DayOfWeekType,
-        "TimeOfDay": str,
-    },
-)
-_OptionalWeeklyStartTimeOutputTypeDef = TypedDict(
-    "_OptionalWeeklyStartTimeOutputTypeDef",
-    {
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-class WeeklyStartTimeOutputTypeDef(
-    _RequiredWeeklyStartTimeOutputTypeDef, _OptionalWeeklyStartTimeOutputTypeDef
-):
-    pass
-
 DescribeConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationRequestRequestTypeDef",
     {
         "ConfigurationId": str,
     },
 )
 
@@ -552,25 +484,14 @@
     "DescribeConfigurationRevisionRequestRequestTypeDef",
     {
         "ConfigurationId": str,
         "ConfigurationRevision": str,
     },
 )
 
-DescribeConfigurationRevisionResponseTypeDef = TypedDict(
-    "DescribeConfigurationRevisionResponseTypeDef",
-    {
-        "ConfigurationId": str,
-        "Created": datetime,
-        "Data": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeUserRequestRequestTypeDef = TypedDict(
     "DescribeUserRequestRequestTypeDef",
     {
         "BrokerId": str,
         "Username": str,
     },
 )
@@ -591,25 +512,20 @@
 )
 
 class UserPendingChangesTypeDef(
     _RequiredUserPendingChangesTypeDef, _OptionalUserPendingChangesTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
-    "ListBrokersRequestListBrokersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListBrokersRequestRequestTypeDef = TypedDict(
     "ListBrokersRequestRequestTypeDef",
     {
@@ -652,22 +568,14 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -680,76 +588,38 @@
 )
 
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-LogsOutputTypeDef = TypedDict(
-    "LogsOutputTypeDef",
-    {
-        "Audit": bool,
-        "General": bool,
-    },
-    total=False,
-)
-
 PendingLogsTypeDef = TypedDict(
     "PendingLogsTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
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
 PromoteRequestRequestTypeDef = TypedDict(
     "PromoteRequestRequestTypeDef",
     {
         "BrokerId": str,
         "Mode": PromoteModeType,
     },
 )
 
-PromoteResponseTypeDef = TypedDict(
-    "PromoteResponseTypeDef",
-    {
-        "BrokerId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RebootBrokerRequestRequestTypeDef = TypedDict(
     "RebootBrokerRequestRequestTypeDef",
     {
         "BrokerId": str,
     },
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
 _RequiredSanitizationWarningTypeDef = TypedDict(
     "_RequiredSanitizationWarningTypeDef",
     {
         "Reason": SanitizationWarningReasonType,
     },
 )
 _OptionalSanitizationWarningTypeDef = TypedDict(
@@ -828,29 +698,20 @@
     {
         "EngineType": EngineTypeType,
         "EngineVersions": List[EngineVersionTypeDef],
     },
     total=False,
 )
 
-ListBrokersResponseTypeDef = TypedDict(
-    "ListBrokersResponseTypeDef",
-    {
-        "BrokerSummaries": List[BrokerSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfigurationsTypeDef = TypedDict(
     "ConfigurationsTypeDef",
     {
-        "Current": ConfigurationIdOutputTypeDef,
-        "History": List[ConfigurationIdOutputTypeDef],
-        "Pending": ConfigurationIdOutputTypeDef,
+        "Current": ConfigurationIdTypeDef,
+        "History": List[ConfigurationIdTypeDef],
+        "Pending": ConfigurationIdTypeDef,
     },
     total=False,
 )
 
 _RequiredConfigurationTypeDef = TypedDict(
     "_RequiredConfigurationTypeDef",
     {
@@ -872,55 +733,14 @@
     },
     total=False,
 )
 
 class ConfigurationTypeDef(_RequiredConfigurationTypeDef, _OptionalConfigurationTypeDef):
     pass
 
-CreateConfigurationResponseTypeDef = TypedDict(
-    "CreateConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "Created": datetime,
-        "Id": str,
-        "LatestRevision": ConfigurationRevisionTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeConfigurationResponseTypeDef = TypedDict(
-    "DescribeConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "AuthenticationStrategy": AuthenticationStrategyType,
-        "Created": datetime,
-        "Description": str,
-        "EngineType": EngineTypeType,
-        "EngineVersion": str,
-        "Id": str,
-        "LatestRevision": ConfigurationRevisionTypeDef,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListConfigurationRevisionsResponseTypeDef = TypedDict(
-    "ListConfigurationRevisionsResponseTypeDef",
-    {
-        "ConfigurationId": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "Revisions": List[ConfigurationRevisionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBrokerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBrokerRequestRequestTypeDef",
     {
         "AutoMinorVersionUpgrade": bool,
         "BrokerName": str,
         "DeploymentMode": DeploymentModeType,
         "EngineType": EngineTypeType,
@@ -979,14 +799,115 @@
 )
 
 class UpdateBrokerRequestRequestTypeDef(
     _RequiredUpdateBrokerRequestRequestTypeDef, _OptionalUpdateBrokerRequestRequestTypeDef
 ):
     pass
 
+CreateBrokerResponseTypeDef = TypedDict(
+    "CreateBrokerResponseTypeDef",
+    {
+        "BrokerArn": str,
+        "BrokerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateConfigurationResponseTypeDef = TypedDict(
+    "CreateConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "Created": datetime,
+        "Id": str,
+        "LatestRevision": ConfigurationRevisionTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBrokerResponseTypeDef = TypedDict(
+    "DeleteBrokerResponseTypeDef",
+    {
+        "BrokerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationResponseTypeDef = TypedDict(
+    "DescribeConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "AuthenticationStrategy": AuthenticationStrategyType,
+        "Created": datetime,
+        "Description": str,
+        "EngineType": EngineTypeType,
+        "EngineVersion": str,
+        "Id": str,
+        "LatestRevision": ConfigurationRevisionTypeDef,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationRevisionResponseTypeDef = TypedDict(
+    "DescribeConfigurationRevisionResponseTypeDef",
+    {
+        "ConfigurationId": str,
+        "Created": datetime,
+        "Data": str,
+        "Description": str,
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
+ListBrokersResponseTypeDef = TypedDict(
+    "ListBrokersResponseTypeDef",
+    {
+        "BrokerSummaries": List[BrokerSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationRevisionsResponseTypeDef = TypedDict(
+    "ListConfigurationRevisionsResponseTypeDef",
+    {
+        "ConfigurationId": str,
+        "MaxResults": int,
+        "NextToken": str,
+        "Revisions": List[ConfigurationRevisionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PromoteResponseTypeDef = TypedDict(
+    "PromoteResponseTypeDef",
+    {
+        "BrokerId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredDataReplicationMetadataOutputTypeDef = TypedDict(
     "_RequiredDataReplicationMetadataOutputTypeDef",
     {
         "DataReplicationRole": str,
     },
 )
 _OptionalDataReplicationMetadataOutputTypeDef = TypedDict(
@@ -1005,29 +926,37 @@
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "BrokerId": str,
         "MaxResults": int,
         "NextToken": str,
         "Users": List[UserSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "BrokerId": str,
         "ConsoleAccess": bool,
         "Groups": List[str],
         "Pending": UserPendingChangesTypeDef,
         "Username": str,
         "ReplicationUser": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListBrokersRequestListBrokersPaginateTypeDef = TypedDict(
+    "ListBrokersRequestListBrokersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 _RequiredLogsSummaryTypeDef = TypedDict(
     "_RequiredLogsSummaryTypeDef",
     {
         "General": bool,
         "GeneralLogGroup": str,
@@ -1051,66 +980,66 @@
     {
         "Arn": str,
         "Created": datetime,
         "Id": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
         "Name": str,
         "Warnings": List[SanitizationWarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBrokerInstanceOptionsResponseTypeDef = TypedDict(
     "DescribeBrokerInstanceOptionsResponseTypeDef",
     {
         "BrokerInstanceOptions": List[BrokerInstanceOptionTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBrokerEngineTypesResponseTypeDef = TypedDict(
     "DescribeBrokerEngineTypesResponseTypeDef",
     {
         "BrokerEngineTypes": List[BrokerEngineTypeTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
         "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBrokerResponseTypeDef = TypedDict(
     "UpdateBrokerResponseTypeDef",
     {
         "AuthenticationStrategy": AuthenticationStrategyType,
         "AutoMinorVersionUpgrade": bool,
         "BrokerId": str,
-        "Configuration": ConfigurationIdOutputTypeDef,
+        "Configuration": ConfigurationIdTypeDef,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
-        "Logs": LogsOutputTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeOutputTypeDef,
+        "Logs": LogsTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "SecurityGroups": List[str],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBrokerResponseTypeDef = TypedDict(
     "DescribeBrokerResponseTypeDef",
     {
         "ActionsRequired": List[ActionRequiredTypeDef],
@@ -1120,21 +1049,21 @@
         "BrokerId": str,
         "BrokerInstances": List[BrokerInstanceTypeDef],
         "BrokerName": str,
         "BrokerState": BrokerStateType,
         "Configurations": ConfigurationsTypeDef,
         "Created": datetime,
         "DeploymentMode": DeploymentModeType,
-        "EncryptionOptions": EncryptionOptionsOutputTypeDef,
+        "EncryptionOptions": EncryptionOptionsTypeDef,
         "EngineType": EngineTypeType,
         "EngineVersion": str,
         "HostInstanceType": str,
         "LdapServerMetadata": LdapServerMetadataOutputTypeDef,
         "Logs": LogsSummaryTypeDef,
-        "MaintenanceWindowStartTime": WeeklyStartTimeOutputTypeDef,
+        "MaintenanceWindowStartTime": WeeklyStartTimeTypeDef,
         "PendingAuthenticationStrategy": AuthenticationStrategyType,
         "PendingEngineVersion": str,
         "PendingHostInstanceType": str,
         "PendingLdapServerMetadata": LdapServerMetadataOutputTypeDef,
         "PendingSecurityGroups": List[str],
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
@@ -1142,10 +1071,10 @@
         "SubnetIds": List[str],
         "Tags": Dict[str, str],
         "Users": List[UserSummaryTypeDef],
         "DataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "DataReplicationMode": DataReplicationModeType,
         "PendingDataReplicationMetadata": DataReplicationMetadataOutputTypeDef,
         "PendingDataReplicationMode": DataReplicationModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/PKG-INFO` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mq
-Version: 1.28.12
-Summary: Type annotations for boto3.MQ 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mq.svg?color=blue)](https://pypi.org/project/mypy-boto3-mq)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mq)](https://pepy.tech/project/mypy-boto3-mq)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MQ 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
+[boto3.MQ 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#MQ)
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
 [mypy-boto3-mq docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mq/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,74 +332,70 @@
 ```python
 from mypy_boto3_mq.type_defs import (
     ActionRequiredTypeDef,
     AvailabilityZoneTypeDef,
     EngineVersionTypeDef,
     BrokerInstanceTypeDef,
     BrokerSummaryTypeDef,
-    ConfigurationIdOutputTypeDef,
     ConfigurationIdTypeDef,
     ConfigurationRevisionTypeDef,
     EncryptionOptionsTypeDef,
     LdapServerMetadataInputTypeDef,
     LogsTypeDef,
     UserTypeDef,
     WeeklyStartTimeTypeDef,
-    CreateBrokerResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateConfigurationRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     CreateUserRequestRequestTypeDef,
     DataReplicationCounterpartTypeDef,
     DeleteBrokerRequestRequestTypeDef,
-    DeleteBrokerResponseTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DescribeBrokerEngineTypesRequestRequestTypeDef,
     DescribeBrokerInstanceOptionsRequestRequestTypeDef,
     DescribeBrokerRequestRequestTypeDef,
-    EncryptionOptionsOutputTypeDef,
     LdapServerMetadataOutputTypeDef,
     UserSummaryTypeDef,
-    WeeklyStartTimeOutputTypeDef,
     DescribeConfigurationRequestRequestTypeDef,
     DescribeConfigurationRevisionRequestRequestTypeDef,
-    DescribeConfigurationRevisionResponseTypeDef,
     DescribeUserRequestRequestTypeDef,
     UserPendingChangesTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListBrokersRequestListBrokersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBrokersRequestRequestTypeDef,
     ListConfigurationRevisionsRequestRequestTypeDef,
     ListConfigurationsRequestRequestTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     ListUsersRequestRequestTypeDef,
-    LogsOutputTypeDef,
     PendingLogsTypeDef,
-    PaginatorConfigTypeDef,
     PromoteRequestRequestTypeDef,
-    PromoteResponseTypeDef,
     RebootBrokerRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SanitizationWarningTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     UpdateUserRequestRequestTypeDef,
     BrokerInstanceOptionTypeDef,
     BrokerEngineTypeTypeDef,
-    ListBrokersResponseTypeDef,
     ConfigurationsTypeDef,
     ConfigurationTypeDef,
+    CreateBrokerRequestRequestTypeDef,
+    UpdateBrokerRequestRequestTypeDef,
+    CreateBrokerResponseTypeDef,
     CreateConfigurationResponseTypeDef,
+    DeleteBrokerResponseTypeDef,
     DescribeConfigurationResponseTypeDef,
+    DescribeConfigurationRevisionResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListBrokersResponseTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
-    CreateBrokerRequestRequestTypeDef,
-    UpdateBrokerRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
+    PromoteResponseTypeDef,
     DataReplicationMetadataOutputTypeDef,
     ListUsersResponseTypeDef,
     DescribeUserResponseTypeDef,
+    ListBrokersRequestListBrokersPaginateTypeDef,
     LogsSummaryTypeDef,
     UpdateConfigurationResponseTypeDef,
     DescribeBrokerInstanceOptionsResponseTypeDef,
     DescribeBrokerEngineTypesResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     UpdateBrokerResponseTypeDef,
     DescribeBrokerResponseTypeDef,
```

### Comparing `mypy-boto3-mq-1.28.12/mypy_boto3_mq.egg-info/SOURCES.txt` & `mypy-boto3-mq-1.28.15/mypy_boto3_mq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mq-1.28.12/setup.py` & `mypy-boto3-mq-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mq",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mq"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MQ 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MQ 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

