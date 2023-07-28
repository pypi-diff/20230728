# Comparing `tmp/mypy-boto3-signer-1.28.12.tar.gz` & `tmp/mypy-boto3-signer-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-signer-1.28.12.tar", last modified: Thu Jul 27 11:49:40 2023, max compression
+gzip compressed data, was "mypy-boto3-signer-1.28.15.tar", last modified: Fri Jul 28 20:43:46 2023, max compression
```

## Comparing `mypy-boto3-signer-1.28.12.tar` & `mypy-boto3-signer-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:40.029305 mypy-boto3-signer-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16210 2023-07-27 11:49:40.029305 mypy-boto3-signer-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14727 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:40.013305 mypy-boto3-signer-1.28.12/mypy_boto3_signer/
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22895 2023-07-27 11:47:01.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22878 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:40.029305 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16210 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 11:49:39.000000 mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:40.029305 mypy-boto3-signer-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 11:47:00.000000 mypy-boto3-signer-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.997895 mypy-boto3-signer-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15991 2023-07-28 20:43:45.997895 mypy-boto3-signer-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.989895 mypy-boto3-signer-1.28.15/mypy_boto3_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21524 2023-07-28 20:39:33.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21507 2023-07-28 20:39:33.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:45.993895 mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15991 2023-07-28 20:43:45.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:45.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:45.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:45.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:45.000000 mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:45.997895 mypy-boto3-signer-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:39:32.000000 mypy-boto3-signer-1.28.15/setup.py
```

### Comparing `mypy-boto3-signer-1.28.12/LICENSE` & `mypy-boto3-signer-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/PKG-INFO` & `mypy-boto3-signer-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.28.12
-Summary: Type annotations for boto3.signer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.signer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,41 +367,37 @@
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
-    SigningMaterialOutputTypeDef,
+    SigningMaterialTypeDef,
     S3DestinationTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
     GetRevocationStatusRequestRequestTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
-    SignatureValidityPeriodOutputTypeDef,
+    SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     PaginatorConfigTypeDef,
     ListSigningJobsRequestRequestTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    SignatureValidityPeriodTypeDef,
-    SigningMaterialTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
-    S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SignPayloadRequestRequestTypeDef,
-    SigningConfigurationOverridesOutputTypeDef,
     SigningConfigurationOverridesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddProfilePermissionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -414,17 +410,15 @@
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
     ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
-    SourceOutputTypeDef,
     SourceTypeDef,
-    SigningPlatformOverridesOutputTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
     StartSigningJobRequestRequestTypeDef,
     DescribeSigningJobResponseTypeDef,
```

### Comparing `mypy-boto3-signer-1.28.12/README.md` & `mypy-boto3-signer-1.28.15/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -335,41 +335,37 @@
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
-    SigningMaterialOutputTypeDef,
+    SigningMaterialTypeDef,
     S3DestinationTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
     GetRevocationStatusRequestRequestTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
-    SignatureValidityPeriodOutputTypeDef,
+    SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     PaginatorConfigTypeDef,
     ListSigningJobsRequestRequestTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    SignatureValidityPeriodTypeDef,
-    SigningMaterialTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
-    S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SignPayloadRequestRequestTypeDef,
-    SigningConfigurationOverridesOutputTypeDef,
     SigningConfigurationOverridesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddProfilePermissionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -382,17 +378,15 @@
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
     ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
-    SourceOutputTypeDef,
     SourceTypeDef,
-    SigningPlatformOverridesOutputTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
     StartSigningJobRequestRequestTypeDef,
     DescribeSigningJobResponseTypeDef,
```

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/__init__.py` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/__init__.pyi` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/__main__.py` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.signer 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.signer 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
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

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/client.py` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/client.pyi` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/literals.py` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/literals.pyi` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/paginator.py` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/paginator.pyi` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/type_defs.py` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,41 +39,37 @@
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
-    "SigningMaterialOutputTypeDef",
+    "SigningMaterialTypeDef",
     "S3DestinationTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
     "GetRevocationStatusRequestRequestTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
-    "SignatureValidityPeriodOutputTypeDef",
+    "SignatureValidityPeriodTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "PaginatorConfigTypeDef",
     "ListSigningJobsRequestRequestTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "SignatureValidityPeriodTypeDef",
-    "SigningMaterialTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
     "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
-    "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
     "SignPayloadRequestRequestTypeDef",
-    "SigningConfigurationOverridesOutputTypeDef",
     "SigningConfigurationOverridesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddProfilePermissionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetRevocationStatusResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -86,17 +82,15 @@
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
     "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
     "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
-    "SourceOutputTypeDef",
     "SourceTypeDef",
-    "SigningPlatformOverridesOutputTypeDef",
     "SigningPlatformOverridesTypeDef",
     "ListSigningProfilesResponseTypeDef",
     "GetSigningPlatformResponseTypeDef",
     "SigningPlatformTypeDef",
     "SigningJobTypeDef",
     "StartSigningJobRequestRequestTypeDef",
     "DescribeSigningJobResponseTypeDef",
@@ -172,16 +166,16 @@
         "reason": str,
         "revokedAt": datetime,
         "revokedBy": str,
     },
     total=False,
 )
 
-SigningMaterialOutputTypeDef = TypedDict(
-    "SigningMaterialOutputTypeDef",
+SigningMaterialTypeDef = TypedDict(
+    "SigningMaterialTypeDef",
     {
         "certificateArn": str,
     },
 )
 
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
@@ -243,16 +237,16 @@
 
 class GetSigningProfileRequestRequestTypeDef(
     _RequiredGetSigningProfileRequestRequestTypeDef, _OptionalGetSigningProfileRequestRequestTypeDef
 ):
     pass
 
 
-SignatureValidityPeriodOutputTypeDef = TypedDict(
-    "SignatureValidityPeriodOutputTypeDef",
+SignatureValidityPeriodTypeDef = TypedDict(
+    "SignatureValidityPeriodTypeDef",
     {
         "value": int,
         "type": ValidityTypeType,
     },
     total=False,
 )
 
@@ -360,30 +354,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-SignatureValidityPeriodTypeDef = TypedDict(
-    "SignatureValidityPeriodTypeDef",
-    {
-        "value": int,
-        "type": ValidityTypeType,
-    },
-    total=False,
-)
-
-SigningMaterialTypeDef = TypedDict(
-    "SigningMaterialTypeDef",
-    {
-        "certificateArn": str,
-    },
-)
-
 RemoveProfilePermissionRequestRequestTypeDef = TypedDict(
     "RemoveProfilePermissionRequestRequestTypeDef",
     {
         "profileName": str,
         "revisionId": str,
         "statementId": str,
     },
@@ -426,23 +404,14 @@
     {
         "bucketName": str,
         "key": str,
     },
     total=False,
 )
 
-S3SourceOutputTypeDef = TypedDict(
-    "S3SourceOutputTypeDef",
-    {
-        "bucketName": str,
-        "key": str,
-        "version": str,
-    },
-)
-
 S3SourceTypeDef = TypedDict(
     "S3SourceTypeDef",
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
@@ -467,23 +436,14 @@
 
 class SignPayloadRequestRequestTypeDef(
     _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
 ):
     pass
 
 
-SigningConfigurationOverridesOutputTypeDef = TypedDict(
-    "SigningConfigurationOverridesOutputTypeDef",
-    {
-        "encryptionAlgorithm": EncryptionAlgorithmType,
-        "hashAlgorithm": HashAlgorithmType,
-    },
-    total=False,
-)
-
 SigningConfigurationOverridesTypeDef = TypedDict(
     "SigningConfigurationOverridesTypeDef",
     {
         "encryptionAlgorithm": EncryptionAlgorithmType,
         "hashAlgorithm": HashAlgorithmType,
     },
     total=False,
@@ -606,16 +566,16 @@
 
 SigningProfileTypeDef = TypedDict(
     "SigningProfileTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
-        "signingMaterial": SigningMaterialOutputTypeDef,
-        "signatureValidityPeriod": SignatureValidityPeriodOutputTypeDef,
+        "signingMaterial": SigningMaterialTypeDef,
+        "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
         "platformId": str,
         "platformDisplayName": str,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "arn": str,
         "tags": Dict[str, str],
     },
@@ -682,39 +642,22 @@
     "SignedObjectTypeDef",
     {
         "s3": S3SignedObjectTypeDef,
     },
     total=False,
 )
 
-SourceOutputTypeDef = TypedDict(
-    "SourceOutputTypeDef",
-    {
-        "s3": S3SourceOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "s3": S3SourceTypeDef,
     },
     total=False,
 )
 
-SigningPlatformOverridesOutputTypeDef = TypedDict(
-    "SigningPlatformOverridesOutputTypeDef",
-    {
-        "signingConfiguration": SigningConfigurationOverridesOutputTypeDef,
-        "signingImageFormat": ImageFormatType,
-    },
-    total=False,
-)
-
 SigningPlatformOverridesTypeDef = TypedDict(
     "SigningPlatformOverridesTypeDef",
     {
         "signingConfiguration": SigningConfigurationOverridesTypeDef,
         "signingImageFormat": ImageFormatType,
     },
     total=False,
@@ -761,17 +704,17 @@
     total=False,
 )
 
 SigningJobTypeDef = TypedDict(
     "SigningJobTypeDef",
     {
         "jobId": str,
-        "source": SourceOutputTypeDef,
+        "source": SourceTypeDef,
         "signedObject": SignedObjectTypeDef,
-        "signingMaterial": SigningMaterialOutputTypeDef,
+        "signingMaterial": SigningMaterialTypeDef,
         "createdAt": datetime,
         "status": SigningStatusType,
         "isRevoked": bool,
         "profileName": str,
         "profileVersion": str,
         "platformId": str,
         "platformDisplayName": str,
@@ -806,21 +749,21 @@
     pass
 
 
 DescribeSigningJobResponseTypeDef = TypedDict(
     "DescribeSigningJobResponseTypeDef",
     {
         "jobId": str,
-        "source": SourceOutputTypeDef,
-        "signingMaterial": SigningMaterialOutputTypeDef,
+        "source": SourceTypeDef,
+        "signingMaterial": SigningMaterialTypeDef,
         "platformId": str,
         "platformDisplayName": str,
         "profileName": str,
         "profileVersion": str,
-        "overrides": SigningPlatformOverridesOutputTypeDef,
+        "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Dict[str, str],
         "createdAt": datetime,
         "completedAt": datetime,
         "signatureExpiresAt": datetime,
         "requestedBy": str,
         "status": SigningStatusType,
         "statusReason": str,
@@ -835,19 +778,19 @@
 GetSigningProfileResponseTypeDef = TypedDict(
     "GetSigningProfileResponseTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
         "revocationRecord": SigningProfileRevocationRecordTypeDef,
-        "signingMaterial": SigningMaterialOutputTypeDef,
+        "signingMaterial": SigningMaterialTypeDef,
         "platformId": str,
         "platformDisplayName": str,
-        "signatureValidityPeriod": SignatureValidityPeriodOutputTypeDef,
-        "overrides": SigningPlatformOverridesOutputTypeDef,
+        "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
+        "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "statusReason": str,
         "arn": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/type_defs.pyi` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -38,41 +38,37 @@
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
-    "SigningMaterialOutputTypeDef",
+    "SigningMaterialTypeDef",
     "S3DestinationTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
     "GetRevocationStatusRequestRequestTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
-    "SignatureValidityPeriodOutputTypeDef",
+    "SignatureValidityPeriodTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
     "PaginatorConfigTypeDef",
     "ListSigningJobsRequestRequestTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "SignatureValidityPeriodTypeDef",
-    "SigningMaterialTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
     "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
-    "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
     "SignPayloadRequestRequestTypeDef",
-    "SigningConfigurationOverridesOutputTypeDef",
     "SigningConfigurationOverridesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddProfilePermissionResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetRevocationStatusResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
@@ -85,17 +81,15 @@
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
     "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
     "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
-    "SourceOutputTypeDef",
     "SourceTypeDef",
-    "SigningPlatformOverridesOutputTypeDef",
     "SigningPlatformOverridesTypeDef",
     "ListSigningProfilesResponseTypeDef",
     "GetSigningPlatformResponseTypeDef",
     "SigningPlatformTypeDef",
     "SigningJobTypeDef",
     "StartSigningJobRequestRequestTypeDef",
     "DescribeSigningJobResponseTypeDef",
@@ -169,16 +163,16 @@
         "reason": str,
         "revokedAt": datetime,
         "revokedBy": str,
     },
     total=False,
 )
 
-SigningMaterialOutputTypeDef = TypedDict(
-    "SigningMaterialOutputTypeDef",
+SigningMaterialTypeDef = TypedDict(
+    "SigningMaterialTypeDef",
     {
         "certificateArn": str,
     },
 )
 
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
@@ -238,16 +232,16 @@
 )
 
 class GetSigningProfileRequestRequestTypeDef(
     _RequiredGetSigningProfileRequestRequestTypeDef, _OptionalGetSigningProfileRequestRequestTypeDef
 ):
     pass
 
-SignatureValidityPeriodOutputTypeDef = TypedDict(
-    "SignatureValidityPeriodOutputTypeDef",
+SignatureValidityPeriodTypeDef = TypedDict(
+    "SignatureValidityPeriodTypeDef",
     {
         "value": int,
         "type": ValidityTypeType,
     },
     total=False,
 )
 
@@ -353,30 +347,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-SignatureValidityPeriodTypeDef = TypedDict(
-    "SignatureValidityPeriodTypeDef",
-    {
-        "value": int,
-        "type": ValidityTypeType,
-    },
-    total=False,
-)
-
-SigningMaterialTypeDef = TypedDict(
-    "SigningMaterialTypeDef",
-    {
-        "certificateArn": str,
-    },
-)
-
 RemoveProfilePermissionRequestRequestTypeDef = TypedDict(
     "RemoveProfilePermissionRequestRequestTypeDef",
     {
         "profileName": str,
         "revisionId": str,
         "statementId": str,
     },
@@ -417,23 +395,14 @@
     {
         "bucketName": str,
         "key": str,
     },
     total=False,
 )
 
-S3SourceOutputTypeDef = TypedDict(
-    "S3SourceOutputTypeDef",
-    {
-        "bucketName": str,
-        "key": str,
-        "version": str,
-    },
-)
-
 S3SourceTypeDef = TypedDict(
     "S3SourceTypeDef",
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
@@ -456,23 +425,14 @@
 )
 
 class SignPayloadRequestRequestTypeDef(
     _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
 ):
     pass
 
-SigningConfigurationOverridesOutputTypeDef = TypedDict(
-    "SigningConfigurationOverridesOutputTypeDef",
-    {
-        "encryptionAlgorithm": EncryptionAlgorithmType,
-        "hashAlgorithm": HashAlgorithmType,
-    },
-    total=False,
-)
-
 SigningConfigurationOverridesTypeDef = TypedDict(
     "SigningConfigurationOverridesTypeDef",
     {
         "encryptionAlgorithm": EncryptionAlgorithmType,
         "hashAlgorithm": HashAlgorithmType,
     },
     total=False,
@@ -593,16 +553,16 @@
 
 SigningProfileTypeDef = TypedDict(
     "SigningProfileTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
-        "signingMaterial": SigningMaterialOutputTypeDef,
-        "signatureValidityPeriod": SignatureValidityPeriodOutputTypeDef,
+        "signingMaterial": SigningMaterialTypeDef,
+        "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
         "platformId": str,
         "platformDisplayName": str,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "arn": str,
         "tags": Dict[str, str],
     },
@@ -669,39 +629,22 @@
     "SignedObjectTypeDef",
     {
         "s3": S3SignedObjectTypeDef,
     },
     total=False,
 )
 
-SourceOutputTypeDef = TypedDict(
-    "SourceOutputTypeDef",
-    {
-        "s3": S3SourceOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceTypeDef = TypedDict(
     "SourceTypeDef",
     {
         "s3": S3SourceTypeDef,
     },
     total=False,
 )
 
-SigningPlatformOverridesOutputTypeDef = TypedDict(
-    "SigningPlatformOverridesOutputTypeDef",
-    {
-        "signingConfiguration": SigningConfigurationOverridesOutputTypeDef,
-        "signingImageFormat": ImageFormatType,
-    },
-    total=False,
-)
-
 SigningPlatformOverridesTypeDef = TypedDict(
     "SigningPlatformOverridesTypeDef",
     {
         "signingConfiguration": SigningConfigurationOverridesTypeDef,
         "signingImageFormat": ImageFormatType,
     },
     total=False,
@@ -748,17 +691,17 @@
     total=False,
 )
 
 SigningJobTypeDef = TypedDict(
     "SigningJobTypeDef",
     {
         "jobId": str,
-        "source": SourceOutputTypeDef,
+        "source": SourceTypeDef,
         "signedObject": SignedObjectTypeDef,
-        "signingMaterial": SigningMaterialOutputTypeDef,
+        "signingMaterial": SigningMaterialTypeDef,
         "createdAt": datetime,
         "status": SigningStatusType,
         "isRevoked": bool,
         "profileName": str,
         "profileVersion": str,
         "platformId": str,
         "platformDisplayName": str,
@@ -791,21 +734,21 @@
 ):
     pass
 
 DescribeSigningJobResponseTypeDef = TypedDict(
     "DescribeSigningJobResponseTypeDef",
     {
         "jobId": str,
-        "source": SourceOutputTypeDef,
-        "signingMaterial": SigningMaterialOutputTypeDef,
+        "source": SourceTypeDef,
+        "signingMaterial": SigningMaterialTypeDef,
         "platformId": str,
         "platformDisplayName": str,
         "profileName": str,
         "profileVersion": str,
-        "overrides": SigningPlatformOverridesOutputTypeDef,
+        "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Dict[str, str],
         "createdAt": datetime,
         "completedAt": datetime,
         "signatureExpiresAt": datetime,
         "requestedBy": str,
         "status": SigningStatusType,
         "statusReason": str,
@@ -820,19 +763,19 @@
 GetSigningProfileResponseTypeDef = TypedDict(
     "GetSigningProfileResponseTypeDef",
     {
         "profileName": str,
         "profileVersion": str,
         "profileVersionArn": str,
         "revocationRecord": SigningProfileRevocationRecordTypeDef,
-        "signingMaterial": SigningMaterialOutputTypeDef,
+        "signingMaterial": SigningMaterialTypeDef,
         "platformId": str,
         "platformDisplayName": str,
-        "signatureValidityPeriod": SignatureValidityPeriodOutputTypeDef,
-        "overrides": SigningPlatformOverridesOutputTypeDef,
+        "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
+        "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "statusReason": str,
         "arn": str,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/waiter.py` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer/waiter.pyi` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/PKG-INFO` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.28.12
-Summary: Type annotations for boto3.signer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.signer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-signer)](https://pepy.tech/project/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
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
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,41 +367,37 @@
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
-    SigningMaterialOutputTypeDef,
+    SigningMaterialTypeDef,
     S3DestinationTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
     GetRevocationStatusRequestRequestTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
-    SignatureValidityPeriodOutputTypeDef,
+    SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
     PaginatorConfigTypeDef,
     ListSigningJobsRequestRequestTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    SignatureValidityPeriodTypeDef,
-    SigningMaterialTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
-    S3SourceOutputTypeDef,
     S3SourceTypeDef,
     SignPayloadRequestRequestTypeDef,
-    SigningConfigurationOverridesOutputTypeDef,
     SigningConfigurationOverridesTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddProfilePermissionResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetRevocationStatusResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -414,17 +410,15 @@
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
     ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
-    SourceOutputTypeDef,
     SourceTypeDef,
-    SigningPlatformOverridesOutputTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
     StartSigningJobRequestRequestTypeDef,
     DescribeSigningJobResponseTypeDef,
```

### Comparing `mypy-boto3-signer-1.28.12/mypy_boto3_signer.egg-info/SOURCES.txt` & `mypy-boto3-signer-1.28.15/mypy_boto3_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.28.12/setup.py` & `mypy-boto3-signer-1.28.15/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-signer",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.signer 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.signer 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

