# Comparing `tmp/mypy-boto3-cloudhsmv2-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudhsmv2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudhsmv2-1.28.12.tar", last modified: Thu Jul 27 05:34:25 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudhsmv2-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-cloudhsmv2-1.28.12.tar` & `mypy-boto3-cloudhsmv2-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.160562 mypy-boto3-cloudhsmv2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-27 05:34:25.160562 mypy-boto3-cloudhsmv2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13043 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.156562 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-07-27 05:18:44.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:25.160562 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:25.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:24.000000 mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:25.160562 mypy-boto3-cloudhsmv2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:18:43.000000 mypy-boto3-cloudhsmv2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.532782 mypy-boto3-cloudhsmv2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-07-28 20:42:25.528782 mypy-boto3-cloudhsmv2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.520782 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-28 20:21:00.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13013 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:59.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.528782 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14474 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:25.000000 mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.532782 mypy-boto3-cloudhsmv2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:20:58.000000 mypy-boto3-cloudhsmv2-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/LICENSE` & `mypy-boto3-cloudhsmv2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/PKG-INFO` & `mypy-boto3-cloudhsmv2-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsmv2
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudHSMV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudHSMV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsmv2)](https://pepy.tech/project/mypy-boto3-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSMV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[boto3.CloudHSMV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [mypy-boto3-cloudhsmv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,60 +331,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_cloudhsmv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsmv2.type_defs import (
-    BackupRetentionPolicyOutputTypeDef,
     BackupRetentionPolicyTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
-    TagTypeDef,
     DestinationBackupTypeDef,
+    ResponseMetadataTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
     InitializeClusterRequestRequestTypeDef,
-    InitializeClusterResponseTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     ModifyBackupAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
-    ListTagsResponseTypeDef,
-    ClusterTypeDef,
-    CreateHsmResponseTypeDef,
     CopyBackupToRegionRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    ClusterTypeDef,
     CopyBackupToRegionResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    InitializeClusterResponseTypeDef,
+    ListTagsResponseTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyOutputTypeDef:
+def get_structure() -> BackupRetentionPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/README.md` & `mypy-boto3-cloudhsmv2-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsmv2)](https://pepy.tech/project/mypy-boto3-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSMV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[boto3.CloudHSMV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [mypy-boto3-cloudhsmv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,60 +299,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_cloudhsmv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsmv2.type_defs import (
-    BackupRetentionPolicyOutputTypeDef,
     BackupRetentionPolicyTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
-    TagTypeDef,
     DestinationBackupTypeDef,
+    ResponseMetadataTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
     InitializeClusterRequestRequestTypeDef,
-    InitializeClusterResponseTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     ModifyBackupAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
-    ListTagsResponseTypeDef,
-    ClusterTypeDef,
-    CreateHsmResponseTypeDef,
     CopyBackupToRegionRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    ClusterTypeDef,
     CopyBackupToRegionResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    InitializeClusterResponseTypeDef,
+    ListTagsResponseTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyOutputTypeDef:
+def get_structure() -> BackupRetentionPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__init__.py` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__init__.pyi` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/__main__.py` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudHSMV2 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudHSMV2 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2\nOther"
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

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/client.py` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/client.pyi` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/literals.py` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/literals.pyi` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/paginator.py` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
         SortAscending: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#describebackupspaginator)
         """
 
 
@@ -72,28 +72,28 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#describeclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#describeclusterspaginator)
         """
 
 
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#listtagspaginator)
         """
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/paginator.pyi` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
         SortAscending: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeBackups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#describebackupspaginator)
         """
 
 class DescribeClustersPaginator(Paginator):
@@ -68,27 +68,27 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#describeclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#describeclusterspaginator)
         """
 
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/paginators/#listtagspaginator)
         """
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/type_defs.py` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cloudhsmv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cloudhsmv2.type_defs import BackupRetentionPolicyOutputTypeDef
+    from mypy_boto3_cloudhsmv2.type_defs import BackupRetentionPolicyTypeDef
 
-    data: BackupRetentionPolicyOutputTypeDef = {...}
+    data: BackupRetentionPolicyTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import BackupStateType, ClusterStateType, HsmStateType
@@ -24,78 +24,67 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "BackupRetentionPolicyOutputTypeDef",
     "BackupRetentionPolicyTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "CertificatesTypeDef",
     "HsmTypeDef",
-    "TagTypeDef",
     "DestinationBackupTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateHsmRequestRequestTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteHsmRequestRequestTypeDef",
-    "DeleteHsmResponseTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "InitializeClusterRequestRequestTypeDef",
-    "InitializeClusterResponseTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ModifyBackupAttributesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreBackupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ModifyClusterRequestRequestTypeDef",
     "BackupTypeDef",
-    "ListTagsResponseTypeDef",
-    "ClusterTypeDef",
-    "CreateHsmResponseTypeDef",
     "CopyBackupToRegionRequestRequestTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ClusterTypeDef",
     "CopyBackupToRegionResponseTypeDef",
+    "CreateHsmResponseTypeDef",
+    "DeleteHsmResponseTypeDef",
+    "InitializeClusterResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "DeleteBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "ModifyBackupAttributesResponseTypeDef",
     "RestoreBackupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DescribeClustersResponseTypeDef",
     "ModifyClusterResponseTypeDef",
 )
 
-BackupRetentionPolicyOutputTypeDef = TypedDict(
-    "BackupRetentionPolicyOutputTypeDef",
-    {
-        "Type": Literal["DAYS"],
-        "Value": str,
-    },
-    total=False,
-)
-
 BackupRetentionPolicyTypeDef = TypedDict(
     "BackupRetentionPolicyTypeDef",
     {
         "Type": Literal["DAYS"],
         "Value": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 CertificatesTypeDef = TypedDict(
@@ -131,33 +120,36 @@
 )
 
 
 class HsmTypeDef(_RequiredHsmTypeDef, _OptionalHsmTypeDef):
     pass
 
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 DestinationBackupTypeDef = TypedDict(
     "DestinationBackupTypeDef",
     {
         "CreateTimestamp": datetime,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "ClusterId": str,
         "AvailabilityZone": str,
     },
 )
@@ -209,28 +201,20 @@
 
 class DeleteHsmRequestRequestTypeDef(
     _RequiredDeleteHsmRequestRequestTypeDef, _OptionalDeleteHsmRequestRequestTypeDef
 ):
     pass
 
 
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "HsmId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Filters": Mapping[str, Sequence[str]],
-        "SortAscending": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
@@ -238,23 +222,14 @@
         "MaxResults": int,
         "Filters": Mapping[str, Sequence[str]],
         "SortAscending": bool,
     },
     total=False,
 )
 
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    {
-        "Filters": Mapping[str, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -266,44 +241,14 @@
     {
         "ClusterId": str,
         "SignedCert": str,
         "TrustAnchor": str,
     },
 )
 
-InitializeClusterResponseTypeDef = TypedDict(
-    "InitializeClusterResponseTypeDef",
-    {
-        "State": ClusterStateType,
-        "StateMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -326,35 +271,14 @@
     "ModifyBackupAttributesRequestRequestTypeDef",
     {
         "BackupId": str,
         "NeverExpires": bool,
     },
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
 RestoreBackupRequestRequestTypeDef = TypedDict(
     "RestoreBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
 )
 
@@ -388,63 +312,24 @@
         "CreateTimestamp": datetime,
         "CopyTimestamp": datetime,
         "NeverExpires": bool,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
         "DeleteTimestamp": datetime,
-        "TagList": List[TagOutputTypeDef],
+        "TagList": List[TagTypeDef],
     },
     total=False,
 )
 
 
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ClusterTypeDef = TypedDict(
-    "ClusterTypeDef",
-    {
-        "BackupPolicy": Literal["DEFAULT"],
-        "BackupRetentionPolicy": BackupRetentionPolicyOutputTypeDef,
-        "ClusterId": str,
-        "CreateTimestamp": datetime,
-        "Hsms": List[HsmTypeDef],
-        "HsmType": str,
-        "PreCoPassword": str,
-        "SecurityGroup": str,
-        "SourceBackupId": str,
-        "State": ClusterStateType,
-        "StateMessage": str,
-        "SubnetMapping": Dict[str, str],
-        "VpcId": str,
-        "Certificates": CertificatesTypeDef,
-        "TagList": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "Hsm": HsmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCopyBackupToRegionRequestRequestTypeDef = TypedDict(
     "_RequiredCopyBackupToRegionRequestRequestTypeDef",
     {
         "DestinationRegion": str,
         "BackupId": str,
     },
 )
@@ -492,80 +377,176 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
+ClusterTypeDef = TypedDict(
+    "ClusterTypeDef",
+    {
+        "BackupPolicy": Literal["DEFAULT"],
+        "BackupRetentionPolicy": BackupRetentionPolicyTypeDef,
+        "ClusterId": str,
+        "CreateTimestamp": datetime,
+        "Hsms": List[HsmTypeDef],
+        "HsmType": str,
+        "PreCoPassword": str,
+        "SecurityGroup": str,
+        "SourceBackupId": str,
+        "State": ClusterStateType,
+        "StateMessage": str,
+        "SubnetMapping": Dict[str, str],
+        "VpcId": str,
+        "Certificates": CertificatesTypeDef,
+        "TagList": List[TagTypeDef],
+    },
+    total=False,
+)
+
 CopyBackupToRegionResponseTypeDef = TypedDict(
     "CopyBackupToRegionResponseTypeDef",
     {
         "DestinationBackup": DestinationBackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
+    {
+        "Hsm": HsmTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
+    {
+        "HsmId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+InitializeClusterResponseTypeDef = TypedDict(
+    "InitializeClusterResponseTypeDef",
+    {
+        "State": ClusterStateType,
+        "StateMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "Filters": Mapping[str, Sequence[str]],
+        "SortAscending": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    {
+        "Filters": Mapping[str, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+
 DeleteBackupResponseTypeDef = TypedDict(
     "DeleteBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyBackupAttributesResponseTypeDef = TypedDict(
     "ModifyBackupAttributesResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreBackupResponseTypeDef = TypedDict(
     "RestoreBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterResponseTypeDef = TypedDict(
     "ModifyClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2/type_defs.pyi` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for cloudhsmv2 service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_cloudhsmv2.type_defs import BackupRetentionPolicyOutputTypeDef
+    from mypy_boto3_cloudhsmv2.type_defs import BackupRetentionPolicyTypeDef
 
-    data: BackupRetentionPolicyOutputTypeDef = {...}
+    data: BackupRetentionPolicyTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import BackupStateType, ClusterStateType, HsmStateType
@@ -23,78 +23,67 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "BackupRetentionPolicyOutputTypeDef",
     "BackupRetentionPolicyTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "CertificatesTypeDef",
     "HsmTypeDef",
-    "TagTypeDef",
     "DestinationBackupTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateHsmRequestRequestTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteHsmRequestRequestTypeDef",
-    "DeleteHsmResponseTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "InitializeClusterRequestRequestTypeDef",
-    "InitializeClusterResponseTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ModifyBackupAttributesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreBackupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ModifyClusterRequestRequestTypeDef",
     "BackupTypeDef",
-    "ListTagsResponseTypeDef",
-    "ClusterTypeDef",
-    "CreateHsmResponseTypeDef",
     "CopyBackupToRegionRequestRequestTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ClusterTypeDef",
     "CopyBackupToRegionResponseTypeDef",
+    "CreateHsmResponseTypeDef",
+    "DeleteHsmResponseTypeDef",
+    "InitializeClusterResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "DeleteBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "ModifyBackupAttributesResponseTypeDef",
     "RestoreBackupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DescribeClustersResponseTypeDef",
     "ModifyClusterResponseTypeDef",
 )
 
-BackupRetentionPolicyOutputTypeDef = TypedDict(
-    "BackupRetentionPolicyOutputTypeDef",
-    {
-        "Type": Literal["DAYS"],
-        "Value": str,
-    },
-    total=False,
-)
-
 BackupRetentionPolicyTypeDef = TypedDict(
     "BackupRetentionPolicyTypeDef",
     {
         "Type": Literal["DAYS"],
         "Value": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
 CertificatesTypeDef = TypedDict(
@@ -128,33 +117,36 @@
     },
     total=False,
 )
 
 class HsmTypeDef(_RequiredHsmTypeDef, _OptionalHsmTypeDef):
     pass
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 DestinationBackupTypeDef = TypedDict(
     "DestinationBackupTypeDef",
     {
         "CreateTimestamp": datetime,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "ClusterId": str,
         "AvailabilityZone": str,
     },
 )
@@ -202,28 +194,20 @@
 )
 
 class DeleteHsmRequestRequestTypeDef(
     _RequiredDeleteHsmRequestRequestTypeDef, _OptionalDeleteHsmRequestRequestTypeDef
 ):
     pass
 
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "HsmId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Filters": Mapping[str, Sequence[str]],
-        "SortAscending": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
@@ -231,23 +215,14 @@
         "MaxResults": int,
         "Filters": Mapping[str, Sequence[str]],
         "SortAscending": bool,
     },
     total=False,
 )
 
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    {
-        "Filters": Mapping[str, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -259,42 +234,14 @@
     {
         "ClusterId": str,
         "SignedCert": str,
         "TrustAnchor": str,
     },
 )
 
-InitializeClusterResponseTypeDef = TypedDict(
-    "InitializeClusterResponseTypeDef",
-    {
-        "State": ClusterStateType,
-        "StateMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -315,35 +262,14 @@
     "ModifyBackupAttributesRequestRequestTypeDef",
     {
         "BackupId": str,
         "NeverExpires": bool,
     },
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
 RestoreBackupRequestRequestTypeDef = TypedDict(
     "RestoreBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
 )
 
@@ -377,61 +303,22 @@
         "CreateTimestamp": datetime,
         "CopyTimestamp": datetime,
         "NeverExpires": bool,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
         "DeleteTimestamp": datetime,
-        "TagList": List[TagOutputTypeDef],
+        "TagList": List[TagTypeDef],
     },
     total=False,
 )
 
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ClusterTypeDef = TypedDict(
-    "ClusterTypeDef",
-    {
-        "BackupPolicy": Literal["DEFAULT"],
-        "BackupRetentionPolicy": BackupRetentionPolicyOutputTypeDef,
-        "ClusterId": str,
-        "CreateTimestamp": datetime,
-        "Hsms": List[HsmTypeDef],
-        "HsmType": str,
-        "PreCoPassword": str,
-        "SecurityGroup": str,
-        "SourceBackupId": str,
-        "State": ClusterStateType,
-        "StateMessage": str,
-        "SubnetMapping": Dict[str, str],
-        "VpcId": str,
-        "Certificates": CertificatesTypeDef,
-        "TagList": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "Hsm": HsmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCopyBackupToRegionRequestRequestTypeDef = TypedDict(
     "_RequiredCopyBackupToRegionRequestRequestTypeDef",
     {
         "DestinationRegion": str,
         "BackupId": str,
     },
 )
@@ -475,80 +362,174 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
+ClusterTypeDef = TypedDict(
+    "ClusterTypeDef",
+    {
+        "BackupPolicy": Literal["DEFAULT"],
+        "BackupRetentionPolicy": BackupRetentionPolicyTypeDef,
+        "ClusterId": str,
+        "CreateTimestamp": datetime,
+        "Hsms": List[HsmTypeDef],
+        "HsmType": str,
+        "PreCoPassword": str,
+        "SecurityGroup": str,
+        "SourceBackupId": str,
+        "State": ClusterStateType,
+        "StateMessage": str,
+        "SubnetMapping": Dict[str, str],
+        "VpcId": str,
+        "Certificates": CertificatesTypeDef,
+        "TagList": List[TagTypeDef],
+    },
+    total=False,
+)
+
 CopyBackupToRegionResponseTypeDef = TypedDict(
     "CopyBackupToRegionResponseTypeDef",
     {
         "DestinationBackup": DestinationBackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
+    {
+        "Hsm": HsmTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
+    {
+        "HsmId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitializeClusterResponseTypeDef = TypedDict(
+    "InitializeClusterResponseTypeDef",
+    {
+        "State": ClusterStateType,
+        "StateMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "Filters": Mapping[str, Sequence[str]],
+        "SortAscending": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    {
+        "Filters": Mapping[str, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceId": str,
     },
 )
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
 
 DeleteBackupResponseTypeDef = TypedDict(
     "DeleteBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyBackupAttributesResponseTypeDef = TypedDict(
     "ModifyBackupAttributesResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreBackupResponseTypeDef = TypedDict(
     "RestoreBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterResponseTypeDef = TypedDict(
     "ModifyClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/PKG-INFO` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudhsmv2
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudHSMV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudHSMV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudhsmv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudhsmv2)](https://pepy.tech/project/mypy-boto3-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudHSMV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
+[boto3.CloudHSMV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [mypy-boto3-cloudhsmv2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudhsmv2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,60 +331,58 @@
 ### Typed dictionaries
 
 `mypy_boto3_cloudhsmv2.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudhsmv2.type_defs import (
-    BackupRetentionPolicyOutputTypeDef,
     BackupRetentionPolicyTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
-    TagTypeDef,
     DestinationBackupTypeDef,
+    ResponseMetadataTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
     InitializeClusterRequestRequestTypeDef,
-    InitializeClusterResponseTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     ModifyBackupAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
-    ListTagsResponseTypeDef,
-    ClusterTypeDef,
-    CreateHsmResponseTypeDef,
     CopyBackupToRegionRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    ClusterTypeDef,
     CopyBackupToRegionResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    InitializeClusterResponseTypeDef,
+    ListTagsResponseTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyOutputTypeDef:
+def get_structure() -> BackupRetentionPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/mypy_boto3_cloudhsmv2.egg-info/SOURCES.txt` & `mypy-boto3-cloudhsmv2-1.28.15/mypy_boto3_cloudhsmv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudhsmv2-1.28.12/setup.py` & `mypy-boto3-cloudhsmv2-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudhsmv2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudhsmv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudHSMV2 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CloudHSMV2 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

