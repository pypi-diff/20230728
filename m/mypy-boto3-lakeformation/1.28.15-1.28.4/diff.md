# Comparing `tmp/mypy-boto3-lakeformation-1.28.15.tar.gz` & `tmp/mypy-boto3-lakeformation-1.28.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lakeformation-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
+gzip compressed data, was "mypy-boto3-lakeformation-1.28.4.tar", last modified: Tue Jul 18 01:01:41 2023, max compression
```

## Comparing `mypy-boto3-lakeformation-1.28.15.tar` & `mypy-boto3-lakeformation-1.28.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.029374 mypy-boto3-lakeformation-1.28.15/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-07-28 20:43:08.025375 mypy-boto3-lakeformation-1.28.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.021374 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37043 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-07-28 20:29:31.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54522 2023-07-28 20:29:32.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54423 2023-07-28 20:29:31.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.025375 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-07-28 20:43:07.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:43:07.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:07.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:07.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:07.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:07.000000 mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.029374 mypy-boto3-lakeformation-1.28.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:29:30.000000 mypy-boto3-lakeformation-1.28.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37102 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37043 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53022 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52937 2023-07-18 01:01:31.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 01:01:30.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19383 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 01:01:41.000000 mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:01:41.969310 mypy-boto3-lakeformation-1.28.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-18 01:01:29.000000 mypy-boto3-lakeformation-1.28.4/setup.py
```

### Comparing `mypy-boto3-lakeformation-1.28.15/LICENSE` & `mypy-boto3-lakeformation-1.28.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.15
-Summary: Type annotations for boto3.LakeFormation 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,25 +357,29 @@
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lakeformation-1.28.15/README.md` & `mypy-boto3-lakeformation-1.28.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,25 +325,29 @@
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/__init__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/__init__.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/__main__.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LakeFormation 1.28.15\nVersion:         1.28.15\nBuilder"
-        " version: 7.16.1\nDocs:           "
+        "Type annotations for boto3.LakeFormation 1.28.4\nVersion:         1.28.4\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15")
+    print("1.28.4")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/client.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/client.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/literals.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,14 @@
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
@@ -292,28 +291,26 @@
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
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/literals.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,14 @@
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
@@ -290,28 +289,26 @@
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
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
-    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/paginator.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/paginator.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/type_defs.py` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,25 +41,29 @@
 __all__ = (
     "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
     "LFTagPairOutputTypeDef",
     "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "RowFilterOutputTypeDef",
+    "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
+    "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
+    "DatabaseResourceOutputTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
     "VirtualObjectTypeDef",
     "DeregisterResourceRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
@@ -266,15 +270,21 @@
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -284,40 +294,28 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
-
 
 ColumnWildcardOutputTypeDef = TypedDict(
     "ColumnWildcardOutputTypeDef",
     {
         "ExcludedColumnNames": List[str],
     },
-    total=False,
 )
 
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
@@ -355,15 +353,24 @@
 
 RowFilterOutputTypeDef = TypedDict(
     "RowFilterOutputTypeDef",
     {
         "FilterExpression": str,
         "AllRowsWildcard": Dict[str, Any],
     },
-    total=False,
+)
+
+DataCellsFilterResourceOutputTypeDef = TypedDict(
+    "DataCellsFilterResourceOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
 )
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
@@ -378,14 +385,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -399,14 +414,22 @@
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
 
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "Name": str,
+    },
+)
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -513,15 +536,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -531,33 +553,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -655,15 +674,14 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
-    total=False,
 )
 
 _RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -742,35 +760,22 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
-
 
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -867,15 +872,14 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
@@ -888,15 +892,14 @@
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
-    total=False,
 )
 
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
@@ -938,37 +941,24 @@
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
         "Name": str,
         "TableWildcard": Dict[str, Any],
     },
-    total=False,
 )
 
-
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
-
-
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
@@ -1158,18 +1148,17 @@
 ):
     pass
 
 
 PrincipalPermissionsOutputTypeDef = TypedDict(
     "PrincipalPermissionsOutputTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
@@ -1179,59 +1168,44 @@
 
 ColumnLFTagTypeDef = TypedDict(
     "ColumnLFTagTypeDef",
     {
         "Name": str,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 LFTagErrorTypeDef = TypedDict(
     "LFTagErrorTypeDef",
     {
         "LFTag": LFTagPairOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 ListLFTagsResponseTypeDef = TypedDict(
     "ListLFTagsResponseTypeDef",
     {
         "LFTags": List[LFTagPairOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
-    },
-)
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
-    {
-        "CatalogId": str,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
-    total=False,
 )
 
-
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1248,41 +1222,28 @@
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
         "RowFilter": RowFilterOutputTypeDef,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
         "VersionId": str,
     },
-    total=False,
 )
 
-
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1303,18 +1264,17 @@
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1465,35 +1425,22 @@
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "ResourceType": ResourceTypeType,
         "Expression": List[LFTagOutputTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
-):
-    pass
-
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
@@ -1637,40 +1584,38 @@
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
     },
 )
 
 DataLakeSettingsOutputTypeDef = TypedDict(
     "DataLakeSettingsOutputTypeDef",
     {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "ReadOnlyAdmins": List[DataLakePrincipalTypeDef],
+        "DataLakeAdmins": List[DataLakePrincipalOutputTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalOutputTypeDef],
         "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
         "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
         "Parameters": Dict[str, str],
         "TrustedResourceOwners": List[str],
         "AllowExternalDataFiltering": bool,
         "AllowFullTableExternalDataAccess": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
         "AuthorizedSessionTagValueList": List[str],
     },
-    total=False,
 )
 
 DataLakeSettingsTypeDef = TypedDict(
     "DataLakeSettingsTypeDef",
     {
         "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
         "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
@@ -1700,15 +1645,14 @@
     "TaggedTableTypeDef",
     {
         "Table": TableResourceOutputTypeDef,
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1788,23 +1732,22 @@
     pass
 
 
 ResourceOutputTypeDef = TypedDict(
     "ResourceOutputTypeDef",
     {
         "Catalog": Dict[str, Any],
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "Table": TableResourceOutputTypeDef,
         "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
-        "DataLocation": DataLocationResourceTypeDef,
-        "DataCellsFilter": DataCellsFilterResourceTypeDef,
+        "DataLocation": DataLocationResourceOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
         "LFTag": LFTagKeyResourceOutputTypeDef,
         "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
     },
-    total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
@@ -1862,49 +1805,34 @@
     {
         "NextToken": str,
         "TableList": List[TaggedTableTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
     {
         "Id": str,
-    },
-)
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
     },
-    total=False,
 )
 
-
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
-
 PrincipalResourcePermissionsTypeDef = TypedDict(
     "PrincipalResourcePermissionsTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
         "AdditionalDetails": DetailsMapTypeDef,
     },
-    total=False,
 )
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
         "LFTags": Sequence[LFTagPairTypeDef],
@@ -2059,15 +1987,14 @@
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
         "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
```

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation/type_defs.pyi` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -40,25 +40,29 @@
 __all__ = (
     "LFTagPairTypeDef",
     "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
+    "DataLakePrincipalOutputTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
     "LFTagPairOutputTypeDef",
     "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
     "CreateLFTagRequestRequestTypeDef",
     "RowFilterOutputTypeDef",
+    "DataCellsFilterResourceOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
+    "DataLocationResourceOutputTypeDef",
     "DataLocationResourceTypeDef",
+    "DatabaseResourceOutputTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
     "VirtualObjectTypeDef",
     "DeregisterResourceRequestRequestTypeDef",
     "DescribeResourceRequestRequestTypeDef",
@@ -259,15 +263,21 @@
 
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
-    total=False,
+)
+
+DataLakePrincipalOutputTypeDef = TypedDict(
+    "DataLakePrincipalOutputTypeDef",
+    {
+        "DataLakePrincipalIdentifier": str,
+    },
 )
 
 DataLakePrincipalTypeDef = TypedDict(
     "DataLakePrincipalTypeDef",
     {
         "DataLakePrincipalIdentifier": str,
     },
@@ -277,38 +287,28 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-_RequiredLFTagPairOutputTypeDef = TypedDict(
-    "_RequiredLFTagPairOutputTypeDef",
+LFTagPairOutputTypeDef = TypedDict(
+    "LFTagPairOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagPairOutputTypeDef = TypedDict(
-    "_OptionalLFTagPairOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
-    pass
 
 ColumnWildcardOutputTypeDef = TypedDict(
     "ColumnWildcardOutputTypeDef",
     {
         "ExcludedColumnNames": List[str],
     },
-    total=False,
 )
 
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
@@ -344,15 +344,24 @@
 
 RowFilterOutputTypeDef = TypedDict(
     "RowFilterOutputTypeDef",
     {
         "FilterExpression": str,
         "AllRowsWildcard": Dict[str, Any],
     },
-    total=False,
+)
+
+DataCellsFilterResourceOutputTypeDef = TypedDict(
+    "DataCellsFilterResourceOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
 )
 
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
@@ -367,14 +376,22 @@
     {
         "FilterExpression": str,
         "AllRowsWildcard": Mapping[str, Any],
     },
     total=False,
 )
 
+DataLocationResourceOutputTypeDef = TypedDict(
+    "DataLocationResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ResourceArn": str,
+    },
+)
+
 _RequiredDataLocationResourceTypeDef = TypedDict(
     "_RequiredDataLocationResourceTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalDataLocationResourceTypeDef = TypedDict(
@@ -386,14 +403,22 @@
 )
 
 class DataLocationResourceTypeDef(
     _RequiredDataLocationResourceTypeDef, _OptionalDataLocationResourceTypeDef
 ):
     pass
 
+DatabaseResourceOutputTypeDef = TypedDict(
+    "DatabaseResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "Name": str,
+    },
+)
+
 _RequiredDatabaseResourceTypeDef = TypedDict(
     "_RequiredDatabaseResourceTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDatabaseResourceTypeDef = TypedDict(
@@ -492,15 +517,14 @@
     "ResourceInfoTypeDef",
     {
         "ResourceArn": str,
         "RoleArn": str,
         "LastModified": datetime,
         "WithFederation": bool,
     },
-    total=False,
 )
 
 DescribeTransactionRequestRequestTypeDef = TypedDict(
     "DescribeTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -510,33 +534,30 @@
     "TransactionDescriptionTypeDef",
     {
         "TransactionId": str,
         "TransactionStatus": TransactionStatusType,
         "TransactionStartTime": datetime,
         "TransactionEndTime": datetime,
     },
-    total=False,
 )
 
 DetailsMapTypeDef = TypedDict(
     "DetailsMapTypeDef",
     {
         "ResourceShare": List[str],
     },
-    total=False,
 )
 
 ExecutionStatisticsTypeDef = TypedDict(
     "ExecutionStatisticsTypeDef",
     {
         "AverageExecutionTimeMillis": int,
         "DataScannedBytes": int,
         "WorkUnitsExecutedCount": int,
     },
-    total=False,
 )
 
 ExtendTransactionRequestRequestTypeDef = TypedDict(
     "ExtendTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
@@ -630,15 +651,14 @@
     "PlanningStatisticsTypeDef",
     {
         "EstimatedDataToScanBytes": int,
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
-    total=False,
 )
 
 _RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
@@ -713,33 +733,22 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
-_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagKeyResourceOutputTypeDef",
+LFTagKeyResourceOutputTypeDef = TypedDict(
+    "LFTagKeyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "TagKey": str,
         "TagValues": List[str],
     },
 )
-_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagKeyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagKeyResourceOutputTypeDef(
-    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
-):
-    pass
 
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
@@ -830,15 +839,14 @@
     {
         "StorageOptimizerType": OptimizerTypeType,
         "Config": Dict[str, str],
         "ErrorMessage": str,
         "Warnings": str,
         "LastRunDetails": str,
     },
-    total=False,
 )
 
 ListTransactionsRequestRequestTypeDef = TypedDict(
     "ListTransactionsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "StatusFilter": TransactionStatusFilterType,
@@ -851,15 +859,14 @@
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
-    total=False,
 )
 
 _RequiredQueryPlanningContextTypeDef = TypedDict(
     "_RequiredQueryPlanningContextTypeDef",
     {
         "DatabaseName": str,
     },
@@ -897,35 +904,24 @@
 )
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
-_RequiredTableResourceOutputTypeDef = TypedDict(
-    "_RequiredTableResourceOutputTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalTableResourceOutputTypeDef = TypedDict(
-    "_OptionalTableResourceOutputTypeDef",
+TableResourceOutputTypeDef = TypedDict(
+    "TableResourceOutputTypeDef",
     {
         "CatalogId": str,
+        "DatabaseName": str,
         "Name": str,
         "TableWildcard": Dict[str, Any],
     },
-    total=False,
 )
 
-class TableResourceOutputTypeDef(
-    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
-):
-    pass
-
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
@@ -1107,18 +1103,17 @@
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
 PrincipalPermissionsOutputTypeDef = TypedDict(
     "PrincipalPermissionsOutputTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Permissions": List[PermissionType],
     },
-    total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Permissions": Sequence[PermissionType],
@@ -1128,57 +1123,44 @@
 
 ColumnLFTagTypeDef = TypedDict(
     "ColumnLFTagTypeDef",
     {
         "Name": str,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 LFTagErrorTypeDef = TypedDict(
     "LFTagErrorTypeDef",
     {
         "LFTag": LFTagPairOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 ListLFTagsResponseTypeDef = TypedDict(
     "ListLFTagsResponseTypeDef",
     {
         "LFTags": List[LFTagPairOutputTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_RequiredTableWithColumnsResourceOutputTypeDef",
+TableWithColumnsResourceOutputTypeDef = TypedDict(
+    "TableWithColumnsResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "DatabaseName": str,
         "Name": str,
-    },
-)
-_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
-    "_OptionalTableWithColumnsResourceOutputTypeDef",
-    {
-        "CatalogId": str,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
-    total=False,
 )
 
-class TableWithColumnsResourceOutputTypeDef(
-    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
-):
-    pass
-
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1193,39 +1175,28 @@
 )
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
-_RequiredDataCellsFilterOutputTypeDef = TypedDict(
-    "_RequiredDataCellsFilterOutputTypeDef",
+DataCellsFilterOutputTypeDef = TypedDict(
+    "DataCellsFilterOutputTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
-    },
-)
-_OptionalDataCellsFilterOutputTypeDef = TypedDict(
-    "_OptionalDataCellsFilterOutputTypeDef",
-    {
         "RowFilter": RowFilterOutputTypeDef,
         "ColumnNames": List[str],
         "ColumnWildcard": ColumnWildcardOutputTypeDef,
         "VersionId": str,
     },
-    total=False,
 )
 
-class DataCellsFilterOutputTypeDef(
-    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
-):
-    pass
-
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1244,18 +1215,17 @@
 
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "LFTags": List[LFTagPairOutputTypeDef],
     },
-    total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
         "AddObject": AddObjectInputTypeDef,
         "DeleteObject": DeleteObjectInputTypeDef,
@@ -1400,33 +1370,22 @@
         "NextToken": str,
         "QueryId": str,
         "WorkUnitRanges": List[WorkUnitRangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceOutputTypeDef",
+LFTagPolicyResourceOutputTypeDef = TypedDict(
+    "LFTagPolicyResourceOutputTypeDef",
     {
+        "CatalogId": str,
         "ResourceType": ResourceTypeType,
         "Expression": List[LFTagOutputTypeDef],
     },
 )
-_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceOutputTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class LFTagPolicyResourceOutputTypeDef(
-    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
-):
-    pass
 
 _RequiredLFTagPolicyResourceTypeDef = TypedDict(
     "_RequiredLFTagPolicyResourceTypeDef",
     {
         "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
@@ -1560,40 +1519,38 @@
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
-    total=False,
 )
 
 StartQueryPlanningRequestRequestTypeDef = TypedDict(
     "StartQueryPlanningRequestRequestTypeDef",
     {
         "QueryPlanningContext": QueryPlanningContextTypeDef,
         "QueryString": str,
     },
 )
 
 DataLakeSettingsOutputTypeDef = TypedDict(
     "DataLakeSettingsOutputTypeDef",
     {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "ReadOnlyAdmins": List[DataLakePrincipalTypeDef],
+        "DataLakeAdmins": List[DataLakePrincipalOutputTypeDef],
+        "ReadOnlyAdmins": List[DataLakePrincipalOutputTypeDef],
         "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
         "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
         "Parameters": Dict[str, str],
         "TrustedResourceOwners": List[str],
         "AllowExternalDataFiltering": bool,
         "AllowFullTableExternalDataAccess": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalOutputTypeDef],
         "AuthorizedSessionTagValueList": List[str],
     },
-    total=False,
 )
 
 DataLakeSettingsTypeDef = TypedDict(
     "DataLakeSettingsTypeDef",
     {
         "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
         "ReadOnlyAdmins": Sequence[DataLakePrincipalTypeDef],
@@ -1623,15 +1580,14 @@
     "TaggedTableTypeDef",
     {
         "Table": TableResourceOutputTypeDef,
         "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
         "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
-    total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1709,23 +1665,22 @@
 ):
     pass
 
 ResourceOutputTypeDef = TypedDict(
     "ResourceOutputTypeDef",
     {
         "Catalog": Dict[str, Any],
-        "Database": DatabaseResourceTypeDef,
+        "Database": DatabaseResourceOutputTypeDef,
         "Table": TableResourceOutputTypeDef,
         "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
-        "DataLocation": DataLocationResourceTypeDef,
-        "DataCellsFilter": DataCellsFilterResourceTypeDef,
+        "DataLocation": DataLocationResourceOutputTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceOutputTypeDef,
         "LFTag": LFTagKeyResourceOutputTypeDef,
         "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
     },
-    total=False,
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
@@ -1781,47 +1736,34 @@
     {
         "NextToken": str,
         "TableList": List[TaggedTableTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+BatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "BatchPermissionsRequestEntryOutputTypeDef",
     {
         "Id": str,
-    },
-)
-_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
-    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
     },
-    total=False,
 )
 
-class BatchPermissionsRequestEntryOutputTypeDef(
-    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
-    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
-):
-    pass
-
 PrincipalResourcePermissionsTypeDef = TypedDict(
     "PrincipalResourcePermissionsTypeDef",
     {
-        "Principal": DataLakePrincipalTypeDef,
+        "Principal": DataLakePrincipalOutputTypeDef,
         "Resource": ResourceOutputTypeDef,
         "Permissions": List[PermissionType],
         "PermissionsWithGrantOption": List[PermissionType],
         "AdditionalDetails": DetailsMapTypeDef,
     },
-    total=False,
 )
 
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
         "LFTags": Sequence[LFTagPairTypeDef],
@@ -1964,15 +1906,14 @@
 
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
         "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
-    total=False,
 )
 
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
```

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/PKG-INFO` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lakeformation
-Version: 1.28.15
-Summary: Type annotations for boto3.LakeFormation 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Version: 1.28.4
+Summary: Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-lakeformation"></a>
 
 # mypy-boto3-lakeformation
 
 [![PyPI - mypy-boto3-lakeformation](https://img.shields.io/pypi/v/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lakeformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/)
-[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lakeformation)](https://pepy.tech/project/mypy-boto3-lakeformation)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-lakeformation?color=blue)](https://pypistats.org/packages/mypy-boto3-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LakeFormation 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
+[boto3.LakeFormation 1.28.4](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [mypy-boto3-lakeformation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lakeformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -357,25 +357,29 @@
 from mypy_boto3_lakeformation.type_defs import (
     LFTagPairTypeDef,
     ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
+    DataLakePrincipalOutputTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
     LFTagPairOutputTypeDef,
     ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
     CreateLFTagRequestRequestTypeDef,
     RowFilterOutputTypeDef,
+    DataCellsFilterResourceOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
+    DataLocationResourceOutputTypeDef,
     DataLocationResourceTypeDef,
+    DatabaseResourceOutputTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
     VirtualObjectTypeDef,
     DeregisterResourceRequestRequestTypeDef,
     DescribeResourceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-lakeformation-1.28.15/mypy_boto3_lakeformation.egg-info/SOURCES.txt` & `mypy-boto3-lakeformation-1.28.4/mypy_boto3_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lakeformation-1.28.15/setup.py` & `mypy-boto3-lakeformation-1.28.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lakeformation",
-    version="1.28.15",
+    version="1.28.4",
     packages=["mypy_boto3_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LakeFormation 1.28.15 service generated with mypy-boto3-builder"
-        " 7.16.1"
+        "Type annotations for boto3.LakeFormation 1.28.4 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

