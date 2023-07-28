# Comparing `tmp/mypy-boto3-amplifybackend-1.28.12.tar.gz` & `tmp/mypy-boto3-amplifybackend-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifybackend-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifybackend-1.28.15.tar", last modified: Fri Jul 28 20:42:12 2023, max compression
```

## Comparing `mypy-boto3-amplifybackend-1.28.12.tar` & `mypy-boto3-amplifybackend-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22983 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48488 2023-07-27 05:17:03.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48419 2023-07-27 05:17:03.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18133 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:16.000000 mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.332584 mypy-boto3-amplifybackend-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:17:02.000000 mypy-boto3-amplifybackend-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23022 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22983 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44075 2023-07-28 20:18:54.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44010 2023-07-28 20:18:53.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:42:12.000000 mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:12.676609 mypy-boto3-amplifybackend-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:18:52.000000 mypy-boto3-amplifybackend-1.28.15/setup.py
```

### Comparing `mypy-boto3-amplifybackend-1.28.12/LICENSE` & `mypy-boto3-amplifybackend-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/PKG-INFO` & `mypy-boto3-amplifybackend-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-amplifybackend
-Version: 1.28.12
-Summary: Type annotations for boto3.AmplifyBackend 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 amplifybackend type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-amplifybackend"></a>
 
 # mypy-boto3-amplifybackend
 
 [![PyPI - mypy-boto3-amplifybackend](https://img.shields.io/pypi/v/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,32 +304,25 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
-    BackendAPIAppSyncAuthSettingsOutputTypeDef,
     BackendAPIAppSyncAuthSettingsTypeDef,
-    BackendAPIConflictResolutionOutputTypeDef,
     BackendAPIConflictResolutionTypeDef,
-    BackendAuthAppleProviderConfigOutputTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
-    BackendAuthSocialProviderConfigOutputTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
     BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    EmailSettingsOutputTypeDef,
-    SmsSettingsOutputTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
-    CreateBackendAuthIdentityPoolConfigOutputTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
     SettingsOutputTypeDef,
     SettingsTypeDef,
     CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
@@ -379,24 +340,21 @@
     GetTokenRequestRequestTypeDef,
     ImportBackendAuthRequestRequestTypeDef,
     ImportBackendStorageRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBackendJobsRequestRequestTypeDef,
     ListS3BucketsRequestRequestTypeDef,
     S3BucketInfoTypeDef,
-    LoginAuthConfigReqObjOutputTypeDef,
     LoginAuthConfigReqObjTypeDef,
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
-    BackendAPIAuthTypeOutputTypeDef,
     BackendAPIAuthTypeTypeDef,
-    SocialProviderSettingsOutputTypeDef,
     SocialProviderSettingsTypeDef,
     GetBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
@@ -419,27 +377,25 @@
     ListBackendJobsResponseTypeDef,
     RemoveAllBackendsResponseTypeDef,
     RemoveBackendConfigResponseTypeDef,
     UpdateBackendAPIResponseTypeDef,
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
-    CreateBackendAuthForgotPasswordConfigOutputTypeDef,
-    CreateBackendAuthVerificationMessageConfigOutputTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
     CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
-    UpdateBackendConfigResponseTypeDef,
     UpdateBackendConfigRequestRequestTypeDef,
+    UpdateBackendConfigResponseTypeDef,
     BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
     CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
     GetBackendStorageResponseTypeDef,
     CreateBackendStorageRequestRequestTypeDef,
@@ -457,15 +413,15 @@
     UpdateBackendAuthResourceConfigTypeDef,
     GetBackendAuthResponseTypeDef,
     CreateBackendAuthRequestRequestTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsOutputTypeDef:
+def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.12/README.md` & `mypy-boto3-amplifybackend-1.28.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-amplifybackend
+Version: 1.28.15
+Summary: Type annotations for boto3.AmplifyBackend 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 amplifybackend type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-amplifybackend"></a>
 
 # mypy-boto3-amplifybackend
 
 [![PyPI - mypy-boto3-amplifybackend](https://img.shields.io/pypi/v/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,32 +336,25 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
-    BackendAPIAppSyncAuthSettingsOutputTypeDef,
     BackendAPIAppSyncAuthSettingsTypeDef,
-    BackendAPIConflictResolutionOutputTypeDef,
     BackendAPIConflictResolutionTypeDef,
-    BackendAuthAppleProviderConfigOutputTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
-    BackendAuthSocialProviderConfigOutputTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
     BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    EmailSettingsOutputTypeDef,
-    SmsSettingsOutputTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
-    CreateBackendAuthIdentityPoolConfigOutputTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
     SettingsOutputTypeDef,
     SettingsTypeDef,
     CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
@@ -347,24 +372,21 @@
     GetTokenRequestRequestTypeDef,
     ImportBackendAuthRequestRequestTypeDef,
     ImportBackendStorageRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBackendJobsRequestRequestTypeDef,
     ListS3BucketsRequestRequestTypeDef,
     S3BucketInfoTypeDef,
-    LoginAuthConfigReqObjOutputTypeDef,
     LoginAuthConfigReqObjTypeDef,
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
-    BackendAPIAuthTypeOutputTypeDef,
     BackendAPIAuthTypeTypeDef,
-    SocialProviderSettingsOutputTypeDef,
     SocialProviderSettingsTypeDef,
     GetBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
@@ -387,27 +409,25 @@
     ListBackendJobsResponseTypeDef,
     RemoveAllBackendsResponseTypeDef,
     RemoveBackendConfigResponseTypeDef,
     UpdateBackendAPIResponseTypeDef,
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
-    CreateBackendAuthForgotPasswordConfigOutputTypeDef,
-    CreateBackendAuthVerificationMessageConfigOutputTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
     CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
-    UpdateBackendConfigResponseTypeDef,
     UpdateBackendConfigRequestRequestTypeDef,
+    UpdateBackendConfigResponseTypeDef,
     BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
     CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
     GetBackendStorageResponseTypeDef,
     CreateBackendStorageRequestRequestTypeDef,
@@ -425,15 +445,15 @@
     UpdateBackendAuthResourceConfigTypeDef,
     GetBackendAuthResponseTypeDef,
     CreateBackendAuthRequestRequestTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsOutputTypeDef:
+def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__init__.py` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__init__.pyi` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/__main__.py` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyBackend 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.AmplifyBackend 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend\nOther"
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

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/client.py` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/client.pyi` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/literals.py` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/literals.pyi` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/paginator.py` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/paginator.pyi` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/type_defs.py` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifybackend service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsOutputTypeDef
+    from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
 
-    data: BackendAPIAppSyncAuthSettingsOutputTypeDef = {...}
+    data: BackendAPIAppSyncAuthSettingsTypeDef = {...}
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AdditionalConstraintsElementType,
@@ -38,32 +38,25 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "BackendAPIAppSyncAuthSettingsOutputTypeDef",
     "BackendAPIAppSyncAuthSettingsTypeDef",
-    "BackendAPIConflictResolutionOutputTypeDef",
     "BackendAPIConflictResolutionTypeDef",
-    "BackendAuthAppleProviderConfigOutputTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
-    "BackendAuthSocialProviderConfigOutputTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
     "BackendStoragePermissionsOutputTypeDef",
     "BackendStoragePermissionsTypeDef",
     "CloneBackendRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "EmailSettingsOutputTypeDef",
-    "SmsSettingsOutputTypeDef",
     "EmailSettingsTypeDef",
     "SmsSettingsTypeDef",
-    "CreateBackendAuthIdentityPoolConfigOutputTypeDef",
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     "SettingsOutputTypeDef",
     "SettingsTypeDef",
     "CreateBackendAuthPasswordPolicyConfigOutputTypeDef",
     "CreateBackendAuthPasswordPolicyConfigTypeDef",
     "CreateBackendConfigRequestRequestTypeDef",
     "CreateBackendRequestRequestTypeDef",
@@ -81,24 +74,21 @@
     "GetTokenRequestRequestTypeDef",
     "ImportBackendAuthRequestRequestTypeDef",
     "ImportBackendStorageRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListBackendJobsRequestRequestTypeDef",
     "ListS3BucketsRequestRequestTypeDef",
     "S3BucketInfoTypeDef",
-    "LoginAuthConfigReqObjOutputTypeDef",
     "LoginAuthConfigReqObjTypeDef",
     "RemoveAllBackendsRequestRequestTypeDef",
     "RemoveBackendConfigRequestRequestTypeDef",
     "UpdateBackendAuthIdentityPoolConfigTypeDef",
     "UpdateBackendAuthPasswordPolicyConfigTypeDef",
     "UpdateBackendJobRequestRequestTypeDef",
-    "BackendAPIAuthTypeOutputTypeDef",
     "BackendAPIAuthTypeTypeDef",
-    "SocialProviderSettingsOutputTypeDef",
     "SocialProviderSettingsTypeDef",
     "GetBackendStorageResourceConfigTypeDef",
     "CreateBackendStorageResourceConfigTypeDef",
     "UpdateBackendStorageResourceConfigTypeDef",
     "CloneBackendResponseTypeDef",
     "CreateBackendAPIResponseTypeDef",
     "CreateBackendAuthResponseTypeDef",
@@ -121,27 +111,25 @@
     "ListBackendJobsResponseTypeDef",
     "RemoveAllBackendsResponseTypeDef",
     "RemoveBackendConfigResponseTypeDef",
     "UpdateBackendAPIResponseTypeDef",
     "UpdateBackendAuthResponseTypeDef",
     "UpdateBackendJobResponseTypeDef",
     "UpdateBackendStorageResponseTypeDef",
-    "CreateBackendAuthForgotPasswordConfigOutputTypeDef",
-    "CreateBackendAuthVerificationMessageConfigOutputTypeDef",
     "CreateBackendAuthForgotPasswordConfigTypeDef",
     "CreateBackendAuthVerificationMessageConfigTypeDef",
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     "UpdateBackendAuthVerificationMessageConfigTypeDef",
     "CreateBackendAuthMFAConfigOutputTypeDef",
     "CreateBackendAuthMFAConfigTypeDef",
     "UpdateBackendAuthMFAConfigTypeDef",
     "ListBackendJobsRequestListBackendJobsPaginateTypeDef",
     "ListS3BucketsResponseTypeDef",
-    "UpdateBackendConfigResponseTypeDef",
     "UpdateBackendConfigRequestRequestTypeDef",
+    "UpdateBackendConfigResponseTypeDef",
     "BackendAPIResourceConfigOutputTypeDef",
     "BackendAPIResourceConfigTypeDef",
     "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
     "GetBackendStorageResponseTypeDef",
     "CreateBackendStorageRequestRequestTypeDef",
@@ -158,29 +146,14 @@
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
     "GetBackendAuthResponseTypeDef",
     "CreateBackendAuthRequestRequestTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
-BackendAPIAppSyncAuthSettingsOutputTypeDef = TypedDict(
-    "BackendAPIAppSyncAuthSettingsOutputTypeDef",
-    {
-        "CognitoUserPoolId": str,
-        "Description": str,
-        "ExpirationTime": float,
-        "OpenIDAuthTTL": str,
-        "OpenIDClientId": str,
-        "OpenIDIatTTL": str,
-        "OpenIDIssueURL": str,
-        "OpenIDProviderName": str,
-    },
-    total=False,
-)
-
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
         "Description": str,
         "ExpirationTime": float,
         "OpenIDAuthTTL": str,
@@ -188,61 +161,33 @@
         "OpenIDIatTTL": str,
         "OpenIDIssueURL": str,
         "OpenIDProviderName": str,
     },
     total=False,
 )
 
-BackendAPIConflictResolutionOutputTypeDef = TypedDict(
-    "BackendAPIConflictResolutionOutputTypeDef",
-    {
-        "ResolutionStrategy": ResolutionStrategyType,
-    },
-    total=False,
-)
-
 BackendAPIConflictResolutionTypeDef = TypedDict(
     "BackendAPIConflictResolutionTypeDef",
     {
         "ResolutionStrategy": ResolutionStrategyType,
     },
     total=False,
 )
 
-BackendAuthAppleProviderConfigOutputTypeDef = TypedDict(
-    "BackendAuthAppleProviderConfigOutputTypeDef",
-    {
-        "ClientId": str,
-        "KeyId": str,
-        "PrivateKey": str,
-        "TeamId": str,
-    },
-    total=False,
-)
-
 BackendAuthAppleProviderConfigTypeDef = TypedDict(
     "BackendAuthAppleProviderConfigTypeDef",
     {
         "ClientId": str,
         "KeyId": str,
         "PrivateKey": str,
         "TeamId": str,
     },
     total=False,
 )
 
-BackendAuthSocialProviderConfigOutputTypeDef = TypedDict(
-    "BackendAuthSocialProviderConfigOutputTypeDef",
-    {
-        "ClientId": str,
-        "ClientSecret": str,
-    },
-    total=False,
-)
-
 BackendAuthSocialProviderConfigTypeDef = TypedDict(
     "BackendAuthSocialProviderConfigTypeDef",
     {
         "ClientId": str,
         "ClientSecret": str,
     },
     total=False,
@@ -333,31 +278,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-EmailSettingsOutputTypeDef = TypedDict(
-    "EmailSettingsOutputTypeDef",
-    {
-        "EmailMessage": str,
-        "EmailSubject": str,
-    },
-    total=False,
-)
-
-SmsSettingsOutputTypeDef = TypedDict(
-    "SmsSettingsOutputTypeDef",
-    {
-        "SmsMessage": str,
-    },
-    total=False,
-)
-
 EmailSettingsTypeDef = TypedDict(
     "EmailSettingsTypeDef",
     {
         "EmailMessage": str,
         "EmailSubject": str,
     },
     total=False,
@@ -367,22 +295,14 @@
     "SmsSettingsTypeDef",
     {
         "SmsMessage": str,
     },
     total=False,
 )
 
-CreateBackendAuthIdentityPoolConfigOutputTypeDef = TypedDict(
-    "CreateBackendAuthIdentityPoolConfigOutputTypeDef",
-    {
-        "IdentityPoolName": str,
-        "UnauthenticatedLogin": bool,
-    },
-)
-
 CreateBackendAuthIdentityPoolConfigTypeDef = TypedDict(
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     {
         "IdentityPoolName": str,
         "UnauthenticatedLogin": bool,
     },
 )
@@ -709,25 +629,14 @@
     {
         "CreationDate": str,
         "Name": str,
     },
     total=False,
 )
 
-LoginAuthConfigReqObjOutputTypeDef = TypedDict(
-    "LoginAuthConfigReqObjOutputTypeDef",
-    {
-        "AwsCognitoIdentityPoolId": str,
-        "AwsCognitoRegion": str,
-        "AwsUserPoolsId": str,
-        "AwsUserPoolsWebClientId": str,
-    },
-    total=False,
-)
-
 LoginAuthConfigReqObjTypeDef = TypedDict(
     "LoginAuthConfigReqObjTypeDef",
     {
         "AwsCognitoIdentityPoolId": str,
         "AwsCognitoRegion": str,
         "AwsUserPoolsId": str,
         "AwsUserPoolsWebClientId": str,
@@ -800,43 +709,23 @@
 
 class UpdateBackendJobRequestRequestTypeDef(
     _RequiredUpdateBackendJobRequestRequestTypeDef, _OptionalUpdateBackendJobRequestRequestTypeDef
 ):
     pass
 
 
-BackendAPIAuthTypeOutputTypeDef = TypedDict(
-    "BackendAPIAuthTypeOutputTypeDef",
-    {
-        "Mode": ModeType,
-        "Settings": BackendAPIAppSyncAuthSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 BackendAPIAuthTypeTypeDef = TypedDict(
     "BackendAPIAuthTypeTypeDef",
     {
         "Mode": ModeType,
         "Settings": BackendAPIAppSyncAuthSettingsTypeDef,
     },
     total=False,
 )
 
-SocialProviderSettingsOutputTypeDef = TypedDict(
-    "SocialProviderSettingsOutputTypeDef",
-    {
-        "Facebook": BackendAuthSocialProviderConfigOutputTypeDef,
-        "Google": BackendAuthSocialProviderConfigOutputTypeDef,
-        "LoginWithAmazon": BackendAuthSocialProviderConfigOutputTypeDef,
-        "SignInWithApple": BackendAuthAppleProviderConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 SocialProviderSettingsTypeDef = TypedDict(
     "SocialProviderSettingsTypeDef",
     {
         "Facebook": BackendAuthSocialProviderConfigTypeDef,
         "Google": BackendAuthSocialProviderConfigTypeDef,
         "LoginWithAmazon": BackendAuthSocialProviderConfigTypeDef,
         "SignInWithApple": BackendAuthAppleProviderConfigTypeDef,
@@ -1205,60 +1094,14 @@
         "BackendEnvironmentName": str,
         "JobId": str,
         "Status": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef",
-    {
-        "DeliveryMethod": DeliveryMethodType,
-    },
-)
-_OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef",
-    {
-        "EmailSettings": EmailSettingsOutputTypeDef,
-        "SmsSettings": SmsSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateBackendAuthForgotPasswordConfigOutputTypeDef(
-    _RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef,
-    _OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef,
-):
-    pass
-
-
-_RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef",
-    {
-        "DeliveryMethod": DeliveryMethodType,
-    },
-)
-_OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef",
-    {
-        "EmailSettings": EmailSettingsOutputTypeDef,
-        "SmsSettings": SmsSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateBackendAuthVerificationMessageConfigOutputTypeDef(
-    _RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef,
-    _OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthForgotPasswordConfigTypeDef",
     {
         "DeliveryMethod": DeliveryMethodType,
     },
 )
 _OptionalCreateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
@@ -1417,25 +1260,14 @@
     {
         "Buckets": List[S3BucketInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBackendConfigResponseTypeDef = TypedDict(
-    "UpdateBackendConfigResponseTypeDef",
-    {
-        "AppId": str,
-        "BackendManagerAppId": str,
-        "Error": str,
-        "LoginAuthConfig": LoginAuthConfigReqObjOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateBackendConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendConfigRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 _OptionalUpdateBackendConfigRequestRequestTypeDef = TypedDict(
@@ -1450,21 +1282,32 @@
 class UpdateBackendConfigRequestRequestTypeDef(
     _RequiredUpdateBackendConfigRequestRequestTypeDef,
     _OptionalUpdateBackendConfigRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateBackendConfigResponseTypeDef = TypedDict(
+    "UpdateBackendConfigResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendManagerAppId": str,
+        "Error": str,
+        "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BackendAPIResourceConfigOutputTypeDef = TypedDict(
     "BackendAPIResourceConfigOutputTypeDef",
     {
-        "AdditionalAuthTypes": List[BackendAPIAuthTypeOutputTypeDef],
+        "AdditionalAuthTypes": List[BackendAPIAuthTypeTypeDef],
         "ApiName": str,
-        "ConflictResolution": BackendAPIConflictResolutionOutputTypeDef,
-        "DefaultAuthType": BackendAPIAuthTypeOutputTypeDef,
+        "ConflictResolution": BackendAPIConflictResolutionTypeDef,
+        "DefaultAuthType": BackendAPIAuthTypeTypeDef,
         "Service": str,
         "TransformSchema": str,
     },
     total=False,
 )
 
 BackendAPIResourceConfigTypeDef = TypedDict(
@@ -1489,15 +1332,15 @@
         "RedirectSignOutURIs": List[str],
     },
 )
 _OptionalCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
     "_OptionalCreateBackendAuthOAuthConfigOutputTypeDef",
     {
         "DomainPrefix": str,
-        "SocialProviderSettings": SocialProviderSettingsOutputTypeDef,
+        "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
 
 class CreateBackendAuthOAuthConfigOutputTypeDef(
     _RequiredCreateBackendAuthOAuthConfigOutputTypeDef,
@@ -1673,19 +1516,19 @@
         "SignInMethod": SignInMethodType,
         "UserPoolName": str,
     },
 )
 _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
     "_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef",
     {
-        "ForgotPassword": CreateBackendAuthForgotPasswordConfigOutputTypeDef,
+        "ForgotPassword": CreateBackendAuthForgotPasswordConfigTypeDef,
         "Mfa": CreateBackendAuthMFAConfigOutputTypeDef,
         "OAuth": CreateBackendAuthOAuthConfigOutputTypeDef,
         "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
-        "VerificationMessage": CreateBackendAuthVerificationMessageConfigOutputTypeDef,
+        "VerificationMessage": CreateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
 
 class CreateBackendAuthUserPoolConfigOutputTypeDef(
     _RequiredCreateBackendAuthUserPoolConfigOutputTypeDef,
@@ -1740,15 +1583,15 @@
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": CreateBackendAuthUserPoolConfigOutputTypeDef,
     },
 )
 _OptionalCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
     "_OptionalCreateBackendAuthResourceConfigOutputTypeDef",
     {
-        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigOutputTypeDef,
+        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigTypeDef,
     },
     total=False,
 )
 
 
 class CreateBackendAuthResourceConfigOutputTypeDef(
     _RequiredCreateBackendAuthResourceConfigOutputTypeDef,
```

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend/type_defs.pyi` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifybackend service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsOutputTypeDef
+    from mypy_boto3_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
 
-    data: BackendAPIAppSyncAuthSettingsOutputTypeDef = {...}
+    data: BackendAPIAppSyncAuthSettingsTypeDef = {...}
     ```
 """
 import sys
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AdditionalConstraintsElementType,
@@ -37,32 +37,25 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "BackendAPIAppSyncAuthSettingsOutputTypeDef",
     "BackendAPIAppSyncAuthSettingsTypeDef",
-    "BackendAPIConflictResolutionOutputTypeDef",
     "BackendAPIConflictResolutionTypeDef",
-    "BackendAuthAppleProviderConfigOutputTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
-    "BackendAuthSocialProviderConfigOutputTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
     "BackendStoragePermissionsOutputTypeDef",
     "BackendStoragePermissionsTypeDef",
     "CloneBackendRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "EmailSettingsOutputTypeDef",
-    "SmsSettingsOutputTypeDef",
     "EmailSettingsTypeDef",
     "SmsSettingsTypeDef",
-    "CreateBackendAuthIdentityPoolConfigOutputTypeDef",
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     "SettingsOutputTypeDef",
     "SettingsTypeDef",
     "CreateBackendAuthPasswordPolicyConfigOutputTypeDef",
     "CreateBackendAuthPasswordPolicyConfigTypeDef",
     "CreateBackendConfigRequestRequestTypeDef",
     "CreateBackendRequestRequestTypeDef",
@@ -80,24 +73,21 @@
     "GetTokenRequestRequestTypeDef",
     "ImportBackendAuthRequestRequestTypeDef",
     "ImportBackendStorageRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListBackendJobsRequestRequestTypeDef",
     "ListS3BucketsRequestRequestTypeDef",
     "S3BucketInfoTypeDef",
-    "LoginAuthConfigReqObjOutputTypeDef",
     "LoginAuthConfigReqObjTypeDef",
     "RemoveAllBackendsRequestRequestTypeDef",
     "RemoveBackendConfigRequestRequestTypeDef",
     "UpdateBackendAuthIdentityPoolConfigTypeDef",
     "UpdateBackendAuthPasswordPolicyConfigTypeDef",
     "UpdateBackendJobRequestRequestTypeDef",
-    "BackendAPIAuthTypeOutputTypeDef",
     "BackendAPIAuthTypeTypeDef",
-    "SocialProviderSettingsOutputTypeDef",
     "SocialProviderSettingsTypeDef",
     "GetBackendStorageResourceConfigTypeDef",
     "CreateBackendStorageResourceConfigTypeDef",
     "UpdateBackendStorageResourceConfigTypeDef",
     "CloneBackendResponseTypeDef",
     "CreateBackendAPIResponseTypeDef",
     "CreateBackendAuthResponseTypeDef",
@@ -120,27 +110,25 @@
     "ListBackendJobsResponseTypeDef",
     "RemoveAllBackendsResponseTypeDef",
     "RemoveBackendConfigResponseTypeDef",
     "UpdateBackendAPIResponseTypeDef",
     "UpdateBackendAuthResponseTypeDef",
     "UpdateBackendJobResponseTypeDef",
     "UpdateBackendStorageResponseTypeDef",
-    "CreateBackendAuthForgotPasswordConfigOutputTypeDef",
-    "CreateBackendAuthVerificationMessageConfigOutputTypeDef",
     "CreateBackendAuthForgotPasswordConfigTypeDef",
     "CreateBackendAuthVerificationMessageConfigTypeDef",
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     "UpdateBackendAuthVerificationMessageConfigTypeDef",
     "CreateBackendAuthMFAConfigOutputTypeDef",
     "CreateBackendAuthMFAConfigTypeDef",
     "UpdateBackendAuthMFAConfigTypeDef",
     "ListBackendJobsRequestListBackendJobsPaginateTypeDef",
     "ListS3BucketsResponseTypeDef",
-    "UpdateBackendConfigResponseTypeDef",
     "UpdateBackendConfigRequestRequestTypeDef",
+    "UpdateBackendConfigResponseTypeDef",
     "BackendAPIResourceConfigOutputTypeDef",
     "BackendAPIResourceConfigTypeDef",
     "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
     "GetBackendStorageResponseTypeDef",
     "CreateBackendStorageRequestRequestTypeDef",
@@ -157,29 +145,14 @@
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
     "GetBackendAuthResponseTypeDef",
     "CreateBackendAuthRequestRequestTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
-BackendAPIAppSyncAuthSettingsOutputTypeDef = TypedDict(
-    "BackendAPIAppSyncAuthSettingsOutputTypeDef",
-    {
-        "CognitoUserPoolId": str,
-        "Description": str,
-        "ExpirationTime": float,
-        "OpenIDAuthTTL": str,
-        "OpenIDClientId": str,
-        "OpenIDIatTTL": str,
-        "OpenIDIssueURL": str,
-        "OpenIDProviderName": str,
-    },
-    total=False,
-)
-
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
         "Description": str,
         "ExpirationTime": float,
         "OpenIDAuthTTL": str,
@@ -187,61 +160,33 @@
         "OpenIDIatTTL": str,
         "OpenIDIssueURL": str,
         "OpenIDProviderName": str,
     },
     total=False,
 )
 
-BackendAPIConflictResolutionOutputTypeDef = TypedDict(
-    "BackendAPIConflictResolutionOutputTypeDef",
-    {
-        "ResolutionStrategy": ResolutionStrategyType,
-    },
-    total=False,
-)
-
 BackendAPIConflictResolutionTypeDef = TypedDict(
     "BackendAPIConflictResolutionTypeDef",
     {
         "ResolutionStrategy": ResolutionStrategyType,
     },
     total=False,
 )
 
-BackendAuthAppleProviderConfigOutputTypeDef = TypedDict(
-    "BackendAuthAppleProviderConfigOutputTypeDef",
-    {
-        "ClientId": str,
-        "KeyId": str,
-        "PrivateKey": str,
-        "TeamId": str,
-    },
-    total=False,
-)
-
 BackendAuthAppleProviderConfigTypeDef = TypedDict(
     "BackendAuthAppleProviderConfigTypeDef",
     {
         "ClientId": str,
         "KeyId": str,
         "PrivateKey": str,
         "TeamId": str,
     },
     total=False,
 )
 
-BackendAuthSocialProviderConfigOutputTypeDef = TypedDict(
-    "BackendAuthSocialProviderConfigOutputTypeDef",
-    {
-        "ClientId": str,
-        "ClientSecret": str,
-    },
-    total=False,
-)
-
 BackendAuthSocialProviderConfigTypeDef = TypedDict(
     "BackendAuthSocialProviderConfigTypeDef",
     {
         "ClientId": str,
         "ClientSecret": str,
     },
     total=False,
@@ -326,31 +271,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-EmailSettingsOutputTypeDef = TypedDict(
-    "EmailSettingsOutputTypeDef",
-    {
-        "EmailMessage": str,
-        "EmailSubject": str,
-    },
-    total=False,
-)
-
-SmsSettingsOutputTypeDef = TypedDict(
-    "SmsSettingsOutputTypeDef",
-    {
-        "SmsMessage": str,
-    },
-    total=False,
-)
-
 EmailSettingsTypeDef = TypedDict(
     "EmailSettingsTypeDef",
     {
         "EmailMessage": str,
         "EmailSubject": str,
     },
     total=False,
@@ -360,22 +288,14 @@
     "SmsSettingsTypeDef",
     {
         "SmsMessage": str,
     },
     total=False,
 )
 
-CreateBackendAuthIdentityPoolConfigOutputTypeDef = TypedDict(
-    "CreateBackendAuthIdentityPoolConfigOutputTypeDef",
-    {
-        "IdentityPoolName": str,
-        "UnauthenticatedLogin": bool,
-    },
-)
-
 CreateBackendAuthIdentityPoolConfigTypeDef = TypedDict(
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     {
         "IdentityPoolName": str,
         "UnauthenticatedLogin": bool,
     },
 )
@@ -686,25 +606,14 @@
     {
         "CreationDate": str,
         "Name": str,
     },
     total=False,
 )
 
-LoginAuthConfigReqObjOutputTypeDef = TypedDict(
-    "LoginAuthConfigReqObjOutputTypeDef",
-    {
-        "AwsCognitoIdentityPoolId": str,
-        "AwsCognitoRegion": str,
-        "AwsUserPoolsId": str,
-        "AwsUserPoolsWebClientId": str,
-    },
-    total=False,
-)
-
 LoginAuthConfigReqObjTypeDef = TypedDict(
     "LoginAuthConfigReqObjTypeDef",
     {
         "AwsCognitoIdentityPoolId": str,
         "AwsCognitoRegion": str,
         "AwsUserPoolsId": str,
         "AwsUserPoolsWebClientId": str,
@@ -773,43 +682,23 @@
 )
 
 class UpdateBackendJobRequestRequestTypeDef(
     _RequiredUpdateBackendJobRequestRequestTypeDef, _OptionalUpdateBackendJobRequestRequestTypeDef
 ):
     pass
 
-BackendAPIAuthTypeOutputTypeDef = TypedDict(
-    "BackendAPIAuthTypeOutputTypeDef",
-    {
-        "Mode": ModeType,
-        "Settings": BackendAPIAppSyncAuthSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 BackendAPIAuthTypeTypeDef = TypedDict(
     "BackendAPIAuthTypeTypeDef",
     {
         "Mode": ModeType,
         "Settings": BackendAPIAppSyncAuthSettingsTypeDef,
     },
     total=False,
 )
 
-SocialProviderSettingsOutputTypeDef = TypedDict(
-    "SocialProviderSettingsOutputTypeDef",
-    {
-        "Facebook": BackendAuthSocialProviderConfigOutputTypeDef,
-        "Google": BackendAuthSocialProviderConfigOutputTypeDef,
-        "LoginWithAmazon": BackendAuthSocialProviderConfigOutputTypeDef,
-        "SignInWithApple": BackendAuthAppleProviderConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 SocialProviderSettingsTypeDef = TypedDict(
     "SocialProviderSettingsTypeDef",
     {
         "Facebook": BackendAuthSocialProviderConfigTypeDef,
         "Google": BackendAuthSocialProviderConfigTypeDef,
         "LoginWithAmazon": BackendAuthSocialProviderConfigTypeDef,
         "SignInWithApple": BackendAuthAppleProviderConfigTypeDef,
@@ -1174,56 +1063,14 @@
         "BackendEnvironmentName": str,
         "JobId": str,
         "Status": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef",
-    {
-        "DeliveryMethod": DeliveryMethodType,
-    },
-)
-_OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef",
-    {
-        "EmailSettings": EmailSettingsOutputTypeDef,
-        "SmsSettings": SmsSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class CreateBackendAuthForgotPasswordConfigOutputTypeDef(
-    _RequiredCreateBackendAuthForgotPasswordConfigOutputTypeDef,
-    _OptionalCreateBackendAuthForgotPasswordConfigOutputTypeDef,
-):
-    pass
-
-_RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef",
-    {
-        "DeliveryMethod": DeliveryMethodType,
-    },
-)
-_OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef",
-    {
-        "EmailSettings": EmailSettingsOutputTypeDef,
-        "SmsSettings": SmsSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class CreateBackendAuthVerificationMessageConfigOutputTypeDef(
-    _RequiredCreateBackendAuthVerificationMessageConfigOutputTypeDef,
-    _OptionalCreateBackendAuthVerificationMessageConfigOutputTypeDef,
-):
-    pass
-
 _RequiredCreateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthForgotPasswordConfigTypeDef",
     {
         "DeliveryMethod": DeliveryMethodType,
     },
 )
 _OptionalCreateBackendAuthForgotPasswordConfigTypeDef = TypedDict(
@@ -1370,25 +1217,14 @@
     {
         "Buckets": List[S3BucketInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateBackendConfigResponseTypeDef = TypedDict(
-    "UpdateBackendConfigResponseTypeDef",
-    {
-        "AppId": str,
-        "BackendManagerAppId": str,
-        "Error": str,
-        "LoginAuthConfig": LoginAuthConfigReqObjOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredUpdateBackendConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendConfigRequestRequestTypeDef",
     {
         "AppId": str,
     },
 )
 _OptionalUpdateBackendConfigRequestRequestTypeDef = TypedDict(
@@ -1401,21 +1237,32 @@
 
 class UpdateBackendConfigRequestRequestTypeDef(
     _RequiredUpdateBackendConfigRequestRequestTypeDef,
     _OptionalUpdateBackendConfigRequestRequestTypeDef,
 ):
     pass
 
+UpdateBackendConfigResponseTypeDef = TypedDict(
+    "UpdateBackendConfigResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendManagerAppId": str,
+        "Error": str,
+        "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BackendAPIResourceConfigOutputTypeDef = TypedDict(
     "BackendAPIResourceConfigOutputTypeDef",
     {
-        "AdditionalAuthTypes": List[BackendAPIAuthTypeOutputTypeDef],
+        "AdditionalAuthTypes": List[BackendAPIAuthTypeTypeDef],
         "ApiName": str,
-        "ConflictResolution": BackendAPIConflictResolutionOutputTypeDef,
-        "DefaultAuthType": BackendAPIAuthTypeOutputTypeDef,
+        "ConflictResolution": BackendAPIConflictResolutionTypeDef,
+        "DefaultAuthType": BackendAPIAuthTypeTypeDef,
         "Service": str,
         "TransformSchema": str,
     },
     total=False,
 )
 
 BackendAPIResourceConfigTypeDef = TypedDict(
@@ -1440,15 +1287,15 @@
         "RedirectSignOutURIs": List[str],
     },
 )
 _OptionalCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
     "_OptionalCreateBackendAuthOAuthConfigOutputTypeDef",
     {
         "DomainPrefix": str,
-        "SocialProviderSettings": SocialProviderSettingsOutputTypeDef,
+        "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
 class CreateBackendAuthOAuthConfigOutputTypeDef(
     _RequiredCreateBackendAuthOAuthConfigOutputTypeDef,
     _OptionalCreateBackendAuthOAuthConfigOutputTypeDef,
@@ -1614,19 +1461,19 @@
         "SignInMethod": SignInMethodType,
         "UserPoolName": str,
     },
 )
 _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
     "_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef",
     {
-        "ForgotPassword": CreateBackendAuthForgotPasswordConfigOutputTypeDef,
+        "ForgotPassword": CreateBackendAuthForgotPasswordConfigTypeDef,
         "Mfa": CreateBackendAuthMFAConfigOutputTypeDef,
         "OAuth": CreateBackendAuthOAuthConfigOutputTypeDef,
         "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
-        "VerificationMessage": CreateBackendAuthVerificationMessageConfigOutputTypeDef,
+        "VerificationMessage": CreateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
 class CreateBackendAuthUserPoolConfigOutputTypeDef(
     _RequiredCreateBackendAuthUserPoolConfigOutputTypeDef,
     _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef,
@@ -1677,15 +1524,15 @@
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": CreateBackendAuthUserPoolConfigOutputTypeDef,
     },
 )
 _OptionalCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
     "_OptionalCreateBackendAuthResourceConfigOutputTypeDef",
     {
-        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigOutputTypeDef,
+        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigTypeDef,
     },
     total=False,
 )
 
 class CreateBackendAuthResourceConfigOutputTypeDef(
     _RequiredCreateBackendAuthResourceConfigOutputTypeDef,
     _OptionalCreateBackendAuthResourceConfigOutputTypeDef,
```

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/PKG-INFO` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifybackend
-Version: 1.28.12
-Summary: Type annotations for boto3.AmplifyBackend 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AmplifyBackend 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifybackend.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifybackend)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifybackend)](https://pepy.tech/project/mypy-boto3-amplifybackend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyBackend 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
+[boto3.AmplifyBackend 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend)
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
 [mypy-boto3-amplifybackend docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifybackend/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,32 +336,25 @@
 ### Typed dictionaries
 
 `mypy_boto3_amplifybackend.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifybackend.type_defs import (
-    BackendAPIAppSyncAuthSettingsOutputTypeDef,
     BackendAPIAppSyncAuthSettingsTypeDef,
-    BackendAPIConflictResolutionOutputTypeDef,
     BackendAPIConflictResolutionTypeDef,
-    BackendAuthAppleProviderConfigOutputTypeDef,
     BackendAuthAppleProviderConfigTypeDef,
-    BackendAuthSocialProviderConfigOutputTypeDef,
     BackendAuthSocialProviderConfigTypeDef,
     BackendJobRespObjTypeDef,
     BackendStoragePermissionsOutputTypeDef,
     BackendStoragePermissionsTypeDef,
     CloneBackendRequestRequestTypeDef,
     ResponseMetadataTypeDef,
-    EmailSettingsOutputTypeDef,
-    SmsSettingsOutputTypeDef,
     EmailSettingsTypeDef,
     SmsSettingsTypeDef,
-    CreateBackendAuthIdentityPoolConfigOutputTypeDef,
     CreateBackendAuthIdentityPoolConfigTypeDef,
     SettingsOutputTypeDef,
     SettingsTypeDef,
     CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
     CreateBackendAuthPasswordPolicyConfigTypeDef,
     CreateBackendConfigRequestRequestTypeDef,
     CreateBackendRequestRequestTypeDef,
@@ -379,24 +372,21 @@
     GetTokenRequestRequestTypeDef,
     ImportBackendAuthRequestRequestTypeDef,
     ImportBackendStorageRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     ListBackendJobsRequestRequestTypeDef,
     ListS3BucketsRequestRequestTypeDef,
     S3BucketInfoTypeDef,
-    LoginAuthConfigReqObjOutputTypeDef,
     LoginAuthConfigReqObjTypeDef,
     RemoveAllBackendsRequestRequestTypeDef,
     RemoveBackendConfigRequestRequestTypeDef,
     UpdateBackendAuthIdentityPoolConfigTypeDef,
     UpdateBackendAuthPasswordPolicyConfigTypeDef,
     UpdateBackendJobRequestRequestTypeDef,
-    BackendAPIAuthTypeOutputTypeDef,
     BackendAPIAuthTypeTypeDef,
-    SocialProviderSettingsOutputTypeDef,
     SocialProviderSettingsTypeDef,
     GetBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     UpdateBackendStorageResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
     CreateBackendAuthResponseTypeDef,
@@ -419,27 +409,25 @@
     ListBackendJobsResponseTypeDef,
     RemoveAllBackendsResponseTypeDef,
     RemoveBackendConfigResponseTypeDef,
     UpdateBackendAPIResponseTypeDef,
     UpdateBackendAuthResponseTypeDef,
     UpdateBackendJobResponseTypeDef,
     UpdateBackendStorageResponseTypeDef,
-    CreateBackendAuthForgotPasswordConfigOutputTypeDef,
-    CreateBackendAuthVerificationMessageConfigOutputTypeDef,
     CreateBackendAuthForgotPasswordConfigTypeDef,
     CreateBackendAuthVerificationMessageConfigTypeDef,
     UpdateBackendAuthForgotPasswordConfigTypeDef,
     UpdateBackendAuthVerificationMessageConfigTypeDef,
     CreateBackendAuthMFAConfigOutputTypeDef,
     CreateBackendAuthMFAConfigTypeDef,
     UpdateBackendAuthMFAConfigTypeDef,
     ListBackendJobsRequestListBackendJobsPaginateTypeDef,
     ListS3BucketsResponseTypeDef,
-    UpdateBackendConfigResponseTypeDef,
     UpdateBackendConfigRequestRequestTypeDef,
+    UpdateBackendConfigResponseTypeDef,
     BackendAPIResourceConfigOutputTypeDef,
     BackendAPIResourceConfigTypeDef,
     CreateBackendAuthOAuthConfigOutputTypeDef,
     CreateBackendAuthOAuthConfigTypeDef,
     UpdateBackendAuthOAuthConfigTypeDef,
     GetBackendStorageResponseTypeDef,
     CreateBackendStorageRequestRequestTypeDef,
@@ -457,15 +445,15 @@
     UpdateBackendAuthResourceConfigTypeDef,
     GetBackendAuthResponseTypeDef,
     CreateBackendAuthRequestRequestTypeDef,
     UpdateBackendAuthRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BackendAPIAppSyncAuthSettingsOutputTypeDef:
+def get_structure() -> BackendAPIAppSyncAuthSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-amplifybackend-1.28.12/mypy_boto3_amplifybackend.egg-info/SOURCES.txt` & `mypy-boto3-amplifybackend-1.28.15/mypy_boto3_amplifybackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifybackend-1.28.12/setup.py` & `mypy-boto3-amplifybackend-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifybackend",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_amplifybackend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AmplifyBackend 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.AmplifyBackend 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

