# Comparing `tmp/mypy-boto3-opsworkscm-1.28.12.tar.gz` & `tmp/mypy-boto3-opsworkscm-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opsworkscm-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
+gzip compressed data, was "mypy-boto3-opsworkscm-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
```

## Comparing `mypy-boto3-opsworkscm-1.28.12.tar` & `mypy-boto3-opsworkscm-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19108 2023-07-27 11:41:04.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19081 2023-07-27 11:41:04.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15837 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:21.000000 mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.801132 mypy-boto3-opsworkscm-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 11:41:03.000000 mypy-boto3-opsworkscm-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.557601 mypy-boto3-opsworkscm-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-07-28 20:43:24.557601 mypy-boto3-opsworkscm-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14282 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.541601 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17626 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-07-28 20:33:01.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.557601 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15781 2023-07-28 20:43:24.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 20:43:24.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:24.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:24.000000 mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.557601 mypy-boto3-opsworkscm-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:33:00.000000 mypy-boto3-opsworkscm-1.28.15/setup.py
```

### Comparing `mypy-boto3-opsworkscm-1.28.12/LICENSE` & `mypy-boto3-opsworkscm-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/PKG-INFO` & `mypy-boto3-opsworkscm-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworkscm
-Version: 1.28.12
-Summary: Type annotations for boto3.OpsWorksCM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpsWorksCM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,44 +372,42 @@
     DeleteServerRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    EngineAttributeOutputTypeDef,
     DescribeServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     AssociateNodeRequestRequestTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
+    ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
     AssociateNodeResponseTypeDef,
     DescribeAccountAttributesResponseTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeServersRequestDescribeServersPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    ServerTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.12/README.md` & `mypy-boto3-opsworkscm-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -340,44 +340,42 @@
     DeleteServerRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    EngineAttributeOutputTypeDef,
     DescribeServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     AssociateNodeRequestRequestTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
+    ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
     AssociateNodeResponseTypeDef,
     DescribeAccountAttributesResponseTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeServersRequestDescribeServersPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    ServerTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__init__.py` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__init__.pyi` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/__main__.py` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpsWorksCM 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.OpsWorksCM 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM\nOther"
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

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/client.py` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/client.pyi` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/literals.py` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/literals.pyi` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/paginator.py` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/paginator.pyi` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/type_defs.py` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,44 +39,42 @@
     "DeleteServerRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "ServerEventTypeDef",
     "WaiterConfigTypeDef",
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
-    "EngineAttributeOutputTypeDef",
     "DescribeServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "RestoreServerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateServerEngineAttributesRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
     "AssociateNodeRequestRequestTypeDef",
     "DisassociateNodeRequestRequestTypeDef",
     "ExportServerEngineAttributeRequestRequestTypeDef",
+    "ServerTypeDef",
     "StartMaintenanceRequestRequestTypeDef",
     "AssociateNodeResponseTypeDef",
     "DescribeAccountAttributesResponseTypeDef",
+    "DescribeNodeAssociationStatusResponseTypeDef",
     "DisassociateNodeResponseTypeDef",
+    "ExportServerEngineAttributeResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateServerRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeServersRequestDescribeServersPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    "ExportServerEngineAttributeResponseTypeDef",
-    "ServerTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateServerResponseTypeDef",
     "DescribeServersResponseTypeDef",
     "RestoreServerResponseTypeDef",
     "StartMaintenanceResponseTypeDef",
     "UpdateServerEngineAttributesResponseTypeDef",
     "UpdateServerResponseTypeDef",
 )
@@ -231,23 +229,14 @@
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ServerName": str,
     },
 )
 
-EngineAttributeOutputTypeDef = TypedDict(
-    "EngineAttributeOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 DescribeServersRequestRequestTypeDef = TypedDict(
     "DescribeServersRequestRequestTypeDef",
     {
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -273,22 +262,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredRestoreServerRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreServerRequestRequestTypeDef",
     {
         "BackupId": str,
         "ServerName": str,
     },
 )
@@ -413,14 +394,45 @@
 class ExportServerEngineAttributeRequestRequestTypeDef(
     _RequiredExportServerEngineAttributeRequestRequestTypeDef,
     _OptionalExportServerEngineAttributeRequestRequestTypeDef,
 ):
     pass
 
 
+ServerTypeDef = TypedDict(
+    "ServerTypeDef",
+    {
+        "AssociatePublicIpAddress": bool,
+        "BackupRetentionCount": int,
+        "ServerName": str,
+        "CreatedAt": datetime,
+        "CloudFormationStackArn": str,
+        "CustomDomain": str,
+        "DisableAutomatedBackup": bool,
+        "Endpoint": str,
+        "Engine": str,
+        "EngineModel": str,
+        "EngineAttributes": List[EngineAttributeTypeDef],
+        "EngineVersion": str,
+        "InstanceProfileArn": str,
+        "InstanceType": str,
+        "KeyPair": str,
+        "MaintenanceStatus": MaintenanceStatusType,
+        "PreferredMaintenanceWindow": str,
+        "PreferredBackupWindow": str,
+        "SecurityGroupIds": List[str],
+        "ServiceRoleArn": str,
+        "Status": ServerStatusType,
+        "StatusReason": str,
+        "SubnetIds": List[str],
+        "ServerArn": str,
+    },
+    total=False,
+)
+
 _RequiredStartMaintenanceRequestRequestTypeDef = TypedDict(
     "_RequiredStartMaintenanceRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalStartMaintenanceRequestRequestTypeDef = TypedDict(
@@ -450,22 +462,40 @@
     "DescribeAccountAttributesResponseTypeDef",
     {
         "Attributes": List[AccountAttributeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    {
+        "NodeAssociationStatus": NodeAssociationStatusType,
+        "EngineAttributes": List[EngineAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DisassociateNodeResponseTypeDef = TypedDict(
     "DisassociateNodeResponseTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ExportServerEngineAttributeResponseTypeDef = TypedDict(
+    "ExportServerEngineAttributeResponseTypeDef",
+    {
+        "EngineAttribute": EngineAttributeTypeDef,
+        "ServerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -537,14 +567,23 @@
 
 class CreateServerRequestRequestTypeDef(
     _RequiredCreateServerRequestRequestTypeDef, _OptionalCreateServerRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
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
@@ -640,72 +679,14 @@
 class DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef(
     _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     _OptionalDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
 ):
     pass
 
 
-DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    {
-        "NodeAssociationStatus": NodeAssociationStatusType,
-        "EngineAttributes": List[EngineAttributeOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExportServerEngineAttributeResponseTypeDef = TypedDict(
-    "ExportServerEngineAttributeResponseTypeDef",
-    {
-        "EngineAttribute": EngineAttributeOutputTypeDef,
-        "ServerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerTypeDef = TypedDict(
-    "ServerTypeDef",
-    {
-        "AssociatePublicIpAddress": bool,
-        "BackupRetentionCount": int,
-        "ServerName": str,
-        "CreatedAt": datetime,
-        "CloudFormationStackArn": str,
-        "CustomDomain": str,
-        "DisableAutomatedBackup": bool,
-        "Endpoint": str,
-        "Engine": str,
-        "EngineModel": str,
-        "EngineAttributes": List[EngineAttributeOutputTypeDef],
-        "EngineVersion": str,
-        "InstanceProfileArn": str,
-        "InstanceType": str,
-        "KeyPair": str,
-        "MaintenanceStatus": MaintenanceStatusType,
-        "PreferredMaintenanceWindow": str,
-        "PreferredBackupWindow": str,
-        "SecurityGroupIds": List[str],
-        "ServiceRoleArn": str,
-        "Status": ServerStatusType,
-        "StatusReason": str,
-        "SubnetIds": List[str],
-        "ServerArn": str,
-    },
-    total=False,
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateServerResponseTypeDef = TypedDict(
     "CreateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/type_defs.pyi` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,44 +38,42 @@
     "DeleteServerRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "ServerEventTypeDef",
     "WaiterConfigTypeDef",
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
-    "EngineAttributeOutputTypeDef",
     "DescribeServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "RestoreServerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateServerEngineAttributesRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
     "AssociateNodeRequestRequestTypeDef",
     "DisassociateNodeRequestRequestTypeDef",
     "ExportServerEngineAttributeRequestRequestTypeDef",
+    "ServerTypeDef",
     "StartMaintenanceRequestRequestTypeDef",
     "AssociateNodeResponseTypeDef",
     "DescribeAccountAttributesResponseTypeDef",
+    "DescribeNodeAssociationStatusResponseTypeDef",
     "DisassociateNodeResponseTypeDef",
+    "ExportServerEngineAttributeResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateServerRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
     "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeServersRequestDescribeServersPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    "ExportServerEngineAttributeResponseTypeDef",
-    "ServerTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "CreateServerResponseTypeDef",
     "DescribeServersResponseTypeDef",
     "RestoreServerResponseTypeDef",
     "StartMaintenanceResponseTypeDef",
     "UpdateServerEngineAttributesResponseTypeDef",
     "UpdateServerResponseTypeDef",
 )
@@ -228,23 +226,14 @@
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ServerName": str,
     },
 )
 
-EngineAttributeOutputTypeDef = TypedDict(
-    "EngineAttributeOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 DescribeServersRequestRequestTypeDef = TypedDict(
     "DescribeServersRequestRequestTypeDef",
     {
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -268,22 +257,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 _RequiredRestoreServerRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreServerRequestRequestTypeDef",
     {
         "BackupId": str,
         "ServerName": str,
     },
 )
@@ -398,14 +379,45 @@
 
 class ExportServerEngineAttributeRequestRequestTypeDef(
     _RequiredExportServerEngineAttributeRequestRequestTypeDef,
     _OptionalExportServerEngineAttributeRequestRequestTypeDef,
 ):
     pass
 
+ServerTypeDef = TypedDict(
+    "ServerTypeDef",
+    {
+        "AssociatePublicIpAddress": bool,
+        "BackupRetentionCount": int,
+        "ServerName": str,
+        "CreatedAt": datetime,
+        "CloudFormationStackArn": str,
+        "CustomDomain": str,
+        "DisableAutomatedBackup": bool,
+        "Endpoint": str,
+        "Engine": str,
+        "EngineModel": str,
+        "EngineAttributes": List[EngineAttributeTypeDef],
+        "EngineVersion": str,
+        "InstanceProfileArn": str,
+        "InstanceType": str,
+        "KeyPair": str,
+        "MaintenanceStatus": MaintenanceStatusType,
+        "PreferredMaintenanceWindow": str,
+        "PreferredBackupWindow": str,
+        "SecurityGroupIds": List[str],
+        "ServiceRoleArn": str,
+        "Status": ServerStatusType,
+        "StatusReason": str,
+        "SubnetIds": List[str],
+        "ServerArn": str,
+    },
+    total=False,
+)
+
 _RequiredStartMaintenanceRequestRequestTypeDef = TypedDict(
     "_RequiredStartMaintenanceRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalStartMaintenanceRequestRequestTypeDef = TypedDict(
@@ -433,22 +445,40 @@
     "DescribeAccountAttributesResponseTypeDef",
     {
         "Attributes": List[AccountAttributeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    {
+        "NodeAssociationStatus": NodeAssociationStatusType,
+        "EngineAttributes": List[EngineAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DisassociateNodeResponseTypeDef = TypedDict(
     "DisassociateNodeResponseTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ExportServerEngineAttributeResponseTypeDef = TypedDict(
+    "ExportServerEngineAttributeResponseTypeDef",
+    {
+        "EngineAttribute": EngineAttributeTypeDef,
+        "ServerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -516,14 +546,23 @@
 )
 
 class CreateServerRequestRequestTypeDef(
     _RequiredCreateServerRequestRequestTypeDef, _OptionalCreateServerRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
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
@@ -613,72 +652,14 @@
 
 class DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef(
     _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     _OptionalDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
 ):
     pass
 
-DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    {
-        "NodeAssociationStatus": NodeAssociationStatusType,
-        "EngineAttributes": List[EngineAttributeOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ExportServerEngineAttributeResponseTypeDef = TypedDict(
-    "ExportServerEngineAttributeResponseTypeDef",
-    {
-        "EngineAttribute": EngineAttributeOutputTypeDef,
-        "ServerName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ServerTypeDef = TypedDict(
-    "ServerTypeDef",
-    {
-        "AssociatePublicIpAddress": bool,
-        "BackupRetentionCount": int,
-        "ServerName": str,
-        "CreatedAt": datetime,
-        "CloudFormationStackArn": str,
-        "CustomDomain": str,
-        "DisableAutomatedBackup": bool,
-        "Endpoint": str,
-        "Engine": str,
-        "EngineModel": str,
-        "EngineAttributes": List[EngineAttributeOutputTypeDef],
-        "EngineVersion": str,
-        "InstanceProfileArn": str,
-        "InstanceType": str,
-        "KeyPair": str,
-        "MaintenanceStatus": MaintenanceStatusType,
-        "PreferredMaintenanceWindow": str,
-        "PreferredBackupWindow": str,
-        "SecurityGroupIds": List[str],
-        "ServiceRoleArn": str,
-        "Status": ServerStatusType,
-        "StatusReason": str,
-        "SubnetIds": List[str],
-        "ServerArn": str,
-    },
-    total=False,
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateServerResponseTypeDef = TypedDict(
     "CreateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/waiter.py` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm/waiter.pyi` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/PKG-INFO` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opsworkscm
-Version: 1.28.12
-Summary: Type annotations for boto3.OpsWorksCM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpsWorksCM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opsworkscm.svg?color=blue)](https://pypi.org/project/mypy-boto3-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opsworkscm)](https://pepy.tech/project/mypy-boto3-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpsWorksCM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
+[boto3.OpsWorksCM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [mypy-boto3-opsworkscm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opsworkscm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -372,44 +372,42 @@
     DeleteServerRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    EngineAttributeOutputTypeDef,
     DescribeServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
     AssociateNodeRequestRequestTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
+    ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
     AssociateNodeResponseTypeDef,
     DescribeAccountAttributesResponseTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
     DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeServersRequestDescribeServersPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
-    ServerTypeDef,
-    ListTagsForResourceResponseTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
```

### Comparing `mypy-boto3-opsworkscm-1.28.12/mypy_boto3_opsworkscm.egg-info/SOURCES.txt` & `mypy-boto3-opsworkscm-1.28.15/mypy_boto3_opsworkscm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opsworkscm-1.28.12/setup.py` & `mypy-boto3-opsworkscm-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opsworkscm",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_opsworkscm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpsWorksCM 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.OpsWorksCM 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

