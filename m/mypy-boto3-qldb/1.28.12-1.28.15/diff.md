# Comparing `tmp/mypy-boto3-qldb-1.28.12.tar.gz` & `tmp/mypy-boto3-qldb-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-qldb-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
+gzip compressed data, was "mypy-boto3-qldb-1.28.15.tar", last modified: Fri Jul 28 20:43:30 2023, max compression
```

## Comparing `mypy-boto3-qldb-1.28.12.tar` & `mypy-boto3-qldb-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.497187 mypy-boto3-qldb-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-07-27 11:49:27.497187 mypy-boto3-qldb-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.485187 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-27 11:41:52.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19276 2023-07-27 11:41:52.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.497187 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:49:27.000000 mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.497187 mypy-boto3-qldb-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 11:41:51.000000 mypy-boto3-qldb-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.709686 mypy-boto3-qldb-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-28 20:43:30.701686 mypy-boto3-qldb-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.697685 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-28 20:33:48.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-28 20:33:48.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.701686 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:30.000000 mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:30.709686 mypy-boto3-qldb-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 20:33:47.000000 mypy-boto3-qldb-1.28.15/setup.py
```

### Comparing `mypy-boto3-qldb-1.28.12/LICENSE` & `mypy-boto3-qldb-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.12/PKG-INFO` & `mypy-boto3-qldb-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.28.12
-Summary: Type annotations for boto3.QLDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,25 +312,22 @@
     CreateLedgerRequestRequestTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
     ValueHolderTypeDef,
-    ValueHolderOutputTypeDef,
     GetDigestRequestRequestTypeDef,
-    KinesisConfigurationOutputTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    S3EncryptionConfigurationOutputTypeDef,
     S3EncryptionConfigurationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
     UpdateLedgerRequestRequestTypeDef,
     CancelJournalKinesisStreamResponseTypeDef,
     CreateLedgerResponseTypeDef,
@@ -338,27 +335,26 @@
     ExportJournalToS3ResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StreamJournalToKinesisResponseTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
-    GetRevisionRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
+    GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     JournalKinesisStreamDescriptionTypeDef,
     StreamJournalToKinesisRequestRequestTypeDef,
     ListLedgersResponseTypeDef,
-    S3ExportConfigurationOutputTypeDef,
     S3ExportConfigurationTypeDef,
     DescribeJournalKinesisStreamResponseTypeDef,
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
-    JournalS3ExportDescriptionTypeDef,
     ExportJournalToS3RequestRequestTypeDef,
+    JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
```

### Comparing `mypy-boto3-qldb-1.28.12/README.md` & `mypy-boto3-qldb-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -280,25 +280,22 @@
     CreateLedgerRequestRequestTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
     ValueHolderTypeDef,
-    ValueHolderOutputTypeDef,
     GetDigestRequestRequestTypeDef,
-    KinesisConfigurationOutputTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    S3EncryptionConfigurationOutputTypeDef,
     S3EncryptionConfigurationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
     UpdateLedgerRequestRequestTypeDef,
     CancelJournalKinesisStreamResponseTypeDef,
     CreateLedgerResponseTypeDef,
@@ -306,27 +303,26 @@
     ExportJournalToS3ResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StreamJournalToKinesisResponseTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
-    GetRevisionRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
+    GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     JournalKinesisStreamDescriptionTypeDef,
     StreamJournalToKinesisRequestRequestTypeDef,
     ListLedgersResponseTypeDef,
-    S3ExportConfigurationOutputTypeDef,
     S3ExportConfigurationTypeDef,
     DescribeJournalKinesisStreamResponseTypeDef,
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
-    JournalS3ExportDescriptionTypeDef,
     ExportJournalToS3RequestRequestTypeDef,
+    JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
```

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/__main__.py` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.QLDB 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.QLDB 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
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

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/client.py` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/client.pyi` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/literals.py` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/literals.pyi` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/type_defs.py` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,36 +27,32 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
     "ValueHolderTypeDef",
-    "ValueHolderOutputTypeDef",
     "GetDigestRequestRequestTypeDef",
-    "KinesisConfigurationOutputTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
     "ListLedgersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "S3EncryptionConfigurationOutputTypeDef",
     "S3EncryptionConfigurationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
     "UpdateLedgerRequestRequestTypeDef",
     "CancelJournalKinesisStreamResponseTypeDef",
     "CreateLedgerResponseTypeDef",
@@ -64,27 +60,26 @@
     "ExportJournalToS3ResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StreamJournalToKinesisResponseTypeDef",
     "UpdateLedgerPermissionsModeResponseTypeDef",
     "DescribeLedgerResponseTypeDef",
     "UpdateLedgerResponseTypeDef",
     "GetBlockRequestRequestTypeDef",
-    "GetRevisionRequestRequestTypeDef",
     "GetBlockResponseTypeDef",
     "GetDigestResponseTypeDef",
+    "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
     "JournalKinesisStreamDescriptionTypeDef",
     "StreamJournalToKinesisRequestRequestTypeDef",
     "ListLedgersResponseTypeDef",
-    "S3ExportConfigurationOutputTypeDef",
     "S3ExportConfigurationTypeDef",
     "DescribeJournalKinesisStreamResponseTypeDef",
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
-    "JournalS3ExportDescriptionTypeDef",
     "ExportJournalToS3RequestRequestTypeDef",
+    "JournalS3ExportDescriptionTypeDef",
     "DescribeJournalS3ExportResponseTypeDef",
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     "ListJournalS3ExportsResponseTypeDef",
 )
 
 CancelJournalKinesisStreamRequestRequestTypeDef = TypedDict(
     "CancelJournalKinesisStreamRequestRequestTypeDef",
@@ -118,21 +113,19 @@
         "Tags": Mapping[str, str],
         "DeletionProtection": bool,
         "KmsKey": str,
     },
     total=False,
 )
 
-
 class CreateLedgerRequestRequestTypeDef(
     _RequiredCreateLedgerRequestRequestTypeDef, _OptionalCreateLedgerRequestRequestTypeDef
 ):
     pass
 
-
 DeleteLedgerRequestRequestTypeDef = TypedDict(
     "DeleteLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -170,86 +163,53 @@
     "_OptionalLedgerEncryptionDescriptionTypeDef",
     {
         "InaccessibleKmsKeyDateTime": datetime,
     },
     total=False,
 )
 
-
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
-
 ValueHolderTypeDef = TypedDict(
     "ValueHolderTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
 
-ValueHolderOutputTypeDef = TypedDict(
-    "ValueHolderOutputTypeDef",
-    {
-        "IonText": str,
-    },
-    total=False,
-)
-
 GetDigestRequestRequestTypeDef = TypedDict(
     "GetDigestRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-_RequiredKinesisConfigurationOutputTypeDef = TypedDict(
-    "_RequiredKinesisConfigurationOutputTypeDef",
-    {
-        "StreamArn": str,
-    },
-)
-_OptionalKinesisConfigurationOutputTypeDef = TypedDict(
-    "_OptionalKinesisConfigurationOutputTypeDef",
-    {
-        "AggregationEnabled": bool,
-    },
-    total=False,
-)
-
-
-class KinesisConfigurationOutputTypeDef(
-    _RequiredKinesisConfigurationOutputTypeDef, _OptionalKinesisConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredKinesisConfigurationTypeDef = TypedDict(
     "_RequiredKinesisConfigurationTypeDef",
     {
         "StreamArn": str,
     },
 )
 _OptionalKinesisConfigurationTypeDef = TypedDict(
     "_OptionalKinesisConfigurationTypeDef",
     {
         "AggregationEnabled": bool,
     },
     total=False,
 )
 
-
 class KinesisConfigurationTypeDef(
     _RequiredKinesisConfigurationTypeDef, _OptionalKinesisConfigurationTypeDef
 ):
     pass
 
-
 LedgerSummaryTypeDef = TypedDict(
     "LedgerSummaryTypeDef",
     {
         "Name": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
     },
@@ -267,22 +227,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListJournalKinesisStreamsForLedgerRequestRequestTypeDef(
     _RequiredListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     _OptionalListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJournalS3ExportsForLedgerRequestRequestTypeDef = TypedDict(
@@ -290,22 +248,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListJournalS3ExportsForLedgerRequestRequestTypeDef(
     _RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef,
     _OptionalListJournalS3ExportsForLedgerRequestRequestTypeDef,
 ):
     pass
 
-
 ListJournalS3ExportsRequestRequestTypeDef = TypedDict(
     "ListJournalS3ExportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -323,56 +279,33 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredS3EncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3EncryptionConfigurationOutputTypeDef",
-    {
-        "ObjectEncryptionType": S3ObjectEncryptionTypeType,
-    },
-)
-_OptionalS3EncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3EncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
-
-class S3EncryptionConfigurationOutputTypeDef(
-    _RequiredS3EncryptionConfigurationOutputTypeDef, _OptionalS3EncryptionConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredS3EncryptionConfigurationTypeDef = TypedDict(
     "_RequiredS3EncryptionConfigurationTypeDef",
     {
         "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
 _OptionalS3EncryptionConfigurationTypeDef = TypedDict(
     "_OptionalS3EncryptionConfigurationTypeDef",
     {
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-
 class S3EncryptionConfigurationTypeDef(
     _RequiredS3EncryptionConfigurationTypeDef, _OptionalS3EncryptionConfigurationTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -404,21 +337,19 @@
     {
         "DeletionProtection": bool,
         "KmsKey": str,
     },
     total=False,
 )
 
-
 class UpdateLedgerRequestRequestTypeDef(
     _RequiredUpdateLedgerRequestRequestTypeDef, _OptionalUpdateLedgerRequestRequestTypeDef
 ):
     pass
 
-
 CancelJournalKinesisStreamResponseTypeDef = TypedDict(
     "CancelJournalKinesisStreamResponseTypeDef",
     {
         "StreamId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -516,20 +447,36 @@
     "_OptionalGetBlockRequestRequestTypeDef",
     {
         "DigestTipAddress": ValueHolderTypeDef,
     },
     total=False,
 )
 
-
 class GetBlockRequestRequestTypeDef(
     _RequiredGetBlockRequestRequestTypeDef, _OptionalGetBlockRequestRequestTypeDef
 ):
     pass
 
+GetBlockResponseTypeDef = TypedDict(
+    "GetBlockResponseTypeDef",
+    {
+        "Block": ValueHolderTypeDef,
+        "Proof": ValueHolderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDigestResponseTypeDef = TypedDict(
+    "GetDigestResponseTypeDef",
+    {
+        "Digest": bytes,
+        "DigestTipAddress": ValueHolderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredGetRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredGetRevisionRequestRequestTypeDef",
     {
         "Name": str,
         "BlockAddress": ValueHolderTypeDef,
         "DocumentId": str,
@@ -539,56 +486,36 @@
     "_OptionalGetRevisionRequestRequestTypeDef",
     {
         "DigestTipAddress": ValueHolderTypeDef,
     },
     total=False,
 )
 
-
 class GetRevisionRequestRequestTypeDef(
     _RequiredGetRevisionRequestRequestTypeDef, _OptionalGetRevisionRequestRequestTypeDef
 ):
     pass
 
-
-GetBlockResponseTypeDef = TypedDict(
-    "GetBlockResponseTypeDef",
-    {
-        "Block": ValueHolderOutputTypeDef,
-        "Proof": ValueHolderOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDigestResponseTypeDef = TypedDict(
-    "GetDigestResponseTypeDef",
-    {
-        "Digest": bytes,
-        "DigestTipAddress": ValueHolderOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetRevisionResponseTypeDef = TypedDict(
     "GetRevisionResponseTypeDef",
     {
-        "Proof": ValueHolderOutputTypeDef,
-        "Revision": ValueHolderOutputTypeDef,
+        "Proof": ValueHolderTypeDef,
+        "Revision": ValueHolderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_RequiredJournalKinesisStreamDescriptionTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
         "StreamId": str,
         "Status": StreamStatusType,
-        "KinesisConfiguration": KinesisConfigurationOutputTypeDef,
+        "KinesisConfiguration": KinesisConfigurationTypeDef,
         "StreamName": str,
     },
 )
 _OptionalJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_OptionalJournalKinesisStreamDescriptionTypeDef",
     {
         "CreationTime": datetime,
@@ -596,21 +523,19 @@
         "ExclusiveEndTime": datetime,
         "Arn": str,
         "ErrorCause": ErrorCauseType,
     },
     total=False,
 )
 
-
 class JournalKinesisStreamDescriptionTypeDef(
     _RequiredJournalKinesisStreamDescriptionTypeDef, _OptionalJournalKinesisStreamDescriptionTypeDef
 ):
     pass
 
-
 _RequiredStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_RequiredStreamJournalToKinesisRequestRequestTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
         "InclusiveStartTime": Union[datetime, str],
         "KinesisConfiguration": KinesisConfigurationTypeDef,
@@ -622,40 +547,29 @@
     {
         "Tags": Mapping[str, str],
         "ExclusiveEndTime": Union[datetime, str],
     },
     total=False,
 )
 
-
 class StreamJournalToKinesisRequestRequestTypeDef(
     _RequiredStreamJournalToKinesisRequestRequestTypeDef,
     _OptionalStreamJournalToKinesisRequestRequestTypeDef,
 ):
     pass
 
-
 ListLedgersResponseTypeDef = TypedDict(
     "ListLedgersResponseTypeDef",
     {
         "Ledgers": List[LedgerSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-S3ExportConfigurationOutputTypeDef = TypedDict(
-    "S3ExportConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-        "Prefix": str,
-        "EncryptionConfiguration": S3EncryptionConfigurationOutputTypeDef,
-    },
-)
-
 S3ExportConfigurationTypeDef = TypedDict(
     "S3ExportConfigurationTypeDef",
     {
         "Bucket": str,
         "Prefix": str,
         "EncryptionConfiguration": S3EncryptionConfigurationTypeDef,
     },
@@ -674,67 +588,63 @@
     {
         "Streams": List[JournalKinesisStreamDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
-    "_RequiredJournalS3ExportDescriptionTypeDef",
+_RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
+    "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
-        "LedgerName": str,
-        "ExportId": str,
-        "ExportCreationTime": datetime,
-        "Status": ExportStatusType,
-        "InclusiveStartTime": datetime,
-        "ExclusiveEndTime": datetime,
-        "S3ExportConfiguration": S3ExportConfigurationOutputTypeDef,
+        "Name": str,
+        "InclusiveStartTime": Union[datetime, str],
+        "ExclusiveEndTime": Union[datetime, str],
+        "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalJournalS3ExportDescriptionTypeDef = TypedDict(
-    "_OptionalJournalS3ExportDescriptionTypeDef",
+_OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
+    "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
-
-class JournalS3ExportDescriptionTypeDef(
-    _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
+class ExportJournalToS3RequestRequestTypeDef(
+    _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
 ):
     pass
 
-
-_RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
-    "_RequiredExportJournalToS3RequestRequestTypeDef",
+_RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
+    "_RequiredJournalS3ExportDescriptionTypeDef",
     {
-        "Name": str,
-        "InclusiveStartTime": Union[datetime, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "LedgerName": str,
+        "ExportId": str,
+        "ExportCreationTime": datetime,
+        "Status": ExportStatusType,
+        "InclusiveStartTime": datetime,
+        "ExclusiveEndTime": datetime,
         "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
-    "_OptionalExportJournalToS3RequestRequestTypeDef",
+_OptionalJournalS3ExportDescriptionTypeDef = TypedDict(
+    "_OptionalJournalS3ExportDescriptionTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
-
-class ExportJournalToS3RequestRequestTypeDef(
-    _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
+class JournalS3ExportDescriptionTypeDef(
+    _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
 ):
     pass
 
-
 DescribeJournalS3ExportResponseTypeDef = TypedDict(
     "DescribeJournalS3ExportResponseTypeDef",
     {
         "ExportDescription": JournalS3ExportDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb/type_defs.pyi` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,35 +27,33 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
     "ValueHolderTypeDef",
-    "ValueHolderOutputTypeDef",
     "GetDigestRequestRequestTypeDef",
-    "KinesisConfigurationOutputTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
     "ListLedgersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "S3EncryptionConfigurationOutputTypeDef",
     "S3EncryptionConfigurationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
     "UpdateLedgerRequestRequestTypeDef",
     "CancelJournalKinesisStreamResponseTypeDef",
     "CreateLedgerResponseTypeDef",
@@ -63,27 +61,26 @@
     "ExportJournalToS3ResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StreamJournalToKinesisResponseTypeDef",
     "UpdateLedgerPermissionsModeResponseTypeDef",
     "DescribeLedgerResponseTypeDef",
     "UpdateLedgerResponseTypeDef",
     "GetBlockRequestRequestTypeDef",
-    "GetRevisionRequestRequestTypeDef",
     "GetBlockResponseTypeDef",
     "GetDigestResponseTypeDef",
+    "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
     "JournalKinesisStreamDescriptionTypeDef",
     "StreamJournalToKinesisRequestRequestTypeDef",
     "ListLedgersResponseTypeDef",
-    "S3ExportConfigurationOutputTypeDef",
     "S3ExportConfigurationTypeDef",
     "DescribeJournalKinesisStreamResponseTypeDef",
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
-    "JournalS3ExportDescriptionTypeDef",
     "ExportJournalToS3RequestRequestTypeDef",
+    "JournalS3ExportDescriptionTypeDef",
     "DescribeJournalS3ExportResponseTypeDef",
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     "ListJournalS3ExportsResponseTypeDef",
 )
 
 CancelJournalKinesisStreamRequestRequestTypeDef = TypedDict(
     "CancelJournalKinesisStreamRequestRequestTypeDef",
@@ -117,19 +114,21 @@
         "Tags": Mapping[str, str],
         "DeletionProtection": bool,
         "KmsKey": str,
     },
     total=False,
 )
 
+
 class CreateLedgerRequestRequestTypeDef(
     _RequiredCreateLedgerRequestRequestTypeDef, _OptionalCreateLedgerRequestRequestTypeDef
 ):
     pass
 
+
 DeleteLedgerRequestRequestTypeDef = TypedDict(
     "DeleteLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -167,80 +166,57 @@
     "_OptionalLedgerEncryptionDescriptionTypeDef",
     {
         "InaccessibleKmsKeyDateTime": datetime,
     },
     total=False,
 )
 
+
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
+
 ValueHolderTypeDef = TypedDict(
     "ValueHolderTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
 
-ValueHolderOutputTypeDef = TypedDict(
-    "ValueHolderOutputTypeDef",
-    {
-        "IonText": str,
-    },
-    total=False,
-)
-
 GetDigestRequestRequestTypeDef = TypedDict(
     "GetDigestRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-_RequiredKinesisConfigurationOutputTypeDef = TypedDict(
-    "_RequiredKinesisConfigurationOutputTypeDef",
-    {
-        "StreamArn": str,
-    },
-)
-_OptionalKinesisConfigurationOutputTypeDef = TypedDict(
-    "_OptionalKinesisConfigurationOutputTypeDef",
-    {
-        "AggregationEnabled": bool,
-    },
-    total=False,
-)
-
-class KinesisConfigurationOutputTypeDef(
-    _RequiredKinesisConfigurationOutputTypeDef, _OptionalKinesisConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredKinesisConfigurationTypeDef = TypedDict(
     "_RequiredKinesisConfigurationTypeDef",
     {
         "StreamArn": str,
     },
 )
 _OptionalKinesisConfigurationTypeDef = TypedDict(
     "_OptionalKinesisConfigurationTypeDef",
     {
         "AggregationEnabled": bool,
     },
     total=False,
 )
 
+
 class KinesisConfigurationTypeDef(
     _RequiredKinesisConfigurationTypeDef, _OptionalKinesisConfigurationTypeDef
 ):
     pass
 
+
 LedgerSummaryTypeDef = TypedDict(
     "LedgerSummaryTypeDef",
     {
         "Name": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
     },
@@ -258,20 +234,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListJournalKinesisStreamsForLedgerRequestRequestTypeDef(
     _RequiredListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     _OptionalListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalListJournalS3ExportsForLedgerRequestRequestTypeDef = TypedDict(
@@ -279,20 +257,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListJournalS3ExportsForLedgerRequestRequestTypeDef(
     _RequiredListJournalS3ExportsForLedgerRequestRequestTypeDef,
     _OptionalListJournalS3ExportsForLedgerRequestRequestTypeDef,
 ):
     pass
 
+
 ListJournalS3ExportsRequestRequestTypeDef = TypedDict(
     "ListJournalS3ExportsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -310,52 +290,35 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredS3EncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3EncryptionConfigurationOutputTypeDef",
-    {
-        "ObjectEncryptionType": S3ObjectEncryptionTypeType,
-    },
-)
-_OptionalS3EncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3EncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
-class S3EncryptionConfigurationOutputTypeDef(
-    _RequiredS3EncryptionConfigurationOutputTypeDef, _OptionalS3EncryptionConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredS3EncryptionConfigurationTypeDef = TypedDict(
     "_RequiredS3EncryptionConfigurationTypeDef",
     {
         "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
 _OptionalS3EncryptionConfigurationTypeDef = TypedDict(
     "_OptionalS3EncryptionConfigurationTypeDef",
     {
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+
 class S3EncryptionConfigurationTypeDef(
     _RequiredS3EncryptionConfigurationTypeDef, _OptionalS3EncryptionConfigurationTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -387,19 +350,21 @@
     {
         "DeletionProtection": bool,
         "KmsKey": str,
     },
     total=False,
 )
 
+
 class UpdateLedgerRequestRequestTypeDef(
     _RequiredUpdateLedgerRequestRequestTypeDef, _OptionalUpdateLedgerRequestRequestTypeDef
 ):
     pass
 
+
 CancelJournalKinesisStreamResponseTypeDef = TypedDict(
     "CancelJournalKinesisStreamResponseTypeDef",
     {
         "StreamId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -497,19 +462,39 @@
     "_OptionalGetBlockRequestRequestTypeDef",
     {
         "DigestTipAddress": ValueHolderTypeDef,
     },
     total=False,
 )
 
+
 class GetBlockRequestRequestTypeDef(
     _RequiredGetBlockRequestRequestTypeDef, _OptionalGetBlockRequestRequestTypeDef
 ):
     pass
 
+
+GetBlockResponseTypeDef = TypedDict(
+    "GetBlockResponseTypeDef",
+    {
+        "Block": ValueHolderTypeDef,
+        "Proof": ValueHolderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDigestResponseTypeDef = TypedDict(
+    "GetDigestResponseTypeDef",
+    {
+        "Digest": bytes,
+        "DigestTipAddress": ValueHolderTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredGetRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredGetRevisionRequestRequestTypeDef",
     {
         "Name": str,
         "BlockAddress": ValueHolderTypeDef,
         "DocumentId": str,
     },
@@ -518,54 +503,38 @@
     "_OptionalGetRevisionRequestRequestTypeDef",
     {
         "DigestTipAddress": ValueHolderTypeDef,
     },
     total=False,
 )
 
+
 class GetRevisionRequestRequestTypeDef(
     _RequiredGetRevisionRequestRequestTypeDef, _OptionalGetRevisionRequestRequestTypeDef
 ):
     pass
 
-GetBlockResponseTypeDef = TypedDict(
-    "GetBlockResponseTypeDef",
-    {
-        "Block": ValueHolderOutputTypeDef,
-        "Proof": ValueHolderOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetDigestResponseTypeDef = TypedDict(
-    "GetDigestResponseTypeDef",
-    {
-        "Digest": bytes,
-        "DigestTipAddress": ValueHolderOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 GetRevisionResponseTypeDef = TypedDict(
     "GetRevisionResponseTypeDef",
     {
-        "Proof": ValueHolderOutputTypeDef,
-        "Revision": ValueHolderOutputTypeDef,
+        "Proof": ValueHolderTypeDef,
+        "Revision": ValueHolderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_RequiredJournalKinesisStreamDescriptionTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
         "StreamId": str,
         "Status": StreamStatusType,
-        "KinesisConfiguration": KinesisConfigurationOutputTypeDef,
+        "KinesisConfiguration": KinesisConfigurationTypeDef,
         "StreamName": str,
     },
 )
 _OptionalJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_OptionalJournalKinesisStreamDescriptionTypeDef",
     {
         "CreationTime": datetime,
@@ -573,19 +542,21 @@
         "ExclusiveEndTime": datetime,
         "Arn": str,
         "ErrorCause": ErrorCauseType,
     },
     total=False,
 )
 
+
 class JournalKinesisStreamDescriptionTypeDef(
     _RequiredJournalKinesisStreamDescriptionTypeDef, _OptionalJournalKinesisStreamDescriptionTypeDef
 ):
     pass
 
+
 _RequiredStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_RequiredStreamJournalToKinesisRequestRequestTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
         "InclusiveStartTime": Union[datetime, str],
         "KinesisConfiguration": KinesisConfigurationTypeDef,
@@ -597,38 +568,31 @@
     {
         "Tags": Mapping[str, str],
         "ExclusiveEndTime": Union[datetime, str],
     },
     total=False,
 )
 
+
 class StreamJournalToKinesisRequestRequestTypeDef(
     _RequiredStreamJournalToKinesisRequestRequestTypeDef,
     _OptionalStreamJournalToKinesisRequestRequestTypeDef,
 ):
     pass
 
+
 ListLedgersResponseTypeDef = TypedDict(
     "ListLedgersResponseTypeDef",
     {
         "Ledgers": List[LedgerSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-S3ExportConfigurationOutputTypeDef = TypedDict(
-    "S3ExportConfigurationOutputTypeDef",
-    {
-        "Bucket": str,
-        "Prefix": str,
-        "EncryptionConfiguration": S3EncryptionConfigurationOutputTypeDef,
-    },
-)
-
 S3ExportConfigurationTypeDef = TypedDict(
     "S3ExportConfigurationTypeDef",
     {
         "Bucket": str,
         "Prefix": str,
         "EncryptionConfiguration": S3EncryptionConfigurationTypeDef,
     },
@@ -647,63 +611,67 @@
     {
         "Streams": List[JournalKinesisStreamDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
-    "_RequiredJournalS3ExportDescriptionTypeDef",
+_RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
+    "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
-        "LedgerName": str,
-        "ExportId": str,
-        "ExportCreationTime": datetime,
-        "Status": ExportStatusType,
-        "InclusiveStartTime": datetime,
-        "ExclusiveEndTime": datetime,
-        "S3ExportConfiguration": S3ExportConfigurationOutputTypeDef,
+        "Name": str,
+        "InclusiveStartTime": Union[datetime, str],
+        "ExclusiveEndTime": Union[datetime, str],
+        "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalJournalS3ExportDescriptionTypeDef = TypedDict(
-    "_OptionalJournalS3ExportDescriptionTypeDef",
+_OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
+    "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
-class JournalS3ExportDescriptionTypeDef(
-    _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
+
+class ExportJournalToS3RequestRequestTypeDef(
+    _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
 ):
     pass
 
-_RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
-    "_RequiredExportJournalToS3RequestRequestTypeDef",
+
+_RequiredJournalS3ExportDescriptionTypeDef = TypedDict(
+    "_RequiredJournalS3ExportDescriptionTypeDef",
     {
-        "Name": str,
-        "InclusiveStartTime": Union[datetime, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "LedgerName": str,
+        "ExportId": str,
+        "ExportCreationTime": datetime,
+        "Status": ExportStatusType,
+        "InclusiveStartTime": datetime,
+        "ExclusiveEndTime": datetime,
         "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
-    "_OptionalExportJournalToS3RequestRequestTypeDef",
+_OptionalJournalS3ExportDescriptionTypeDef = TypedDict(
+    "_OptionalJournalS3ExportDescriptionTypeDef",
     {
         "OutputFormat": OutputFormatType,
     },
     total=False,
 )
 
-class ExportJournalToS3RequestRequestTypeDef(
-    _RequiredExportJournalToS3RequestRequestTypeDef, _OptionalExportJournalToS3RequestRequestTypeDef
+
+class JournalS3ExportDescriptionTypeDef(
+    _RequiredJournalS3ExportDescriptionTypeDef, _OptionalJournalS3ExportDescriptionTypeDef
 ):
     pass
 
+
 DescribeJournalS3ExportResponseTypeDef = TypedDict(
     "DescribeJournalS3ExportResponseTypeDef",
     {
         "ExportDescription": JournalS3ExportDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/PKG-INFO` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-qldb
-Version: 1.28.12
-Summary: Type annotations for boto3.QLDB 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-qldb.svg?color=blue)](https://pypi.org/project/mypy-boto3-qldb)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-qldb)](https://pepy.tech/project/mypy-boto3-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QLDB 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[boto3.QLDB 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [mypy-boto3-qldb docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,25 +312,22 @@
     CreateLedgerRequestRequestTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
     ValueHolderTypeDef,
-    ValueHolderOutputTypeDef,
     GetDigestRequestRequestTypeDef,
-    KinesisConfigurationOutputTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    S3EncryptionConfigurationOutputTypeDef,
     S3EncryptionConfigurationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
     UpdateLedgerRequestRequestTypeDef,
     CancelJournalKinesisStreamResponseTypeDef,
     CreateLedgerResponseTypeDef,
@@ -338,27 +335,26 @@
     ExportJournalToS3ResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StreamJournalToKinesisResponseTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
-    GetRevisionRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
+    GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
     JournalKinesisStreamDescriptionTypeDef,
     StreamJournalToKinesisRequestRequestTypeDef,
     ListLedgersResponseTypeDef,
-    S3ExportConfigurationOutputTypeDef,
     S3ExportConfigurationTypeDef,
     DescribeJournalKinesisStreamResponseTypeDef,
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
-    JournalS3ExportDescriptionTypeDef,
     ExportJournalToS3RequestRequestTypeDef,
+    JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
```

### Comparing `mypy-boto3-qldb-1.28.12/mypy_boto3_qldb.egg-info/SOURCES.txt` & `mypy-boto3-qldb-1.28.15/mypy_boto3_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-qldb-1.28.12/setup.py` & `mypy-boto3-qldb-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-qldb",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.QLDB 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.QLDB 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

